---
title: Не
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Not
api_type:
- schema
ms.assetid: 1aa16318-7e90-4b19-bce8-dd1a20a66223
description: Элемент Not представляет выражение поиска, которое отменяет значение Boolean содержащемся в нем выражения поиска.
ms.openlocfilehash: a62a964043d85033ceffc5ca380468e0aeebdfc3
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59541961"
---
# <a name="not"></a>Не

Элемент **Not** представляет выражение поиска, которое отменяет значение Boolean содержащемся в нем выражения поиска. 
  
```xml
<Not>
   <SearchExpression/>
</Not>
```

 **NotType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[SearchExpression](searchexpression.md) <br/> | Представляет базовый класс для выражений в пределах ограничения. <br/><br/>Один из следующих элементов должен быть заменен **элементом SearchExpression:** <br/> <br/>- [Существует](exists.md) <br/>- [Исключает](excludes.md) <br/>- [IsEqualTo](isequalto.md) <br/>- [IsNotEqualTo](isnotequalto.md) <br/>- [IsGreaterThan](isgreaterthan.md) <br/>- [IsGreaterThanOrEqualTo](isgreaterthanorequalto.md) <br/>- [IsLessThan](islessthan.md) <br/>- [IsLessThanOrEqualTo](islessthanorequalto.md) <br/>- [Содержит](contains.md) <br/>- **Не** <br/>- [И](and.md) <br/>- [Or](or.md) <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Restriction](restriction.md) <br/> |Представляет ограничение или запрос, используемый для фильтрации элементов или папок в операциях FindItem/FindFolder и папках поиска.  <br/> |
|**Not** <br/> |Представляет выражение поиска, которое отменяет значение Boolean содержащемся в нем выражения поиска.  <br/> |
|[And](and.md) <br/> |Представляет выражение поиска, которое позволяет выполнять операцию Boolean **и** между двумя или более выражениями поиска. Результат операции **AND** является **верным,** если все выражения поиска, содержащиеся в **элементе And,** **верны.**  <br/> |
|[Or](or.md) <br/> |Представляет выражение поиска, которое выполняет логическую **операцию OR** в выражении поиска, которое оно содержит. **Или** будет **возвращаться верно,** если любой из его детей **возвращается true**. **Или** должны иметь двух или более детей.  <br/> |
   
## <a name="remarks"></a>Заметки

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

