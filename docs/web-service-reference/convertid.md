---
title: ConvertId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- ConvertId
api_type:
- schema
ms.assetid: 9684c22c-29d4-4f7f-befc-8cd41da56d38
description: Элемент ConvertId определяет запрос на преобразование идентификаторов элементов и папок между поддерживаемой Exchange форматами. Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).
ms.openlocfilehash: fe7d46697ba72ba6458136541488f5cd498169f4
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59545561"
---
# <a name="convertid"></a>ConvertId

Элемент **ConvertId** определяет запрос на преобразование идентификаторов элементов и папок между поддерживаемой Exchange форматами. Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1). 
  
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
|**DestinationFormat** <br/> |Описывает формат идентификатора, который будет возвращен для всех преобразованных идентификаторов. DestinationFormat описывается IdFormatType.  <br/> |
   
#### <a name="destinationformat-attribute"></a>Атрибут DestinationFormat

|**Значение**|**Описание**|
|:-----|:-----|
|**EwsLegacyId** <br/> |Представляет формат идентификаторов, используемый для идентификаторов Exchange веб-служб, представленных в начальной версии Exchange 2007 г.  <br/> |
|**EwsId** <br/> |Представляет формат идентификатора, который используется для идентификаторов Exchange веб-служб, начиная с Exchange Server 2007 sp1.  <br/> |
|**EntryId** <br/> |Представляет идентификатор MAPI, как и в свойстве PR_ENTRYID.  <br/> |
|**HexEntryId** <br/> |Представляет идентификатор события календаря доступности. Это кодированное в hexadecimal представление свойства PR_ENTRYID.  <br/> |
|**StoreId** <br/> |Представляет идентификатор Exchange магазина.  <br/> |
|**OwaId** <br/> |Представляет формат идентификатора Outlook веб-доступа.  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[SourceIds](sourceids.md) <br/> |Содержит исходные идентификаторы для преобразования.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

Нет.
  
## <a name="remarks"></a>Заметки

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

