---
title: MicrosoftOnline (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 0b88f02a-9c50-44b3-841b-560b24e37af5
description: Элемент MicrosoftOnline содержит значение, которое указывает, размещается ли почтовый ящик пользователя в Exchange Online или Exchange Online в составе Office 365.
ms.openlocfilehash: b952bfda17b30dcf29812697d225db32718d9781
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834458"
---
# <a name="microsoftonline-pox"></a>MicrosoftOnline (POX)

Элемент **MicrosoftOnline** содержит значение, которое указывает, размещается ли почтовый ящик пользователя в Exchange Online или Exchange Online в составе Office 365. 
  
[Служба автообнаружения (POX)](autodiscover-pox.md)
  
[Ответ (POX)](response-pox.md)
  
[Учетная запись (POX)](account-pox.md)
  
[MicrosoftOnline (POX)](microsoftonline-pox.md)
  
```XML
<MicrosoftOnline/>
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
|[Учетная запись (POX)](account-pox.md) <br/> |Задает параметры учетной записи пользователя или содержит ошибочные ответы.  <br/> |
   
## <a name="remarks"></a>Примечания

Текстовое значение указывает, размещен ли почтовый ящик пользователя в Exchange Online. Значение **true** , если почтовый ящик пользователя размещен в Exchange Online; в противном случае — **false**.
  
## <a name="see-also"></a>См. также



[XML-элементы автообнаружения POX для Exchange](pox-autodiscover-xml-elements-for-exchange.md)

