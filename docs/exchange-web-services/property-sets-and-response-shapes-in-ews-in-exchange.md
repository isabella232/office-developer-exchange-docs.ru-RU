---
title: Наборы свойств и ответ с фигурами в веб-служб Exchange в Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 04a29804-6067-48e7-9f5c-534e253a230e
description: Сведения для управления ответа фигуры и наборы свойств, возвращаемых веб-служб Exchange управляемые API и веб-служб Exchange в Exchange.
ms.openlocfilehash: d9fd6c155438dfd03cfc9536397316cf3faa2287
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761257"
---
# <a name="property-sets-and-response-shapes-in-ews-in-exchange"></a>Наборы свойств и ответ с фигурами в веб-служб Exchange в Exchange

Сведения для управления ответа фигуры и наборы свойств, возвращаемых веб-служб Exchange управляемые API и веб-служб Exchange в Exchange.
  
Хранилище данных Exchange предоставляет гибкие хранилища решение, которое позволяет хранить различные элементы, например контакты и элементы календаря в той же папке; Тем не менее он может усложнить для управления данными, который возвращается из вызова операции EWS или управляемый метод API.
  
Для упрощения управления данными, который возвращается с Exchange Online, Exchange Online, как набор Office 365 или версии Excahange, начиная с Exchange 2013 управляемый API EWS использует наборы свойств и ответа фигур с помощью веб-служб Exchange. Это предварительно определенные коллекции, которые обеспечивают основные свойства элемента хранилища. Набор свойств, который возвращается определяется тип элемента. Это означает, что при связывании элемента с помощью метода управляемый API Exchange [Item.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) вы получаете другой набор свойств, в зависимости от типа элемента, к которой выполняется привязка. Привязка к элементу календаря возвращает другой набор свойств, чем привязки для элемента контакта. Аналогичным образом при использовании веб-служб Exchange [операции GetItem](http://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) возвращает другой набор свойств, основанных на тип элемента, который возвращается. 
  
Привязка к папке с помощью метода [Folder.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) или с помощью [операции GetFolder](http://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) также возвращает различные наборы свойств, основанных на к папке, где вы запрашиваете. 
  
**В таблице 1. Предварительно определенные ответа фигур**

|**Фигура ответа**|**Управляемый API EWS эквивалент**|**Описание**|
|:-----|:-----|:-----|
|Только идентификатор  <br/> |[BasePropertySet.IdOnly](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.basepropertyset%28v=exchg.80%29.aspx) <br/> |Возвращает только идентификатор элемента или папки. Большинство приложений необходимо использовать эту фигуру ответа и указать дополнительные свойства, которые необходимы.  <br/> |
|Значение по умолчанию  <br/> |Нет  <br/> |Возвращает набор свойств, которые по умолчанию для элемента или папки (EWS).  <br/> |
|Все свойства  <br/> |[BasePropertySet.FirstClassProperties](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.basepropertyset%28v=exchg.80%29.aspx) <br/> |Возвращает свойства, которые наиболее часто используемых клиентских приложений. С помощью свойства путь можно вернуть дополнительные свойства.  <br/> |
   
## <a name="default-response-shapes"></a>По умолчанию ответа фигур

Веб-служб Exchange включает набор фигур ответа по умолчанию для папок и элементов. 
  
В следующей таблице приведены свойства по умолчанию, которые возвращаются для каждой папки с помощью операций [FindFolder](http://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx) и [GetFolder](http://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) веб-служб Exchange. 
  
**В таблице 2. Свойства папки по умолчанию**

|**Свойство**|**Папки «Входящие»**|**Календарь**|**Контакты**|**"Удаленные"**|**Черновики**|**Примечания**|**Другие папки**|**Исходящие**|
|:-----|:-----|:-----|:-----|:-----|:-----|:-----|:-----|:-----|
|Отображаемое имя  <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |
|Идентификатор папки  <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |
|Count вложенной папке  <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |
|Общее число  <br/> |X   <br/> ||X   <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |
|Число непрочтенных сообщений  <br/> |X   <br/> |||X   <br/> |X   <br/> ||X   <br/> |X   <br/> |
   
В следующей таблице приведены свойства по умолчанию, возвращаемое для каждого типа элемента с помощью операций [FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) и [GetItem](http://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) веб-служб Exchange. 
  
**В таблице 3. По умолчанию свойства элемента**

|**Свойство**|**Элемент календаря**|**Элемента контакта**|**Элемент сообщения**|**Элемент "Задача"**|
|:-----|:-----|:-----|:-----|:-----|
|Body  <br/> |||X(1)  <br/> ||
|CalendarItemType  <br/> ||x  <br/> |||
|Название организации  <br/> ||x  <br/> |||
|CompleteName  <br/> ||x  <br/> |||
|DateTimeCreated  <br/> |||x  <br/> ||
|DateTimeSent  <br/> |||x  <br/> ||
|DueDate  <br/> ||||x(2)  <br/> |
|EmailAddresses  <br/> ||x  <br/> |||
|End  <br/> |x  <br/> ||||
|FileAs  <br/> ||x  <br/> |||
|From  <br/> |||x  <br/> ||
|HasAttachments  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|ImAddresses  <br/> ||x  <br/> |||
|IsAssociated  <br/> |x  <br/> ||x  <br/> ||
|IsDeliveryReceiptRequested  <br/> |||x  <br/> ||
|Идентификатор элемента  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|Название должности  <br/> ||x  <br/> |||
|LegacyFreeBusyStatus  <br/> |x  <br/> ||||
|Location  <br/> |x  <br/> ||||
|Organizer  <br/> |x  <br/> ||||
|PercentComplete  <br/> ||||x  <br/> |
|PhoneNumbers  <br/> ||x  <br/> |||
|PhysicalAddresses  <br/> ||x  <br/> |||
|ResponseObjects  <br/> |x(1)  <br/> ||x(1)  <br/> ||
|Sensitity  <br/> |||x  <br/> ||
|Размер  <br/> |||x  <br/> ||
|Дата начала  <br/> ||||x(2)  <br/> |
|Состояние  <br/> ||||x  <br/> |
|Subject  <br/> |x  <br/> ||x  <br/> |x  <br/> |
   
Примечания.
  
1. Включены в ответ от операции **GetItem** . Не включаются в ответ от операции **FindItem** . 
    
2. Если поле содержит данные только включенных в ответ. Если это поле не заполнено не включаются в ответе.
    
### <a name="all-properties-set-and-response-shape"></a>Все свойства набора и ответа фигуры

В следующей таблице приведены первого класса свойства, возвращаемые путем вызова управляемый API EWS [Item.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) и управляемый API EWS [Item.FindItems](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) методы и возвращаемых [FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) и [форма ответа «все свойства» GetItem](http://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) операции веб-служб Exchange. 
  
Можно добавить дополнительные свойства к свойству установить или включить расширенные свойства. Для получения дополнительных сведений просмотрите [Свойства и расширенные свойства в веб-службах Exchange](properties-and-extended-properties-in-ews-in-exchange.md).
  
**В таблице 4. Свойства первого класса**

|||||||
|:-----|:-----|:-----|:-----|:-----|:-----|
|Свойство  <br/> |Элемент календаря  <br/> |Элемента контакта  <br/> |Элемент сообщения  <br/> |Элемента записи  <br/> |Элемент "Задача"  <br/> |
|ActualWork  <br/> |||||x  <br/> |
|AdjacentMeetingCount  <br/> |x  <br/> |||||
|AdjacentMeetings  <br/> |x  <br/> |||||
|Alias  <br/> ||x  <br/> ||||
|AllowNewTimeProposal  <br/> |x  <br/> |||||
|AppointmentReplyTime  <br/> |x  <br/> |||||
|AppointmentSequenceNumber  <br/> |x  <br/> |||||
|AppointmentState  <br/> |x  <br/> |||||
|AssignedTime  <br/> |||||x  <br/> |
|AssistantName  <br/> ||x  <br/> ||||
|BccRecipients  <br/> |||x  <br/> |||
|BillingInformation  <br/> |||||x  <br/> |
|Body  <br/> |x(1)  <br/> |x(1)  <br/> |x(1)  <br/> ||x(1)  <br/> |
|BusinessHomePage  <br/> ||x  <br/> |x  <br/> |||
|CalendarItemType  <br/> |x  <br/> |||||
|Categories  <br/> |x  <br/> ||x  <br/> |x  <br/> |x  <br/> |
|CcRecipients  <br/> |||x  <br/> |||
|ChangeCount  <br/> |||||x  <br/> |
|Дочерние объекты  <br/> ||x  <br/> ||||
|Companies  <br/> |||||x  <br/> |
|CompleteDate  <br/> |||||x  <br/> |
|CompleteName  <br/> ||x  <br/> ||||
|ConferenceType  <br/> |x  <br/> |||||
|ConflictingMeetingCount  <br/> |x  <br/> |||||
|ConflictingMeetings  <br/> |x  <br/> |||||
|Контакты  <br/> |||||x  <br/> |
|ContactSource  <br/> ||x  <br/> ||||
|ConversationId  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|ConversationIndex  <br/> |||x  <br/> |x  <br/> ||
|ConversationTopic  <br/> |||x  <br/> |x  <br/> ||
|Culture  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|DateTimeCreated  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|DateTimeReceived  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|DateTimeSent  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|DateTimeStamp  <br/> |x  <br/> |||||
|DelegationState  <br/> |||||x  <br/> |
|Представитель  <br/> |||||x  <br/> |
|DeletedOccurances  <br/> |x  <br/> |||||
|Отдел  <br/> ||x  <br/> ||||
|DirectoryId  <br/> ||x  <br/> ||||
|DirectReports  <br/> ||x  <br/> ||||
|DisplayCc  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|DisplayName  <br/> ||x  <br/> ||||
|DisplayTo  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|DueDate  <br/> |||||x  <br/> |
|Продолжительность  <br/> |x  <br/> |||||
|EffectiveRights  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|EmailAddresses  <br/> ||x  <br/> ||||
|End  <br/> |x  <br/> |||||
|EndTimeZone  <br/> |x  <br/> |||||
|FileAs  <br/> ||x  <br/> ||||
|FileAsMapping  <br/> ||x  <br/> ||||
|FirstOccurance  <br/> |x  <br/> |||||
|From  <br/> |||x  <br/> |x  <br/> ||
|Создание  <br/> ||x  <br/> ||||
|GivenName  <br/> ||x  <br/> ||||
|HasAttachments  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|HasPicture  <br/> ||x  <br/> ||||
|ImAddresses  <br/> ||x  <br/> ||||
|Важность  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|Инициалы  <br/> ||x  <br/> ||||
|InReplyTo  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|InternetMessageId  <br/> |||x  <br/> |x  <br/> ||
|InternetMessageHeaders  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|IsAllDayEvent  <br/> |x  <br/> |||||
|IsAssociated  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|IsCancelled  <br/> |x  <br/> |||||
|IsComplete  <br/> |||||x  <br/> |
|IsDeliveryReceiptRequested  <br/> |||x  <br/> |||
|IsDraft  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|IsFromMe  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|IsMeeting  <br/> |x  <br/> |||||
|IsOnlineMeeting  <br/> |x  <br/> |||||
|IsRead  <br/> |||x  <br/> |||
|IsReadReceiptRequested  <br/> |||x  <br/> |||
|IsRecurring  <br/> |x  <br/> ||||x  <br/> |
|IsResend  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|IsResponseRequested  <br/> |x  <br/> ||x  <br/> |||
|IsSubmitted  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|IsUnmodified  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|ItemClass  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|Идентификатор элемента  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|Название должности  <br/> ||x  <br/> ||||
|LastModifiedName  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|LastModifiedTime  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|LastOccurrance  <br/> |x  <br/> |||||
|LegacyFreeBusyStatus  <br/> |x  <br/> |||||
|Location  <br/> |x  <br/> |||||
|Руководитель  <br/> ||x  <br/> ||||
|MeetingRequestWasSent  <br/> |x  <br/> |||||
|MeetingTimeZone  <br/> |x  <br/> |||||
|MeetingWorkspaceUrl  <br/> |x  <br/> |||||
|MiddleName  <br/> ||x  <br/> ||||
|Расстояние  <br/> ||x  <br/> |||x  <br/> |
|ModifiedOccurrances  <br/> |x  <br/> |||||
|MyResponseType  <br/> |x  <br/> |||||
|NetShowUrl  <br/> |x  <br/> |||||
|Понятное имя  <br/> ||x  <br/> ||||
|����������  <br/> ||x  <br/> ||||
|Расположение компании  <br/> ||x  <br/> ||||
|OptionalAttendees  <br/> |x  <br/> |||||
|Organizer  <br/> |x  <br/> |||||
|OriginalStart  <br/> |x  <br/> |||||
|Owner  <br/> |||||x  <br/> |
|ParentFolderId  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|PercentComplete  <br/> |||||x  <br/> |
|PhoneNumbers  <br/> ||x  <br/> ||||
|PhoneticFirstName  <br/> ||x  <br/> ||||
|PhoneticFullName  <br/> ||x  <br/> ||||
|PhoneticLastName  <br/> ||x  <br/> ||||
|Photo  <br/> ||x  <br/> ||||
|PhysicalAddresses  <br/> ||x  <br/> ||||
|PostalAddressIndex  <br/> ||x  <br/> ||||
|PostedTime  <br/> ||||x  <br/> ||
|Род занятий  <br/> ||x  <br/> ||||
|Получил  <br/> |||x  <br/> |||
|ReceivedRepresenting  <br/> |||x  <br/> |||
|Reccurrence  <br/> |x  <br/> ||||x  <br/> |
|Справочные материалы  <br/> |||x  <br/> |x  <br/> ||
|ReminderDueBy  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|ReminderIsSet  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|ReminderMinutesBeforeStart  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|ReplyTo  <br/> |||x  <br/> |||
|RequiredAttendees  <br/> |x  <br/> |||||
|Ресурсы  <br/> |x  <br/> |||||
|ResponseObjects  <br/> |x(1)  <br/> |x(1)  <br/> |x(1)  <br/> |x(1)  <br/> |x(1)  <br/> |
|Отправитель  <br/> |||x  <br/> |x  <br/> ||
|Уровень конфиденциальности сообщения  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|Размер  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|SpouseName  <br/> ||x  <br/> ||||
|Начало  <br/> |x  <br/> |||||
|Дата начала  <br/> |||||x  <br/> |
|StartTimeZone  <br/> |x  <br/> |||||
|Состояние  <br/> |||||x  <br/> |
|StatusDescription  <br/> |||||x  <br/> |
|Subject  <br/> |x  <br/> |x  <br/> |x  <br/> ||x  <br/> |
|Фамилия  <br/> ||x  <br/> ||||
|TimeZone  <br/> |x  <br/> |||||
|ToRecipients  <br/> |||x  <br/> |||
|TotalWork  <br/> |||||x  <br/> |
|WebClientEditFormQueryString  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|WebClientReadFormQueryString  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
   
Примечания.
  
1. Включенные при [привязке к элементу](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) и в ответ от [операции GetItem](http://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx). Не включается в результат метода [Item.FindItems](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) или ответ от [FindItem операции](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx).
    
## <a name="see-also"></a>См. также

- [Разработка клиентов веб-служб для Exchange](develop-web-service-clients-for-exchange.md)
    
- [FindItem Operation](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx)
    
- [GetItem Operation](http://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx)
    
- [FindFolder Operation](http://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx)
    
- [GetFolder Operation](http://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx)
    

