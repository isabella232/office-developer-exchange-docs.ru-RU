---
title: BaseShape
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- BaseShape
api_type:
- schema
ms.assetid: 42c04f3b-abaa-4197-a3d6-d21677ffb1c0
description: Элемент BaseShape определяет набор свойств, возвращаемого в ответе элемента или папки.
ms.openlocfilehash: b4e7f5c6d6520e7338f274b6275e371366b1bed5
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59514860"
---
# <a name="baseshape"></a>BaseShape

Элемент **BaseShape** определяет набор свойств, возвращаемого в ответе элемента или папки. 
  
```xml
<BaseShape>IdOnly or Default or AllProperties</BaseShape>
```

 **DefaultShapeNamesType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[FolderShape](foldershape.md) <br/> | Определяет свойства папок, которые необходимо включить в ответ GetFolder, FindFolder или SyncFolderHierarchy.<br/><br/>Ниже приводится выражение XPath к этому элементу:<br/><br/>`/GetFolder/FolderShape` <br/>  `/FindFolder/FolderShape` <br/>  `/SyncFolderHierarchy/FolderShape` <br/> |
|[ItemShape](itemshape.md) <br/> | Определяет свойства и содержимое элемента, которые необходимо включить в ответ GetItem, FindItem или SyncFolderItems.<br/><br/>Ниже приводится выражение XPath к этому элементу:<br/><br/>`/GetItem/ItemShape` <br/>  `/FindItem/ItemShape` <br/>  `/SyncFolderItems/ItemShape` <br/> |
   
## <a name="text-value"></a>Текстовое значение

Требуется текстовое значение. В следующей таблице перечислены возможные текстовые значения.
  
**Текстовые значения элемента BaseShape**

|**Значение**|**Описание**|
|:-----|:-----|
|IdOnly  <br/> |Возвращает только элемент или папку.  <br/> |
|По умолчанию  <br/> |Возвращает набор свойств, определяемого как по умолчанию для элемента или папки.  <br/> |
|AllProperties  <br/> |Возвращает все свойства, используемые в Exchange бизнес-логики для построения папки.  <br/> |
   
В следующей таблице перечислены свойства по умолчанию, возвращаемые для запроса FindFolder. Все подмостки данной папки возвращаются в порядке по имени.
  
**Свойства по умолчанию**

|**Folder**|**Свойства по умолчанию**|
|:-----|:-----|
|Inbox;  <br/> |FolderId, display name, unread count, total count, subfolder count  <br/> |
|Контакты  <br/> |FolderId, display name, total count, subfolder count  <br/> |
|Календарь  <br/> |FolderId, display name, subfolder count  <br/> |
|Черновики  <br/> |FolderId, display name, unread count, total count, subfolder count  <br/> |
|Удаленные элементы  <br/> |FolderId, display name, unread count, total count, subfolder count  <br/> |
|Другие папки  <br/> |FolderId, display name, unread count, total count, subfolder count  <br/> |
|Исходящие  <br/> |FolderId, display name, unread count, total count, subfolder count  <br/> |
|Задачи  <br/> |FolderId, display name, past due count, total count, subfolder count  <br/> |
|Примечания.  <br/> |FolderId, display name, total count, subfolder count  <br/> |
   
## <a name="remarks"></a>Заметки

Чтобы вернуть свойства в дополнение к свойствам, идентифицированным элементом [BaseShape,](baseshape.md) используйте [элемент AdditionalProperties.](additionalproperties.md) 
  
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
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [FolderShape](foldershape.md)
- [ItemShape](itemshape.md)

