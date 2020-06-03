---
title: ретурнневитемидс
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: aeef79e4-31e1-4213-b627-9bac676be018
description: Элемент Ретурнневитемидс указывает, возвращаются ли в ответе идентификаторы элементов новых элементов.
ms.openlocfilehash: 003676c4c034454aa551e42bf3af976183117b8c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465116"
---
# <a name="returnnewitemids"></a>ретурнневитемидс

Элемент **ретурнневитемидс** указывает, возвращаются ли в ответе идентификаторы элементов новых элементов. 
  
```XML
<ReturnNewItemIds/>
```

 **xs: Boolean**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

Отсутствуют.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[CopyItem](copyitem.md) <br/> |Определяет запрос на копирование элемента в почтовом ящике в хранилище Exchange.  <br/> |
|[MoveItem](moveitem.md) <br/> |Определяет запрос на перемещение элемента в хранилище Exchange.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение **true** для элемента **ретурнневитемидс** указывает на то, что в ответе возвращаются новые идентификаторы элементов. Значение **false** указывает, что новые идентификаторы элементов не возвращаются в ответе. 
  
## <a name="remarks"></a>Примечания

Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.Этот элемент появился в Exchange Server 2010 с пакетом обновления 1 (SP1).
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема сообщения  <br/> |
|Файл проверки  <br/> |Messages. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   

