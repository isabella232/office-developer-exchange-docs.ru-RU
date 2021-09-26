---
title: Address (EmailAddressType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Address
api_type:
- schema
ms.assetid: 518641c8-7f6f-496c-86f9-341e7c1bb44c
description: Элемент Address представляет полностью разрешенный адрес электронной почты.
ms.openlocfilehash: ff26a8d6de1e9bf36bb8dff5bc0141974220cf90
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59546814"
---
# <a name="address-emailaddresstype"></a>Address (EmailAddressType)

Элемент **Address** представляет полностью разрешенный адрес электронной почты. 
  
```XML
<Address>
   <Name/>
   <EmailAddress/>
   <RoutingType/>
   <MailboxType/>
   <ItemId/>
</Address >
```

 **EmailAddressType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Name (EmailAddressType)](name-emailaddresstype.md) <br/> |Определяет имя пользователя почтового ящика. Этот элемент является необязательным.  <br/> |
|[EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) <br/> |Определяет простой адрес протокола передачи почты (SMTP) пользователя почтового ящика. Этот элемент является необязательным.  <br/> |
|[RoutingType (EmailAddress)](routingtype-emailaddress.md) <br/> |Определяет маршрутику, используемую для почтового ящика. По умолчанию значение SMTP. Этот элемент является необязательным.  <br/> |
|[MailboxType](mailboxtype.md) <br/> |Определяет тип почтового ящика пользователя почтового ящика. Этот элемент является необязательным.  <br/> |
|[ItemId](itemid.md) <br/> |Определяет идентификатор элемента контактного или частного списка рассылки для получателей из папки Контакты пользователя. Этот элемент является необязательным.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[OriginalRecipients](originalrecipients.md) <br/> |Содержит коллекцию адресов электронной почты, которые представляют исходные получатели отслеживаемого сообщения.  <br/> |
|[RoomLists](roomlists.md) <br/> |Содержит список комнат собраний в организации.  <br/> |
|[SentToAddresses](senttoaddresses.md) <br/> |Содержит список адресов электронной почты, на которые необходимо отправлять входящие сообщения, чтобы применить условие или исключение.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Нет.
  
## <a name="remarks"></a>Заметки

Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Операция GetMessageTrackingReport](getmessagetrackingreport-operation.md) 
- [Операция GetRoomLists](getroomlists-operation.md)
- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

