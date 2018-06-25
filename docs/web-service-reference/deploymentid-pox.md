---
title: DeploymentId (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: b879c134-307e-4645-bb53-55d8ba4fad9c
description: Элемент DeploymentId однозначно определяет леса Microsoft Exchange Server 2007.
ms.openlocfilehash: 4f2548709753d8407d02218acecd9233f0ba764f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762069"
---
# <a name="deploymentid-pox"></a>DeploymentId (POX)

Элемент **DeploymentId** однозначно определяет леса Microsoft Exchange Server 2007. 
  
- [Автообнаружение (POX)](autodiscover-pox.md)  
- [Ответ (POX)](response-pox.md) 
- [Пользователь (POX)](user-pox.md)  
- [DeploymentId (POX)](deploymentid-pox.md)
  
```xml
<DeploymentId/>
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
|[Пользователь (POX)](user-pox.md) <br/> |Предоставляет сведения о пользователе.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение однозначно определяет леса Exchange 2007 в формате GUID.
  
## <a name="remarks"></a>Замечания

Если удалить и переустановить Exchange 2007 и использовать то же имя сервера, возвращается значение **DeploymentId** . 
  
## <a name="see-also"></a>См. также

- [Элементы XML автоматического обнаружения POX для Exchange](pox-autodiscover-xml-elements-for-exchange.md)

