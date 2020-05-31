---
title: SyncFolderHierarchy
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SyncFolderHierarchy
api_type:
- schema
ms.assetid: 55df4d01-e48e-4263-a851-78a66ad1093a
description: Элемент SyncFolderHierarchy определяет запрос на синхронизацию иерархии папок в клиенте.
ms.openlocfilehash: f72640e5605dd83e92cd323cb00e4d2f64406245
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19840122"
---
# <a name="syncfolderhierarchy"></a>SyncFolderHierarchy

Элемент **SyncFolderHierarchy** определяет запрос на синхронизацию иерархии папок в клиенте. 
  
```xml
<SyncFolderHierarchy>
   <FolderShape/>   <SyncFolderId/>
   <SyncState/>
</SyncFolderHierarchy>
```

 **синкфолдерхиерарчитипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[фолдершапе](foldershape.md) <br/> |Определяет свойства папки, включаемые в ответ [SyncFolderHierarchy](syncfolderhierarchy.md) .  <br/> |
|[синкфолдерид](syncfolderid.md) <br/> |Представляет папку, содержащую синхронизируемые элементы. Этот элемент является необязательным.  <br/> |
|[синкстате](syncstate-ex15websvcsotherref.md) <br/> |Содержит форму синхронизации данных с кодировкой base64, которая обновляется после каждого успешного выполнения запроса. Используется для определения состояния синхронизации.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

Нет.
  
## <a name="remarks"></a>Примечания

Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операция SyncFolderHierarchy](syncfolderhierarchy-operation.md)


- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

