---
title: IsNotEqualTo
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- IsNotEqualTo
api_type:
- schema
ms.assetid: e2eff26c-3403-45cd-bb74-1eb98c7dbfcd
description: Элемент IsNotEqualTo представляет выражение поиска, которое сравнивает свойство с постоянным значением или другим свойством и возвращает значение true, если значения не одинаковы.
ms.openlocfilehash: 8bfd8006eab0578c49d604b7583afe35beef17a7
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59539418"
---
# <a name="isnotequalto"></a>IsNotEqualTo

Элемент **IsNotEqualTo** представляет выражение поиска, которое сравнивает свойство с постоянным значением  или другим свойством и возвращает значение true, если значения не одинаковы. 
  
```xml
<IsNotEqualTo>
   <FieldURI/>
   <FieldURIOrConstant/>
</IsNotEqualTo>
```

```xml
<IsNotEqualTo>
   <ExtendedFieldURI/> 
   <FieldURIOrConstant/>
</IsNotEqualTo>
```

```xml
<IsNotEqualTo>
   <IndexedFieldURI/>
   <FieldURIOrConstant/>
</IsNotEqualTo>
```

**IsNotEqualToType**

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
|[FieldURIOrConstant](fielduriorconstant.md) <br/> |Представляет свойство или постоянное значение, используемого при сравнении с другим свойством.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Restriction](restriction.md) <br/> |Представляет ограничение или запрос, используемый для фильтрации элементов или папок в операциях FindItem/FindFolder и папках поиска.  <br/> |
|[Not](not.md) <br/> |Представляет выражение поиска, которое отменяет значение Boolean содержащемся в нем выражения поиска.  <br/> |
|[And](and.md) <br/> |Представляет выражение поиска, которое позволяет выполнять boolean и операцию между двумя или более выражениями поиска. Результат операции And является **верным,** если все выражения поиска, содержащиеся в И являются **верными.**  <br/> |
|[Or](or.md) <br/> |Представляет выражение поиска, которое выполняет логическое или логическое выражение поиска, содержащемся в нем. [Или](or.md) будет **возвращаться верно,** если любой из его детей **возвращается true**. **Или** должны иметь двух или более детей.  <br/> |
   
## <a name="remarks"></a>Заметки

Чтобы выполнить сравнение строк, рассмотрите возможность использования элемента [Contains,](contains.md) так как он предоставляет параметры сопоставления, такие как корпус и белое пространство. Для [отмены](not.md) результата используйте элемент Not в сочетании с элементом [Contains.](contains.md) 
  
Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

