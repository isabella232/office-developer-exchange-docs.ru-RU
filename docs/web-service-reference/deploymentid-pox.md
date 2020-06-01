---
title: Деплойментид (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: b879c134-307e-4645-bb53-55d8ba4fad9c
description: Элемент Деплойментид однозначно идентифицирует лес Microsoft Exchange Server 2007.
ms.openlocfilehash: 4986a3404763e88fb3e84d52a5d30d54c810f93a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44467923"
---
# <a name="deploymentid-pox"></a>Деплойментид (POX)

Элемент **деплойментид** однозначно идентифицирует лес Microsoft Exchange Server 2007. 
  
- [Служба автообнаружения (POX)](autodiscover-pox.md)  
- [Ответ (POX)](response-pox.md) 
- [Пользователь (POX)](user-pox.md)  
- [Деплойментид (POX)](deploymentid-pox.md)
  
```xml
<DeploymentId/>
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
|[Пользователь (POX)](user-pox.md) <br/> |Предоставляет сведения, относящиеся к пользователю.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение однозначно определяет лес Exchange 2007 в формате GUID.
  
## <a name="remarks"></a>Примечания

Если вы удаляете и затем переустанавливаете Exchange 2007 и используете одно и то же имя сервера, значение **деплойментид** изменяется. 
  
## <a name="see-also"></a>См. также

- [XML-элементы автообнаружения POX для Exchange](pox-autodiscover-xml-elements-for-exchange.md)

