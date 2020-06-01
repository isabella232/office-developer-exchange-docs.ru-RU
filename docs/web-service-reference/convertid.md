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
description: Элемент ConvertId определяет запрос на преобразование идентификаторов элементов и папок между поддерживаемыми форматами Exchange. Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).
ms.openlocfilehash: d421baf1f29fb59a8c6eb2b09e1fa0e8a38ffaa4
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44452540"
---
# <a name="convertid"></a>ConvertId

Элемент **ConvertId** определяет запрос на преобразование идентификаторов элементов и папок между поддерживаемыми форматами Exchange. Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1). 
  
```xml
<ConvertId DestinationFormat="">
   <SourceIds/>
</ConvertId>
```

 **конвертидтипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|**дестинатионформат** <br/> |Описывает формат идентификатора, который будет возвращен для всех преобразованных идентификаторов. Дестинатионформат описывается в Идформаттипе.  <br/> |
   
#### <a name="destinationformat-attribute"></a>Атрибут Дестинатионформат

|**Значение**|**Описание**|
|:-----|:-----|
|**евслегациид** <br/> |Представляет формат идентификатора, который используется для идентификаторов веб-служб Exchange, предоставляемых в исходной версии Exchange 2007.  <br/> |
|**евсид** <br/> |Представляет формат идентификатора, используемого для идентификаторов веб-служб Exchange, начиная с Exchange Server 2007 с пакетом обновления 1 (SP1).  <br/> |
|**Код** <br/> |Представляет идентификатор MAPI, как в свойстве PR_ENTRYID.  <br/> |
|**хексентрид** <br/> |Представляет идентификатор события календаря доступности. Это представление свойства PR_ENTRYID в шестнадцатеричной кодировке.  <br/> |
|**StoreId** <br/> |Представляет идентификатор хранилища Exchange.  <br/> |
|**оваид** <br/> |Представляет формат идентификатора веб-клиента Outlook.  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[саурцеидс](sourceids.md) <br/> |Содержит идентификаторы источников для преобразования.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

Нет.
  
## <a name="remarks"></a>Примечания

Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |схема сообщений  <br/> |
|Файл проверки  <br/> |Messages. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операция ConvertId](convertid-operation.md)


- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)


[Преобразование идентификаторов](https://msdn.microsoft.com/library/a5391746-b6ef-4f48-8fc8-8255258651aa%28Office.15%29.aspx)

