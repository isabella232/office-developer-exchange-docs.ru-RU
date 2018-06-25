---
title: BccRecipients
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- BccRecipients
api_type:
- schema
ms.assetid: c4e05168-d36b-4740-a526-4b7da53553c1
description: Элемент BccRecipients представляет коллекцию получателей скрытой копии (СК) сообщения электронной почты.
ms.openlocfilehash: 858fe74c32cb7d1ed624888c06bba4ffe09d489e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761553"
---
# <a name="bccrecipients"></a>BccRecipients

Информация, содержащаяся в этом документе, может относиться к функциям и продуктам предварительной версии и может претерпеть значительные изменения до окончательного коммерческого выпуска. Настоящий документ предоставляется "как есть" и служит только для информационных целей. Корпорация Майкрософт не предоставляет никаких гарантий, явных или подразумеваемых, в связи с этим документом Элемент **BccRecipients** представляет коллекцию получателей скрытой копии (СК) сообщения электронной почты. 
  
```xml
<BccRecipients>
   <Mailbox/>
</BccRecipients>
```

 **ArrayOfRecipientsType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Mailbox](mailbox.md) <br/> |Определяет объект службы каталогов с включенной поддержкой почты Active Directory.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[RemoveItem](removeitem.md) <br/> |Удаляет элемент из хранилища Exchange.  <br/> |
|[Message](message-ex15websvcsotherref.md) <br/> |Представляет сообщение электронной почты Exchange.  <br/> |
|[MeetingMessage](meetingmessage.md) <br/> |Представляет собрание в хранилище Exchange.  <br/> |
|[MeetingRequest](meetingrequest.md) <br/> |Представляет приглашение на собрание в хранилище Exchange.  <br/> |
|[MeetingResponse](meetingresponse.md) <br/> |Представляет ответ на приглашение на собрание в хранилище Exchange.  <br/> |
|[MeetingCancellation](meetingcancellation.md) <br/> |Представляет отмену собрания в хранилище Exchange.  <br/> |
|[AcceptItem](acceptitem.md) <br/> |Представляет ответ на принять приглашение на собрание.  <br/> |
|[TentativelyAcceptItem](tentativelyacceptitem.md) <br/> |Представляет под вопросом обслуживаемых ответ на приглашения на собрание.  <br/> |
|[DeclineItem](declineitem.md) <br/> |Представляет отклонить ответ на приглашения на собрание.  <br/> |
|[ReplyToItem](replytoitem.md) <br/> |Содержит ответ создателем элемента в хранилище Exchange.  <br/> |
|[ReplyAllToItem](replyalltoitem.md) <br/> |Содержит ответить всем получателям определенного элемента в хранилище Exchange.  <br/> |
|[ForwardItem](forwarditem.md) <br/> |Содержит элемент хранилища Exchange переадресация получателям.  <br/> |
|[CancelCalendarItem](cancelcalendaritem.md) <br/> |Представляет объект ответа, которая используется для отмены собрания.  <br/> |
   
## <a name="remarks"></a>Замечания

Не удается получить **BccRecipients** с помощью запроса FindItem. Используйте GetItem запрос для получения **BccRecipients**.
  
Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

