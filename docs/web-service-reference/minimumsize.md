---
title: MinimumSize
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 841d229c-140c-48bd-b3a7-21478fcea2fb
description: Элемент MinimumSize представляет минимальный размер сообщения, который должен быть для применения условия или исключения.
ms.openlocfilehash: c3f1284a5a82731093863b0a621bcf2f7f55cf22
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59540652"
---
# <a name="minimumsize"></a>MinimumSize

Элемент **MinimumSize** представляет минимальный размер сообщения, который должен быть для применения условия или исключения. 
  
```XML
<MinimumSize/>
```

 **int**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[WithinSizeRange](withinsizerange.md) <br/> |Указывает минимальные и максимальные размеры входящих сообщений для применения условия или исключения.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение — это integer, который определяет минимальный размер сообщения в bytes.
  
## <a name="remarks"></a>Заметки

Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |True  <br/> |
   
## <a name="see-also"></a>См. также



[MaximumSize](maximumsize.md)


- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

