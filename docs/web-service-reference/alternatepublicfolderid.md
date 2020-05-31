---
title: алтернатепубликфолдерид
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
description: Элемент Алтернатепубликфолдерид описывает идентификатор общедоступной папки для преобразования в другой формат идентификатора. Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).
ms.openlocfilehash: 32e6e75eb381e479baf5fdb5ad0a40b32c1b02a9
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761377"
---
# <a name="alternatepublicfolderid"></a>алтернатепубликфолдерид

Элемент **алтернатепубликфолдерид** описывает идентификатор общедоступной папки для преобразования в другой формат идентификатора. Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1). 
  
- [ConvertId](convertid.md)
  
- [саурцеидс](sourceids.md)
  
- [алтернатепубликфолдерид](alternatepublicfolderid.md)
  
```xml
<AlternatePublicFolderId FolderId="" Format="" />
```

 **алтернатепубликфолдеридтипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|FolderId  <br/> |Содержит идентификатор общедоступной папки для преобразования. Этот атрибут является обязательным.  <br/> |
|Format  <br/> |Определяет формат, описывающий преобразуемый идентификатор общедоступной папки. Этот атрибут является обязательным.  <br/> |
   
#### <a name="format-attribute"></a>Атрибут Format

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
|[саурцеидс](sourceids.md) <br/> |Содержит идентификаторы источников для преобразования. Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).  <br/> |
   
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

