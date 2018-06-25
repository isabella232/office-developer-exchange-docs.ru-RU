---
title: ConvertId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ConvertId
api_type:
- schema
ms.assetid: 9684c22c-29d4-4f7f-befc-8cd41da56d38
description: Элемент ConvertId определяет запрос на преобразование идентификаторы элементов и папок между форматы, поддерживаемые Exchange. Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).
ms.openlocfilehash: 956f6464fd9013f9e72d2915f21c3b011d0add5b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761825"
---
# <a name="convertid"></a>ConvertId

Элемент **ConvertId** определяет запрос на преобразование идентификаторы элементов и папок между форматы, поддерживаемые Exchange. Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1). 
  
```xml
<ConvertId DestinationFormat="">
   <SourceIds/>
</ConvertId>
```

 **ConvertIdType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|**DestinationFormat** <br/> |Описывает формат идентификатора, будут возвращены все преобразованные идентификаторов. Описывается DestinationFormat IdFormatType.  <br/> |
   
#### <a name="destinationformat-attribute"></a>Атрибут DestinationFormat

|**Значение**|**Описание**|
|:-----|:-----|
|**EwsLegacyId** <br/> |Представляет идентификатор формата, который используется для идентификаторов веб-служб Exchange, которые предоставляются в первоначальной версии Exchange 2007.  <br/> |
|**EwsId** <br/> |Представляет идентификатор формата, который используется для идентификаторов веб-служб Exchange, начиная с Exchange Server 2007 с пакетом обновления 1.  <br/> |
|**Идентификатор записи** <br/> |Представляет идентификатор MAPI, как и свойство PR_ENTRYID.  <br/> |
|**HexEntryId** <br/> |Представляет идентификатор события календаря доступности. Это представление шестнадцатеричном формате PR_ENTRYID свойства.  <br/> |
|**StoreId** <br/> |Представляет идентификатор хранилища Exchange.  <br/> |
|**OwaId** <br/> |Представляет формат идентификатора Outlook Web Access.  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[SourceIds](sourceids.md) <br/> |Содержит идентификаторы источника для преобразования.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

Нет.
  
## <a name="remarks"></a>Замечания

Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема сообщения  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операция ConvertId](convertid-operation.md)


- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)


[Преобразование идентификаторов](http://msdn.microsoft.com/library/a5391746-b6ef-4f48-8fc8-8255258651aa%28Office.15%29.aspx)

