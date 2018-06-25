---
title: ParentFolderIds
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ParentFolderIds
api_type:
- schema
ms.assetid: e7998023-e5e0-465c-91fa-2aa6d1559f64
description: Элемент ParentFolderIds определяет папок для операций FindItem и FindFolder для поиска.
ms.openlocfilehash: 4dd23b45dcc397e29e67fc08b29dd773e50f0db1
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834688"
---
# <a name="parentfolderids"></a>ParentFolderIds

Элемент **ParentFolderIds** определяет папок для операций FindItem и FindFolder для поиска. 
  
```xml
<ParentFolderIds>
   <DistinguishedFolderId/>
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
|[FolderId](folderid.md) <br/> |Содержит идентификатор и ключ изменения папки. Элемент **ParentFolderIds** необходимо использовать этот элемент или элемент [DistinguishedFolderId](distinguishedfolderid.md) .  <br/> |
|[DistinguishedFolderId](distinguishedfolderid.md) <br/> |Идентифицирует папок Microsoft Exchange Server 2007, которые можно ссылаться по имени. Элемент **ParentFolderIds** необходимо использовать этот элемент или элемент [FolderId](folderid.md) .  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[FindFolder](findfolder.md) <br/> |Определяет запрос для определения папок в почтовом ящике.  <br/> |
|[FindItem](finditem.md) <br/> |Определяет запрос для поиска элементов в почтовом ящике.  <br/> |
|[ResolveNames](resolvenames.md) <br/> |Определяет запрос для разрешения неоднозначных имен.  <br/> |
   
## <a name="remarks"></a>Замечания

Элемент **ParentFolderIds** необходимо использовать [FolderId](folderid.md) или элемент [DistinguishedFolderId](distinguishedfolderid.md) . Неограниченное число папок, которые могут задаваться для поиска. 
  
## <a name="example"></a>Пример

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
  xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <FindFolder Traversal="Shallow" xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [FindFolder Operation](findfolder-operation.md)  
- [FindItem Operation](finditem-operation.md) 
- [Операция ResolveNames](resolvenames-operation.md)

