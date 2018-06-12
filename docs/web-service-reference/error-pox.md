---
title: Ошибка (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 91c63b62-ab68-4c32-a2f7-5a87c188335b
description: Элемент ошибки содержит возврату ошибки службы автообнаружения.
ms.openlocfilehash: 3135a352365fe3000ce2d202ad78452d5c8ccc7f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762376"
---
# <a name="error-pox"></a>Ошибка (POX)

Элемент **ошибки** содержит возврату ошибки службы автообнаружения. 
  
[Автообнаружение (POX)](autodiscover-pox.md)
  
[Ответ (POX)](response-pox.md)
  
[Учетная запись (POX)](account-pox.md)
  
[Ошибка (POX)](error-pox.md)
  
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
|Время  <br/> |Представляет время, когда была возвращена ошибка ответа.  <br/> |
|Id  <br/> |Представляет хэш-имя компьютера, на котором выполняется Microsoft Exchange Server 2007 с установленной ролью сервера клиентского доступа.  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Код ошибки (POX)](errorcode-pox.md) <br/> |Содержит код ошибки для ошибки ответа службы автообнаружения.  <br/> |
|[Сообщение (POX)](message-pox.md) <br/> |Содержит сообщение об ошибке Ошибка ответа службы автообнаружения.  <br/> |
|[DebugData (POX)](debugdata-pox.md) <br/> |Содержит данные отладки при возникновении ошибки ответа службы автообнаружения.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Учетная запись (POX)](account-pox.md) <br/> |Содержит возврату ошибки службы автообнаружения.  <br/> |
   
## <a name="see-also"></a>См. также



[Элементы XML автоматического обнаружения POX для Exchange](pox-autodiscover-xml-elements-for-exchange.md)

