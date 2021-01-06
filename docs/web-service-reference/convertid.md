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
description: Элемент ConvertId определяет запрос на преобразование идентификаторов элементов и папок между поддерживаемами форматами Exchange. Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).
ms.openlocfilehash: d421baf1f29fb59a8c6eb2b09e1fa0e8a38ffaa4
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44452540"
---
# <a name="convertid"></a>ConvertId

Элемент **ConvertId** определяет запрос на преобразование идентификаторов элементов и папок между поддерживаемами форматами Exchange. Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1). 
  
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
|**DestinationFormat** <br/> |Описывает формат идентификатора, который будет возвращен для всех преобразованных идентификаторов. DestinationFormat описывается с помощью IdFormatType.  <br/> |
   
#### <a name="destinationformat-attribute"></a>Атрибут DestinationFormat

|**Значение**|**Описание**|
|:-----|:-----|
|**EwsLegacyId** <br/> |Представляет формат идентификатора, используемый для идентификаторов веб-служб Exchange, предоставленных в первоначальной версии выпуска Exchange 2007.  <br/> |
|**EwsId** <br/> |Представляет формат идентификатора, используемый для идентификаторов веб-служб Exchange, начиная с Exchange Server 2007 SP1.  <br/> |
|**EntryId** <br/> |Представляет идентификатор MAPI, как в свойстве PR_ENTRYID.  <br/> |
|**HexEntryId** <br/> |Представляет идентификатор события календаря доступности. Это представление свойства, закодированное в PR_ENTRYID кодировки.  <br/> |
|**StoreId** <br/> |Представляет идентификатор магазина Exchange.  <br/> |
|**OwaId** <br/> |Представляет формат идентификатора Outlook Web Access.  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[SourceIds](sourceids.md) <br/> |Содержит идентификаторы источника, которые необходимо преобразовать.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

Нет.
  
## <a name="remarks"></a>Примечания

Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |схема сообщений  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операция ConvertId](convertid-operation.md)


- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)


[Преобразование идентификаторов](https://msdn.microsoft.com/library/a5391746-b6ef-4f48-8fc8-8255258651aa%28Office.15%29.aspx)

