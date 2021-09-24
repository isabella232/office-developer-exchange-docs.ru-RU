---
title: Domain (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: 849629a0-0467-422f-88f6-3b8a95c17bba
description: Элемент Domain содержит федерационный домен в ответе GetFederationInformation или содержит домен, параметры конфигурации которого запрашиваются в запросе GetDomainSettings.
ms.openlocfilehash: a2e69dc845f9841931263fe90e39550bceb81ab8
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59520824"
---
# <a name="domain-soap"></a>Domain (SOAP)

Элемент **Domain** содержит федерационный домен в **ответе GetFederationInformation** или содержит домен, параметры конфигурации которого запрашиваются в **запросе GetDomainSettings.** 
  
```XML
<Domain/> 
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
|[Domains (SOAP)](domains-soap.md) <br/> |Представляет домены, параметры конфигурации для которых возвращаются в операции **GetDomainSettings** или домены, которые организация федерационная в операции **GetFederationInformation.**  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение элемента **Domain** представляет доменное имя. 
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Имя схемы  <br/> |Схема автооткрытия  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |True  <br/> |
   

