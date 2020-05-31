---
title: Тип
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 488ee828-343f-4382-a5e8-eed1005f5dbc
description: Элемент ResultType содержит тип выполняемого поиска. Тип поиска может иметь только статистику или только предварительный просмотр.
ms.openlocfilehash: 750f53ae05a7ad9f5aefc9396911a23ef32cdfc2
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835211"
---
# <a name="resulttype"></a>Тип

Элемент **resultType** содержит тип выполняемого поиска. Тип поиска может иметь только статистику или только предварительный просмотр. 
  
```XML
<ResultType>StatisticsOnly | PreviewOnly</ResultType>
```

 **сеарчресулттипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

[Сеарчмаилбоксесресулт](searchmailboxesresult.md) | [SearchMailboxes](searchmailboxes.md)
  
## <a name="text-value"></a>Текстовое значение

Текстовое значение элемента **resultType** — это тип результата, возвращаемого для поиска при обнаружении. Текстовое значение **статистиксонли** будет возвращать статистику поиска. Текстовое значение **превиевонли** будет возвращать сведения о предварительном просмотре элемента. 
  
## <a name="remarks"></a>Примечания

Этот элемент появился в Exchange Server 2013.
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages. xsd  <br/> |
|Может быть пустым  <br/> |false  <br/> |
   

