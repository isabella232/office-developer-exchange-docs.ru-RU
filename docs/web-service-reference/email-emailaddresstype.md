---
title: Электронная почта (EmailAddressType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Email
api_type:
- schema
ms.assetid: dfffa1d5-2c3c-4f56-af63-5853df462e58
description: Элемент email представляет пользователя почтового ящика для запроса GetUserAvailability.
ms.openlocfilehash: 2ed8de9c011a385ec6c4ebd2f8d1d47304343a0e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459232"
---
# <a name="email-emailaddresstype"></a>Электронная почта (EmailAddressType)

Элемент **Email** представляет пользователя почтового ящика для запроса GetUserAvailability. 
  
- [жетусераваилабилитирекуест](getuseravailabilityrequest.md)  
- [маилбоксдатааррай](mailboxdataarray.md) 
- [MailboxData](mailboxdata.md) 
- [Электронная почта (EmailAddressType)](email-emailaddresstype.md)
  
```xml
<Email>
   <Name>...</Name>
   <Address>...</Address>
   <RoutingType>...</RoutingType>
</Email>
```

 **EmailAddressType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Имя (EmailAddress)](name-emailaddress.md) <br/> |Представляет отображаемое имя пользователя почтового ящика.  <br/> |
|[Address (строка)](address-string.md) <br/> |Представляет адрес электронной почты пользователя почтового ящика.  <br/> |
|[Раутингтипе (EmailAddress)](routingtype-emailaddress.md) <br/> |Представляет протокол маршрутизации для сообщения.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[MailboxData](mailboxdata.md) <br/> |Представляет отдельного пользователя почтового ящика и параметры возвращаемого типа данных об этом пользователе.  <br/> XPath для этого элемента:  <br/>  `/GetUserAvailabilityRequest/MailboxDataArray[i]/MailboxData` <br/> |
   
## <a name="remarks"></a>Примечания

Схема с описанием этого элемента находится в каталоге /EWS/ на компьютере, на котором запущено приложение MicrosoftExchange Server 2007 с установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Операция GetUserAvailability](getuseravailability-operation.md)  
- [жетусераваилабилитирекуест](getuseravailabilityrequest.md)
- [Getting User Availability](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

