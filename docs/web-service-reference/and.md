---
title: и
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- And
api_type:
- schema
ms.assetid: 790246c2-37ad-49a8-91b9-6186d743b011
description: Элемент And представляет выражение поиска, который позволяет выполнить операцию логическое и между двумя или более выражений для поиска. Значение true, если все выражения поиска, содержащиеся в элементе и результат операции.
ms.openlocfilehash: d287d57d68aeca7127325dc8fb65fd0190e5b5eb
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761381"
---
# <a name="and"></a>и

Элемент **и** представляет выражение поиска, которое позволяет выполнять операцию логическое **AND** между двумя или более выражений для поиска. Результат **операции** является **значение true** , если все выражения поиска, содержащиеся в элементе **и** имеют **значение true**.
  
```xml
<And>
   <SearchExpression/>
   <SearchExpression/>
</And>
```

 **AndType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[SearchExpression](searchexpression.md) <br/> | Представляет базовый класс для выражений с ограничением. Должен быть более двух выражений поиска в операции.<br/><br/>  Элемент **SearchExpression** необходимо заменить один из следующих элементов:<ul><li> [Существует](exists.md)</li><li>[Исключает](excludes.md)</li><li>[Выражение IsEqualTo](isequalto.md)</li><li>[IsNotEqualTo](isnotequalto.md)</li><li>[IsGreaterThan](isgreaterthan.md)</li><li>[IsGreaterThanOrEqualTo](isgreaterthanorequalto.md)</li><li>[IsLessThan](islessthan.md)</li><li>[IsLessThanOrEqualTo](islessthanorequalto.md)</li><li>[Contains](contains.md)</li><li>[Не](not.md)</li><li>**И**</li><li>[Или](or.md) </li></ul> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Ограничения](restriction.md) <br/> |Представляет ограничение или запрос, используемый для фильтрации элементов или папок в папке операциях FindItem/FindFolder и поиска.  <br/> |
|[Не](not.md) <br/> |Представляет выражение поиска, которое Инвертирует логическое значение выражения поиска, который он содержит.  <br/> |
|**И** <br/> |Представляет выражение поиска, которое позволяет выполнять операцию логическое **AND** между двумя или более выражений для поиска. **Операции** получается **значение true,** **Если все выражения поиска, содержащиеся в элементе **и** **.  <br/> |
|[Или](or.md) <br/> |Представляет выражение поиска, которое выполняет операцию логической **или** на нем выражением поиска. **Или** возвращает **значение true,** Если какие-либо из их дочерних элементов возвращало **значение true**. **Или** должен иметь два или несколько дочерних элементов.  <br/> |
   
## <a name="remarks"></a>Замечания

Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

