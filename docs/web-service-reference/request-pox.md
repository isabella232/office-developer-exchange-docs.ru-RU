---
title: Request (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: da54eb32-7ce5-4384-9893-255a2243a959
description: Элемент запрос содержит запрос к службе автообнаружения.
ms.openlocfilehash: 3f5d5258a92840fe79c4936370323b78aa4715b3
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/28/2018
ms.locfileid: "21354430"
---
# <a name="request-pox"></a>Request (POX)

Элемент **запрос** содержит запрос к службе автообнаружения. 
  
- [AutoDiscover (POX)](autodiscover-pox.md) 
- [Request (POX)](request-pox.md)
  
```xml
<Request>
   <AcceptableResponseSchema/>
   <EMailAddress/>
</Request>
```

```xml
<Request>
   <AcceptableResponseSchema/> 
   <LegacyDN/>
</Request>
```

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[AcceptableResponseSchema (POX)](acceptableresponseschema-pox.md) <br/> |Определяет схему для ответа на службы автообнаружения.  <br/> |
|[EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) <br/> |Указывает адрес электронной почты пользователя.  <br/> |
|[LegacyDN (POX)](legacydn-pox.md) <br/> |Определяет, устаревшее различающееся имя почтового ящика пользователя.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[AutoDiscover (POX)](autodiscover-pox.md) <br/> |Корневой элемент в запросе службы автообнаружения.  <br/> |
   
## <a name="see-also"></a>См. также

- [Элементы XML автоматического обнаружения POX для Exchange](pox-autodiscover-xml-elements-for-exchange.md)

