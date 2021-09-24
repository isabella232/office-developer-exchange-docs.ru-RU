---
title: RedirectAddr (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: 0e9fa6b6-7991-4dc1-a59a-48e5f8e041e4
description: Элемент RedirectAddr указывает адрес электронной почты, который следует использовать для последующего запроса автооткрытия.
ms.openlocfilehash: 75db62a84ccce743e73c812082ab9dbbc4fdb1cd
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59540596"
---
# <a name="redirectaddr-pox"></a>RedirectAddr (POX)

Элемент **RedirectAddr** указывает адрес электронной почты, который следует использовать для последующего запроса автооткрытия. 
  
[AutoDiscover (POX)](autodiscover-pox.md)
  
[Response (POX)](response-pox.md)
  
[Account (POX)](account-pox.md)
  
[RedirectAddr (POX)](redirectaddr-pox.md)
  
```xml
<RedirectAddr/>
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
|[Account (POX)](account-pox.md) <br/> |Указывает параметры учетной записи для пользователя.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение представляет адрес электронной почты, который следует использовать для последующего запроса автооткрытия.
  
## <a name="remarks"></a>Заметки

Если этот элемент присутствует в ответе автооткрытия, сделайте другой запрос, используя текстовое значение элемента **RedirectAddr.** 
  
## <a name="see-also"></a>См. также



[Элементы XML автооткрытия POX для Exchange](pox-autodiscover-xml-elements-for-exchange.md)

