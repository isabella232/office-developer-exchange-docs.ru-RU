---
title: OrganizationRelationshipSettingsCollection (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 33456abf-a1b6-46da-a864-3ec8af2780de
description: Элемент OrganizationRelationshipSettingsCollection представляет список отношений организации, которые соответствуют запроса. Элемент OrganizationRelationshipSettingsCollection — только для внутреннего использования. Этот элемент не используется с клиентами.
ms.openlocfilehash: 18e71ce39d48598868d677a37d5ba439fa6d59c4
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834663"
---
# <a name="organizationrelationshipsettingscollection-soap"></a>OrganizationRelationshipSettingsCollection (SOAP)

Элемент **OrganizationRelationshipSettingsCollection** представляет список отношений организации, которые соответствуют запроса. Элемент **OrganizationRelationshipSettingsCollection** — только для внутреннего использования. Этот элемент не используется с клиентами. 
  
```XML
<OrganizationRelationshipSettingsCollection>
   <OrganizationRelationshipSettings/>
</OrganizationRelationshipSettingsCollection>
```

 **OrganizationRelationshipSettingsCollection**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[OrganizationRelationshipSettings (SOAP)](organizationrelationshipsettings-soap.md) <br/> |Представляет список отношения организации для выбранного организации и SMTP-адреса.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Ответ (GetOrganizationRelationship) (SOAP)](response-getorganizationrelationshipsoap.md) <br/> |Содержит сведения, ответа [GetOrganizationRelationshipSettings операции (SOAP)](getorganizationrelationshipsettings-operation-soap.md) .  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Нет.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Имя схемы  <br/> |Схема службы автообнаружения  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |True  <br/> |
   
## <a name="see-also"></a>См. также



[Операция GetOrganizationRelationshipSettings (SOAP)](getorganizationrelationshipsettings-operation-soap.md)

