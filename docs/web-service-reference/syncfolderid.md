---
title: SyncFolderId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SyncFolderId
api_type:
- schema
ms.assetid: 3645fa03-236d-4e5f-b8b9-5d98f7f35fa2
description: Элемент SyncFolderId представляет папку, содержащую элементы для синхронизации.
ms.openlocfilehash: c90a20095ca4706f0c6edae3e98eaadd6024d817
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/28/2018
ms.locfileid: "21354402"
---
# <a name="syncfolderid"></a>SyncFolderId

Элемент **SyncFolderId** представляет папку, содержащую элементы для синхронизации. 
  
```xml
<SyncFolderId>
   <FolderId/>
</SyncFolderId>
```

```xml
<SyncFolderId>
   <DistinguishedFolderId/> 
</SyncFolderId>
```

**TargetFolderIdType**

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[FolderId](folderid.md) <br/> |Содержит идентификатор и ключ изменения папки.  <br/> |
|[DistinguishedFolderId](distinguishedfolderid.md) <br/> |Идентифицирует MicrosoftExchange Server 2007 папок, которые можно ссылаться по имени.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[SyncFolderHierarchy](syncfolderhierarchy.md) <br/> |Определяет запрос для синхронизации иерархии папок в хранилище Exchange.  <br/> |
|[SyncFolderItems](syncfolderitems.md) <br/> |Определяет запрос для синхронизации элементов в папке хранилища Exchange.  <br/> |
   
## <a name="remarks"></a>Замечания

Схема, описывающая этот элемент находится в виртуальном каталоге EWS компьютера, на котором работает Exchange Server 2007 с установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Операция SyncFolderItems](syncfolderitems-operation.md)
- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

