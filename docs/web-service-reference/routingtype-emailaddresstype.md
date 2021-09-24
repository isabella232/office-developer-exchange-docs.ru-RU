---
title: RoutingType (EmailAddressType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- RoutingType
api_type:
- schema
ms.assetid: 683216be-9972-4f48-a148-c34bfe7f53e5
description: Элемент RoutingType определяет тип адреса для почтового ящика.
ms.openlocfilehash: fdbe40bd74debe517739e0fe0c47ed108bd614c6
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59509370"
---
# <a name="routingtype-emailaddresstype"></a>RoutingType (EmailAddressType)

Элемент **RoutingType** определяет тип адреса для почтового ящика. 
  
```XML
<RoutingType/>
```

 **NonEmptyStringType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[ActingAs](actingas.md) <br/> |Определяет, кому отправляется вызываемая.  <br/> |
|[Mailbox](mailbox.md) <br/> |Определяет полностью разрешенный адрес электронной почты.  <br/> |
|[RoomList](roomlist.md) <br/> |Определяет список комнат собраний.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение представляет тип маршрутивки. SMTP — это типичное текстовое значение для этого элемента.
  
## <a name="remarks"></a>Заметки

Этот элемент необязателен в [элементе Почтовый ящик.](mailbox.md) Другой [элемент RoutingType (EmailAddress)](routingtype-emailaddress.md) используется для операций доступности. 
  
Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

