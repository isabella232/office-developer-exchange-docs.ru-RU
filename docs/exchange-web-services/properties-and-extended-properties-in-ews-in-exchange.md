---
title: Свойства и расширенные свойства в веб-службах Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 68623048-060e-4602-b3fa-62617a94cf72
description: Узнайте, как можно определить и доступ к свойствам элементов и папок с помощью веб-служб Exchange в Exchange.
ms.openlocfilehash: 0c01d9bd21cbef0a3536c8dbd85e192199b7b8ab
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761240"
---
# <a name="properties-and-extended-properties-in-ews-in-exchange"></a>Свойства и расширенные свойства в веб-службах Exchange

Узнайте, как можно определить и доступ к свойствам элементов и папок с помощью веб-служб Exchange в Exchange.
  
Почтовый ящик Exchange содержит большое число элементов, включая сообщения электронной почты, встреч, собраний и т. д. Эти элементы состоят из свойств; свойства описывают элементы. Свойства элемента можно использовать для выполнения [поиска](search-and-ews-in-exchange.md), [Синхронизация изменений элементов](mailbox-synchronization-and-ews-in-exchange.md)и [создавать типы настраиваемых свойств](http://code.msdn.microsoft.com/exchange/Exchange-2013-Create-314db25a). В этой статье Обзор свойств и как можно работать со свойствами в приложении.
  
## <a name="exchange-item-properties"></a>Свойства элемента Exchange
<a name="ItemsAreProperties"> </a>

Элементов и папок в Exchange, по сути строк в таблицах. Основные свойства, которое определяет элемента или папки — это [идентификатор веб-служб Exchange](ews-identifiers-in-exchange.md). Несмотря на то, что в базе данных Exchange, для веб-служб Exchange, имеются другие свойства, связанные с идентификатором идентификатор веб-служб Exchange действует как основной ключ для коллекции свойств, которые описывают элемента. Свойство идентификатора веб-служб Exchange состоит из двух частей:
  
- [Идентификатор элемента](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) или [FolderId](http://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx) свойство, которое определяет элемент 
    
- Свойство **ChangeKey** , содержит информацию о состояниях о элемента или папки изменилось ли 
    
Все элементы в почтовом ящике, хранятся в той же базе данных Exchange и использовать ту же схему базы данных. Элементы различаются по сочетание свойство [ItemClass](http://msdn.microsoft.com/library/56020078-50b4-4880-894a-a9f234033cfb%28Office.15%29.aspx) , ограничения и уровни бизнес-логики, влияющих на способ управления в Exchange хранения. В таблице 1 приведены применение свойства в различных типов элементов; в этом примере, электронной почты и встречи элементы. Оба элемента имеют значение для свойства [темы](http://msdn.microsoft.com/library/c140d6c2-deb1-4f67-a908-9397197c4ae7%28Office.15%29.aspx) . Но Обратите внимание на то, что свойство [IsAllDayEvent](http://msdn.microsoft.com/library/29140a64-9d7a-4a14-a10d-c98197c9831b%28Office.15%29.aspx) не имеет значение для элемента электронной почты и встречи не установлено свойство **IsReadReceiptRequested** . К счастью вам не нужно знать, какие свойства могут быть применены для каждого элемента класса; Веб-служб Exchange обрабатывает их для вас. 
  
**В таблице 1. Сравнение свойства встречи и адрес электронной почты**

|**Тип элемента**|**Класс элемента**|**Subject**|**IsAllDayEvent**|**IsReadReceiptRequested**|
|:-----|:-----|:-----|:-----|:-----|
|Электронная почта  <br/> |IPM. Примечание  <br/> |Отчет о состоянии: выполнения проекта X  <br/> |NULL  <br/> |true  <br/> |
|Appointment  <br/> |IPM.Appointment  <br/> |Компания Contoso собрания  <br/> |Нет  <br/> |NULL  <br/> |
   
Схема веб-служб Exchange поддерживает многие из ограничений, управляются в базе данных Exchange и уровни бизнес-логики от веб-служб Exchange и базы данных Exchange. Схема веб-служб Exchange применяется определенного набора свойств каждого типа элемента. Ниже приведены строго типизированных Exchange базы данных элементов, предоставленных веб-служб Exchange. 
  
- Сообщения электронной почты
    
- Встречи
    
- Контакты
    
- Списки рассылки
    
- Сообщений о собрании
    
- Приглашения на собрания
    
- Ответы на приглашения
    
- Отмен собрания
    
- Задачи
    
- Элементы
    
Веб-служб Exchange возвращает универсальный элементов как сообщения электронной почты. Управляемый API EWS реализует все эти типы элементов.
  
> [!NOTE]
> Объекты ответа только отправленный клиентом на сервер в ответ на элементы, полученные от других пользователей. Они не существуют в базе данных Exchange. 
  
## <a name="what-are-properties-in-ews"></a>Что такое свойствами в веб-служб Exchange?
<a name="WhatAreEWSProperties"> </a>

Схема веб-служб Exchange описывает данные, пересылаемые между клиентов веб-служб Exchange и Exchange. Большая часть схемы представлены свойства элемента и папки, доступные в базе данных Exchange. Схема веб-служб Exchange описывает XML-представление свойств базы данных Exchange, доступные для приложения. Конкретный набор свойств, в которых свойства доступны, что форме, они перевод и значения, они возвращают различаться в зависимости от какой вы пытаетесь выполнить. Например в ходе операции **FindItem** свойство **Body** будет возвращать только первые 512 символов, но операции **GetItem** возвращает полный текст элемента. Хотя большинство свойств, устанавливаемых и могут быть получены, некоторые свойства устанавливаются только с Exchange. Каждое свойство существует в схеме в формате XML, либо отражает свойства, как оно хранится в базе данных Exchange или вычисляется на основе свойств, хранящихся в базе данных Exchange. Свойство **Subject** приведен пример настраиваемые свойства. Свойство **UnreadCount** в папке является примером вычисляемого свойства. Базовый набор свойств являются общими для основных типов элементов. 
  
Что набора свойств, что приложение получает из Exchange следует принимать во внимание следующие факторы: 
  
- Операция, вызов приложения
    
- Фигура базового ответа
    
- Тип элемента
    
- Указанное свойство пути
    
Важно понимать, как эти различные факторы влияют на данные, можно получить доступ. Как в примере свойство **Body** , уже упоминалось ранее, некоторые данные доступна условно в зависимости от различных факторов. Общие сведения об этих факторов может сэкономить время, помогая Выбор правильных параметров для доступа к сведениям, который будет. Чтобы использовать функцию обнаружения свойств, которые доступны, необходимо тестирование этих факторов для определения способа доступа к свойствам потребностей приложения. В этом разделе описывается влияние этих факторов на свойств, которые возвращаются в ответы веб-служб Exchange. 
  
### <a name="ews-response-shapes"></a>Фигур ответа веб-служб Exchange

Exchange хранится много информации об элементах. В некоторых случаях приложение может не все эти сведения, а во многих случаях рекомендуется не получите все. [Фигур ответа веб-служб Exchange](property-sets-and-response-shapes-in-ews-in-exchange.md), также называемых свойство фигур указывают свойств, которые возвращаются из сервера. Элемент основной фигуры ответа — это базовый фигуры. Базовый фигура — контейнер предварительно свойств по умолчанию для строго типизированных элементов. Управляемый API EWS эквивалент базового фигуры является [BasePropertySet](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.basepropertyset%28v=exchg.80%29.aspx). Веб-служб Exchange включает в себя три фигуры ответа по умолчанию.
  
**В таблице 2. По умолчанию ответа фигур**

|**Имя формы ответа по умолчанию**|**Управляемый API EWS эквивалент**|**Описание**|
|:-----|:-----|:-----|
|IdOnly  <br/> |Значение BasePropertySet.IdOnly  <br/> |Возвращаются только идентификатор веб-служб Exchange и изменить ключ. Если клиент использует все свойства, возвращаемые фигуры AllProperties или по умолчанию, используйте фигуры IdOnly и задавать дополнительные свойства с помощью устанавливать класса **PropertySet** путь к свойству. Большинство приложений следует использовать фигуры IdOnly ответа с помощью дополнительных свойств, указанных. Это позволяет сократить объем запрашиваемых клиентами неиспользуемых данных.  <br/> |
|Значение по умолчанию  <br/> |Нет  <br/> |Набор стандартных свойств с типом элемента. Используйте этой фигуры ответа только в том случае, если приложение использует все свойства.  <br/> |
|AllProperties  <br/> |Значение BasePropertySet.FirstClassProperties  <br/> |Большим набором свойств чем фигуры по умолчанию. Несмотря на то, что названия его, этот параметр не возвращает все свойства элемента. Этот набор свойств возвращает свойства, которые наиболее часто используемых клиентских приложений. Если требуются дополнительные свойства, их можно запросить по пути свойства.  <br/> Если ваше приложение не использует всех свойств, возвращаемых с этой фигуры ответа, используйте фигуры ответа IdOnly с помощью дополнительных свойств, указанных.  <br/> |
   
Многие операции EWS возврата элементов и их свойства. Независимо от того, фигур ответа, которые можно указать разных операций можно вернуть наборы различных свойств. Различных типов элементов также получить различные свойства, в зависимости от операции и форма ответа указан. Следующие операции использование ответа фигур для идентификации свойств, которые необходимо вернуть.
  
**В таблице 3. Операции, использующие ответа фигур**

|**Операция служб EWS**|**Метод управляемого API EWS**|
|:-----|:-----|
|[GetConversationItems](http://msdn.microsoft.com/library/8ae00a99-b37b-4194-829c-fe300db6ab99%28Office.15%29.aspx) <br/> |[Метод ExchangeService.GetConversationItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.getconversationitems%28v=exchg.80%29.aspx) <br/> |
|[GetFolder](http://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) <br/> |[Метод Folder.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) <br/> |
|[GetItem](http://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) <br/> |[Метод Item.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) <br/> [Метод ExchangeService.BindToItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.bindtoitems%28v=exchg.80%29.aspx) <br/> |
|[FindConversation](http://msdn.microsoft.com/library/2384908a-c203-45b6-98aa-efd6a4c23aac%28Office.15%29.aspx) <br/> |[Метод ExchangeService.FindConversation](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.findconversation%28v=exchg.80%29.aspx) <br/> |
|[FindFolder](http://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx) <br/> |[Метод Folder.FindFolders](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.findfolders%28v=exchg.80%29.aspx) <br/> [Метод ExchangeService.FindFolders](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.findfolders%28v=exchg.80%29.aspx) <br/> |
|[FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) <br/> |[Метод Folder.FindItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.finditems%28v=exchg.80%29.aspx) <br/> [Метод ExchangeService.FindItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) <br/> |
|[FindPeople](http://msdn.microsoft.com/library/446106b7-ff2d-4107-90c1-29f4d38ba128%28Office.15%29.aspx) <br/> |Не реализован.  <br/> |
|[ResolveNames](http://msdn.microsoft.com/library/6b4eb4b3-9ad6-4804-a09f-7e20cfea4dbb%28Office.15%29.aspx) <br/> |[Метод ExchangeService.ResolveNames](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.resolvename%28v=exchg.80%29.aspx) <br/> |
|[SearchMailboxes](http://msdn.microsoft.com/library/8a67c1d8-d021-4e68-aa62-35f7d9c2edc7%28Office.15%29.aspx) <br/> |[Метод ExchangeService.SearchMailboxes](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.searchmailboxes%28v=exchg.80%29.aspx) <br/> [Метод ExchangeService.BeginSearchMailboxes](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.beginsearchmailboxes%28v=exchg.80%29.aspx) <br/> |
|[SyncFolderHierarchy](http://msdn.microsoft.com/library/b31916b1-bc6c-4451-a475-b7c5417f752d%28Office.15%29.aspx) <br/> |[Метод ExchangeService.SyncFolderHierarchy](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.syncfolderhierarchy%28v=exchg.80%29.aspx) <br/> |
|[SyncFolderItems](http://msdn.microsoft.com/library/7f0de089-8876-47ec-a871-df118ceae75d%28Office.15%29.aspx) <br/> |[Метод ExchangeService.SyncFolderItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.syncfolderitems%28v=exchg.80%29.aspx) <br/> |
   
Свойство фигуры являются одним элементарные способ определения свойств, которые будут приложения для возврата. В некоторых случаях однако приложению более качественных набор свойств. Для этого можно использовать путь к свойству.
  
### <a name="choose-properties-by-their-property-path"></a>Выберите пункт Свойства путем их свойства

Свойство путь к веб-служб Exchange — это метаданные, которые используются для определения свойства в запроса или ответа. 
  
**В таблице 4. Типы свойств путь**

|**Тип свойства пути**|**Тип схемы**|**Управляемый API EWS реализации**|**Описание**|
|:-----|:-----|:-----|:-----|
|FieldUri  <br/> |PathToUnindexedFieldType  <br/> |Типы, наследующие от [ServiceObjectSchema](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.serviceobjectschema%28v=exchg.80%29.aspx).  <br/> |Наиболее распространенные путь к свойству. Пути свойств FieldUri заданы для объекта **PropertySet** в управляемый API веб-служб Exchange. Большая часть свойств веб-служб Exchange можно задать с путь к свойству FieldUri. Описывается UnindexedFieldURIType в схеме веб-служб Exchange.  <br/> Путь к свойству FieldUri XML выглядит следующим образом:  <br/> ```XML<FieldURI FieldURI="item:Subject"/>```Этот путь свойство эквивалентно ItemSchema.Subject в управляемый API веб-служб Exchange.  <br/> |
|IndexedFieldUri  <br/> |PathToIndexedFieldType  <br/> |Типы, наследующие от [ItemSchema](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.itemschema%28v=exchg.80%29.aspx).  <br/> |Задает свойства словаря, которым требуется индекс свойства, чтобы указать значение, возвращаемое. Используйте этот путь, если свойство может иметь более одного значения. Описывается **DictionaryURIType** свойства в схеме веб-служб Exchange. Пути свойств **DictionaryURIType** заданы для объекта **PropertySet** в управляемый API веб-служб Exchange.  <br/> Путь к свойству IndexedFieldUri XML выглядит следующим образом:  <br/> ```XML<IndexedFieldURI FieldURI="contacts:PhysicalAddress:Street FieldIndex="Home"/>```|
|ExtendedFieldUri  <br/> |PathToExtendedFieldType  <br/> |[ExtendedPropertyDefinition](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.extendedpropertydefinition%28v=exchg.80%29.aspx) <br/> |Идентифицирует определения расширенных свойств, который определяет пользовательские или не Схематизированный свойств элементов.  <br/> Путь к свойству ExtendedFieldUri XML выглядит следующим образом:  <br/> ```XML<ExtendedFieldURI> PropertyTag="0x1234" PropertyType="Integer" />```|
|ExceptionFieldUri  <br/> |ExceptionFieldURI  <br/> |[ServiceResponse](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.serviceresponse%28v=exchg.80%29.aspx) <br/> |Задает свойства, связанные с сообщением об ошибке в ответа на веб-служб Exchange. Описывается тип **ExceptionPropertyURIType** в схеме веб-служб Exchange. Это происходит только в элементе **MessageXml** сообщений об ошибках, возникающих при работе с шаблоны повторения календаря.  <br/> |
   
Рекомендуется при запросе свойства, используйте базовый фигуры IdOnly ([BasePropertySet.IdOnly](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.basepropertyset%28v=exchg.80%29.aspx) в управляемый API EWS) и запросите только свойства, приложению путем указания пути свойств. 
  
### <a name="schematized-properties"></a>Схематизированный свойства

Большая часть свойств, которые требуется клиент веб-служб Exchange, описаны в схеме, веб-служб Exchange. Основную папку и определения типов элементов, которые содержат определения свойств, находятся в схеме types.xsd. Следующие типы схемы содержат определения свойств для большинства объектов, которые можно использовать.
  
**В таблице 5. Типы схемы, которые содержат определения свойств**

|**Тип схемы веб-служб Exchange**|**Управляемый API EWS тип эквивалент**|**Определяет...**|
|:-----|:-----|:-----|
|**ItemType** <br/> |[Класс элемента](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item%28v=exchg.80%29.aspx) <br/> |Набор свойств типа базового элемента. Этот тип может быть создан с помощью клиента, но никогда не возвращается по Exchange. Exchange возвращает объект MessageType для всех универсальных объектов.  <br/> |
|**MessageType** <br/> |[Класс EmailMessage](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage%28v=exchg.80%29.aspx) <br/> |Набор свойств объекта сообщения электронной почты и свойства для всех универсальных объектов.  <br/> |
|**CalendarItemType** <br/> |[Класс встречи](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) <br/> |Установка свойств элемента календаря; Этот компонент включает одиночные и повторяющихся встреч.  <br/> |
|**ContactItemType** <br/> |[Обратитесь в класс](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.contact%28v=exchg.80%29.aspx) <br/> |Набор свойств элемента контакта.  <br/> |
|**DistributionListType** <br/> |[Класс ContactGroup](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.contactgroup%28v=exchg.80%29.aspx) <br/> |Набор свойств списка рассылки.  <br/> |
|**MeetingMessageType** <br/> |[Класс MeetingMessage](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.meetingmessage%28v=exchg.80%29.aspx) <br/> |Задайте свойство type сообщения на собрания.  <br/> |
|**MeetingRequestMessageType** <br/> |[Класс MeetingRequest](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.meetingrequest%28v=exchg.80%29.aspx) <br/> |Задайте свойство type запрос на собрание.  <br/> |
|**MeetingResponseMessageType** <br/> |[Класс MeetingResponse](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.meetingresponse%28v=exchg.80%29.aspx) <br/> |Задать свойство тип ответа на собрания.  <br/> |
|**MeetingCancellationMessageType** <br/> |[Класс MeetingCancellation](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.meetingcancellation%28v=exchg.80%29.aspx) <br/> |Задайте свойство type отмены собрания.  <br/> |
|**Тип задачи** <br/> |[Класс задач](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.task%28v=exchg.80%29.aspx) <br/> |Задать свойство типа задачи.  <br/> |
|**PostItemType** <br/> |[Класс postItem](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.postitem%28v=exchg.80%29.aspx) <br/> |Набор свойств, postitem типа.  <br/> |
|**FolderType** <br/> |[Класс папки](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder%28v=exchg.80%29.aspx) <br/> |Набор свойств типа папки.  <br/> |
|**CalendarFolderType** <br/> |[Класс CalendarFolder](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.calendarfolder%28v=exchg.80%29.aspx) <br/> |Набор свойств типа SearchFolder.  <br/> |
|**ContactsFolderType** <br/> |[Класс ContactsFolder](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.contactsfolder%28v=exchg.80%29.aspx) <br/> |Набор свойств типа ContactsFolder.  <br/> |
|**SearchFolderType** <br/> |[Класс SearchFolder](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.searchfolder%28v=exchg.80%29.aspx) <br/> |Набор свойств типа SearchFolder.  <br/> |
|**TasksFolderType** <br/> |[Класс TasksFolder](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.tasksfolder%28v=exchg.80%29.aspx) <br/> |Набор свойств типа TasksFolder.  <br/> |
|**UserConfigurationType** <br/> |[Класс UserConfiguration](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.userconfiguration%28v=exchg.80%29.aspx) <br/> |Набор свойств типа UserConfiguration.  <br/> |
   
Хотя для свойств в схеме веб-служб Exchange достаточно для многих приложений, не может реализовать некоторые сценарии с помощью только что описанных в этой схеме. Для этих сценариев можно расширенные свойства. 
  
### <a name="extended-properties-aka-non-schematized-properties"></a>Расширенные свойства (также называемого-Схематизированный)

Расширенные свойства позволяют создавать настраиваемые свойства, которые обеспечивают доступ к свойствам элементов и папок в хранилище Exchange, которые не определены в схеме веб-служб Exchange. Их можно использовать для доступа к собственный MAPI папки и элемента свойства в базе данных Exchange. Расширенные свойства можно использовать для доступа к Схематизированный свойства, поскольку на внутреннем этих Схематизированный свойства — это не более чем свойства MAPI в базе данных Exchange. 
  
Тип PathToExtendedFieldType схемы в схеме types.xsd определяет XML, представляющий расширенные свойства. Этот тип схемы определяет элемент [ExtendedFieldURI](http://msdn.microsoft.com/library/b3c6ea3a-9ead-44b9-9d99-64ecf12bde23%28Office.15%29.aspx) в экземпляры XML; Другими словами он определяет XML-данные, пересылаемые между службы и клиента. Тип схемы ExtendedPropertyType определяет, как элемент [ExtendedFieldURI](http://msdn.microsoft.com/library/b3c6ea3a-9ead-44b9-9d99-64ecf12bde23%28Office.15%29.aspx) и значение или массив значений, которые содержит расширенные свойства. Ниже указаны приблизительно, например сопоставление расширенные свойства XML и реализации на элементы в управляемый API веб-служб Exchange. 
  
**В таблице 6. Расширенные свойства XML, реализованные в управляемый API веб-служб Exchange**

|**Управляемый API EWS реализации**|**Он содержит**|**Сопоставляет с**|
|:-----|:-----|:-----|
|[Свойство Item.ExtendedProperties](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.extendedproperties%28v=exchg.80%29.aspx) <br/> |Коллекция расширенные свойства элемента.  <br/> |Один или несколько экземпляров расширенные свойства элемента.  <br/> |
|[Класс ExtendedProperty](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.extendedproperty%28v=exchg.80%29.aspx) <br/> |Определение расширенные свойства и значения.  <br/> |Тип схемы ExtendedPropertyType.  <br/> |
|[Класс ExtendedPropertyDefinition](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.extendedpropertydefinition%28v=exchg.80%29.aspx) <br/> |Определение расширенных свойств.  <br/> |Тип схемы PathToExtendedFieldType.  <br/> |
   
Если требуется для получения дополнительных сведений об использовании расширенных свойств в приложении, можно изучить следующие примеры кода: 
  
- [Mfcmapi (en)](http://mfcmapi.codeplex.com/)
    
- [Exchange 2013: Подготовка пользовательских X-заголовков программными средствами](http://code.msdn.microsoft.com/exchange/Exchange-2013-Provision-d4ef5719)
    
- [Exchange 2013: Доступ к свойству, его свойство tag](http://code.msdn.microsoft.com/exchange/Exchange-2013-Access-a-719875ac)
    
- [Exchange 2013: Доступ к именованное свойство по идентификатору](http://code.msdn.microsoft.com/exchange/Exchange-2013-Access-a-02dbe22f)
    
- [Exchange 2013: Доступ к именованное свойство по имени](http://code.msdn.microsoft.com/exchange/Exchange-2013-Access-a-6556e183)
    
- [Exchange 2013: Доступ к идентификатор GUID набора свойств, свойств и имя](http://code.msdn.microsoft.com/exchange/Exchange-2013-Access-a-4021f971)
    
- [Exchange 2013: Создание настраиваемых расширенные свойства программными средствами](http://code.msdn.microsoft.com/exchange/Exchange-2013-Create-314db25a)
    
## <a name="in-this-section"></a>В этом разделе
<a name="bk_inthissection"> </a>

- [Подготовка к работе x заголовков с помощью веб-служб Exchange в Exchange](how-to-provision-x-headers-by-using-ews-in-exchange.md)
    
- [Ошибки, связанные с свойство веб-служб Exchange](ews-property-related-errors.md)
    
## <a name="see-also"></a>См. также


- [Начать работу с использованием веб-служб Exchange](start-using-web-services-in-exchange.md)
    
- [Mfcmapi (en)](http://mfcmapi.codeplex.com/)
    

