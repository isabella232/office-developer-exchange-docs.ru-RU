---
title: Mailbox (доступность)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Mailbox
api_type:
- schema
ms.assetid: affd192e-8914-473f-9098-d9bdf898de2c
description: Элемент почтовых ящиков представляет пользователя почтового ящика для запроса SetUserOofSettings или GetUserOofSettings.
ms.openlocfilehash: 5e32c4be807dae92b27df7012caa8eb1b295b26c
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59522924"
---
# <a name="mailbox-availability"></a>Mailbox (доступность)

Элемент **почтовых ящиков** представляет пользователя почтового ящика для запроса SetUserOofSettings или GetUserOofSettings. 
  
```xml
<Mailbox>
   <Name>...</Name>
   <Address>...</Address>
   <RoutingType>...</RoutingType>
</Mailbox>
```

**EmailAddressType**

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Name (EmailAddress)](name-emailaddress.md) <br/> |Отображает имя пользователя почтового ящика. Этот элемент необязателен в SetUserOofSettingsRequest. GetUserOofSettingsRequest возвращает этот элемент.  <br/> |
|[Address (строка)](address-string.md) <br/> |Представляет адрес электронной почты пользователя почтового ящика. Этот элемент обязательный.  <br/> |
|[RoutingType (EmailAddress)](routingtype-emailaddress.md) <br/> |Представляет протокол маршрутивки для сообщения. Этот элемент необязателен в SetUserOofSettingsRequest. GetUserOofSettingsRequest возвращает этот элемент.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[GetUserOofSettingsRequest](getuseroofsettingsrequest.md) <br/> |Используется для получения параметров и сообщений пользователя Office (OOF).  <br/> Ниже приводится выражение XPath к этому элементу:  <br/>  `/GetUserOofSettingsRequest` <br/> |
|[SetUserOofSettingsRequest](setuseroofsettingsrequest.md) <br/> |Используется для установки параметров OOF и сообщений пользователя почтового ящика.  <br/> Ниже приводится выражение XPath к этому элементу:  <br/>  `/SetUserOofSettingsRequest` <br/> |
   
## <a name="remarks"></a>Заметки

Адрес электронной почты используется для идентификации папки календаря, которая содержит параметры OOF. 
  
Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Операция GetUserOofSettings](getuseroofsettings-operation.md)
- [Операция SetUserOofSettings](setuseroofsettings-operation.md)

