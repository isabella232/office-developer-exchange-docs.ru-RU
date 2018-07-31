---
title: ContextFolderId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ContextFolderId
api_type:
- schema
ms.assetid: 48de92aa-e124-42b5-89bc-cdce5e93d78b
description: Элемент ContextFolderId указывает папку, предназначенное для действий, использующих папок. Этот элемент должен присутствовать при копирование, удаление, перемещение и настройка состояние чтения элементов беседы в целевой папке.
ms.openlocfilehash: 94428a079be6da8873c777556771579a7110fb62
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/28/2018
ms.locfileid: "21354283"
---
# <a name="contextfolderid"></a>ContextFolderId

Элемент **ContextFolderId** указывает папку, предназначенное для действий, использующих папок. Этот элемент должен присутствовать при копирование, удаление, перемещение и настройка состояние чтения элементов беседы в целевой папке. 
  
- [ApplyConversationAction](applyconversationaction.md) 
- [ConversationActions](conversationactions.md)
- [ConversationAction](conversationaction.md)
- [ContextFolderId](contextfolderid.md)
  
```XML
<ContextFolderId>
   <FolderId/>
</ContextFolderId>
```

```XML
<ContextFolderId>
   <DistinguishedFolderId/>
</ContextFolderId>
```


**TargetFolderIdType**

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[FolderId](folderid.md) <br/> |Содержит идентификатор и меняет ключ контекстной папки.  <br/> |
|[DistinguishedFolderId](distinguishedfolderid.md) <br/> |Идентифицирует папки, которые можно ссылаться по имени.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[ConversationAction](conversationaction.md) <br/> |Содержит одно действие должен применяться к разговора.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Нет.
  
## <a name="remarks"></a>Замечания

Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.Этот элемент появился в Exchange Server 2010 с пакетом обновления 1 (SP1).
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Операция ApplyConversationAction](applyconversationaction-operation.md)

