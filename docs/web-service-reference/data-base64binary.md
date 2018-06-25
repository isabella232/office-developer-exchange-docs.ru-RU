---
title: Данные (base64Binary)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Data
api_type:
- schema
ms.assetid: 26d8c2d0-bed2-4aed-b381-20e2ace6892f
description: Элемент Data содержит данные из экспортированного одного элемента или элемент, чтобы отправить в почтовый ящик.
ms.openlocfilehash: 9560273e31a64edb2254489961733dfe7360ad01
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761960"
---
# <a name="data-base64binary"></a>Данные (base64Binary)

Элемент **Data** содержит данные из экспортированного одного элемента или элемент, чтобы отправить в почтовый ящик. 
  
```XML
<Data/>
```

**xs:base64Binary**

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[ExportItemsResponseMessage](exportitemsresponsemessage.md) <br/> |Содержит состояние и результаты запроса на экспорт элемента одного почтового ящика.  <br/> |
|[Элемент (UploadItemType)](item-uploaditemtype.md) <br/> |Представляет один элемент для передачи в почтовый ящик.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Элемент **Data** содержит имена свойств и значений для экспортированного элемента или элементов, которые будут отправлены в почтовый ящик. 
  
## <a name="remarks"></a>Замечания

Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.Этот элемент появился в Exchange Server 2010 с пакетом обновления 1 (SP1).
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема сообщения  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Операция ExportItems](exportitems-operation.md)
- [Операция UploadItems](uploaditems-operation.md)

