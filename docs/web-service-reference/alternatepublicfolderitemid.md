---
title: алтернатепубликфолдеритемид
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
description: Элемент Алтернатепубликфолдеритемид описывает идентификатор элемента общедоступной папки, который необходимо преобразовать в другой формат идентификатора. Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).
ms.openlocfilehash: 2240f3ff80c2c5b705611c3cf9286faa62d204cc
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761376"
---
# <a name="alternatepublicfolderitemid"></a>алтернатепубликфолдеритемид

Элемент **алтернатепубликфолдеритемид** описывает идентификатор элемента общедоступной папки, который необходимо преобразовать в другой формат идентификатора. Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1). 
  
- [ConvertId](convertid.md)
  
- [саурцеидс](sourceids.md)
  
- [алтернатепубликфолдеритемид](alternatepublicfolderitemid.md)
  
```xml
<AlternatePublicFolderItemId FolderId="" Format="" ItemId=""/>
```

 **алтернатепубликфолдеритемидтипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|FolderId  <br/> |Определяет общую папку, содержащую элемент общедоступной папки. Этот атрибут является обязательным.  <br/> |
|Format  <br/> |Определяет формат, описывающий идентификатор элемента общедоступной папки, который требуется преобразовать. Этот атрибут является обязательным.  <br/> |
|Идентификатор  <br/> |Identifier — элемент общедоступной папки, который требуется преобразовать. Этот атрибут является обязательным.  <br/> |
   
#### <a name="format-attribute-values"></a>Форматирование значений атрибутов

|**Значение**|**Описание**|
|:-----|:-----|
|евслегациид  <br/> |Описывает идентификаторы, созданные веб-службами Exchange в исходной версии Exchange 2007.  <br/> |
|евсид  <br/> |Описание идентификаторов, создаваемых веб-службами Exchange начиная с Exchange 2007 с пакетом обновления 1 (SP1).  <br/> |
|Код  <br/> |Описывает идентификаторы MAPI, как в свойстве PR_ENTRYID.  <br/> |
|хексентрид  <br/> |Описывает представление свойства PR_ENTRYID в шестнадцатеричном формате. Это формат идентификаторов событий календаря доступности.  <br/> |
|StoreId  <br/> |Описывает идентификаторы хранилища Exchange.  <br/> |
|оваид  <br/> |Описывает идентификатор Outlook Web Access.  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[саурцеидс](sourceids.md) <br/> |Содержит идентификаторы источников для преобразования. Этот элемент появился в Exchange 2007 с пакетом обновления 1.  <br/> |
   
## <a name="remarks"></a>Примечания

Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> |True  <br/> |
   
## <a name="see-also"></a>См. также

- [Операция ConvertId](convertid-operation.md)
- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)
- [Преобразование идентификаторов](http://msdn.microsoft.com/library/a5391746-b6ef-4f48-8fc8-8255258651aa%28Office.15%29.aspx)

