---
title: Запрос (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: da54eb32-7ce5-4384-9893-255a2243a959
description: Элемент Request содержит запрос к службе автообнаружения.
ms.openlocfilehash: 3f5d5258a92840fe79c4936370323b78aa4715b3
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/28/2018
ms.locfileid: "21354430"
---
# <a name="request-pox"></a>Запрос (POX)

Элемент **request** содержит запрос к службе автообнаружения. 
  
- [Служба автообнаружения (POX)](autodiscover-pox.md) 
- [Запрос (POX)](request-pox.md)
  
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

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Акцептаблереспонсесчема (POX)](acceptableresponseschema-pox.md) <br/> |Определяет схему ответа автообнаружения.  <br/> |
|[EmailAddress (Нонемптистрингтипе)](emailaddress-nonemptystringtype.md) <br/> |Определяет адрес электронной почты пользователя.  <br/> |
|[LegacyDN (POX)](legacydn-pox.md) <br/> |Определяет почтовый ящик пользователя, используя устаревшее различающееся имя.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Служба автообнаружения (POX)](autodiscover-pox.md) <br/> |Корневой элемент запроса на обнаружение.  <br/> |
   
## <a name="see-also"></a>См. также

- [XML-элементы автообнаружения POX для Exchange](pox-autodiscover-xml-elements-for-exchange.md)

