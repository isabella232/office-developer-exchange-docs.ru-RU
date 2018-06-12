---
title: DeleteItemField
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DeleteItemField
api_type:
- schema
ms.assetid: 3893be6a-49a7-49f6-bf53-c7f819ec3f87
description: Элемент DeleteItemField представляет операцию для удаления заданного свойства из элемента во время вызова UpdateItem.
ms.openlocfilehash: 2388bd10379211a31890b7c4f27920431ce444c8
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762044"
---
# <a name="deleteitemfield"></a>DeleteItemField

Элемент **DeleteItemField** представляет операцию для удаления заданного свойства из элемента во время вызова UpdateItem. 
 
- [UpdateItem](updateitem.md)  
- [ItemChanges](itemchanges.md) 
- [ItemChange](itemchange.md) 
- [Обновления (элемент)](updates-item.md) 
- [DeleteItemField](deleteitemfield.md)
  
```xml
<DeleteItemField>
   <FieldURI/>
</DeleteItemField>
```

 **DeleteItemFieldType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[FieldURI](fielduri.md) <br/> |Идентифицирует часто упоминаемые свойства по URI.  <br/> |
|[IndexedFieldURI](indexedfielduri.md) <br/> |Идентифицирует отдельным членам свойства словаря.  <br/> |
|[ExtendedFieldURI](extendedfielduri.md) <br/> |Задает расширенные свойства MAPI.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Обновления (элемент)](updates-item.md) <br/> |Содержит набор элементов, которые определяют добавьте, Установка и удаление изменения свойств элемента.  <br/><br/>Ниже приведен выражение XPath для этого элемента.<br/>`/UpdateItem/ItemChanges/ItemChange[i]/Updates` <br/> |
   
## <a name="remarks"></a>Замечания

Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |типы схемы  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [UpdateItem Operation](updateitem-operation.md)

