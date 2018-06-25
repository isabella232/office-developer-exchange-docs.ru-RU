---
title: Домен (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 849629a0-0467-422f-88f6-3b8a95c17bba
description: Элемент домена содержит федеративного домена в ответ GetFederationInformation или домена, параметры конфигурации, для которого запрашивается в запросе GetDomainSettings.
ms.openlocfilehash: 411ca866800322ef06eeecc2ab92adc6f711917c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762203"
---
# <a name="domain-soap"></a>Домен (SOAP)

Элемент **домена** содержит федеративного домена в ответ **GetFederationInformation** или домена, параметры конфигурации, для которого запрашивается в запросе **GetDomainSettings** . 
  
```XML
<Domain/> 
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
|[Домены (SOAP)](domains-soap.md) <br/> |Представляет доменов, параметры конфигурации, для которого возвращаются в ходе операции **GetDomainSettings** или домены, которые организации федеративных в **GetFederationInformation** операции.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение элемента **домена** представляет имя домена. 
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Имя схемы  <br/> |Схема службы автообнаружения  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |True  <br/> |
   

