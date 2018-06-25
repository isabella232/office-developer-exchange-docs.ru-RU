---
title: Адрес (строка)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Address
api_type:
- schema
ms.assetid: a3cdfcbd-d0c5-46d6-8daa-52405fc63ff0
description: Элемент адрес — адрес электронной почты пользователя почтового ящика.
ms.openlocfilehash: 07c634d6166d88a8912bc66081a13671e600c801
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761357"
---
# <a name="address-string"></a>Адрес (строка)

Элемент **адрес** — адрес электронной почты пользователя почтового ящика. 
  
```xml
<Address>...</Address>
```

 **string**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Электронной почты (EmailAddressType)](email-emailaddresstype.md) <br/> |Указывает адрес электронной почты объекта MailboxData. Данный элемент используется в [операции GetUserAvailability](getuseravailability-operation.md).<br/><br/> XPath для этого элемента:<br/><br/>  `/GetUserAvailabilityRequest/MailboxDataArray/MailboxData[i]/Email` <br/> |
|[Почтовый ящик (доступность)](mailbox-availability.md) <br/> | Представляет пользователя почтового ящика для SetUserOofSettings или GetUserOofSettings запроса.<br/><br/>  Ниже приведены выражения XPath для этого элемента.<br/><br/>  `/GetUserOofSettingsRequest/Mailbox` <br/>  `/SetUserOofSettingsRequest/Mailbox` <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение является обязательным, если данный элемент используется.
  
## <a name="remarks"></a>Замечания

Этот элемент может возникнуть только один раз в элементе [электронной почты (EmailAddressType)](email-emailaddresstype.md) и элемент [почтового ящика (доступность)](mailbox-availability.md) . 
  
> [!NOTE]
> Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа. 
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Операция GetUserAvailability](getuseravailability-operation.md)
- [Операция GetUserOofSettings](getuseroofsettings-operation.md)
- [Операция SetUserOofSettings](setuseroofsettings-operation.md)
- [GetUserAvailabilityRequest](getuseravailabilityrequest.md)
- [GetUserOofSettingsRequest](getuseroofsettingsrequest.md)
- [SetUserOofSettingsRequest](setuseroofsettingsrequest.md)
- [Getting User Availability](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

