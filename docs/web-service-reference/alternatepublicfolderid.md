---
title: AlternatePublicFolderId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- AlternatePublicFolderId
api_type:
- schema
ms.assetid: 0a4dc1cc-959e-4b93-aa3a-3020ca8b8a02
description: Элемент AlternatePublicFolderId описывает идентификатор общедоступных папок для преобразования в другой формат идентификатора. Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).
ms.openlocfilehash: 7c4471c0c1e3e1eee3b47eba42f924340891c777
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59525360"
---
# <a name="alternatepublicfolderid"></a>AlternatePublicFolderId

Элемент **AlternatePublicFolderId** описывает идентификатор общедоступных папок для преобразования в другой формат идентификатора. Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1). 
  
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
|FolderId  <br/> |Содержит идентификатор общедоступных папок для преобразования. Этот атрибут является обязательным.  <br/> |
|Формат  <br/> |Определяет формат, который описывает идентификатор общедоступных папок для преобразования. Этот атрибут является обязательным.  <br/> |
   
#### <a name="format-attribute"></a>Атрибут Format

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
|[SourceIds](sourceids.md) <br/> |Содержит исходные идентификаторы для преобразования. Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).  <br/> |
   
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

