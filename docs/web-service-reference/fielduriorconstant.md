---
title: FieldURIOrConstant
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FieldURIOrConstant
api_type:
- schema
ms.assetid: 89d7a87e-7c93-49b8-83ec-8798e08c1052
description: Элемент FieldURIOrConstant представляет свойство или постоянное значение для использования при сравнении с другого свойства.
ms.openlocfilehash: 5195feec2a314d9ec15dc4a25a7a014aded1696a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762535"
---
# <a name="fielduriorconstant"></a>FieldURIOrConstant

Элемент **FieldURIOrConstant** представляет свойство или постоянное значение для использования при сравнении с другого свойства. 
  
```xml
<FieldURIOrConstant>
   <Constant/>
</FieldURIOrConstant>
```

 **FieldURIOrConstantType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Константы](constant.md) <br/> |Задает значение константы в качестве ограничения.  <br/> |
|[FieldURI](fielduri.md) <br/> |Идентифицирует часто упоминаемые свойства по URI.  <br/> |
|[IndexedFieldURI](indexedfielduri.md) <br/> |Идентифицирует отдельных элементов словаря.  <br/> |
|[ExtendedFieldURI](extendedfielduri.md) <br/> |Задает свойства MAPI.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Выражение IsEqualTo](isequalto.md) <br/> |Представляет выражение поиска, которое сравнивает свойство с постоянным значением или другим свойством и возвращает значение true, если они равны.  <br/> |
|[IsGreaterThan](isgreaterthan.md) <br/> |Представляет выражение поиска, которое сравнивает свойство с постоянным значением или другим свойством и возвращает значение true, если первое свойство больше.  <br/> |
|[IsGreaterThanOrEqualTo](isgreaterthanorequalto.md) <br/> |Представляет выражение поиска, которое сравнивает свойство с постоянным значением или другим свойством и возвращает значение true, если первое свойство больше или равно второе значение или свойству.  <br/> |
|[IsLessThan](islessthan.md) <br/> |Представляет выражение поиска, которое сравнивает свойство с постоянным значением или другим свойством и возвращает значение true, если первое свойство меньше, чем второе значение или свойство.  <br/> |
|[IsLessThanOrEqualTo](islessthanorequalto.md) <br/> |Представляет выражение поиска, которое сравнивает свойство с постоянным значением или другим свойством и возвращает значение true, если первое свойство меньше или равно второе значение или свойству.  <br/> |
|[IsNotEqualTo](isnotequalto.md) <br/> |Представляет выражение поиска, которое сравнивает свойство с постоянным значением или другим свойством и возвращает значение true, если значения не совпадают.  <br/> |
   
## <a name="remarks"></a>Замечания

Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.
  
## <a name="example"></a>Пример

В следующем примере XML показан элемент FieldURIOrConstant, используемый как константа, так и поле URI.
  
```
[xml]
<Restriction>
  <Or xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
    <IsEqualTo>
      <FieldURI FieldURI="item:DateTimeCreated"/>
      <FieldURIOrConstant>
        <FieldURI FieldURI="item:DateTimeReceived"/>
      </FieldURIOrConstant>
    </IsEqualTo>
    <IsEqualTo>
      <FieldURI FieldURI="item:Subject"/>
      <FieldURIOrConstant>
        <Constant Value="Here is a test message"/>
      </FieldURIOrConstant>
    </IsEqualTo>
  </Or>
</Restriction>
```

## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

