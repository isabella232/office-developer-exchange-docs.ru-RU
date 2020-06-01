---
title: минимумсизе
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 841d229c-140c-48bd-b3a7-21478fcea2fb
description: Элемент Минимумсизе представляет минимальный размер сообщения, которое должно быть применено к определенному условию или исключению.
ms.openlocfilehash: b43a8b5916747c4e3e4ca9b66cf8b9d73f5f8942
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/01/2020
ms.locfileid: "44464205"
---
# <a name="minimumsize"></a>минимумсизе

Элемент **минимумсизе** представляет минимальный размер сообщения, которое должно быть применено к определенному условию или исключению. 
  
```XML
<MinimumSize/>
```

 **int**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

Отсутствуют.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[висинсизеранже](withinsizerange.md) <br/> |Указывает минимальный и максимальный размеры для входящих сообщений, для которых необходимо применить условие или исключение.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение — это целое число, определяющее минимальный размер сообщения в байтах.
  
## <a name="remarks"></a>Примечания

Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages. xsd  <br/> |
|Может быть пустым  <br/> |True  <br/> |
   
## <a name="see-also"></a>См. также



[максимумсизе](maximumsize.md)


- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

