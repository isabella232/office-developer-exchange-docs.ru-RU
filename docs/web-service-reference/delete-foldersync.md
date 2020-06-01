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
ms.openlocfilehash: 68f8687b8cf0723d7fd63a3d55da8ef7c2f98f8e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44454983"
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

Отсутствуют.
  
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
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Операция SyncFolderHierarchy](syncfolderhierarchy-operation.md)
- [Справка по службам EWS для Exchange](ews-reference-for-exchange.md)
- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

