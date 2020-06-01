---
title: дистингуишедграупби
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DistinguishedGroupBy
api_type:
- schema
ms.assetid: 6ff3ac48-02ba-40ec-a71b-c401bb2b127c
description: Элемент Дистингуишедграупби предоставляет стандартные группирования для запросов FindItem.
ms.openlocfilehash: 004613d55419a19f69e960203ae13d8d906b74c8
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463141"
---
# <a name="distinguishedgroupby"></a>дистингуишедграупби

Элемент **дистингуишедграупби** предоставляет стандартные группирования для запросов FindItem. 
  
- [FindItem](finditem.md) 
- [дистингуишедграупби](distinguishedgroupby.md)
  
```xml
<DistinguishedGroupBy>
   <StandardGroupBy/>
</DistinguishedGroupBy>
```

 **дистингуишедграупбитипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[стандардграупби](standardgroupby.md) <br/> |Представляет стандартные механизмы группирования и агрегирования для операции сгруппированной операции FindItem.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[FindItem](finditem.md) <br/> |Определяет запрос на поиск элементов в почтовом ящике.<br/><br/>Ниже приведено выражение XPath для этого элемента:`/FindItem` <br/> |
   
## <a name="remarks"></a>Примечания

Элемент **дистингуишедграупби** можно добавить в операцию FindItem при условии, что результаты должны быть сгруппированы, а одна из стандартных групп соответствует требованиям к группированию. Если не указан ни элемент **дистингуишедграупби** , ни элемент [GroupBy](groupby.md) , результаты FindItem будут отходиться на несгруппированные результаты. 
  
Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Операция FindItem](finditem-operation.md)
- [Поиск элементов](https://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)

