---
title: GroupingInformation (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 2d8a007f-d79c-43c8-90e3-2c6d883f3a7c
description: Элемент GroupingInformation содержит значение, которое используется для группирования почтового ящика пользователя на обслуживание сходства, когда подписка на уведомления в нескольких почтовых ящиках.
ms.openlocfilehash: bcde002c794ac79d9515befc0755c1f954ee8706
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833781"
---
# <a name="groupinginformation-pox"></a>GroupingInformation (POX)

Элемент **GroupingInformation** содержит значение, которое используется для группирования почтового ящика пользователя на [обслуживание сходства](http://msdn.microsoft.com/library/1bda4094-88c3-4f61-9219-6ee70f6e81cf%28Office.15%29.aspx) при присоединении к уведомлений в нескольких почтовых ящиках. 
  
[Автообнаружение (POX)](autodiscover-pox.md)
  
[Ответ (POX)](response-pox.md)
  
[Учетная запись (POX)](account-pox.md)
  
[Протокол (POX)](protocol-pox.md)
  
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
|[Протокол (POX)](protocol-pox.md) <br/> |Содержит спецификации для подключения клиента к серверу Exchange.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение сравнивается с значение элемента **GroupingInformation** для другого почтового ящика. Почтовые ящики, которые имеют одинаковые значения и использовать одной конечной точки веб-служб Exchange (EWS) можно объединять для обеспечения соответствия. Для получения дополнительных сведений см [Ведение сходства между группой подписок и сервера почтовых ящиков в Exchange](http://msdn.microsoft.com/library/1bda4094-88c3-4f61-9219-6ee70f6e81cf%28Office.15%29.aspx).
  
## <a name="remarks"></a>Замечания

Элемент **GroupingInformation** применим только к элементам **протокола** , имеющие [Тип (POX)](type-pox.md) дочерний элемент со значением «EXPR». 
  
## <a name="see-also"></a>См. также

- [Элементы XML автоматического обнаружения POX для Exchange](pox-autodiscover-xml-elements-for-exchange.md)
- [Поддержка сходства между группой подписок и сервера почтовых ящиков в Exchange](http://msdn.microsoft.com/library/1bda4094-88c3-4f61-9219-6ee70f6e81cf%28Office.15%29.aspx)

