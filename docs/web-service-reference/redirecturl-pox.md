---
title: RedirectUrl адресом (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: c54f310f-8c99-4c37-8e73-ac87722b6229
description: Элемент redirectUrl адресом содержит URL-адрес компьютера, на котором работает Microsoft Exchange Server 2007 с установленной ролью сервера клиентского доступа, который следует использовать для получения параметров автообнаружения.
ms.openlocfilehash: 3b634f1a3a3d44b6aae1a826a005149200641dcb
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835027"
---
# <a name="redirecturl-pox"></a>RedirectUrl адресом (POX)

Элемент **redirectUrl адресом** содержит URL-адрес компьютера, на котором работает Microsoft Exchange Server 2007 с установленной ролью сервера клиентского доступа, который следует использовать для получения параметров автообнаружения. 
  
[Служба автообнаружения (POX)](autodiscover-pox.md)
  
[Ответ (POX)](response-pox.md)
  
[Учетная запись (POX)](account-pox.md)
  
[RedirectUrl адресом (POX)](redirecturl-pox.md)
  
```xml
<RedirectUrl/>
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

Текстовое значение представляет URL-адрес сервера клиентского доступа, который должен использоваться для получения параметров автообнаружения.
  
## <a name="remarks"></a>Примечания

Клиентское приложение должно прекратить перенаправление после 10 перенаправлений.
  
## <a name="see-also"></a>См. также



[XML-элементы автообнаружения POX для Exchange](pox-autodiscover-xml-elements-for-exchange.md)

