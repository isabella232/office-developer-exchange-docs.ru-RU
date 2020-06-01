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
ms.openlocfilehash: 5400b1e7a4bb7ebebc58b6a0f1fc9bf37f5a2e22
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44468091"
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

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

Отсутствуют.
  
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

