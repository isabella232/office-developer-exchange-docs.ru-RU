---
title: SavedItemFolderId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SavedItemFolderId
api_type:
- schema
ms.assetid: 4b8b475c-9ca5-48c9-acb0-8848b53be1ce
description: Элемент SavedItemFolderId определяет папку назначения для операций, обновление, отправка и создавать элементы в почтовом ящике.
ms.openlocfilehash: c57a7fb4abc2f7ee7b599f56f016811d6ff2c21c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19835277"
---
# <a name="saveditemfolderid"></a>SavedItemFolderId

Элемент **SavedItemFolderId** определяет папку назначения для операций, обновление, отправка и создавать элементы в почтовом ящике. 
  
```xml
<SavedItemFolderId>
   <FolderId/>
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
|[FolderId](folderid.md) <br/> |Содержит идентификатор и меняет ключ папку назначения для операций обновления, отправки и создания элементов в хранилище Exchange.  <br/> |
|[DistinguishedFolderId](distinguishedfolderid.md) <br/> |Определяет целевой папке по именованные идентификатор для операций, обновление, отправка и создания элементов в хранилище Exchange.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[CreateItem](createitem.md) <br/> |Определяет запрос на создание элемента в хранилище Exchange.  <br/> Ниже приведен выражение XPath для этого элемента.  <br/>  `/CreateItem` <br/> |
|[UpdateItem](updateitem.md) <br/> |Определяет запрос на обновление элемента в хранилище Exchange.  <br/> Ниже приведен выражение XPath для этого элемента.  <br/>  `/UpdateItem` <br/> |
|[SendItem](senditem.md) <br/> |Определяет запрос для отправки элемента в хранилище Exchange.  <br/> Ниже приведен выражение XPath для этого элемента.  <br/>  `/SendItem` <br/> |
   
## <a name="remarks"></a>Замечания

Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   

