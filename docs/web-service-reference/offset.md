---
title: Offset
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Offset
api_type:
- schema
ms.assetid: dcbb9d85-d90c-4363-b4c9-d081ad03f407
description: Элемент Offset описывает смещение из BaseOffset. Вместе с элементом BaseOffset элемент Offset определяет, является ли время стандартным или летнее.
ms.openlocfilehash: af9a2f7a94ae0cd736a4fe6f11b8a5a77673bbe3
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59515392"
---
# <a name="offset"></a>Offset

Элемент **Offset** описывает смещение из [BaseOffset.](baseoffset.md) Вместе с **элементом BaseOffset** элемент **Offset** определяет, является ли время стандартным или летнее. 
  
```xml
<Offset/>
```

 **duration**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Daylight](daylight.md) <br/> |Представляет дату и время, когда время меняется с летнего времени на обычное.  <br/> |
|[Standard](standard.md) <br/> |Представляет дату и время, когда время меняется с летнего времени на обычное.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение представляет смещение из согласованного универсального времени (UTC).
  
## <a name="remarks"></a>Заметки

Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

