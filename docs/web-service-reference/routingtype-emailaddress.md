---
title: Раутингтипе (EmailAddress)
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
ms.assetid: 74d83198-0d9d-4c78-a2bc-9a671859ff37
description: Элемент Раутингтипе представляет протокол маршрутизации для получателя.
ms.openlocfilehash: a0a6cf312bcb1d4b4818a82bc8d8d3e3f33ad6f6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835255"
---
# <a name="routingtype-emailaddress"></a>Раутингтипе (EmailAddress)

Элемент **раутингтипе** представляет протокол маршрутизации для получателя. 
  
```XML
<RoutingType/>
```

 **строка**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Электронная почта (EmailAddressType)](email-emailaddresstype.md) <br/> |Задает адрес электронной почты объекта MailboxData. Этот элемент используется в [операции GetUserAvailability](getuseravailability-operation.md).  <br/><br/> XPath для этого элемента:  <br/><br/>  `/GetUserAvailabilityRequest/MailboxDataArray/MailboxData[i]/Email` <br/> |
|[Mailbox (доступность)](mailbox-availability.md) <br/> | Представляет пользователя почтового ящика для запроса SetUserOofSettings или GetUserOofSettings.  <br/><br/>  Ниже приведены выражения XPath для этого элемента. <br/> <br/>  `/GetUserOofSettingsRequest/Mailbox` <br/><br/>  `/SetUserOofSettingsRequest/Mailbox` <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение является необязательным. Единственным допустимым значением является SMTP. Если значение не указано, используется значение по умолчанию (SMTP).
  
## <a name="remarks"></a>Примечания

Этот элемент может встречаться в элементе [электронной почты (EmailAddressType)](email-emailaddresstype.md) не чаще, чем один раз. Этот элемент не является обязательным. Этот элемент существует для включения будущих протоколов. Другой элемент **раутингтипе** используется для доступа к элементам в почтовом ящике пользователя. 
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Операция GetUserAvailability](getuseravailability-operation.md)
- [жетусераваилабилитирекуест](getuseravailabilityrequest.md)
- [Getting User Availability](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

