---
title: AlternatePublicFolderId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AlternatePublicFolderId
api_type:
- schema
ms.assetid: 0a4dc1cc-959e-4b93-aa3a-3020ca8b8a02
description: Элемент AlternatePublicFolderId описывает идентификатор общих папок для преобразования в другой формат идентификатора. Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).
ms.openlocfilehash: 32e6e75eb381e479baf5fdb5ad0a40b32c1b02a9
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761377"
---
# <a name="alternatepublicfolderid"></a>AlternatePublicFolderId

Элемент **AlternatePublicFolderId** описывает идентификатор общих папок для преобразования в другой формат идентификатора. Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1). 
  
- [ConvertId](convertid.md)
  
- [SourceIds](sourceids.md)
  
- [AlternatePublicFolderId](alternatepublicfolderid.md)
  
```xml
<AlternatePublicFolderId FolderId="" Format="" />
```

 **AlternatePublicFolderIdType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|FolderId  <br/> |Содержит идентификатор общей папки для преобразования. Этот атрибут является обязательным.  <br/> |
|Формат  <br/> |Определяет формат, который описывает идентификатор общей папки для преобразования. Этот атрибут является обязательным.  <br/> |
   
#### <a name="format-attribute"></a>Атрибут формата

|**Значение**|**Описание**|
|:-----|:-----|
|EwsLegacyId  <br/> |Описываются идентификаторы, которые создаются веб-служб Exchange в первоначальной версии Exchange 2007.  <br/> |
|EwsId  <br/> |Описываются идентификаторы, которые создаются веб-служб Exchange, начиная с Exchange 2007 с пакетом обновления 1.  <br/> |
|Идентификатор записи  <br/> |Описываются идентификаторы MAPI, как и свойство PR_ENTRYID.  <br/> |
|HexEntryId  <br/> |Описывает представление шестнадцатеричном формате PR_ENTRYID свойства. Это формат идентификаторы событий календаря доступности.  <br/> |
|StoreId  <br/> |Описываются идентификаторы хранилища Exchange.  <br/> |
|OwaId  <br/> |Описывает идентификатор Outlook Web Access.  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[SourceIds](sourceids.md) <br/> |Содержит идентификаторы источника для преобразования. Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).  <br/> |
   
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |True  <br/> |
   
## <a name="see-also"></a>См. также

- [Операция ConvertId](convertid-operation.md)
- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)
- [Преобразование идентификаторов](http://msdn.microsoft.com/library/a5391746-b6ef-4f48-8fc8-8255258651aa%28Office.15%29.aspx)

