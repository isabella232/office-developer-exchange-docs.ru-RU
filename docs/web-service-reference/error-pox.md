---
title: Error (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: 91c63b62-ab68-4c32-a2f7-5a87c188335b
description: Элемент Error содержит ответ на ошибку автонаруже.
ms.openlocfilehash: 2f96f8b9d6d154aac6f10924095b5a5864e76750
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59530891"
---
# <a name="error-pox"></a>Error (POX)

Элемент **Error** содержит ответ на ошибку автонаруже. 
  
[AutoDiscover (POX)](autodiscover-pox.md)
  
[Response (POX)](response-pox.md)
  
[Account (POX)](account-pox.md)
  
[Error (POX)](error-pox.md)
  
```xml
<Error Time="" Id="">
   <ErrorCode/>
   <Message/>
   <DebugData/>
</Error>
```

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|Time  <br/> |Представляет время, когда был возвращен ответ на ошибку.  <br/> |
|Id  <br/> |Представляет собой хаш имени компьютера, запущенного Microsoft Exchange Server 2007 года с установленной ролью сервера клиентского доступа.  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[ErrorCode (POX)](errorcode-pox.md) <br/> |Содержит код ошибки для ответа автооткрытия ошибки.  <br/> |
|[Message (POX)](message-pox.md) <br/> |Содержит сообщение об ошибке для ответа автооткрытия ошибки.  <br/> |
|[DebugData (POX)](debugdata-pox.md) <br/> |Содержит данные отлаговки для ответа автообнаружаемой ошибки.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Account (POX)](account-pox.md) <br/> |Содержит ответ на ошибку автонаруже.  <br/> |
   
## <a name="see-also"></a>См. также



[Элементы XML автооткрытия POX для Exchange](pox-autodiscover-xml-elements-for-exchange.md)

