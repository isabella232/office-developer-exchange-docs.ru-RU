---
title: Mailbox (доступность)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Mailbox
api_type:
- schema
ms.assetid: affd192e-8914-473f-9098-d9bdf898de2c
description: Элемент Mailbox представляет пользователя почтового ящика для запроса SetUserOofSettings или GetUserOofSettings.
ms.openlocfilehash: 2e901ae0df56542f56f247184254294735018468
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834254"
---
# <a name="mailbox-availability"></a>Mailbox (доступность)

Элемент **Mailbox** представляет пользователя почтового ящика для запроса SetUserOofSettings или GetUserOofSettings. 
  
```xml
<Mailbox>
   <Name>...</Name>
   <Address>...</Address>
   <RoutingType>...</RoutingType>
</Mailbox>
```

**EmailAddressType**

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Имя (EmailAddress)](name-emailaddress.md) <br/> |Представляет отображаемое имя пользователя почтового ящика. Этот элемент является необязательным в Сетусеруфсеттингсрекуест. Жетусеруфсеттингсрекуест будет возвращать этот элемент.  <br/> |
|[Address (строка)](address-string.md) <br/> |Представляет адрес электронной почты пользователя почтового ящика. Этот элемент обязательный.  <br/> |
|[Раутингтипе (EmailAddress)](routingtype-emailaddress.md) <br/> |Представляет протокол маршрутизации для сообщения. Этот элемент является необязательным в Сетусеруфсеттингсрекуест. Жетусеруфсеттингсрекуест будет возвращать этот элемент.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[жетусеруфсеттингсрекуест](getuseroofsettingsrequest.md) <br/> |Используется для получения параметров и сообщений пользователя почтового ящика.  <br/> Ниже приведено выражение XPath для этого элемента:  <br/>  `/GetUserOofSettingsRequest` <br/> |
|[сетусеруфсеттингсрекуест](setuseroofsettingsrequest.md) <br/> |Используется для настройки параметров и сообщений пользователя почтового ящика.  <br/> Ниже приведено выражение XPath для этого элемента:  <br/>  `/SetUserOofSettingsRequest` <br/> |
   
## <a name="remarks"></a>Примечания

Адрес электронной почты используется для определения папки календаря, в которой содержатся параметры отсутствия на работе. 
  
Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Операция GetUserOofSettings](getuseroofsettings-operation.md)
- [Операция SetUserOofSettings](setuseroofsettings-operation.md)

