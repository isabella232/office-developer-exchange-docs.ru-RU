---
title: Timeout (продолжительность)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: bb15f9a7-8ea5-4765-9877-762c3f98bf50
description: Элемент Timeout указывает продолжительность времени, прежде чем на сервере будет приумножаться подписка на тягу.
ms.openlocfilehash: a5a9e094c25f609c0bcfa207ab96ae7f0877f43f
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59545771"
---
# <a name="timeout-duration"></a>Timeout (продолжительность)

Элемент **Timeout** указывает продолжительность времени, прежде чем на сервере будет приумножаться подписка на тягу. 
  
```XML
<Timeout></Timeout>
```

 **SubscriptionTimeoutType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

[PullSubscriptionRequest](pullsubscriptionrequest.md)
  
## <a name="text-value"></a>Текстовое значение

Текстовое значение элемента **Timeout** — это время, за несколько минут до того, как сервер приумносит подписку на тягу. Минимальное значение — 1; максимальное значение — 1440. 
  
## <a name="remarks"></a>Заметки

Этот элемент появился в Exchange Server 2013.
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> ||
   

