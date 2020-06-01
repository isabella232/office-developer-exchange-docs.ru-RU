---
title: парентфолдеридс
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
description: Элемент Парентфолдеридс определяет папки для операций FindItem и FindFolder для поиска.
ms.openlocfilehash: 6bc4b9cfe96c6c83cbeb623ec176e33177356bbc
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465431"
---
# <a name="parentfolderids"></a>парентфолдеридс

Элемент **парентфолдеридс** определяет папки для операций FindItem и FindFolder для поиска. 
  
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

**нонемптяррайофбасефолдеридстипе**

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[FolderId](folderid.md) <br/> |Содержит идентификатор и ключ изменения папки. Элемент **парентфолдеридс** должен использовать либо этот элемент, либо элемент [дистингуишедфолдерид](distinguishedfolderid.md) .  <br/> |
|[дистингуишедфолдерид](distinguishedfolderid.md) <br/> |Определяет папки Microsoft Exchange Server 2007, на которые можно ссылаться по имени. Элемент **парентфолдеридс** должен использовать либо этот элемент, либо элемент [FolderId](folderid.md) .  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[FindFolder](findfolder.md) <br/> |Определяет запрос на идентификацию папок в почтовом ящике.  <br/> |
|[FindItem](finditem.md) <br/> |Определяет запрос на поиск элементов в почтовом ящике.  <br/> |
|[ResolveNames](resolvenames.md) <br/> |Определяет запрос на разрешение неоднозначных имен.  <br/> |
   
## <a name="remarks"></a>Примечания

Элемент **парентфолдеридс** должен использовать элемент [FolderId](folderid.md) или [дистингуишедфолдерид](distinguishedfolderid.md) . Для поиска может быть определено неограниченное количество папок. 
  
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
|Файл проверки  <br/> |Messages. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Операция FindFolder](findfolder-operation.md)  
- [Операция FindItem](finditem-operation.md) 
- [Операция ResolveNames](resolvenames-operation.md)

