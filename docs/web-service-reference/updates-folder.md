---
title: Обновления (папка)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Updates
api_type:
- schema
ms.assetid: b047e3a4-a5ab-4098-b7a0-273bc809e702
description: Элемент Updates содержит набор элементов, которые определяют добавьте, Установка и удаление изменения свойств папки.
ms.openlocfilehash: 31f25b1e88fb8756f189a6d75259dd4fc198582f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19840379"
---
# <a name="updates-folder"></a>Обновления (папка)

Элемент **Updates** содержит набор элементов, которые определяют добавьте, Установка и удаление изменения свойств папки. 
  
- [UpdateFolder](updatefolder.md)
  
- [FolderChanges](folderchanges.md)
  
- [FolderChange](folderchange.md)
  
- [Обновления (папка)](updates-folder.md)
  
```xml
<Updates>
   <AppendToFolderField/>
   <SetFolderField/>
   <DeleteFolderField/>
</Updates>
```

**NonEmptyArrayOfFolderChangeDescriptionsType**

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[AppendToFolderField](appendtofolderfield.md) <br/> |Представляет данные для добавления к папке свойство во время [операции UpdateFolder](updatefolder-operation.md).  <br/> |
|[SetFolderField](setfolderfield.md) <br/> |Представляет обновление для одного свойства папки в рамках одной [операции UpdateFolder](updatefolder-operation.md).  <br/> |
|[DeleteFolderField](deletefolderfield.md) <br/> |Представляет операцию удаление указанного свойства из папки при выполнении [операции UpdateFolder](updatefolder-operation.md).  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[FolderChange](folderchange.md) <br/> |Представляет коллекцию изменений выполняется на одной папке.  <br/> Ниже приведен выражение XPath для этого элемента.`/UpdateFolder/FolderChanges/FolderChange[i]` <br/> |
   
## <a name="remarks"></a>Замечания

Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Операцию UpdateFolder](updatefolder-operation.md)
- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

