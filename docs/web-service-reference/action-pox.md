---
title: Action (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: a3462c6b-453c-462a-830d-f29ee4a2babb
description: Элемент Action предоставляет сведения, которые используются для определения того, требуется ли другой запрос автооткрытия для возврата сведений о конфигурации пользователя.
ms.openlocfilehash: b1c07fefc6b8033b9b93bd044c04fb07ba289177
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59513859"
---
# <a name="action-pox"></a>Action (POX)

Элемент **Action** предоставляет сведения, которые используются для определения того, требуется ли другой запрос автооткрытия для возврата сведений о конфигурации пользователя. 
  
- [AutoDiscover (POX)](autodiscover-pox.md)
  
- [Response (POX)](response-pox.md)
  
- [Account (POX)](account-pox.md)
  
- [Action (POX)](action-pox.md)
  
```xml
<Action>redirectUrl or redirectAddr or settings</Action>
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

Текстовое значение представляет, необходим ли другой запрос автооткрытия для получения сведений о конфигурации пользователя. В следующей таблице перечислены возможные значения.
  
|**Значение**|**Описание**|
|:-----|:-----|
|redirectUrl  <br/> |Если это значение задано, элемент [RedirectUrl (POX)](redirecturl-pox.md) укавит URL-адрес сервера клиентского доступа, который будет использоваться в последующем запросе автооткрытия. Клиентская заявка должна прекратить перенаправление после 10 перенаправлений.  <br/> |
|redirectAddr  <br/> |Если это значение задано, элемент [RedirectAddr (POX)](redirectaddr-pox.md) указывает адрес электронной почты, который следует использовать для последующего запроса автооткрытия.  <br/> |
|settings  <br/> |Если это значение задано, ответ автооткрытия содержит параметры, используемые для настройки учетной записи. Большинство параметров можно найти в элементе [Protocol (POX).](protocol-pox.md)  <br/> |
   
## <a name="see-also"></a>См. также

- [Элементы XML автооткрытия POX для Exchange](pox-autodiscover-xml-elements-for-exchange.md)

