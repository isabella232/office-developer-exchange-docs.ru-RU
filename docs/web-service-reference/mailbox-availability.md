---
title: Почтовый ящик (доступность)
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
description: Представляет элемент почтового ящика пользователя почтового ящика для SetUserOofSettings или GetUserOofSettings запроса.
ms.openlocfilehash: 2e901ae0df56542f56f247184254294735018468
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19834254"
---
# <a name="mailbox-availability"></a>Почтовый ящик (доступность)

Представляет элемент **почтового ящика** пользователя почтового ящика для SetUserOofSettings или GetUserOofSettings запроса. 
  
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
|[Имя (EmailAddress)](name-emailaddress.md) <br/> |Представляет отображаемое имя пользователя почтового ящика. Этот элемент является необязательным в SetUserOofSettingsRequest. GetUserOofSettingsRequest возвращает этот элемент.  <br/> |
|[Адрес (строка)](address-string.md) <br/> |Представляет адрес электронной почты пользователя почтового ящика. Этот элемент обязательный.  <br/> |
|[RoutingType (EmailAddress)](routingtype-emailaddress.md) <br/> |Представляет протокол маршрутизации для сообщения. Этот элемент является необязательным в SetUserOofSettingsRequest. GetUserOofSettingsRequest возвращает этот элемент.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[GetUserOofSettingsRequest](getuseroofsettingsrequest.md) <br/> |Используется для получения параметров из Office (OOF) и сообщения пользователя почтового ящика.  <br/> Ниже приведен выражение XPath для этого элемента.  <br/>  `/GetUserOofSettingsRequest` <br/> |
|[SetUserOofSettingsRequest](setuseroofsettingsrequest.md) <br/> |Используется для задания параметров об отсутствии на работе и сообщения пользователя почтового ящика.  <br/> Ниже приведен выражение XPath для этого элемента.  <br/>  `/SetUserOofSettingsRequest` <br/> |
   
## <a name="remarks"></a>Замечания

Адрес электронной почты используется для идентификации в папке календаря, содержащим параметры об отсутствии на работе. 
  
Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Операция GetUserOofSettings](getuseroofsettings-operation.md)
- [Операция SetUserOofSettings](setuseroofsettings-operation.md)

