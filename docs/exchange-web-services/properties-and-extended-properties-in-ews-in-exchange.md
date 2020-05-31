---
title: Свойства и расширенные свойства в веб-службах Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 68623048-060e-4602-b3fa-62617a94cf72
description: Узнайте, как можно определять свойства элементов и папок и получать к ним доступ с помощью EWS в Exchange.
ms.openlocfilehash: 0c01d9bd21cbef0a3536c8dbd85e192199b7b8ab
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761240"
---
# <a name="properties-and-extended-properties-in-ews-in-exchange"></a>Свойства и расширенные свойства в веб-службах Exchange

Узнайте, как можно определять свойства элементов и папок и получать к ним доступ с помощью EWS в Exchange.
  
Почтовый ящик Exchange содержит большое количество элементов, включая сообщения электронной почты, встречи, собрания и т. д. Эти элементы состоят из свойств; свойства описывают элементы. Свойства элемента можно использовать для выполнения [поиска](search-and-ews-in-exchange.md), [синхронизации изменений элементов](mailbox-synchronization-and-ews-in-exchange.md)и [создания пользовательских типов свойств](http://code.msdn.microsoft.com/exchange/Exchange-2013-Create-314db25a). В этой статье приводятся общие сведения о свойствах и способах работы со свойствами в приложении.
  
## <a name="exchange-item-properties"></a>Свойства элемента Exchange
<a name="ItemsAreProperties"> </a>

Элементы и папки в Exchange по сути являются строками в таблицах. Свойство Main, идентифицирующее элемент или папку, является [идентификатором EWS](ews-identifiers-in-exchange.md). Несмотря на то что в базе данных Exchange есть другие свойства, связанные с идентификатором, идентификатор EWS выступает в качестве первичного ключа для коллекции свойств, описывающих элемент. Свойство идентификатора EWS состоит из двух частей:
  
- Свойство [ItemId](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) или [FolderId](http://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx) , идентифицирующее элемент 
    
- Свойство **чанжекэй** , содержащее сведения о состоянии изменения элемента или папки 
    
Все элементы в почтовом ящике хранятся в одной и той же базе данных Exchange и используют одну и ту же схему базы данных. Элементы различаются с помощью комбинации свойства [ItemClass](http://msdn.microsoft.com/library/56020078-50b4-4880-894a-a9f234033cfb%28Office.15%29.aspx) , ограничений свойств и уровней бизнес-логики, которые влияют на то, как они управляются в хранилище Exchange. В таблице 1 показано, как свойства применяются к различным типам элементов; в этом примере элементы электронной почты и встречи. Оба элемента имеют значение для свойства [subject](http://msdn.microsoft.com/library/c140d6c2-deb1-4f67-a908-9397197c4ae7%28Office.15%29.aspx) . Обратите внимание, что для элемента электронной почты не задано свойство [исаллдайевент](http://msdn.microsoft.com/library/29140a64-9d7a-4a14-a10d-c98197c9831b%28Office.15%29.aspx) , а для встречи не задано свойство **исреадрецеиптрекуестед** . К счастью, вам не нужно знать, какие свойства применяются к каждому классу Item; Эта проблема обрабатывается EWS. 
  
**Таблица 1. Сравнение свойств встречи и электронной почты**

|**Тип элемента**|**Класс элемента**|**Тема**|**исаллдайевент**|**исреадрецеиптрекуестед**|
|:-----|:-----|:-----|:-----|:-----|
|Электронная почта  <br/> |IPM.Note  <br/> |Отчет о состоянии: завершено для проекта X  <br/> |ОПРЕДЕЛЕН  <br/> |true  <br/> |
|Appointment  <br/> |IPM.Appointment  <br/> |Собрание компании Contoso  <br/> |false  <br/> |ОПРЕДЕЛЕН  <br/> |
   
Схема EWS поддерживает многие ограничения, управляемые базой данных Exchange и уровнями бизнес-логики между EWS и базой данных Exchange. Схема EWS применяет определенный набор свойств к каждому типу элемента. Ниже приведены строго типизированные элементы базы данных Exchange, предоставляемые EWS: 
  
- Сообщения электронной почты.
    
- Встречи
    
- Контакты
    
- Списки рассылки
    
- Сообщения о собрании
    
- Приглашения на собрания
    
- Ответы на приглашения на собрания
    
- Отмены собраний
    
- Задачи
    
- Размещение элементов
    
Стандартные элементы возвращаются в службах EWS как сообщения электронной почты. Управляемый API EWS реализует все эти типы элементов.
  
> [!NOTE]
> Объекты ответа отправляются клиентом на сервер в ответ на элементы, полученные от других пользователей. Они не существуют в базе данных Exchange. 
  
## <a name="what-are-properties-in-ews"></a>Что такое свойства в EWS?
<a name="WhatAreEWSProperties"> </a>

Схема EWS описывает данные, которые передаются между клиентом EWS и Exchange. Большая часть схемы описывает свойства элементов и папок, к которым можно получить доступ в базе данных Exchange. Схема EWS описывает XML-представление свойств базы данных Exchange, доступных вашему приложению. Фактические свойства, в зависимости от того, какие свойства доступны, какие формы они выполняют и какие значения они возвращают, зависят от того, что вы пытались выполнить. Например, свойство **Body** будет возвращать только первые 512 символов в операции **FindItem** , но операция **GetItem** возвращает весь текст элемента. Несмотря на то, что большинство свойств являются устанавливаемыми и доступны для извлечения, некоторые свойства задаются только Exchange. Каждое свойство существует в схеме в формате XML, которое отражает свойство в том виде, в котором оно хранится в базе данных Exchange, или вычисляется на основе свойств, хранящихся в базе данных Exchange. Свойство **subject** является примером настраиваемого свойства; Свойство **унреадкаунт** папки — это пример вычисляемого свойства. Основной набор свойств, распространенных для основных типов элементов. 
  
Следующие факторы определяют набор свойств, который приложение получает от Exchange: 
  
- Операция, с которой вызывается приложение
    
- Базовая фигура ответа
    
- Тип элемента
    
- Пути к указанным свойствам
    
Важно понимать, как эти разные факторы влияют на данные, к которым вы можете получить доступ. Как и в примере упомянутого выше свойства **Body** , некоторые сведения являются условно доступными в зависимости от различных факторов. Понимание этих факторов может сэкономить время, помогая выбрать правильные параметры для доступа к нужной информации. Чтобы узнать, какие свойства доступны, необходимо протестировать эти факторы, чтобы определить, как получить доступ к свойствам, необходимым приложению. В этом разделе описывается, как эти факторы влияют на то, какие свойства возвращаются в ответах EWS. 
  
### <a name="ews-response-shapes"></a>Фигуры ответа EWS

В Exchange хранится множество сведений об элементах. Иногда приложению не нужны все эти сведения, и во многих случаях лучше всего не получать его все. [Фигуры ответа EWS](property-sets-and-response-shapes-in-ews-in-exchange.md), также называемые фигурами свойств, указывают, какие свойства возвращаются с сервера. Основным элементом фигуры ответа является базовая фигура. Базовая фигура — это заданный по умолчанию набор свойств для строго типизированных элементов. Управляемый API EWS эквивалентом базовой фигуры является [басепропертисет](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.basepropertyset%28v=exchg.80%29.aspx). EWS включает три стандартные фигуры ответа.
  
**Таблица 2. Фигуры ответа по умолчанию**

|**Имя фигуры ответа по умолчанию**|**Эквивалент управляемого API EWS**|**Описание**|
|:-----|:-----|:-----|
|идонли  <br/> |Значение Басепропертисет. Идонли  <br/> |Возвращаются только идентификатор и ключ изменения EWS. Если клиент не использует все свойства, возвращенные формой Аллпропертиес или формой по умолчанию, используйте фигуру Идонли и укажите дополнительные свойства, используя путь к свойству, заданный для класса набора **свойств** . Большинство приложений должны использовать фигуру ответа Идонли с указанием дополнительных свойств. Это сокращает количество неиспользуемых данных, запрашиваемых клиентами.  <br/> |
|По умолчанию  <br/> |Н/Д  <br/> |Набор стандартных свойств для типа элемента. Эту фигуру ответа следует использовать только в том случае, если приложение использует все свойства.  <br/> |
|аллпропертиес  <br/> |Значение Басепропертисет. Фирсткласспропертиес  <br/> |Более крупный набор свойств, чем фигура по умолчанию. Несмотря на то, что это имя предполагается, этот параметр не возвращает все свойства элемента. Это свойство Set возвращает свойства, которые используются клиентскими приложениями чаще. Если требуются дополнительные свойства, их можно запросить по пути к свойству.  <br/> Если ваше приложение не использует все свойства, возвращенные с этой фигурой ответа, используйте фигуру ответа Идонли с дополнительными свойствами.  <br/> |
   
Многие операции, возвращающие службы EWS, возвращают элементы и их свойства. Независимо от указанных фигур ответа различные операции могут возвращать разные наборы свойств. Различные типы элементов также возвращают различные свойства, в зависимости от операции и указанной формы ответа. Следующие операции используют фигуры ответа для определения возвращаемых свойств.
  
**Таблица 3. Операции, использующие фигуры ответа**

|**Операция служб EWS**|**Метод управляемого API EWS**|
|:-----|:-----|
|[GetConversationItems](http://msdn.microsoft.com/library/8ae00a99-b37b-4194-829c-fe300db6ab99%28Office.15%29.aspx) <br/> |[Метод ExchangeService. GetConversationItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.getconversationitems%28v=exchg.80%29.aspx) <br/> |
|[GetFolder](http://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) <br/> |[Метод Folder. Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) <br/> |
|[GetItem](http://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) <br/> |[Метод Item. Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) <br/> [Метод ExchangeService. Биндтоитемс](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.bindtoitems%28v=exchg.80%29.aspx) <br/> |
|[FindConversation](http://msdn.microsoft.com/library/2384908a-c203-45b6-98aa-efd6a4c23aac%28Office.15%29.aspx) <br/> |[Метод ExchangeService. FindConversation](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.findconversation%28v=exchg.80%29.aspx) <br/> |
|[FindFolder](http://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx) <br/> |[Метод Folder. Финдфолдерс](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.findfolders%28v=exchg.80%29.aspx) <br/> [Метод ExchangeService. Финдфолдерс](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.findfolders%28v=exchg.80%29.aspx) <br/> |
|[FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) <br/> |[Метод Folder. FindItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.finditems%28v=exchg.80%29.aspx) <br/> [Метод ExchangeService. FindItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) <br/> |
|[FindPeople](http://msdn.microsoft.com/library/446106b7-ff2d-4107-90c1-29f4d38ba128%28Office.15%29.aspx) <br/> |Не реализовано.  <br/> |
|[ResolveNames](http://msdn.microsoft.com/library/6b4eb4b3-9ad6-4804-a09f-7e20cfea4dbb%28Office.15%29.aspx) <br/> |[Метод ExchangeService. ResolveNames](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.resolvename%28v=exchg.80%29.aspx) <br/> |
|[SearchMailboxes](http://msdn.microsoft.com/library/8a67c1d8-d021-4e68-aa62-35f7d9c2edc7%28Office.15%29.aspx) <br/> |[Метод ExchangeService. SearchMailboxes](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.searchmailboxes%28v=exchg.80%29.aspx) <br/> [Метод ExchangeService. Бегинсеарчмаилбоксес](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.beginsearchmailboxes%28v=exchg.80%29.aspx) <br/> |
|[SyncFolderHierarchy](http://msdn.microsoft.com/library/b31916b1-bc6c-4451-a475-b7c5417f752d%28Office.15%29.aspx) <br/> |[Метод ExchangeService. SyncFolderHierarchy](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.syncfolderhierarchy%28v=exchg.80%29.aspx) <br/> |
|[SyncFolderItems](http://msdn.microsoft.com/library/7f0de089-8876-47ec-a871-df118ceae75d%28Office.15%29.aspx) <br/> |[Метод ExchangeService. SyncFolderItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.syncfolderitems%28v=exchg.80%29.aspx) <br/> |
   
Фигуры свойств — это один, элементарный способ определения свойств, которые должно возвращать приложение. Однако иногда приложению требуется более детальный набор определенных свойств. Для этого можно использовать путь к свойству.
  
### <a name="choose-properties-by-their-property-path"></a>Выбор свойств по пути к свойствам

Путь к свойству EWS — это метаданные, которые используются для идентификации свойств в запросе или ответе. 
  
**Таблица 4. Типы путей к свойствам**

|**Тип пути свойства**|**Тип схемы**|**Реализация управляемого API EWS**|**Описание**|
|:-----|:-----|:-----|:-----|
|фиелдури  <br/> |пастауниндекседфиелдтипе  <br/> |Типы, которые наследуются от [сервицеобжектсчема](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.serviceobjectschema%28v=exchg.80%29.aspx).  <br/> |Наиболее распространенный путь свойства. Пути к свойствам Фиелдури указаны для объекта набор **свойств** в УПРАВЛЯЕМОМ API EWS. Большинство свойств EWS можно задать с помощью пути к свойству Фиелдури. Это описывается в Униндекседфиелдуритипе в схеме EWS.  <br/> XML-код пути свойства Фиелдури выглядит следующим образом:  <br/> ```XML<FieldURI FieldURI="item:Subject"/>```Этот путь свойства эквивалентен Итемсчема. subject в управляемом API EWS.  <br/> |
|индекседфиелдури  <br/> |пастоиндекседфиелдтипе  <br/> |Типы, которые наследуются от [итемсчема](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.itemschema%28v=exchg.80%29.aspx).  <br/> |Определяет свойства словаря, для которых требуется индекс свойства, чтобы указать возвращаемое значение. Используйте этот путь, если свойство может иметь более одного значения. Это описывается свойством **диктионарюритипе** в схеме EWS. Пути к свойствам **диктионарюритипе** указаны для объекта набор **свойств** в управляемом API EWS.  <br/> XML-код пути свойства Индекседфиелдури выглядит следующим образом:  <br/> ```XML<IndexedFieldURI FieldURI="contacts:PhysicalAddress:Street FieldIndex="Home"/>```|
|екстендедфиелдури  <br/> |пастоекстендедфиелдтипе  <br/> |[екстендедпропертидефинитион](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.extendedpropertydefinition%28v=exchg.80%29.aspx) <br/> |Определяет определение расширенного свойства, которое определяет настраиваемые свойства или свойства, не относящиеся к схематизированные, для элементов.  <br/> XML-код пути свойства Екстендедфиелдури выглядит следующим образом:  <br/> ```XML<ExtendedFieldURI> PropertyTag="0x1234" PropertyType="Integer" />```|
|ексцептионфиелдури  <br/> |ексцептионфиелдури  <br/> |[сервицереспонсе](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.serviceresponse%28v=exchg.80%29.aspx) <br/> |Задает свойства, связанные с ошибкой в отклике EWS. Это описывается типом **ексцептионпропертюритипе** в схеме EWS. Это происходит только в элементе **мессажексмл** откликов об ошибках, возникающих при работе с расписаниями повторения календаря.  <br/> |
   
При запросе свойств рекомендуется использовать базовую фигуру Идонли ([басепропертисет. идонли](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.basepropertyset%28v=exchg.80%29.aspx) в УПРАВЛЯЕМОМ API EWS), а затем запросить только те свойства, которые требуются приложению, указав пути свойств. 
  
### <a name="schematized-properties"></a>Свойства схематизированные

Большинство свойств, необходимых для клиента EWS, описаны в схеме EWS. Определения основных папок и типов элементов, содержащие определения свойств, находятся в схеме Types. xsd. В следующих типах схемы содержатся определения свойств для большинства объектов, которые можно использовать.
  
**Таблица 5. Типы схемы, содержащие определения свойств**

|**Тип схемы EWS**|**Эквивалент типа управляемого API EWS**|**Определяет...**|
|:-----|:-----|:-----|
|**ItemType** <br/> |[Класс элемента](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item%28v=exchg.80%29.aspx) <br/> |Набор свойств базового типа элемента. Этот тип можно создать из клиента, но никогда не возвращается сервером Exchange. Exchange возвращает объект MessageType для всех универсальных объектов.  <br/> |
|**MessageType** <br/> |[Класс EmailMessage](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage%28v=exchg.80%29.aspx) <br/> |Набор свойств объекта сообщения электронной почты и свойство, заданное для всех универсальных объектов.  <br/> |
|**календаритемтипе** <br/> |[Класс встречи](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) <br/> |Набор свойств элемента календаря; Сюда входят отдельные и повторяющиеся встречи.  <br/> |
|**контактитемтипе** <br/> |[Класс контакта](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.contact%28v=exchg.80%29.aspx) <br/> |Набор свойств элемента контакта.  <br/> |
|**дистрибутионлисттипе** <br/> |[Класс ContactGroup](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.contactgroup%28v=exchg.80%29.aspx) <br/> |Набор свойств личного списка рассылки.  <br/> |
|**митингмессажетипе** <br/> |[Класс Митингмессаже](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.meetingmessage%28v=exchg.80%29.aspx) <br/> |Набор свойств типа сообщения о собрании.  <br/> |
|**митингрекуестмессажетипе** <br/> |[Класс свойство meetingrequest](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.meetingrequest%28v=exchg.80%29.aspx) <br/> |Набор свойств типа приглашения на собрание.  <br/> |
|**митингреспонсемессажетипе** <br/> |[Класс Митингреспонсе](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.meetingresponse%28v=exchg.80%29.aspx) <br/> |Набор свойств типа ответа на собрание.  <br/> |
|**митингканцеллатионмессажетипе** <br/> |[Класс Митингканцеллатион](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.meetingcancellation%28v=exchg.80%29.aspx) <br/> |Свойство типа отмены собрания задано.  <br/> |
|**тасктипе** <br/> |[Класс Task](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.task%28v=exchg.80%29.aspx) <br/> |Набор свойств типа задачи.  <br/> |
|**Неitemtype** <br/> |[Класс элемента списка](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.postitem%28v=exchg.80%29.aspx) <br/> |Набор свойств "тип элемента".  <br/> |
|**фолдертипе** <br/> |[Класс Folder](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder%28v=exchg.80%29.aspx) <br/> |Набор свойств типа папки.  <br/> |
|**календарфолдертипе** <br/> |[Класс Календарфолдер](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.calendarfolder%28v=exchg.80%29.aspx) <br/> |Набор свойств типа SearchFolder.  <br/> |
|**контактсфолдертипе** <br/> |[Класс Контактсфолдер](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.contactsfolder%28v=exchg.80%29.aspx) <br/> |Набор свойств типа Контактсфолдер.  <br/> |
|**сеарчфолдертипе** <br/> |[Класс SearchFolder](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.searchfolder%28v=exchg.80%29.aspx) <br/> |Набор свойств типа SearchFolder.  <br/> |
|**тасксфолдертипе** <br/> |[Класс Тасксфолдер](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.tasksfolder%28v=exchg.80%29.aspx) <br/> |Набор свойств типа Тасксфолдер.  <br/> |
|**усерконфигуратионтипе** <br/> |[Класс Усерконфигуратион](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.userconfiguration%28v=exchg.80%29.aspx) <br/> |Набор свойств типа Усерконфигуратион.  <br/> |
   
Несмотря на то, что свойства в схеме EWS достаточны для многих приложений, невозможно реализовать некоторые сценарии, используя только то, что описывается в схеме. В этих сценариях можно расширять свойства. 
  
### <a name="extended-properties-aka-non-schematized-properties"></a>Расширенные свойства (или свойства, отличные от схематизированные)

Расширенные свойства позволяют создавать настраиваемые свойства, которые предоставляют доступ к свойствам элементов и папок в хранилище Exchange, которые не определены в схеме EWS. Их можно использовать для доступа к встроенным свойствам элементов и папок MAPI в базе данных Exchange. С помощью расширенных свойств можно получить доступ ко всем свойствам схематизированные, так как в этом случае свойства схематизированные не являются свойствами MAPI в базе данных Exchange. 
  
Тип схемы Пастоекстендедфиелдтипе, расположенный в схеме Types. xsd, определяет XML, представляющий расширенное свойство. Этот тип схемы определяет элемент [екстендедфиелдури](http://msdn.microsoft.com/library/b3c6ea3a-9ead-44b9-9d99-64ecf12bde23%28Office.15%29.aspx) в экземплярах XML; другими словами, он определяет XML-код, который передается между службой и клиентом. Тип схемы Екстендедпропертитипе определяет как элемент [екстендедфиелдури](http://msdn.microsoft.com/library/b3c6ea3a-9ead-44b9-9d99-64ecf12bde23%28Office.15%29.aspx) , так и значение или массив значений, содержащихся в расширенном свойстве. В приведенной ниже таблице показано приближенное сопоставление XML-кода расширенного свойства и его реализации для элементов в управляемом API EWS. 
  
**Таблица 6. Расширенное свойство XML в соответствии с реализацией в управляемом API EWS**

|**Реализация управляемого API EWS**|**Сведения, которые он содержит**|**Сведения, с которыми он сопоставлен**|
|:-----|:-----|:-----|
|[Свойство Item. Екстендедпропертиес](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.extendedproperties%28v=exchg.80%29.aspx) <br/> |Коллекция расширенных свойств элемента.  <br/> |Один или несколько экземпляров расширенных свойств элемента.  <br/> |
|[Класс ExtendedProperty](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.extendedproperty%28v=exchg.80%29.aspx) <br/> |Определение и значения расширенного свойства.  <br/> |Тип схемы Екстендедпропертитипе.  <br/> |
|[Класс Екстендедпропертидефинитион](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.extendedpropertydefinition%28v=exchg.80%29.aspx) <br/> |Определение расширенного свойства.  <br/> |Тип схемы Пастоекстендедфиелдтипе.  <br/> |
   
Если вы хотите узнать больше о том, как использовать расширенные свойства в вашем приложении, вы можете изучить следующие примеры кода: 
  
- [MFCMapi](http://mfcmapi.codeplex.com/)
    
- [Exchange 2013: подготовка настраиваемых X – заголовков программным способом](http://code.msdn.microsoft.com/exchange/Exchange-2013-Provision-d4ef5719)
    
- [Exchange 2013: доступ к свойству по тегу свойства](http://code.msdn.microsoft.com/exchange/Exchange-2013-Access-a-719875ac)
    
- [Exchange 2013: доступ к именованному свойству по его идентификатору](http://code.msdn.microsoft.com/exchange/Exchange-2013-Access-a-02dbe22f)
    
- [Exchange 2013: доступ к именованному свойству по его имени](http://code.msdn.microsoft.com/exchange/Exchange-2013-Access-a-6556e183)
    
- [Exchange 2013: доступ к свойству с помощью идентификатора GUID и имени набора свойств](http://code.msdn.microsoft.com/exchange/Exchange-2013-Access-a-4021f971)
    
- [Exchange 2013: создание настраиваемых расширенных свойств программным способом](http://code.msdn.microsoft.com/exchange/Exchange-2013-Create-314db25a)
    
## <a name="in-this-section"></a>В этом разделе:
<a name="bk_inthissection"> </a>

- [Подготовка заголовков x с помощью EWS в Exchange](how-to-provision-x-headers-by-using-ews-in-exchange.md)
    
- [Ошибки, связанные со свойством EWS](ews-property-related-errors.md)
    
## <a name="see-also"></a>См. также


- [Начало работы с веб-службами Exchange](start-using-web-services-in-exchange.md)
    
- [MFCMapi](http://mfcmapi.codeplex.com/)
    

