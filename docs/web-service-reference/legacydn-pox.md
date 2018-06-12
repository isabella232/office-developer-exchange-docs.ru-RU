---
title: LegacyDN (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 9fb9529f-52c5-4907-a84b-935b78de16c3
description: Элемент LegacyDN определяет почтовый ящик пользователя с устаревшее различающееся имя.
ms.openlocfilehash: f7ec1dea29a7d3ad6d470ef7812390d179fe1d2a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19834243"
---
# <a name="legacydn-pox"></a>LegacyDN (POX)

Элемент **LegacyDN** определяет почтовый ящик пользователя с устаревшее различающееся имя. 
  
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
|[Запрос (POX)](request-pox.md) <br/> |Содержит запрос к службе автообнаружения.  <br/> |
|[Пользователь (POX)](user-pox.md) <br/> |Предоставляет сведения о пользователе.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение представляет адреса прежних версий электронной почты пользователя.
  
## <a name="remarks"></a>Замечания

Элемент [EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) — это Замещающий элемент для запроса службы автообнаружения. Он используется, когда почтовый ящик существует на компьютере, на котором выполняется Microsoft Exchange Server 2007. 
  
## <a name="see-also"></a>См. также

- [Элементы XML автоматического обнаружения POX для Exchange](pox-autodiscover-xml-elements-for-exchange.md)

