---
title: Наборы свойств и формы ответа в веб-службах Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 04a29804-6067-48e7-9f5c-534e253a230e
description: Сведения об управлении формами ответа и наборами свойств, которые возвращаются управляемым API EWS и EWS в Exchange.
ms.openlocfilehash: d9fd6c155438dfd03cfc9536397316cf3faa2287
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761257"
---
# <a name="property-sets-and-response-shapes-in-ews-in-exchange"></a>Наборы свойств и формы ответа в веб-службах Exchange

Сведения об управлении формами ответа и наборами свойств, которые возвращаются управляемым API EWS и EWS в Exchange.
  
Хранилище данных Exchange предоставляет гибкое решение для хранения, которое позволяет хранить в одной папке различные элементы, например контакты и записи календаря. Тем не менее, это может усложнить управление данными, возвращаемыми при вызове в операцию EWS или метод управляемого API EWS.
  
Для упрощения управления данными, возвращаемыми Exchange Online, Exchange Online в составе Office 365 или версией Екскаханже, начиная с Exchange 2013, управляемый API EWS использует наборы свойств, а EWS использует фигуры ответа. Это Предопределенные коллекции, которые предоставляют наиболее распространенные свойства элемента хранилища. Набор возвращаемых свойств определяется типом элемента. Это означает, что при привязке элемента с помощью метода [. Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) в управляемом API Exchange можно получить другой набор свойств в зависимости от типа элемента, с которым выполняется привязка. Привязка к элементу календаря возвратит другой набор свойств, чем привязку к элементу контакта. Аналогично, при использовании EWS [Операция GetItem](http://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) возвращает другой набор свойств на основе типа возвращаемого элемента. 
  
Привязка к папке с помощью метода [Folder. Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) или [операции-папки](http://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) также возвращает различные наборы свойств на основе запрашиваемой папки. 
  
**Таблица 1. Предварительно определенные фигуры ответа**

|**Фигура ответа**|**Эквивалент управляемого API EWS**|**Описание**|
|:-----|:-----|:-----|
|Только идентификатор  <br/> |[Басепропертисет. Идонли](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.basepropertyset%28v=exchg.80%29.aspx) <br/> |Возвращает только идентификатор элемента или папки. Большинство приложений должны использовать эту фигуру ответа и указывать необходимые дополнительные свойства.  <br/> |
|По умолчанию  <br/> |Н/Д  <br/> |Возвращает предопределенный набор свойств, используемых по умолчанию для элемента или папки (только для EWS).  <br/> |
|Все свойства  <br/> |[Басепропертисет. Фирсткласспропертиес](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.basepropertyset%28v=exchg.80%29.aspx) <br/> |Возвращает свойства, наиболее часто используемые клиентскими приложениями. Вы можете вернуть дополнительные свойства, используя путь к свойству.  <br/> |
   
## <a name="default-response-shapes"></a>Фигуры ответа по умолчанию

EWS включает набор стандартных форм ответа для папок и элементов. 
  
В приведенной ниже таблице перечислены свойства по умолчанию, которые возвращаются для каждой папки с помощью операций [FindFolder](http://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx) и [Folders](http://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) EWS. 
  
**Таблица 2. Свойства папки по умолчанию**

|**Свойство**|**Входящие**|**Календарь**|**Контакты**|**Удаленные элементы**|**"Черновики"**|**Примечания**|**Другие папки**|**Ходящие**|
|:-----|:-----|:-----|:-----|:-----|:-----|:-----|:-----|:-----|
|Различающееся имя (DN)  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |
|Идентификатор папки  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |
|Число вложенных папок  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |
|Общее количество  <br/> |X  <br/> ||X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |
|Количество непрочитанных  <br/> |X  <br/> |||X  <br/> |X  <br/> ||X  <br/> |X  <br/> |
   
В приведенной ниже таблице перечислены свойства по умолчанию, которые возвращаются для каждого типа элемента с помощью операций [FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) и [GetItem](http://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) EWS. 
  
**Таблица 3. Свойства элемента по умолчанию**

|**Свойство**|**Элемент календаря**|**Элемент "Контакт"**|**Элемент Message**|**Элемент "Задача"**|
|:-----|:-----|:-----|:-----|:-----|
|Основной текст  <br/> |||X (1)  <br/> ||
|календаритемтипе  <br/> ||x  <br/> |||
|CompanyName  <br/> ||x  <br/> |||
|комплетенаме  <br/> ||x  <br/> |||
|DateTimeCreated  <br/> |||x  <br/> ||
|датетимесент  <br/> |||x  <br/> ||
|Дата выполнения  <br/> ||||x (2)  <br/> |
|EmailAddresses  <br/> ||x  <br/> |||
|Конец  <br/> |x  <br/> ||||
|FileAs  <br/> ||x  <br/> |||
|From  <br/> |||x  <br/> ||
|HasAttachments  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|Адреса  <br/> ||x  <br/> |||
|Связанный  <br/> |x  <br/> ||x  <br/> ||
|исделиверирецеиптрекуестед  <br/> |||x  <br/> ||
|Идентификатор  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|JobTitle  <br/> ||x  <br/> |||
|легацифрибусистатус  <br/> |x  <br/> ||||
|Расположение  <br/> |x  <br/> ||||
|Организатор  <br/> |x  <br/> ||||
|PercentComplete  <br/> ||||x  <br/> |
|PhoneNumbers  <br/> ||x  <br/> |||
|фисикаладдрессес  <br/> ||x  <br/> |||
|респонсеобжектс  <br/> |x (1)  <br/> ||x (1)  <br/> ||
|сенситити  <br/> |||x  <br/> ||
|Размер  <br/> |||x  <br/> ||
|StartDate  <br/> ||||x (2)  <br/> |
|Состояние  <br/> ||||x  <br/> |
|Subject  <br/> |x  <br/> ||x  <br/> |x  <br/> |
   
Примечания.
  
1. Включается в ответ операции **GetItem** . Не включается в ответ операции **FindItem** . 
    
2. Включается в ответ только в том случае, если поле содержит данные. Не включается в ответ, если поле пустое.
    
### <a name="all-properties-set-and-response-shape"></a>Все наборы свойств и форма ответа

В следующей таблице перечислены свойства первого класса, возвращаемые при вызове элемента управляемого API EWS [. Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) и [Item. FindItems](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) , методы управляемого API EWS, а также фигура ответа "все свойства", возвращаемая операциями [FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) и [GetItem](http://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) EWS. 
  
Вы можете добавить дополнительные свойства в набор свойств или включить расширенные свойства. Дополнительные сведения см. в статье [Свойства и расширенные свойства в службах EWS в Exchange](properties-and-extended-properties-in-ews-in-exchange.md).
  
**Таблица 4. Свойства первого класса**

|||||||
|:-----|:-----|:-----|:-----|:-----|:-----|
|Свойство  <br/> |Элемент календаря  <br/> |Элемент "Контакт"  <br/> |Элемент Message  <br/> |Элемент POST  <br/> |Элемент "Задача"  <br/> |
|ActualWork  <br/> |||||x  <br/> |
|аджацентмитингкаунт  <br/> |x  <br/> |||||
|аджацентмитингс  <br/> |x  <br/> |||||
|Псевдоним  <br/> ||x  <br/> ||||
|алловневтимепропосал  <br/> |x  <br/> |||||
|аппоинтментреплитиме  <br/> |x  <br/> |||||
|аппоинтментсекуенценумбер  <br/> |x  <br/> |||||
|аппоинтментстате  <br/> |x  <br/> |||||
|ассигнедтиме  <br/> |||||x  <br/> |
|AssistantName  <br/> ||x  <br/> ||||
|BccRecipients  <br/> |||x  <br/> |||
|BillingInformation  <br/> |||||x  <br/> |
|Основной текст  <br/> |x (1)  <br/> |x (1)  <br/> |x (1)  <br/> ||x (1)  <br/> |
|BusinessHomePage  <br/> ||x  <br/> |x  <br/> |||
|календаритемтипе  <br/> |x  <br/> |||||
|Категории  <br/> |x  <br/> ||x  <br/> |x  <br/> |x  <br/> |
|CcRecipients  <br/> |||x  <br/> |||
|чанжекаунт  <br/> |||||x  <br/> |
|Дети  <br/> ||x  <br/> ||||
|Компании  <br/> |||||x  <br/> |
|комплетедате  <br/> |||||x  <br/> |
|комплетенаме  <br/> ||x  <br/> ||||
|конференцетипе  <br/> |x  <br/> |||||
|конфликтингмитингкаунт  <br/> |x  <br/> |||||
|конфликтингмитингс  <br/> |x  <br/> |||||
|Контакты  <br/> |||||x  <br/> |
|контактсаурце  <br/> ||x  <br/> ||||
|ConversationId  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|ConversationIndex  <br/> |||x  <br/> |x  <br/> ||
|ConversationTopic  <br/> |||x  <br/> |x  <br/> ||
|Culture  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|DateTimeCreated  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|DateTimeReceived  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|датетимесент  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|датетиместамп  <br/> |x  <br/> |||||
|DelegationState  <br/> |||||x  <br/> |
|Delegator  <br/> |||||x  <br/> |
|делетедоккуранцес  <br/> |x  <br/> |||||
|Отдел  <br/> ||x  <br/> ||||
|директорид  <br/> ||x  <br/> ||||
|DirectReports  <br/> ||x  <br/> ||||
|дисплайкк  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|DisplayName  <br/> ||x  <br/> ||||
|дисплайто  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|Дата выполнения  <br/> |||||x  <br/> |
|Длительность  <br/> |x  <br/> |||||
|еффективеригхтс  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|EmailAddresses  <br/> ||x  <br/> ||||
|Конец  <br/> |x  <br/> |||||
|EndTimeZone  <br/> |x  <br/> |||||
|FileAs  <br/> ||x  <br/> ||||
|филеасмаппинг  <br/> ||x  <br/> ||||
|фирстоккуранце  <br/> |x  <br/> |||||
|From  <br/> |||x  <br/> |x  <br/> ||
|Generation  <br/> ||x  <br/> ||||
|GivenName  <br/> ||x  <br/> ||||
|HasAttachments  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|HasPicture  <br/> ||x  <br/> ||||
|Адреса  <br/> ||x  <br/> ||||
|Важность  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|Инициалы  <br/> ||x  <br/> ||||
|инреплито  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|InternetMessageId  <br/> |||x  <br/> |x  <br/> ||
|InternetMessageHeaders  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|исаллдайевент  <br/> |x  <br/> |||||
|Связанный  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|С отменой  <br/> |x  <br/> |||||
|Выполнение  <br/> |||||x  <br/> |
|исделиверирецеиптрекуестед  <br/> |||x  <br/> |||
|Черновик  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|исфромме  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|"Собрание"  <br/> |x  <br/> |||||
|исонлинемитинг  <br/> |x  <br/> |||||
|IsRead  <br/> |||x  <br/> |||
|исреадрецеиптрекуестед  <br/> |||x  <br/> |||
|IsRecurring  <br/> |x  <br/> ||||x  <br/> |
|исресенд  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|исреспонсерекуестед  <br/> |x  <br/> ||x  <br/> |||
|Отправлено  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|исунмодифиед  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|ItemClass  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|Идентификатор  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|JobTitle  <br/> ||x  <br/> ||||
|ластмодифиеднаме  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|LastModifiedTime  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|ластоккурранце  <br/> |x  <br/> |||||
|легацифрибусистатус  <br/> |x  <br/> |||||
|Расположение  <br/> |x  <br/> |||||
|Директор  <br/> ||x  <br/> ||||
|митингрекуествассент  <br/> |x  <br/> |||||
|митингтимезоне  <br/> |x  <br/> |||||
|митингворкспацеурл  <br/> |x  <br/> |||||
|MiddleName  <br/> ||x  <br/> ||||
|Расстояние  <br/> ||x  <br/> |||x  <br/> |
|модифиедоккурранцес  <br/> |x  <br/> |||||
|миреспонсетипе  <br/> |x  <br/> |||||
|нетшовурл  <br/> |x  <br/> |||||
|NickName  <br/> ||x  <br/> ||||
|Примечания  <br/> ||x  <br/> ||||
|OfficeLocation  <br/> ||x  <br/> ||||
|OptionalAttendees  <br/> |x  <br/> |||||
|Организатор  <br/> |x  <br/> |||||
|оригиналстарт  <br/> |x  <br/> |||||
|Владелец  <br/> |||||x  <br/> |
|ParentFolderId  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|PercentComplete  <br/> |||||x  <br/> |
|PhoneNumbers  <br/> ||x  <br/> ||||
|фонетикфирстнаме  <br/> ||x  <br/> ||||
|фонетикфуллнаме  <br/> ||x  <br/> ||||
|фонетикластнаме  <br/> ||x  <br/> ||||
|Фотография  <br/> ||x  <br/> ||||
|фисикаладдрессес  <br/> ||x  <br/> ||||
|посталаддрессиндекс  <br/> ||x  <br/> ||||
|постедтиме  <br/> ||||x  <br/> ||
|Профессия  <br/> ||x  <br/> ||||
|рецеиведби  <br/> |||x  <br/> |||
|рецеиведрепресентинг  <br/> |||x  <br/> |||
|реккурренце  <br/> |x  <br/> ||||x  <br/> |
|Ссылки  <br/> |||x  <br/> |x  <br/> ||
|реминдердуеби  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|реминдериссет  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|ReminderMinutesBeforeStart  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|ReplyTo  <br/> |||x  <br/> |||
|RequiredAttendees  <br/> |x  <br/> |||||
|Ресурсы  <br/> |x  <br/> |||||
|респонсеобжектс  <br/> |x (1)  <br/> |x (1)  <br/> |x (1)  <br/> |x (1)  <br/> |x (1)  <br/> |
|Sender  <br/> |||x  <br/> |x  <br/> ||
|Конфиденциальность  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|Размер  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|спаусенаме  <br/> ||x  <br/> ||||
|Начало  <br/> |x  <br/> |||||
|StartDate  <br/> |||||x  <br/> |
|StartTimeZone  <br/> |x  <br/> |||||
|Состояние  <br/> |||||x  <br/> |
|статусдескриптион  <br/> |||||x  <br/> |
|Subject  <br/> |x  <br/> |x  <br/> |x  <br/> ||x  <br/> |
|ФИО  <br/> ||x  <br/> ||||
|TimeZone  <br/> |x  <br/> |||||
|ToRecipients  <br/> |||x  <br/> |||
|TotalWork  <br/> |||||x  <br/> |
|вебклиентедитформкуеристринг  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|вебклиентреадформкуеристринг  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
   
Примечания.
  
1. Включается при выполнении [привязки к элементу](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) и в ответе [операции GetItem](http://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx). Не включается в результат выполнения метода [Item. FindItems](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) или ответа [операции FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx).
    
## <a name="see-also"></a>См. также

- [Разработка клиентов веб-служб для Exchange](develop-web-service-clients-for-exchange.md)
    
- [Операция FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx)
    
- [Операция GetItem](http://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx)
    
- [Операция FindFolder](http://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx)
    
- [Операция GetFolder](http://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx)
    

