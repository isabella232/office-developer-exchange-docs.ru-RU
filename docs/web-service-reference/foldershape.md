---
title: FolderShape
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FolderShape
api_type:
- schema
ms.assetid: 244f4f46-a33d-4764-92e3-1bddb4dc6a49
description: Элемент FolderShape определяет свойства папки для включения в GetFolder, FindFolder или SyncFolderHierarchy ответа.
ms.openlocfilehash: 8ebdd70ef13ee9f0cce9020b9212576cba782be4
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762640"
---
# <a name="foldershape"></a>FolderShape

Элемент **FolderShape** определяет свойства папки для включения в [GetFolder](getfolder.md), [FindFolder](findfolder.md)или [SyncFolderHierarchy](syncfolderhierarchy.md) ответа. 
  
```xml
<FolderShape>
   <BaseShape/>
   <AdditionalProperties/>
</FolderShape>
```

 **FolderResponseShapeType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[BaseShape](baseshape.md) <br/> |Определяет базовую конфигурацию свойства, возвращаемые в ответе.  <br/> |
|[AdditionalProperties](additionalproperties.md) <br/> |Определяет дополнительные свойства, возвращаемые в ответе.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[FindFolder](findfolder.md) <br/> |Определяет запрос для определения папок в почтовом ящике.  <br/> Ниже приведен выражение XPath для этого элемента.  <br/>  `/FindFolder` <br/> |
|[GetFolder](getfolder.md) <br/> |Определяет запрос на получение папки из хранилища Exchange.  <br/> Ниже приведен выражение XPath для этого элемента.  <br/>  `/GetFolder` <br/> |
|[SyncFolderHierarchy](syncfolderhierarchy.md) <br/> |Определяет запрос для синхронизации иерархии папок на клиенте.  <br/> Ниже приведен выражение XPath для этого элемента.  <br/>  `/SyncFolderHierarchy` <br/> |
   
## <a name="remarks"></a>Замечания

Элемент **FolderShape** является обязательным дочерним элементом элемента [FindFolder](findfolder.md) . 
  
Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.
  
## <a name="example"></a>Пример

Следующий пример запроса показано, как найти все папки, расположенной в первый уровень папки "Входящие".
  
```
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



[FindFolder](findfolder.md)

