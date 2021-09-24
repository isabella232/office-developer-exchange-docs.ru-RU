---
title: LegacyDN (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: 9fb9529f-52c5-4907-a84b-935b78de16c3
description: Элемент LegacyDN идентифицирует почтовый ящик пользователя по устаревшему имени.
ms.openlocfilehash: bd65e18daf1b05f66ebd767635cbe6a3135f1abf
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59540834"
---
# <a name="legacydn-pox"></a>LegacyDN (POX)

Элемент **LegacyDN** идентифицирует почтовый ящик пользователя по устаревшему имени. 
  
```xml
<LegacyDN/>
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
|[Request (POX)](request-pox.md) <br/> |Содержит запрос в службу автооткрытия.  <br/> |
|[User (POX)](user-pox.md) <br/> |Предоставляет сведения о пользователях.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение представляет устаревший адрес электронной почты пользователя.
  
## <a name="remarks"></a>Заметки

Элемент [EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) является альтернативным элементом запроса автооткрытия. Он используется, когда почтовый ящик существует на компьютере, который Microsoft Exchange Server 2007. 
  
## <a name="see-also"></a>См. также

- [Элементы XML автооткрытия POX для Exchange](pox-autodiscover-xml-elements-for-exchange.md)

