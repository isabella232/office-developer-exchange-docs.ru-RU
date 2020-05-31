---
title: граупедитемс
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GroupedItems
api_type:
- schema
ms.assetid: 53170df4-4272-4b37-b23f-cd8e2d4a7396
description: Элемент Граупедитемс представляет коллекцию элементов, которые являются результатом вызова сгруппированной операции FindItem.
ms.openlocfilehash: f8aed9b78fc54307f44b96a45e5c31a4cc76ab50
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833756"
---
# <a name="groupeditems"></a>граупедитемс

Элемент **граупедитемс** представляет коллекцию элементов, которые являются результатом вызова сгруппированной [операции FindItem](finditem-operation.md) . 
  
[финдитемреспонсе](finditemresponse.md)
  
[респонсемессажес](responsemessages.md)
  
[финдитемреспонсемессаже](finditemresponsemessage.md)
  
[Рутфолдер (Финдитемреспонсемессаже)](rootfolder-finditemresponsemessage.md)
  
[Группы](groups.md)
  
[граупедитемс](groupeditems.md)
  
```xml
<GroupedItems>
   <GroupIndex/>
   <Items/>
</GroupedItems>
```

 **граупедитемстипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[граупиндекс](groupindex.md) <br/> |Представляет значение свойства, используемое для группировки элементов в сгруппированном вызове [операции FindItem](finditem-operation.md) .  <br/> |
|[Items](items.md) <br/> |Содержит массив сгруппированных элементов.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Группы](groups.md) <br/> |Содержит коллекцию групп, найденных с помощью критериев поиска и объединения, которые определены в запросе [операции FindItem](finditem-operation.md) .  <br/> |
   
## <a name="remarks"></a>Примечания

Схема, описывающая этот элемент, находится в виртуальном каталоге EWS компьютера под управлением Microsoft Exchange Server 2010, на котором установлена роль сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операция FindItem](finditem-operation.md)


[Поиск элементов](http://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)

