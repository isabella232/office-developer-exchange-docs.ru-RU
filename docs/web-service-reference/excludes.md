---
title: Excludes
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Excludes
api_type:
- schema
ms.assetid: bbaeddf6-9a67-4ee0-af99-7a7a5bbdc0e1
description: Элемент Excludes выполняет немного более ровную маску указанного свойства и поставленное значение.
ms.openlocfilehash: 7923c31a4a1fea0270c9a4372072d7b0a3b79c76
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59510143"
---
# <a name="excludes"></a>Excludes

Элемент **Excludes** выполняет немного более ровную маску указанного свойства и поставленное значение. 
  
```xml
<Excludes>
   <FieldURI/>
   <Bitmask/>
</Excludes>
```

```xml
<Excludes>
   <ExtendedFieldURI/> 
   <Bitmask/>
</Excludes>
```

```xml
<Excludes>
   <IndexedFieldURI/> 
   <Bitmask/>
</Excludes>
```

**ExcludesType**

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[FieldURI](fielduri.md) <br/> |Определяет часто ссылаясь свойства по URI.  <br/> |
|[IndexedFieldURI](indexedfielduri.md) <br/> |Определяет отдельных членов словаря.  <br/> |
|[ExtendedFieldURI](extendedfielduri.md) <br/> |Определяет свойства MAPI.  <br/> |
|[Bitmask](bitmask.md) <br/> |Представляет гексадецимальную или десятичной маску, которая будет использоваться во время операции [ограничений Excludes.](excludes.md) Если битмаска представляет собой hexadecimal номер, она должна быть префиксом 0x или 0X. В противном случае он будет считаться десятичной.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Restriction](restriction.md) <br/> |Представляет ограничение или запрос, используемый для фильтрации элементов или папок в операциях FindItem/FindFolder и папках поиска.  <br/> |
|[Not](not.md) <br/> |Представляет выражение поиска, которое отменяет значение Boolean содержащемся в нем выражения поиска.  <br/> |
|[And](and.md) <br/> |Представляет выражение поиска, которое позволяет выполнять boolean и операцию между двумя или более выражениями поиска. Результат операции And является **верным,** если все выражения поиска, содержащиеся в И являются **верными.**  <br/> |
|[Or](or.md) <br/> |Представляет выражение поиска, которое выполняет логическое или логическое выражение поиска, содержащемся в нем. Элемент [Or](or.md) возвращается **true,** если любой из его детей **возвращается true**.  <br/> |
   
## <a name="remarks"></a>Заметки

**Исключения будут** разрешать до **true,** если операция AND, выполненная в следующих разрешениях, будет выполнена до 0: 
  
1. Битумное значение для свойства
    
2. Значение bitmask для свойства
    
**Исключения могут** применяться только к свойству, которое имеет многостраничная величина. Если тип свойства не является частью, в ответ возвращается код **ошибки ErrorUnsupportedPathForQuery.** 
  
Вы можете выполнить обратную операцию, позвонив не(исключает).
  
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

