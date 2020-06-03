---
title: Имя (EmailAddress)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Name
api_type:
- schema
ms.assetid: c719c55f-d625-4e64-846f-50ac91881443
description: Элемент Name представляет отображаемое имя пользователя почтового ящика.
ms.openlocfilehash: 2c6b29f1b069f9cc72ac84e7aebfff99437e630a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44466957"
---
# <a name="name-emailaddress"></a>Имя (EmailAddress)

Элемент **Name** представляет отображаемое имя пользователя почтового ящика. 
  
```xml
<Name/>
```

**String**

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

Отсутствуют.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Электронная почта (EmailAddressType)](email-emailaddresstype.md) <br/> |Представляет пользователя почтового ящика для запроса GetUserAvailability.  <br/> <br/>XPath для этого элемента:  <br/><br/>  `/GetUserAvailabilityRequest/MailboxDataArray/MailboxData[i]/Email` <br/> |
|[Mailbox (доступность)](mailbox-availability.md) <br/> | Представляет пользователя почтового ящика для запроса SetUserOofSettings или GetUserOofSettings.  <br/><br/>  Ниже приведены выражения XPath для этого элемента.  <br/><br/>  `/GetUserOofSettingsRequest/Mailbox` <br/><br/>  `/SetUserOofSettingsRequest/Mailbox` <br/> |
   
## <a name="text-value"></a>Текстовое значение

При использовании этого элемента необходимо указать текстовое значение.
  
## <a name="remarks"></a>Примечания

Этот элемент может встречаться в элементе [электронной почты (EmailAddressType)](email-emailaddresstype.md) не чаще, чем один раз. Этот элемент не является обязательным. 
  
> [!NOTE]
> Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа. 
  
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

