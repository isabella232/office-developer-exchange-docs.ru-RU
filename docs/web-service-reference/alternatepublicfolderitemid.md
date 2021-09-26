---
title: AlternatePublicFolderItemId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- AlternatePublicFolderItemId
api_type:
- schema
ms.assetid: a67df9b9-8fdb-42de-b9c5-8377b71fa3d9
description: Элемент AlternatePublicFolderItemId описывает идентификатор элемента общедоступных папок для преобразования в другой формат идентификатора. Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).
ms.openlocfilehash: e3d71d17c6e9321a1accfbaf90967d2b504f5efe
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59543711"
---
# <a name="alternatepublicfolderitemid"></a>AlternatePublicFolderItemId

Элемент **AlternatePublicFolderItemId** описывает идентификатор элемента общедоступных папок для преобразования в другой формат идентификатора. Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1). 
  
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
|FolderId  <br/> |Определяет общедоступные папки, которые содержат элемент общедоступных папок. Этот атрибут является обязательным.  <br/> |
|Формат  <br/> |Определяет формат, который описывает идентификатор элемента общедоступных папок для преобразования. Этот атрибут является обязательным.  <br/> |
|ItemId  <br/> |Идентификатор элемента общедоступных папок для преобразования. Этот атрибут является обязательным.  <br/> |
   
#### <a name="format-attribute-values"></a>Значения атрибута формата

|**Значение**|**Описание**|
|:-----|:-----|
|EwsLegacyId  <br/> |Описывает идентификаторы, которые Exchange веб-служб в начальной версии Exchange 2007 г.  <br/> |
|EwsId  <br/> |Описывает идентификаторы, которые Exchange веб-Exchange 2007 года.  <br/> |
|EntryId  <br/> |Описывает идентификаторы MAPI, как в PR_ENTRYID свойстве.  <br/> |
|HexEntryId  <br/> |Описывает кодированное с гексадецимальным кодом представление свойства PR_ENTRYID. Это формат идентификаторов событий календаря доступности.  <br/> |
|StoreId  <br/> |Описывает Exchange идентификаторы магазина.  <br/> |
|OwaId  <br/> |Описывает идентификатор Outlook веб-доступа.  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[SourceIds](sourceids.md) <br/> |Содержит исходные идентификаторы для преобразования. Этот элемент появился в Exchange 2007 с пакетом обновления 1.  <br/> |
   
## <a name="remarks"></a>Заметки

Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |True  <br/> |
   
## <a name="see-also"></a>См. также

- [Операция ConvertId](convertid-operation.md)
- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)
- [Преобразование идентификаторов](https://msdn.microsoft.com/library/a5391746-b6ef-4f48-8fc8-8255258651aa%28Office.15%29.aspx)

