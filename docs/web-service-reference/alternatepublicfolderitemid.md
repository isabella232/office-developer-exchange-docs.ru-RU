---
title: AlternatePublicFolderItemId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AlternatePublicFolderItemId
api_type:
- schema
ms.assetid: a67df9b9-8fdb-42de-b9c5-8377b71fa3d9
description: Элемент AlternatePublicFolderItemId описывает идентификатор элемента общей папки для преобразования в другой формат идентификатора. Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).
ms.openlocfilehash: 2240f3ff80c2c5b705611c3cf9286faa62d204cc
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761376"
---
# <a name="alternatepublicfolderitemid"></a>AlternatePublicFolderItemId

Элемент **AlternatePublicFolderItemId** описывает идентификатор элемента общей папки для преобразования в другой формат идентификатора. Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1). 
  
- [ConvertId](convertid.md)
  
- [SourceIds](sourceids.md)
  
- [AlternatePublicFolderItemId](alternatepublicfolderitemid.md)
  
```xml
<AlternatePublicFolderItemId FolderId="" Format="" ItemId=""/>
```

 **AlternatePublicFolderItemIdType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|FolderId  <br/> |Определяет общую папку, содержащую элемент общей папки. Этот атрибут является обязательным.  <br/> |
|Формат  <br/> |Определяет формат, который описывает идентификатор элемента общей папки для преобразования. Этот атрибут является обязательным.  <br/> |
|Идентификатор элемента  <br/> |Идентификатор элемента общей папки для преобразования. Этот атрибут является обязательным.  <br/> |
   
#### <a name="format-attribute-values"></a>Значения атрибутов формата

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
|[SourceIds](sourceids.md) <br/> |Содержит идентификаторы источника для преобразования. Этот элемент появился в Exchange 2007 с пакетом обновления 1.  <br/> |
   
## <a name="remarks"></a>Замечания

Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.
  
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

