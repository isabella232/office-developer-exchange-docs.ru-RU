---
title: ParentFolderIds
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- ParentFolderIds
api_type:
- schema
ms.assetid: e7998023-e5e0-465c-91fa-2aa6d1559f64
description: Элемент ParentFolderIds определяет папки для операций FindItem и FindFolder для поиска.
ms.openlocfilehash: e9e0f14651b205ad64be04dbe1d0707a109f3edc
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59512907"
---
# <a name="parentfolderids"></a>ParentFolderIds

Элемент **ParentFolderIds** определяет папки для операций FindItem и FindFolder для поиска. 
  
```xml
<ParentFolderIds>
   <DistinguishedFolderId/>
<ParentFolderIds>
```

```xml
<ParentFolderIds>
   <FolderId/> 
<ParentFolderIds>
```

**NonEmptyArrayOfBaseFolderIdsType**

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[FolderId](folderid.md) <br/> |Содержит идентификатор и ключ изменения папки. Элемент **ParentFolderIds должен** использовать либо этот элемент, либо [элемент DistinguishedFolderId.](distinguishedfolderid.md)  <br/> |
|[DistinguishedFolderId](distinguishedfolderid.md) <br/> |Определяет Microsoft Exchange Server 2007 года, на которые можно ссылаться по имени. Элемент **ParentFolderIds должен** использовать либо этот элемент, либо [элемент FolderId.](folderid.md)  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[FindFolder](findfolder.md) <br/> |Определяет запрос на идентификацию папок в почтовом ящике.  <br/> |
|[FindItem](finditem.md) <br/> |Определяет запрос на поиск элементов в почтовом ящике.  <br/> |
|[ResolveNames](resolvenames.md) <br/> |Определяет запрос на разрешение неоднозначных имен.  <br/> |
   
## <a name="remarks"></a>Заметки

Элемент **ParentFolderIds** должен использовать элемент [FolderId](folderid.md) или [DistinguishedFolderId.](distinguishedfolderid.md) Для поиска можно определить неограниченное количество папок. 
  
## <a name="example"></a>Пример

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
  xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <FindFolder Traversal="Shallow" xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <FolderShape>
        <t:BaseShape>Default</t:BaseShape>
      </FolderShape>
      <ParentFolderIds>
        <t:DistinguishedFolderId Id="inbox"/>
      </ParentFolderIds>
    </FindFolder>
  </soap:Body>
</soap:Envelope>
```

## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Операция FindFolder](findfolder-operation.md)  
- [Операция FindItem](finditem-operation.md) 
- [Операция ResolveNames](resolvenames-operation.md)

