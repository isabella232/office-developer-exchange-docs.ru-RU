---
title: Или
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Or
api_type:
- schema
ms.assetid: 4876d83a-73a3-4953-9d95-3048e6b76ccb
description: Элемент или представляет выражение поиска, используемая для выполнения логического или на нем выражением поиска. Или возвращает значение true, если какие-либо из их дочерних элементов возвращало значение true. Или должны иметь два или несколько дочерних элементов.
ms.openlocfilehash: 46cf031047aeb09e05a385150ab7587968aef345
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834661"
---
# <a name="or"></a>Или

Элемент **или** представляет выражение поиска, которое выполняет логической **или** на нем выражением поиска. **Или** возвращает **значение true,** Если какие-либо из их дочерних элементов возвращало **значение true**. **Или** должен иметь два или несколько дочерних элементов. 
  
```xml
<Or>
   <SearchExpression/>
   <SearchExpression/>
</Or>
```

 **OrType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[SearchExpression](searchexpression.md) <br/> | Представляет базовый класс для выражений с ограничением. <br/><br/>Элемент **SearchExpression** необходимо заменить один из следующих элементов: <br/> <br/>- [Существует](exists.md) <br/>- [Исключает](excludes.md) <br/>- [Выражение IsEqualTo](isequalto.md) <br/>- [IsNotEqualTo](isnotequalto.md) <br/>- [IsGreaterThan](isgreaterthan.md) <br/>- [IsGreaterThanOrEqualTo](isgreaterthanorequalto.md) <br/>- [IsLessThan](islessthan.md) <br/>- [IsLessThanOrEqualTo](islessthanorequalto.md) <br/>- [Содержит](contains.md) <br/>- [Не](not.md) <br/>- [И](and.md) <br/>- **Или** <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Ограничения](restriction.md) <br/> |Представляет ограничение или запрос, используемый для фильтрации элементов или папок в папке операциях FindItem/FindFolder и поиска.  <br/> |
|[Не](not.md) <br/> |Представляет выражение поиска, которое Инвертирует логическое значение выражения поиска, который он содержит.  <br/> |
|[И](and.md) <br/> |Представляет выражение поиска, которое позволяет выполнять операцию логическое **AND** между двумя или более выражений для поиска. Результат **операции** является **значение true** , если все выражения поиска, содержащиеся в элементе **и** имеют **значение true**.  <br/> |
|**Или** <br/> |Представляет выражение поиска, которое выполняет операцию логической **или** на нем выражением поиска. **Или** возвращает **значение true,** Если какие-либо из их дочерних элементов возвращало **значение true**. **Или** должен иметь два или несколько дочерних элементов.  <br/> |
   
## <a name="remarks"></a>Замечания

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

