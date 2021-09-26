---
title: Name (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: dce6d823-dc33-4a47-babe-6370a15ac7b4
description: Элемент Name представляет имя параметра.
ms.openlocfilehash: 39bb2b6bbf7e29dedb13a9bf828f130c076dfb6b
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59541996"
---
# <a name="name-soap"></a>Name (SOAP)

Элемент **Name** представляет имя параметра. 
  
```XML
<Name/>
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
|[DomainSetting (SOAP)](domainsetting-soap.md) <br/> |Содержит параметры домена, возвращаемые по запросу [Операции GetDomainSettings (SOAP).](getdomainsettings-operation-soap.md)  <br/> |
|[DomainStringSetting (SOAP)](domainstringsetting-soap.md) <br/> |Представляет домен, значение которого — строка типа.  <br/> |
|[OrganizationRelationshipSettings (SOAP)](organizationrelationshipsettings-soap.md) <br/> |Представляет список отношений организации для одной организации.  <br/> |
|[UserSetting (SOAP)](usersetting-soap.md) <br/> |Представляет один параметр пользователя.  <br/> |
|[ProtocolConnectionCollectionSetting (SOAP)](protocolconnectioncollectionsetting-soap.md) <br/> |Представляет коллекцию параметров подключения к протоколу сервера.  <br/> |
|[StringSetting (SOAP)](stringsetting-soap.md) <br/> |Представляет пользователя, заметив значение, для которого имеется строка типа.  <br/> |
|[WebClientUrlCollectionSetting (SOAP)](webclienturlcollectionsetting-soap.md) <br/> |Представляет параметр пользователя, который представляет коллекцию URL-адресов Exchange веб-клиентов.  <br/> |
|[AlternateMailboxCollectionSetting (SOAP)](alternatemailboxcollectionsetting-soap.md) <br/> |Содержит коллекцию параметров альтернативных почтовых ящиков.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение элемента **Name** — это имя параметра. 
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Имя схемы  <br/> |Схема автооткрытия  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |True  <br/> |
   
## <a name="see-also"></a>См. также

- [Операция GetDomainSettings (SOAP)](getdomainsettings-operation-soap.md)
- [Операция GetUserSettings (SOAP)](getusersettings-operation-soap.md)
- [Операция GetFederationInformation (SOAP)](getfederationinformation-operation-soap.md)
- [Операция GetOrganizationRelationshipSettings (SOAP)](getorganizationrelationshipsettings-operation-soap.md)

