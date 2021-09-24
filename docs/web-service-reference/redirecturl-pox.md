---
title: RedirectUrl (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: c54f310f-8c99-4c37-8e73-ac87722b6229
description: Элемент RedirectUrl содержит URL-адрес компьютера 2007 Microsoft Exchange Server 2007 года с установленной ролью сервера клиентского доступа, который следует использовать для получения параметров автооткрытия.
ms.openlocfilehash: d515f3f79f2370dc496614bab0a3f77300ad4e30
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59513530"
---
# <a name="redirecturl-pox"></a>RedirectUrl (POX)

Элемент **RedirectUrl** содержит URL-адрес компьютера, на Microsoft Exchange Server 2007 года с установленной ролью сервера клиентского доступа, который следует использовать для получения параметров автооткрытия. 
  
[AutoDiscover (POX)](autodiscover-pox.md)
  
[Response (POX)](response-pox.md)
  
[Account (POX)](account-pox.md)
  
[RedirectUrl (POX)](redirecturl-pox.md)
  
```xml
<RedirectUrl/>
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

Текстовое значение представляет URL-адрес сервера клиентского доступа, который необходимо использовать для получения параметров автооткрытия.
  
## <a name="remarks"></a>Заметки

Клиентская заявка должна прекратить перенаправление после 10 перенаправлений.
  
## <a name="see-also"></a>См. также



[Элементы XML автооткрытия POX для Exchange](pox-autodiscover-xml-elements-for-exchange.md)

