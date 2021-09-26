---
title: And
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- And
api_type:
- schema
ms.assetid: 790246c2-37ad-49a8-91b9-6186d743b011
description: Элемент And представляет выражение поиска, которое позволяет выполнять операцию Boolean И между двумя или более выражениями поиска. Результат операции AND является верным, если все выражения поиска, содержащиеся в элементе And, верны.
ms.openlocfilehash: b6cf8ffbb19ea3aff917493e6ae4e324025c6ac9
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59541534"
---
# <a name="and"></a>And

Элемент **And** представляет выражение поиска, которое позволяет выполнять операцию Boolean **И** между двумя или более выражениями поиска. Результат операции **AND** является **верным,** если все выражения поиска, содержащиеся в **элементе And,** **верны.**
  
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
|[SearchExpression](searchexpression.md) <br/> | Представляет базовый класс для выражений в пределах ограничения. В операции And должно быть два или более выражений поиска.<br/><br/>  Один из следующих элементов должен быть заменен **элементом SearchExpression:**<ul><li> [Exists](exists.md)</li><li>[Исключает](excludes.md)</li><li>[IsEqualTo](isequalto.md)</li><li>[IsNotEqualTo](isnotequalto.md)</li><li>[IsGreaterThan](isgreaterthan.md)</li><li>[IsGreaterThanOrEqualTo](isgreaterthanorequalto.md)</li><li>[IsLessThan](islessthan.md)</li><li>[IsLessThanOrEqualTo](islessthanorequalto.md)</li><li>[Contains](contains.md)</li><li>[Not](not.md)</li><li>**And**</li><li>[Or](or.md) </li></ul> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Restriction](restriction.md) <br/> |Представляет ограничение или запрос, используемый для фильтрации элементов или папок в операциях FindItem/FindFolder и папках поиска.  <br/> |
|[Not](not.md) <br/> |Представляет выражение поиска, которое отменяет значение Boolean содержащемся в нем выражения поиска.  <br/> |
|**And** <br/> |Представляет выражение поиска, которое позволяет выполнять операцию Boolean **и** между двумя или более выражениями поиска. Результат операции **AND** является **верным,** если все выражения поиска, содержащиеся в элементе **And,** **верны.**  <br/> |
|[Or](or.md) <br/> |Представляет выражение поиска, которое выполняет логическую **операцию OR** в выражении поиска, которое оно содержит. **Или** будет **возвращаться верно,** если любой из его детей **возвращается true**. **Или** должны иметь двух или более детей.  <br/> |
   
## <a name="remarks"></a>Заметки

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

