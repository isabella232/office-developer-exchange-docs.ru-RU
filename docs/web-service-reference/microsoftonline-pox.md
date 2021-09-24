---
title: MicrosoftOnline (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
ms.assetid: 0b88f02a-9c50-44b3-841b-560b24e37af5
description: Элемент MicrosoftOnline содержит значение, которое указывает, размещен ли почтовый ящик пользователя в Exchange Online или Exchange Online в Office 365.
ms.openlocfilehash: fbf230df18ca488babb1523cc7f689923eaeb55b
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59510947"
---
# <a name="microsoftonline-pox"></a>MicrosoftOnline (POX)

Элемент **MicrosoftOnline** содержит значение, которое указывает, размещен ли почтовый ящик пользователя в Exchange Online или Exchange Online в Office 365. 
  
[AutoDiscover (POX)](autodiscover-pox.md)
  
[Response (POX)](response-pox.md)
  
[Account (POX)](account-pox.md)
  
[MicrosoftOnline (POX)](microsoftonline-pox.md)
  
```XML
<MicrosoftOnline/>
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
|[Account (POX)](account-pox.md) <br/> |Указывает параметры учетной записи для пользователя или содержит ответы на ошибки.  <br/> |
   
## <a name="remarks"></a>Заметки

Текстовое значение указывает, находится ли почтовый ящик пользователя в Exchange Online. Значение **верно, если** почтовый ящик пользователя находится в Exchange Online; в противном **случае, false**.
  
## <a name="see-also"></a>См. также



[Элементы XML автооткрытия POX для Exchange](pox-autodiscover-xml-elements-for-exchange.md)

