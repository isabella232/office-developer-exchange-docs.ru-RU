---
title: TTL (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: 178eefa1-995c-4bea-930b-e51293961191
description: Элемент TTL указывает время для жизни в часах, в течение которых параметры остаются действительными.
ms.openlocfilehash: 6850f104fe90ae941f9d1d522fa3d3641e433c5f
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59515105"
---
# <a name="ttl-pox"></a>TTL (POX)

Элемент **TTL** указывает время для жизни в часах, в течение которых параметры остаются действительными. 
  
[AutoDiscover (POX)](autodiscover-pox.md)
  
[Response (POX)](response-pox.md)
  
[Account (POX)](account-pox.md)
  
[Protocol (POX)](protocol-pox.md)
  
[TTL (POX)](ttl-pox.md)
  
```xml
<TTL/>
```

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Protocol (POX)](protocol-pox.md) <br/> |Содержит спецификации для подключения клиента к компьютеру 2007 Exchange Server, на котором установлена роль сервера клиентского доступа.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение представляет время для жизни в часах, в течение которых параметры остаются действительными. Значение нуля указывает на то, что зановое открытие не требуется. Если не указано значение, значение по умолчанию для этого элемента составляет 1 час.
  
## <a name="remarks"></a>Заметки

После окончания времени, которое представлено элементом **TTL,** параметры должны быть заново открыты с помощью запроса автооткрытия. 
  
## <a name="see-also"></a>См. также



[Элементы XML автооткрытия POX для Exchange](pox-autodiscover-xml-elements-for-exchange.md)

