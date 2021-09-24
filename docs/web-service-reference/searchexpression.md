---
title: SearchExpression
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- SearchExpression
api_type:
- schema
ms.assetid: daa179b6-8c7f-4268-a312-c2acc67fa7c3
description: Элемент SearchExpression — это абстрактный элемент, представляюющий замещающий элемент в пределах ограничения. Все выражения поиска вытекают из этого базового типа. Этот элемент не используется в документе экземпляра XML.
ms.openlocfilehash: e8047d333b36d77bc6823efd6488a15a6d2501a4
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59517849"
---
# <a name="searchexpression"></a>SearchExpression

Элемент **SearchExpression** — это абстрактный элемент, представляюющий замещающий элемент в пределах ограничения. Все выражения поиска вытекают из этого базового типа. Этот элемент не используется в документе экземпляра XML. 
  
```xml
<SearchExpression/>
```

 **SearchExpressionType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Restriction](restriction.md) <br/> |Представляет ограничение или запрос, используемый для фильтрации элементов или папок в операциях FindItem/FindFolder и папках поиска.  <br/> |
|[Not](not.md) <br/> |Представляет выражение поиска, которое отменяет значение Boolean содержащемся в нем выражения поиска.  <br/> |
|[And](and.md) <br/> |Представляет выражение поиска, которое позволяет выполнять операцию Boolean **и** между двумя или более выражениями поиска. Результат операции **AND** является **верным,** если все выражения поиска, содержащиеся в **элементе And,** **верны.**  <br/> |
|[Or](or.md) <br/> |Представляет выражение поиска, которое выполняет логическую **операцию OR** в выражении поиска, которое оно содержит. **Или** будет **возвращаться верно,** если любой из его детей **возвращается true**. **Или** должны иметь двух или более детей.  <br/> |
   
## <a name="remarks"></a>Заметки

Любой элемент фильтра, который входит в группу замены SearchExpression, может отображаться на месте элемента SearchExpression.
  
> [!NOTE]
> Этот элемент никогда не будет происходить непосредственно в документе экземпляра. 
  
Следующие элементы являются членами группы замены SearchExpression:
  
- [Exists](exists.md)
    
- [Исключает](excludes.md)
    
- [IsEqualTo](isequalto.md)
    
- [IsNotEqualTo](isnotequalto.md)
    
- [IsGreaterThan](isgreaterthan.md)
    
- [IsGreaterThanOrEqualTo](isgreaterthanorequalto.md)
    
- [IsLessThan](islessthan.md)
    
- [IsLessThanOrEqualTo](islessthanorequalto.md)
    
- [Contains](contains.md)
    
- [Not](not.md)
    
- [And](and.md)
    
- [Or](or.md)
    
Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

