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
ms.openlocfilehash: fe15054b9962fc2decf52ac3c42536e36358948a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835020"
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

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
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

