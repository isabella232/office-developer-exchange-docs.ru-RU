---
title: Delete (Фолдерсинк)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Delete
api_type:
- schema
ms.assetid: c4397d91-43ef-40a9-a80e-d31501a33caa
description: Элемент Delete определяет отдельную папку, которую необходимо удалить из локального хранилища клиентов.
ms.openlocfilehash: 5cad36c6fcff782195fdb285e2d3c4f3c5ec0f1e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762015"
---
# <a name="delete-foldersync"></a>Delete (Фолдерсинк)

Элемент **Delete** определяет отдельную папку, которую необходимо удалить из локального хранилища клиентов. 
  
- [синкфолдерхиерарчиреспонсе](syncfolderhierarchyresponse.md)  
- [респонсемессажес](responsemessages.md)  
- [синкфолдерхиерарчиреспонсемессаже](syncfolderhierarchyresponsemessage.md)  
- [Изменения (иерархия)](changes-hierarchy.md)  
- [Delete (Фолдерсинк)](delete-foldersync.md)
  
```xml
<Delete>
   <FolderId/>
</Delete>
```

**синкфолдерхиерарчиделететипе**

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[FolderId](folderid.md) <br/> |Содержит идентификатор и ключ изменения папки.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Изменения (иерархия)](changes-hierarchy.md) <br/> |Содержит упорядоченный массив типов изменений, которые представляют тип различий между папками на клиенте и папками на компьютере, на котором работает Microsoft Exchange Server 2007.  <br/> |
   
## <a name="remarks"></a>Примечания

Схема, описывающая этот элемент, находится в виртуальном каталоге EWS компьютера Exchange 2007, на котором установлена роль сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Операция SyncFolderHierarchy](syncfolderhierarchy-operation.md)
- [Справка по службам EWS для Exchange](ews-reference-for-exchange.md)
- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

