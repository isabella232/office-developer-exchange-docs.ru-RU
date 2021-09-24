---
title: InternetMessageHeaders
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- InternetMessageHeaders
api_type:
- schema
ms.assetid: 4dcf8671-96df-4a2d-9836-7e8e3a67e0db
description: Элемент InternetMessageHeaders содержит коллекцию некоторых заголовок интернет-сообщений, содержащихся в элементе в почтовом ящике. Чтобы получить всю коллекцию заглавных сообщений в Интернете, используйте свойство PR_TRANSPORT_MESSAGE_HEADERS. Дополнительные сведения о EWS и загонах интернет-сообщений см. в дополнительных сведениях о EWS и internet message headersin EWS, MIME и отсутствующих загонах интернет-сообщений.
ms.openlocfilehash: 1ea49f2d5cc31aef09a9bc6d38dff25652696842
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59541083"
---
# <a name="internetmessageheaders"></a>InternetMessageHeaders

Элемент **InternetMessageHeaders** содержит коллекцию некоторых заголовок интернет-сообщений, содержащихся в элементе в почтовом ящике. Чтобы получить всю коллекцию загона интернет-сообщений, используйте **свойство PR_TRANSPORT_MESSAGE_HEADERS.** Дополнительные сведения о EWS и загонах интернет-сообщений см. в руберсе "Получение заглавных сообщений в Интернете" в [EWS, MIME](https://msdn.microsoft.com/library/exchange/hh545614%28v=exchg.140%29.aspx)и отсутствующих загонах сообщений в Интернете.
  
```XML
<InternetMessageHeaders>
   <InternetMessageHeader/>
</InternetMessageHeaders>
```

 **NonEmptyArrayOfInternetHeadersType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[InternetMessageHeader](internetmessageheader.md) <br/> |Представляет заготчик интернет-сообщений для данного загона в коллекции заготчиков.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[AcceptItem](acceptitem.md) <br/> |Представляет ответ на принять приглашение на собрание.  <br/> |
|[CalendarItem](calendaritem.md) <br/> |Представляет элемент календаря Exchange.  <br/> |
|[Контакт](contact.md) <br/> |Представляет элемент контакта Exchange.  <br/> |
|[DeclineItem](declineitem.md) <br/> |Представляет отклонить ответ на приглашения на собрание.  <br/> |
|[DistributionList](distributionlist.md) <br/> |Представляет список рассылки.  <br/> |
|[Элемент](item.md) <br/> |Представляет элемент в хранилище Exchange.  <br/> |
|[MeetingCancellation](meetingcancellation.md) <br/> |Представляет отмену собрания в хранилище Exchange.  <br/> |
|[MeetingMessage](meetingmessage.md) <br/> |Представляет собрание в хранилище Exchange.  <br/> |
|[MeetingRequest](meetingrequest.md) <br/> |Представляет приглашение на собрание в хранилище Exchange.  <br/> |
|[MeetingResponse](meetingresponse.md) <br/> |Представляет ответ на приглашение на собрание в хранилище Exchange.  <br/> |
|[Message](message-ex15websvcsotherref.md) <br/> |Представляет сообщение электронной почты Exchange.  <br/> |
|[RemoveItem](removeitem.md) <br/> |Удаляет элемент из хранилища Exchange.  <br/> |
|[Задача](task.md) <br/> |Представляет задачу в хранилище Exchange.  <br/> |
|[TentativelyAcceptItem](tentativelyacceptitem.md) <br/> |Представляет под вопросом обслуживаемых ответ на приглашения на собрание.  <br/> |
   
## <a name="remarks"></a>Заметки

Ниже приводится расширенное определение расширенного свойства управляемого API **PR_TRANSPORT_MESSAGE_HEADERS** EWS. 
  
```cs
ExtendedPropertyDefinition transportMsgHdr = new ExtendedPropertyDefinition(0x007D, MapiPropertyType.String);
```

Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)


[EWS, MIME и отсутствующие заглавные сообщения в Интернете](https://msdn.microsoft.com/library/exchange/hh545614%28v=exchg.140%29.aspx)

