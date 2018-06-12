---
title: SearchExpression
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SearchExpression
api_type:
- schema
ms.assetid: daa179b6-8c7f-4268-a312-c2acc67fa7c3
description: Элемент SearchExpression является абстрактный элемент, представляющий переданный элемент с ограничением. Все выражения поиска являются производными от этого базового типа. Этот элемент не используется в экземпляре документа XML.
ms.openlocfilehash: 8e0d09aec079280816cd9dfe2c1a55c88bb959a7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19835286"
---
# <a name="searchexpression"></a>SearchExpression

Элемент **SearchExpression** является абстрактный элемент, представляющий переданный элемент с ограничением. Все выражения поиска являются производными от этого базового типа. Этот элемент не используется в экземпляре документа XML. 
  
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
|[Ограничения](restriction.md) <br/> |Представляет ограничение или запрос, используемый для фильтрации элементов или папок в папке операциях FindItem/FindFolder и поиска.  <br/> |
|[Не](not.md) <br/> |Представляет выражение поиска, которое Инвертирует логическое значение выражения поиска, который он содержит.  <br/> |
|[И](and.md) <br/> |Представляет выражение поиска, которое позволяет выполнять операцию логическое **AND** между двумя или более выражений для поиска. Результат **операции** является **значение true** , если все выражения поиска, содержащиеся в элементе **и** имеют **значение true**.  <br/> |
|[Или](or.md) <br/> |Представляет выражение поиска, которое выполняет операцию логической **или** на нем выражением поиска. **Или** возвращает **значение true,** Если какие-либо из их дочерних элементов возвращало **значение true**. **Или** должен иметь два или несколько дочерних элементов.  <br/> |
   
## <a name="remarks"></a>Замечания

Любой элемент фильтра, который является частью группы подстановки SearchExpression могут появляться, вместо SearchExpression элемента.
  
> [!NOTE]
> Этот элемент никогда не происходит непосредственно в экземпляре документа. 
  
Следующие элементы являются участниками группы подстановки SearchExpression:
  
- [Существует](exists.md)
    
- [Исключает](excludes.md)
    
- [Выражение IsEqualTo](isequalto.md)
    
- [IsNotEqualTo](isnotequalto.md)
    
- [IsGreaterThan](isgreaterthan.md)
    
- [IsGreaterThanOrEqualTo](isgreaterthanorequalto.md)
    
- [IsLessThan](islessthan.md)
    
- [IsLessThanOrEqualTo](islessthanorequalto.md)
    
- [Contains](contains.md)
    
- [Не](not.md)
    
- [И](and.md)
    
- [Или](or.md)
    
Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

