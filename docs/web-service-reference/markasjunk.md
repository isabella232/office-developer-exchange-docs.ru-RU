---
title: MarkAsJunk
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f06bafc6-7ee3-4b2b-9fd1-7c51328f4729
description: Элемент MarkAsJunk указывает запрос на перемещение элемента в папку нежелательной почты и Добавление отправителя в список заблокированных отправителей.
ms.openlocfilehash: fbb3eee7ce350954888931ca55b27f596656b161
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834350"
---
# <a name="markasjunk"></a>MarkAsJunk

Элемент **MarkAsJunk** указывает запрос на перемещение элемента в папку нежелательной почты и Добавление отправителя в список заблокированных отправителей. 
  
```XML
<MarkAsJunk IsJunk="true | false" MoveItem="true | false">
   <ItemIds/>
</MarkAsJunk>
```

 **маркасжунктипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|Нежелательная почта  <br/> |Текстовое значение **true** **для атрибута InAttribute** указывает, что отправитель электронной почты добавляется в список заблокированных отправителей. Значение **false** указывает, что отправитель электронной почты удаляется из списка заблокированных отправителей, если он уже есть в списке.  <br/> |
|MoveItem  <br/> |Текстовое значение **true** для атрибута **MoveItem** указывает на то, что элемент перемещается в папку нежелательной почты по умолчанию. Значение **false** указывает на то, что элемент не перемещается в папку нежелательной почты по умолчанию.  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

[итемидс](itemids.md)
  
### <a name="parent-elements"></a>Родительские элементы

Нет.
  
## <a name="remarks"></a>Примечания

Этот элемент появился в Exchange Server 2013.
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |messages. xsd  <br/> |
|Может быть пустым  <br/> ||
   

