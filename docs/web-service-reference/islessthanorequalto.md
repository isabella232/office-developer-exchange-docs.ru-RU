---
title: ислесссанорекуалто
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsLessThanOrEqualTo
api_type:
- schema
ms.assetid: b5d85eb2-5e15-4d01-ad49-6289e735ad8a
description: Элемент Ислесссанорекуалто представляет выражение поиска, которое сравнивает свойство со значением константы или другим свойством и возвращает значение true, если первое свойство меньше второго или равно ему.
ms.openlocfilehash: 7b153803b1c895c86e74428468c8e592c02a0acc
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530031"
---
# <a name="islessthanorequalto"></a>ислесссанорекуалто

Элемент **ислесссанорекуалто** представляет выражение поиска, которое сравнивает свойство со значением константы или другим свойством и возвращает **значение true** , если первое свойство меньше второго или равно ему. 
  
```xml
<IsLessThanOrEqualTo>
   <FieldURI/>
   <FieldURIOrConstant/>
</IsLessThanOrEqualTo>
```

```xml
<IsLessThanOrEqualTo>
   <IndexedFieldURI/> 
   <FieldURIOrConstant/>
</IsLessThanOrEqualTo>
```

```xml
<IsLessThanOrEqualTo>
   <ExtendedFieldURI/> 
   <FieldURIOrConstant/>
</IsLessThanOrEqualTo>
```

**ислесссанорекуалтотипе**

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[фиелдури](fielduri.md) <br/> |Определяет часто упоминаемые свойства по URI.  <br/> |
|[индекседфиелдури](indexedfielduri.md) <br/> |Определяет отдельные элементы словаря.  <br/> |
|[екстендедфиелдури](extendedfielduri.md) <br/> |Определяет свойства MAPI.  <br/> |
|[фиелдуриорконстант](fielduriorconstant.md) <br/> |Представляет свойство или значение константы, которое будет использоваться при сравнении с другим свойством.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Restriction](restriction.md) <br/> |Представляет ограничение или запрос, используемый для фильтрации элементов или папок в операциях FindItem/FindFolder и папках поиска.  <br/> |
|[Not](not.md) <br/> |Представляет выражение поиска, которое инвертирует логическое значение содержащегося в нем выражения поиска.  <br/> |
|[And](and.md) <br/> |Представляет выражение поиска, которое позволяет выполнять логическое действие и операцию между двумя или более выражениями поиска. Результат операции and имеет **значение true** , если все выражения поиска, содержащиеся в элементе и, имеют **значение true**.  <br/> |
|[Or](or.md) <br/> |Представляет выражение поиска, которое выполняет операцию логического или для содержащегося в нем выражения поиска. [Или](or.md) возвращает **значение true** , если любой из дочерних элементов возвращает значение true. [Или](or.md) должно иметь не менее двух дочерних элементов.  <br/> |
   
## <a name="remarks"></a>Примечания

Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

