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
description: Элемент LegacyDN определяет почтовый ящик пользователя по устаревшему различающеу имени.
ms.openlocfilehash: b9af4278a5421dc932573396c3563a64a78de41e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44526384"
---
# <a name="legacydn-pox"></a>LegacyDN (POX)

Элемент **LegacyDN** определяет почтовый ящик пользователя по устаревшему различающеу имени. 
  
```xml
<LegacyDN/>
```

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

Отсутствуют.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Запрос (POX)](request-pox.md) <br/> |Содержит запрос к службе автообнаружения.  <br/> |
|[Пользователь (POX)](user-pox.md) <br/> |Предоставляет сведения, относящиеся к пользователю.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение представляет устаревший адрес электронной почты пользователя.
  
## <a name="remarks"></a>Примечания

Элемент [EmailAddress (нонемптистрингтипе)](emailaddress-nonemptystringtype.md) является альтернативным элементом для запроса автообнаружения. Он используется при наличии почтового ящика на компьютере под управлением Microsoft Exchange Server 2007. 
  
## <a name="see-also"></a>См. также

- [XML-элементы автообнаружения POX для Exchange](pox-autodiscover-xml-elements-for-exchange.md)

