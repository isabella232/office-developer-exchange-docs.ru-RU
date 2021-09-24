---
title: RoutingType (EmailAddress)
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
ms.assetid: 74d83198-0d9d-4c78-a2bc-9a671859ff37
description: Элемент RoutingType представляет протокол маршрутивки для получателя.
ms.openlocfilehash: cc4d18ff9fa18f0ec2024f15cb6a3bd4199832de
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59534431"
---
# <a name="routingtype-emailaddress"></a>RoutingType (EmailAddress)

Элемент **RoutingType** представляет протокол маршрутивки для получателя. 
  
```XML
<RoutingType/>
```

 **строка**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Email (EmailAddressType)](email-emailaddresstype.md) <br/> |Указывает адрес электронной почты объекта MailboxData. Этот элемент используется в [операции GetUserAvailability.](getuseravailability-operation.md)  <br/><br/> XPath для этого элемента:  <br/><br/>  `/GetUserAvailabilityRequest/MailboxDataArray/MailboxData[i]/Email` <br/> |
|[Mailbox (доступность)](mailbox-availability.md) <br/> | Представляет пользователя почтового ящика для запроса SetUserOofSettings или GetUserOofSettings.  <br/><br/>  Ниже приводится выражение XPath к этому элементу: <br/> <br/>  `/GetUserOofSettingsRequest/Mailbox` <br/><br/>  `/SetUserOofSettingsRequest/Mailbox` <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение необязательно. Ниже перечислены возможные значения.

* SMTP
* EX

Если значение не предоставляется, используется значение SMTP по умолчанию.
  
## <a name="remarks"></a>Заметки

Этот элемент может возникать как минимум один раз в [элементе Email (EmailAddressType).](email-emailaddresstype.md) Этот элемент не требуется. Этот элемент существует для включения будущих протоколов. Другой **элемент RoutingType** используется для доступа к элементам в почтовом ящике пользователя. 
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Операция GetUserAvailability](getuseravailability-operation.md)
- [GetUserAvailabilityRequest](getuseravailabilityrequest.md)
- [Getting User Availability](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

