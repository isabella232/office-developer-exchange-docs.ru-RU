---
title: Address (строка)
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
ms.assetid: a3cdfcbd-d0c5-46d6-8daa-52405fc63ff0
description: Элемент Address представляет адрес электронной почты пользователя почтового ящика.
ms.openlocfilehash: a3648246b6be8c4f7d6421fc979a57e782ef3598
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59543802"
---
# <a name="address-string"></a>Address (строка)

Элемент **Address** представляет адрес электронной почты пользователя почтового ящика. 
  
```xml
<Address>...</Address>
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
|[Email (EmailAddressType)](email-emailaddresstype.md) <br/> |Указывает адрес электронной почты объекта MailboxData. Этот элемент используется в [операции GetUserAvailability.](getuseravailability-operation.md)<br/><br/> XPath для этого элемента:<br/><br/>  `/GetUserAvailabilityRequest/MailboxDataArray/MailboxData[i]/Email` <br/> |
|[Mailbox (доступность)](mailbox-availability.md) <br/> | Представляет пользователя почтового ящика для запроса SetUserOofSettings или GetUserOofSettings.<br/><br/>  Ниже приводится выражение XPath к этому элементу:<br/><br/>  `/GetUserOofSettingsRequest/Mailbox` <br/>  `/SetUserOofSettingsRequest/Mailbox` <br/> |
   
## <a name="text-value"></a>Текстовое значение

Если используется этот элемент, требуется текстовое значение.
  
## <a name="remarks"></a>Заметки

Этот элемент может возникать как минимум один раз в [элементе Email (EmailAddressType)](email-emailaddresstype.md) и [элементе Почтовый ящик (Доступность).](mailbox-availability.md) 
  
> [!NOTE]
> Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа. 
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
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
- [Getting User Availability](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

