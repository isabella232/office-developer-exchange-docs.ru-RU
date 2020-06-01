---
title: фолдершапе
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
description: Элемент Фолдершапе определяет свойства папки, которые необходимо включить в ответ "GetResponse Folder", "FindFolder" и SyncFolderHierarchy.
ms.openlocfilehash: f841fcc4570604c474387dfa24ec07c9d2784f62
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44461347"
---
# <a name="foldershape"></a>фолдершапе

Элемент **фолдершапе** определяет свойства папки, которые необходимо включить в ответ "GetResponse [Folder](getfolder.md)", " [FindFolder](findfolder.md)" и [SyncFolderHierarchy](syncfolderhierarchy.md) . 
  
```xml
<FolderShape>
   <BaseShape/>
   <AdditionalProperties/>
</FolderShape>
```

 **фолдерреспонсешапетипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[басешапе](baseshape.md) <br/> |Определяет базовую конфигурацию свойств, возвращаемых в ответе.  <br/> |
|[аддитионалпропертиес](additionalproperties.md) <br/> |Определяет дополнительные свойства, возвращаемые в ответе.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[FindFolder](findfolder.md) <br/> |Определяет запрос на идентификацию папок в почтовом ящике.  <br/> Ниже приведено выражение XPath для этого элемента:  <br/>  `/FindFolder` <br/> |
|[GetFolder](getfolder.md) <br/> |Определяет запрос на получение папки из хранилища Exchange.  <br/> Ниже приведено выражение XPath для этого элемента:  <br/>  `/GetFolder` <br/> |
|[SyncFolderHierarchy](syncfolderhierarchy.md) <br/> |Определяет запрос на синхронизацию иерархии папок в клиенте.  <br/> Ниже приведено выражение XPath для этого элемента:  <br/>  `/SyncFolderHierarchy` <br/> |
   
## <a name="remarks"></a>Примечания

Элемент **фолдершапе** является обязательным дочерним элементом элемента [FindFolder](findfolder.md) . 
  
Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.
  
## <a name="example"></a>Пример

В приведенном ниже примере запроса показано, как найти все папки, расположенные на первом уровне папки "Входящие".
  
```
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



[FindFolder](findfolder.md)

