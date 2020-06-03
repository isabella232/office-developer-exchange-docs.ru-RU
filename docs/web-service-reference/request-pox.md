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
ms.openlocfilehash: bc215d614441ed8f12c0f1490f4abdbb7b574ad0
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459548"
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

Отсутствуют.
  
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

