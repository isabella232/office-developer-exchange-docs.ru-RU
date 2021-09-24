---
title: Domains (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: 5f81d1b7-c6a4-456f-9935-13d04a3d92d7
description: Элемент Domains представляет коллекцию доменов, возвращаемую в операции GetDomainSettings (SOAP), домены, которые организация федераторила в операции GetFederationInformation (SOAP), или домены с отношением организации, возвращенные операцией GetOrganizationRelationshipSettings (SOAP).
ms.openlocfilehash: 667b2611ce8b393252f9bdda6dd7ec201b605047
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59538325"
---
# <a name="domains-soap"></a>Domains (SOAP)

Элемент **Domains** представляет коллекцию доменов, возвращаемую в операции [GetDomainSettings (SOAP),](getdomainsettings-operation-soap.md)домены, которые организация федераторила в операции [GetFederationInformation (SOAP)](getfederationinformation-operation-soap.md)или домены с отношениями организации, возвращаемые операцией [GetOrganizationRelationshipSettings (SOAP).](getorganizationrelationshipsettings-operation-soap.md)
  
```XML
<Domains>
   <Domain/>
</Domains>
```

 **Домены**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Domain (SOAP)](domain-soap.md) <br/> |Представляет один домен.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[GetDomainSettingsRequest (SOAP)](getdomainsettingsrequest-soap.md) <br/> |Представляет запрос [на операцию GetDomainSettings (SOAP).](getdomainsettings-operation-soap.md)  <br/> |
|[Response (GetFederationInformation) (SOAP)](response-getfederationinformationsoap.md) <br/> |Содержит сведения [о ответе операции GetFederationInformation (SOAP).](getfederationinformation-operation-soap.md)  <br/> |
|[GetOrganizationRelationshipSettingsRequest (SOAP)](getorganizationrelationshipsettingsrequest-soap.md) <br/> |Представляет запрос [на операцию GetOrganizationRelationshipSettings (SOAP).](getorganizationrelationshipsettings-operation-soap.md)  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Нет.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Имя схемы  <br/> |Схема автооткрытия  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |True  <br/> |
   
## <a name="see-also"></a>См. также

- [GetDomainSettingsRequest (SOAP)](getdomainsettingsrequest-soap.md)  
- [GetFederationInformationResponse (SOAP)](getfederationinformationresponse-soap.md)

