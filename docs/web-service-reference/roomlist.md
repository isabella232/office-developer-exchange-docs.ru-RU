---
title: RoomList
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- RoomList
api_type:
- schema
ms.assetid: cb02bdf0-df9f-4e31-b7dd-cd9f2f2cc2b2
description: Элемент RoomList представляет адрес электронной почты, который определяет список комнат собраний.
ms.openlocfilehash: ae461424b6affbc3dd362d5a7d0a5cc3fdc46fab
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59524492"
---
# <a name="roomlist"></a>RoomList

Элемент **RoomList** представляет адрес электронной почты, который определяет список комнат собраний. 
  
[GetRooms](getrooms.md)
  
[RoomList](roomlist.md)
  
```XML
<RoomList>
   <Name/>
   <EmailAddress/>
   <RoutingType/>
   <MailboxType/>
   <ItemId/>
</RoomList>
```

 **EmailAddressType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Name (EmailAddressType)](name-emailaddresstype.md) <br/> |Определяет имя отображения списка номеров. Этот элемент является необязательным.  <br/> |
|[EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) <br/> |Определяет простой протокол передачи почты (SMTP) списка номеров. Этот элемент является необязательным.  <br/> |
|[RoutingType (EmailAddress)](routingtype-emailaddress.md) <br/> |Определяет маршрутику, используемую для почтового ящика. По умолчанию значение SMTP. Этот элемент является необязательным.  <br/> |
|[MailboxType](mailboxtype.md) <br/> |Определяет тип почтового ящика пользователя почтового ящика. Этот элемент является необязательным.  <br/> |
|[ItemId](itemid.md) <br/> |Определяет идентификатор элемента контактного или частного списка рассылки для получателей из папки Контакты пользователя. Этот элемент является необязательным.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[GetRooms](getrooms.md) <br/> |Корневой элемент запроса для получения списка комнат в определенном списке комнат.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Нет.
  
## <a name="remarks"></a>Заметки

Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операция GetRooms](getrooms-operation.md)


- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

