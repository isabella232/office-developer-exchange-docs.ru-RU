---
title: граупиндекс
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GroupIndex
api_type:
- schema
ms.assetid: 7a596ff7-6cc3-4626-a52c-538a92202337
description: Элемент Граупиндекс представляет значение свойства, которое используется для группировки элементов для текущей группы элементов в вызове операции FindItem.
ms.openlocfilehash: 8b23f5142a15c099c30209ea48cd04f4af4e8c6a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833762"
---
# <a name="groupindex"></a>граупиндекс

Элемент **граупиндекс** представляет значение свойства, которое используется для группировки элементов для текущей группы элементов в вызове [операции FindItem](finditem-operation.md) . 
  
[финдитемреспонсе](finditemresponse.md)
  
[респонсемессажес](responsemessages.md)
  
[финдитемреспонсемессаже](finditemresponsemessage.md)
  
[Рутфолдер (Финдитемреспонсемессаже)](rootfolder-finditemresponsemessage.md)
  
[Группы](groups.md)
  
[граупедитемс](groupeditems.md)
  
[граупиндекс](groupindex.md)
  
```xml
<GroupIndex/>
```

 **строка**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[граупедитемс](groupeditems.md) <br/> |Представляет коллекцию элементов, которая является результатом сгруппированного вызова [операции FindItem](finditem-operation.md) .  <br/> Ниже приведено выражение XPath для этого элемента:  <br/>  `/FindItemResponse/ResponseMessages/FindItemResponseMessage/RootFolder/Groups/GroupedItems[i]` <br/> |
   
## <a name="text-value"></a>Текстовое значение

Необходимо указать текстовое значение. Это свойство доступно только для чтения.
  
## <a name="remarks"></a>Примечания

Этот элемент встречается только в отклике [операции FindItem](finditem-operation.md) . 
  
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

