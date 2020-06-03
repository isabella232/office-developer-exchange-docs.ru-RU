---
title: Редиректаддр (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 0e9fa6b6-7991-4dc1-a59a-48e5f8e041e4
description: Элемент Редиректаддр указывает адрес электронной почты, который будет использоваться для последующего запроса автообнаружения.
ms.openlocfilehash: 6bff28001851f421b4c7429770185401f2f0a743
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529877"
---
# <a name="redirectaddr-pox"></a>Редиректаддр (POX)

Элемент **редиректаддр** указывает адрес электронной почты, который будет использоваться для последующего запроса автообнаружения. 
  
[Служба автообнаружения (POX)](autodiscover-pox.md)
  
[Ответ (POX)](response-pox.md)
  
[Учетная запись (POX)](account-pox.md)
  
[Редиректаддр (POX)](redirectaddr-pox.md)
  
```xml
<RedirectAddr/>
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
|[Учетная запись (POX)](account-pox.md) <br/> |Задает параметры учетной записи пользователя.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение представляет адрес электронной почты, который будет использоваться для последующего запроса автообнаружения.
  
## <a name="remarks"></a>Примечания

Если этот элемент присутствует в ответе автообнаружения, выполните другой запрос, используя текстовое значение элемента **редиректаддр** . 
  
## <a name="see-also"></a>См. также



[XML-элементы автообнаружения POX для Exchange](pox-autodiscover-xml-elements-for-exchange.md)

