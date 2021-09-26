---
title: MarkAsJunk
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: f06bafc6-7ee3-4b2b-9fd1-7c51328f4729
description: Элемент MarkAsJunk указывает запрос на перемещение элемента в папку нежелательной почты и добавление отправитель в заблокированный список отправитель.
ms.openlocfilehash: 252c36b8bb3662ffd6c0fe470a81b6f0b55acb69
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59544089"
---
# <a name="markasjunk"></a>MarkAsJunk

Элемент **MarkAsJunk** указывает запрос на перемещение элемента в папку нежелательной почты и добавление отправитель в заблокированный список отправитель. 
  
```XML
<MarkAsJunk IsJunk="true | false" MoveItem="true | false">
   <ItemIds/>
</MarkAsJunk>
```

 **MarkAsJunkType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|IsJunk  <br/> |Значение текста, **истинное для** атрибута **IsJunk,** указывает, что отправитель электронной почты добавляется в заблокированный список отправитель. Значение false **указывает,** что отправитель электронной почты удаляется из заблокированного списка отправитель, если отправитель электронной почты уже находится в списке.  <br/> |
|MoveItem  <br/> |Значение текста, **истинное для** атрибута **MoveItem,** указывает на то, что элемент перемещается в папку нежелательной почты по умолчанию. Значение false **указывает,** что элемент не перемещается в папку нежелательной почты по умолчанию.  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

[ItemIds](itemids.md)
  
### <a name="parent-elements"></a>Родительские элементы

Нет.
  
## <a name="remarks"></a>Заметки

Этот элемент появился в Exchange Server 2013.
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |messages.xsd  <br/> |
|Может быть пустым  <br/> ||
   

