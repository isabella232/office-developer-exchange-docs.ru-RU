---
title: SizeRequested
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: e86f98b6-83b5-4530-80eb-dc5df42e2c62
description: Элемент SizeRequested содержит запрашиваемую фотографию для операции GetUserPhoto.
ms.openlocfilehash: 799869a85d7f72e79753a73f9c259388a2702bf5
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59545918"
---
# <a name="sizerequested"></a>SizeRequested

Элемент **SizeRequested** содержит запрашиваемую фотографию для операции **GetUserPhoto.** 
  
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

Текстовое значение элемента **SizeRequested** — запрашиваемого размера фотографии цифрового изображения, возвращаемого с сервера. В следующей таблице определяются текстовые значения элемента **SizeRequested.** 
  
|**Значение**|**Смысл**|
|:-----|:-----|
|HR48x48  <br/> |Изображение высотой 48 пикселей и шириной 48 пикселей.  <br/> |
|HR64x64  <br/> |Изображение имеет высоту 64 пикселя и ширину 64 пикселя.  <br/> |
|HR96x96  <br/> |Изображение высотой 96 пикселей и шириной 96 пикселей.  <br/> |
|HR120x120  <br/> |Изображение высотой 120 пикселей и шириной 120 пикселей.  <br/> |
|HR240x240  <br/> |Изображение высотой 240 пикселей и шириной 240 пикселей.  <br/> |
|HR360x360  <br/> |Изображение имеет высоту 360 пикселей и ширину 360 пикселей.  <br/> |
|HR432x432  <br/> |Изображение имеет высоту 432 пикселя и ширину 432 пикселя.  <br/> |
|HR504x504  <br/> |Изображение имеет высоту 504 пикселя и ширину 504 пикселя.  <br/> |
|HR648x648  <br/> |Изображение высотой 648 пикселей и шириной 648 пикселей.  <br/> |
   
## <a name="remarks"></a>Заметки

Этот элемент появился в Exchange Server 2013.
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> ||
   

