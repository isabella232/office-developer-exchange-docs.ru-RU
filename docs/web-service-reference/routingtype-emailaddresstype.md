---
title: RoutingType (EmailAddressType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RoutingType
api_type:
- schema
ms.assetid: 683216be-9972-4f48-a148-c34bfe7f53e5
description: Элемент RoutingType определяет тип адреса для почтового ящика.
ms.openlocfilehash: a02c3b5711a657311428d67cccabd9c8c231db67
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835256"
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
|[ActingAs](actingas.md) <br/> |Определяет, как отправляющего вызывающего абонента.  <br/> |
|[Mailbox](mailbox.md) <br/> |Определяет адрес электронной почты полностью разрешенной.  <br/> |
|[RoomList](roomlist.md) <br/> |Определяет список конференц-залы.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение представляет тип маршрутизации. SMTP — типичное текстовое значение для этого элемента.
  
## <a name="remarks"></a>Замечания

Этот элемент является необязательным в элементе [почтового ящика](mailbox.md) . Другой элемент [RoutingType (EmailAddress)](routingtype-emailaddress.md) используется для операций доступности. 
  
Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

