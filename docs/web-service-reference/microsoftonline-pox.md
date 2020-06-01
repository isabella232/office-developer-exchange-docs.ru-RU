---
title: MicrosoftOnline (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 0b88f02a-9c50-44b3-841b-560b24e37af5
description: Элемент MicrosoftOnline содержит значение, которое указывает, размещается ли почтовый ящик пользователя в Exchange Online или Exchange Online в составе Office 365.
ms.openlocfilehash: f3144a673a4c98aad821e21c562141b0ae00f426
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44467986"
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

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

Отсутствуют.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Учетная запись (POX)](account-pox.md) <br/> |Задает параметры учетной записи пользователя или содержит ошибочные ответы.  <br/> |
   
## <a name="remarks"></a>Примечания

Текстовое значение указывает, размещен ли почтовый ящик пользователя в Exchange Online. Значение **true** , если почтовый ящик пользователя размещен в Exchange Online; в противном случае — **false**.
  
## <a name="see-also"></a>См. также



[XML-элементы автообнаружения POX для Exchange](pox-autodiscover-xml-elements-for-exchange.md)

