---
title: IsGreaterThan
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsGreaterThan
api_type:
- schema
ms.assetid: a6e9d462-cfa7-40ec-903e-128c95050352
description: Элемент IsGreaterThan представляет выражение поиска, которое сравнивает свойство с постоянным значением или другим свойством и возвращает значение true, если первое свойство больше.
ms.openlocfilehash: dfa7c221bb04e59f1ae12eeb5b9f2e1f09aea3ce
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/28/2018
ms.locfileid: "21353492"
---
# <a name="isgreaterthan"></a>IsGreaterThan

Элемент **IsGreaterThan** представляет выражение поиска, которое сравнивает свойство с постоянным значением или другим свойством и возвращает **значение true,** Если первое свойство больше. 
  
```xml
<IsGreaterThan>
   <FieldURI/>
   <FieldURIOrConstant/>
</IsGreaterThan>
```

```xml
<IsGreaterThan>
   <IndexedFieldURI/> 
   <FieldURIOrConstant/>
</IsGreaterThan>
```

```xml
<IsGreaterThan>
   <ExtendedFieldURI/>
   <FieldURIOrConstant/>
</IsGreaterThan>
```

**IsGreaterThanType**

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[FieldURI](fielduri.md) <br/> |Идентифицирует часто упоминаемые свойства по URI.  <br/> |
|[IndexedFieldURI](indexedfielduri.md) <br/> |Идентифицирует отдельных элементов словаря.  <br/> |
|[ExtendedFieldURI](extendedfielduri.md) <br/> |Задает свойства MAPI.  <br/> |
|[FieldURIOrConstant](fielduriorconstant.md) <br/> |Представляет свойство или постоянное значение для использования при сравнении с другого свойства.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Restriction](restriction.md) <br/> |Представляет ограничение или запрос, используемый для фильтрации элементов или папок в папке операциях FindItem/FindFolder и поиска.  <br/> |
|[Не](not.md) <br/> |Представляет выражение поиска, которое Инвертирует логическое значение выражения поиска, который он содержит.  <br/> |
|[И](and.md) <br/> |Представляет выражение поиска, которое позволяет выполнять логическое и операции между двумя или более выражений для поиска. Результат операции является **значение true** , если все выражения поиска, содержащихся в And имеют **значение true**.  <br/> |
|[Или](or.md) <br/> |Представляет выражение поиска, используемая для выполнения логического или выражения поиска, которые он содержит. [Или](or.md) возвращает **значение true,** Если какие-либо из их дочерних элементов возвращало **значение true**.  <br/> |
   
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

