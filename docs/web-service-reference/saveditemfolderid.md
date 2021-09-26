---
title: SavedItemFolderId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- SavedItemFolderId
api_type:
- schema
ms.assetid: 4b8b475c-9ca5-48c9-acb0-8848b53be1ce
description: Элемент SavedItemFolderId определяет целевую папку для операций, которые обновляют, отправляют и создают элементы в почтовом ящике.
ms.openlocfilehash: 75245cf842336621aa098c115d62a7802711dd54
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59546121"
---
# <a name="saveditemfolderid"></a>SavedItemFolderId

Элемент **SavedItemFolderId** определяет целевую папку для операций, которые обновляют, отправляют и создают элементы в почтовом ящике. 
  
```xml
<SavedItemFolderId>
   <FolderId/>
</SavedItemFolderId>
```

```xml
<SavedItemFolderId>
   <DistinguishedFolderId/>
</SavedItemFolderId>
```

**TargetFolderIdType**

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[FolderId](folderid.md) <br/> |Содержит идентификатор и ключ изменения целевой папки для операций, которые обновляют, отправляют и создают элементы в Exchange магазине.  <br/> |
|[DistinguishedFolderId](distinguishedfolderid.md) <br/> |Определяет целевую папку по имени идентификатора для операций, которые обновляют, отправляют и создают элементы в Exchange магазине.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[CreateItem](createitem.md) <br/> |Определяет запрос на создание элемента в Exchange магазине.  <br/> Ниже приводится выражение XPath к этому элементу:  <br/>  `/CreateItem` <br/> |
|[UpdateItem](updateitem.md) <br/> |Определяет запрос на обновление элемента в Exchange магазине.  <br/> Ниже приводится выражение XPath к этому элементу:  <br/>  `/UpdateItem` <br/> |
|[SendItem](senditem.md) <br/> |Определяет запрос на отправку элемента в Exchange магазине.  <br/> Ниже приводится выражение XPath к этому элементу:  <br/>  `/SendItem` <br/> |
   
## <a name="remarks"></a>Заметки

Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   

