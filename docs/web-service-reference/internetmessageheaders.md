---
title: InternetMessageHeaders
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- InternetMessageHeaders
api_type:
- schema
ms.assetid: 4dcf8671-96df-4a2d-9836-7e8e3a67e0db
description: Элемент InternetMessageHeaders содержит коллекцию заголовков сообщений Интернета, содержащихся в элемента в почтовом ящике. Чтобы получить вся коллекция заголовков сообщений Интернета, используйте свойство PR_TRANSPORT_MESSAGE_HEADERS. Дополнительные сведения о веб-служб Exchange и заголовки сообщений Интернета, seeGetting Интернет сообщение headersin веб-служб Exchange, MIME и отсутствующие заголовков сообщений Интернета.
ms.openlocfilehash: 2da529a8a3532cebb2791b285b7673c962a2a656
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833954"
---
# <a name="internetmessageheaders"></a>InternetMessageHeaders

Элемент **InternetMessageHeaders** содержит коллекцию заголовков сообщений Интернета, содержащихся в элемента в почтовом ящике. Чтобы получить вся коллекция заголовков сообщений Интернета, используйте свойство **PR_TRANSPORT_MESSAGE_HEADERS** . Дополнительные сведения о веб-служб Exchange и Интернет заголовки сообщений содержатся в разделе «Приступая к Интернету заголовки сообщений» в [веб-служб Exchange, MIME и отсутствующие заголовков сообщений Интернета](http://msdn.microsoft.com/en-us/library/exchange/hh545614%28v=exchg.140%29.aspx).
  
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
|[InternetMessageHeader](internetmessageheader.md) <br/> |Представляет заголовок сообщения Интернета для заданного заголовка в коллекции заголовков.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[AcceptItem](acceptitem.md) <br/> |Представляет ответ на принять приглашение на собрание.  <br/> |
|[Элемента календаря, имеющего](calendaritem.md) <br/> |Представляет элемент календаря Exchange.  <br/> |
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
   
## <a name="remarks"></a>Замечания

Ниже приведен управляемый API EWS расширенные определений для свойства **PR_TRANSPORT_MESSAGE_HEADERS** . 
  
```cs
ExtendedPropertyDefinition transportMsgHdr = new ExtendedPropertyDefinition(0x007D, MapiPropertyType.String);
```

Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)


[Веб-служб Exchange, MIME и отсутствующие заголовков сообщений Интернета](http://msdn.microsoft.com/en-us/library/exchange/hh545614%28v=exchg.140%29.aspx)

