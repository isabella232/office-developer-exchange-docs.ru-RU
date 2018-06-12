---
title: BaseShape
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- BaseShape
api_type:
- schema
ms.assetid: 42c04f3b-abaa-4197-a3d6-d21677ffb1c0
description: Элемент BaseShape определяет набор свойств, чтобы вернуться в элемент или папку ответ.
ms.openlocfilehash: 69b27d23fd75d4c1a274f31dfa419b759dbb2bbe
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761555"
---
# <a name="baseshape"></a>BaseShape

Элемент **BaseShape** определяет набор свойств, чтобы вернуться в элемент или папку ответ. 
  
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
|[FolderShape](foldershape.md) <br/> | Задает свойства папки для включения в ответе GetFolder, FindFolder или SyncFolderHierarchy.<br/><br/>Ниже приведены выражения XPath для этого элемента.<br/><br/>`/GetFolder/FolderShape` <br/>  `/FindFolder/FolderShape` <br/>  `/SyncFolderHierarchy/FolderShape` <br/> |
|[ItemShape](itemshape.md) <br/> | Определяет свойства элемента и содержимого для включения в GetItem, FindItem или SyncFolderItems ответа.<br/><br/>Ниже приведены выражения XPath для этого элемента.<br/><br/>`/GetItem/ItemShape` <br/>  `/FindItem/ItemShape` <br/>  `/SyncFolderItems/ItemShape` <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение является обязательным. В следующей таблице перечислены возможные текстовые значения.
  
**Текстовые значения для элемента BaseShape**

|**Значение**|**Описание**|
|:-----|:-----|
|IdOnly  <br/> |Возвращает только идентификатор элемента или папки  <br/> |
|Значение по умолчанию  <br/> |Возвращает набор свойств, которые определены по умолчанию для элемента или папки.  <br/> |
|AllProperties  <br/> |Возвращает все свойства, используемые уровнем бизнес-логики Exchange для создания папки.  <br/> |
   
В следующей таблице приведены свойства по умолчанию, возвращенных по запросу FindFolder. Все вложенные папки указанной папки возвращаются в порядке по имени.
  
**Свойства по умолчанию**

|**Folder**|**Свойства по умолчанию**|
|:-----|:-----|
|Inbox  <br/> |FolderId, отображаемое имя, число непрочтенных сообщений, общее число, число вложенной папке  <br/> |
|Контакты  <br/> |FolderId, отображаемое имя, общее число, число вложенной папке  <br/> |
|Календарь  <br/> |FolderId, отображаемое имя вложенной папке count  <br/> |
|���������  <br/> |FolderId, отображаемое имя, число непрочтенных сообщений, общее число, число вложенной папке  <br/> |
|"Удаленные"  <br/> |FolderId, отображаемое имя, число непрочтенных сообщений, общее число, число вложенной папке  <br/> |
|Другие папки  <br/> |FolderId, отображаемое имя, число непрочтенных сообщений, общее число, число вложенной папке  <br/> |
|Исходящие  <br/> |FolderId, отображаемое имя, число непрочтенных сообщений, общее число, число вложенной папке  <br/> |
|Задачи  <br/> |FolderId, отображаемое имя просроченных count, общее число, число вложенной папке  <br/> |
|����������  <br/> |FolderId, отображаемое имя, общее число, число вложенной папке  <br/> |
   
## <a name="remarks"></a>Замечания

Чтобы вернуть свойства помимо тех, обнаруженных в элементе [BaseShape](baseshape.md) , используйте элемент [AdditionalProperties](additionalproperties.md) . 
  
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
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [FolderShape](foldershape.md)
- [ItemShape](itemshape.md)

