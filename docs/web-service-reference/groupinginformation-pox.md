---
title: GroupingInformation (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
ms.assetid: 2d8a007f-d79c-43c8-90e3-2c6d883f3a7c
description: Элемент GroupingInformation содержит значение, которое используется для группировки почтового ящика пользователя для сохранения сродства при подписке на уведомления в нескольких почтовых ящиках.
ms.openlocfilehash: 14e751adcd0b966907ce495a2753b2b26d812a86
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59525886"
---
# <a name="groupinginformation-pox"></a>GroupingInformation (POX)

Элемент **GroupingInformation** содержит значение, которое используется для группировки [](https://msdn.microsoft.com/library/1bda4094-88c3-4f61-9219-6ee70f6e81cf%28Office.15%29.aspx) почтового ящика пользователя для сохранения сродства при подписке на уведомления в нескольких почтовых ящиках. 
  
[AutoDiscover (POX)](autodiscover-pox.md)
  
[Response (POX)](response-pox.md)
  
[Account (POX)](account-pox.md)
  
[Protocol (POX)](protocol-pox.md)
  
[GroupingInformation (POX)](groupinginformation-pox.md)
  
```XML
<GroupingInformation/>
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
|[Protocol (POX)](protocol-pox.md) <br/> |Содержит спецификации для подключения клиента к Exchange серверу.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение сравнивается со значением элемента **GroupingInformation** для других почтовых ящиков. Почтовые ящики, которые имеют одинаковое значение и используют ту же конечную точку Exchange веб-службы (EWS), можно сгруппить для сохранения сродства. Дополнительные сведения см. в [материале Maintain affinity between a group of subscriptions and the Mailbox server in Exchange.](https://msdn.microsoft.com/library/1bda4094-88c3-4f61-9219-6ee70f6e81cf%28Office.15%29.aspx)
  
## <a name="remarks"></a>Заметки

Элемент **GroupingInformation** применим только к элементам **Протокола,** которые имеют детский элемент [Type (POX)](type-pox.md) со значением "EXPR". 
  
## <a name="see-also"></a>См. также

- [Элементы XML автооткрытия POX для Exchange](pox-autodiscover-xml-elements-for-exchange.md)
- [Поддержание сходства между группой подписок и сервером почтовых ящиков в Exchange](https://msdn.microsoft.com/library/1bda4094-88c3-4f61-9219-6ee70f6e81cf%28Office.15%29.aspx)

