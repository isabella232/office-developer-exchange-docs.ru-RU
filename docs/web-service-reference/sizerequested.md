---
title: SizeRequested
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: e86f98b6-83b5-4530-80eb-dc5df42e2c62
description: Элемент SizeRequested содержит размер запрошенного фотографии для выполнения операции GetUserPhoto.
ms.openlocfilehash: 43e422512b1e8f06e410e533e9ae1dc49283d5f6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19835504"
---
# <a name="sizerequested"></a>SizeRequested

Элемент **SizeRequested** содержит размер запрошенного фотографии для выполнения операции **GetUserPhoto** . 
  
```XML
<SizeRequested>HR48x48 | HR64x64 | HR96X96 | HR120X120 | HR240X240 | HR360X360 | HR432X432 | HR504X504 | HR648X648</SizeRequested>
```

 **UserPhotoSizeType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

[GetUserPhoto](getuserphoto.md)
  
## <a name="text-value"></a>Текстовое значение

Текстовое значение элемента **SizeRequested** — размер запрошенного фотографий цифровые изображения, возвращенный с сервера. В следующей таблице указываются текстовые значения для элемента **SizeRequested** . 
  
|**Значение**|**Значение**|
|:-----|:-----|
|HR48x48  <br/> |Изображения — 48 пикселей в высоту и 48 пикселей в высоту.  <br/> |
|HR64x64  <br/> |Изображения — 64 пикселей в высоту и ширину 64 x.  <br/> |
|HR96x96  <br/> |Изображения — 96 пикселей в высоту и ширину 96 пикселей.  <br/> |
|HR120x120  <br/> |Изображения — 120 пикселей в высоту и ширину 120 пикселей.  <br/> |
|HR240x240  <br/> |Изображения — 240 пикселов и 240 пикселов.  <br/> |
|HR360x360  <br/> |Изображения — 360 пикселей в высоту и ширину 360 пикселей.  <br/> |
|HR432x432  <br/> |Изображения — 432 пикселей в высоту и 432 пикселов.  <br/> |
|HR504x504  <br/> |Изображения — 504 пиксела в высоту и 504 пикселов.  <br/> |
|HR648x648  <br/> |Изображения — 648 пикселей в высоту и ширину 648 пикселей.  <br/> |
   
## <a name="remarks"></a>Замечания

Этот элемент появился в Exchange Server 2013.
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> ||
   

