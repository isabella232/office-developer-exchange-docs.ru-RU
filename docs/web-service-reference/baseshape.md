---
title: басешапе
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
description: Элемент Басешапе определяет набор свойств, возвращаемых в ответе элемента или папки.
ms.openlocfilehash: 9b3f00ff94fbfe6ad6373b16ad95eb9136f81c64
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44464492"
---
# <a name="baseshape"></a>басешапе

Элемент **басешапе** определяет набор свойств, возвращаемых в ответе элемента или папки. 
  
```xml
<BaseShape>IdOnly or Default or AllProperties</BaseShape>
```

 **дефаултшапенаместипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

Нет
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[фолдершапе](foldershape.md) <br/> | Определяет свойства папки, которые необходимо включить в ответ "GetResponse Folder", "FindFolder" или "SyncFolderHierarchy".<br/><br/>Ниже приведены выражения XPath для этого элемента.<br/><br/>`/GetFolder/FolderShape` <br/>  `/FindFolder/FolderShape` <br/>  `/SyncFolderHierarchy/FolderShape` <br/> |
|[итемшапе](itemshape.md) <br/> | Определяет свойства и контент элемента, включаемые в ответ GetItem, FindItem или SyncFolderItems.<br/><br/>Ниже приведены выражения XPath для этого элемента.<br/><br/>`/GetItem/ItemShape` <br/>  `/FindItem/ItemShape` <br/>  `/SyncFolderItems/ItemShape` <br/> |
   
## <a name="text-value"></a>Текстовое значение

Необходимо указать текстовое значение. В приведенной ниже таблице перечислены возможные текстовые значения.
  
**Текстовые значения для элемента Басешапе**

|**Значение**|**Описание**|
|:-----|:-----|
|идонли  <br/> |Возвращает только идентификатор элемента или папки.  <br/> |
|По умолчанию  <br/> |Возвращает набор свойств, которые определены как значения по умолчанию для элемента или папки.  <br/> |
|аллпропертиес  <br/> |Возвращает все свойства, используемые уровнем бизнес-логики Exchange для создания папки.  <br/> |
   
В следующей таблице перечислены свойства по умолчанию, которые возвращаются для запроса FindFolder. Все подпапки данной папки возвращаются в порядке по имени.
  
**Свойства по умолчанию**

|**Folder**|**Свойства по умолчанию**|
|:-----|:-----|
|Inbox;  <br/> |FolderId, отображаемое имя, непрочтенное количество, общее количество, число вложений  <br/> |
|Контакты  <br/> |FolderId, отображаемое имя, общее количество, число вложенных папок  <br/> |
|Календарь  <br/> |FolderId, отображаемое имя, число вложенных папок  <br/> |
|Черновики  <br/> |FolderId, отображаемое имя, непрочтенное количество, общее количество, число вложений  <br/> |
|Удаленные элементы  <br/> |FolderId, отображаемое имя, непрочтенное количество, общее количество, число вложений  <br/> |
|Другие папки  <br/> |FolderId, отображаемое имя, непрочтенное количество, общее количество, число вложений  <br/> |
|Исходящие  <br/> |FolderId, отображаемое имя, непрочтенное количество, общее количество, число вложений  <br/> |
|Задачи  <br/> |FolderId, отображаемое имя, количество просроченных, общее количество, число вложенных папок  <br/> |
|Примечания  <br/> |FolderId, отображаемое имя, общее количество, число вложенных папок  <br/> |
   
## <a name="remarks"></a>Примечания

Чтобы вернуть свойства в дополнение к элементам, идентифицируемым элементом [басешапе](baseshape.md) , используйте элемент [аддитионалпропертиес](additionalproperties.md) . 
  
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
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [фолдершапе](foldershape.md)
- [итемшапе](itemshape.md)

