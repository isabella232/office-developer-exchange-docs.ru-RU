---
title: Имя (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: dce6d823-dc33-4a47-babe-6370a15ac7b4
description: Элемент Name представляет имя параметра.
ms.openlocfilehash: 74e6d6b59d972d7230c23b38cd3f4a8591401bbd
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44466887"
---
# <a name="name-soap"></a>Имя (SOAP)

Элемент **Name** представляет имя параметра. 
  
```XML
<Name/>
```

**строка**

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

Отсутствуют.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Домаинсеттинг (SOAP)](domainsetting-soap.md) <br/> |Содержит параметры домена, которые возвращаются запросом [операции жетдомаинсеттингс (SOAP)](getdomainsettings-operation-soap.md) .  <br/> |
|[Домаинстрингсеттинг (SOAP)](domainstringsetting-soap.md) <br/> |Представляет параметр домена со значением типа String.  <br/> |
|[Организатионрелатионшипсеттингс (SOAP)](organizationrelationshipsettings-soap.md) <br/> |Представляет список отношений Организации для одной организации.  <br/> |
|[Усерсеттинг (SOAP)](usersetting-soap.md) <br/> |Представляет один параметр пользователя.  <br/> |
|[Протоколконнектионколлектионсеттинг (SOAP)](protocolconnectioncollectionsetting-soap.md) <br/> |Представляет коллекцию параметров подключения по протоколу сервера.  <br/> |
|[Стрингсеттинг (SOAP)](stringsetting-soap.md) <br/> |Представляет пользовательское значение, для которого задано значение типа String.  <br/> |
|[Вебклиентурлколлектионсеттинг (SOAP)](webclienturlcollectionsetting-soap.md) <br/> |Представляет параметр пользователя, который является коллекцией URL-адресов веб-клиента Exchange.  <br/> |
|[Алтернатемаилбоксколлектионсеттинг (SOAP)](alternatemailboxcollectionsetting-soap.md) <br/> |Содержит коллекцию альтернативных параметров почтового ящика.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение элемента **Name** — имя параметра. 
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Имя схемы  <br/> |Схема автообнаружения  <br/> |
|Файл проверки  <br/> |Messages. xsd  <br/> |
|Может быть пустым  <br/> |True  <br/> |
   
## <a name="see-also"></a>См. также

- [Операция Жетдомаинсеттингс (SOAP)](getdomainsettings-operation-soap.md)
- [Операция GetUserSettings (SOAP)](getusersettings-operation-soap.md)
- [Операция Жетфедератионинформатион (SOAP)](getfederationinformation-operation-soap.md)
- [Операция Жеторганизатионрелатионшипсеттингс (SOAP)](getorganizationrelationshipsettings-operation-soap.md)

