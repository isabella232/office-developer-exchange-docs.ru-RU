---
title: DeploymentId (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: b879c134-307e-4645-bb53-55d8ba4fad9c
description: Элемент DeploymentId уникально определяет лес Microsoft Exchange Server 2007 года.
ms.openlocfilehash: 37d66eadb38f02e75a35d0516b36aff07dfdafa6
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59545358"
---
# <a name="deploymentid-pox"></a>DeploymentId (POX)

Элемент **DeploymentId** уникально определяет лес Microsoft Exchange Server 2007 года. 
  
- [AutoDiscover (POX)](autodiscover-pox.md)  
- [Response (POX)](response-pox.md) 
- [User (POX)](user-pox.md)  
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
|[User (POX)](user-pox.md) <br/> |Предоставляет сведения о пользователях.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение уникально определяет лес 2007 Exchange в формате GUID.
  
## <a name="remarks"></a>Заметки

Если удалить и переустановить Exchange 2007 и использовать одно имя сервера, значение **DeploymentId** изменится. 
  
## <a name="see-also"></a>См. также

- [Элементы XML автооткрытия POX для Exchange](pox-autodiscover-xml-elements-for-exchange.md)

