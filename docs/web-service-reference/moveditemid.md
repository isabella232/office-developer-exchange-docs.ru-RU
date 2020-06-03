---
title: моведитемид
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 7d5425ab-1e75-43d1-b801-802ff5139df6
description: Элемент Моведитемид указывает идентификатор элемента, перемещенного операцией MarkAsJunk.
ms.openlocfilehash: 5cf8800ec672278691348bbcd8c6c8cc7a12905b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44468616"
---
# <a name="moveditemid"></a>моведитемид

Элемент **моведитемид** указывает идентификатор элемента, перемещенного операцией **MarkAsJunk** . 
  
```XML
<MovedItemId Id="" ChangeKey=""/>
```

 **итемидтипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|Id  <br/> |Значение атрибута **ID** — это идентификатор элемента, который перемещается с помощью операции **MarkAsJunk** . После перемещения идентификатор элемента останется прежним.  <br/> |
|чанжекэй  <br/> |Значение атрибута **чанжекэй** — это ключ изменения перемещенного элемента. Изменение ключа изменения после перемещения элемента с помощью операции **MarkAsJunk** .  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

Отсутствуют.
  
### <a name="parent-elements"></a>Родительские элементы

[маркасжункреспонсемессаже](markasjunkresponsemessage.md)
  
## <a name="remarks"></a>Примечания

Этот элемент появился в Exchange Server 2013.
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |messages. xsd  <br/> |
|Может быть пустым  <br/> ||
   

