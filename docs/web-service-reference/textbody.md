---
title: TextBody
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: bd0c0bce-3e7c-47c7-af7f-5ee5f5ad9820
description: Элемент TextBody указывает body текст.
ms.openlocfilehash: 78b18b27891d571605d2eeeeffb5c252cc790c11
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19840152"
---
# <a name="textbody"></a>TextBody

Элемент **TextBody** указывает body текст. 
  
```XML
<TextBody BodyTypeType=" HTML | Text" IsTruncated=" true | false"></TextBody>
```

 **BodyType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|BodyTypeType  <br/> |Указывает тип основного текста. Значение **текста** в атрибуте **BodyTypeType** указывает текст в виде обычного текста. Значение **HTML-код** для атрибута **BodyTypeType** указывает текст в формате HTML. Атрибут **BodyTypeType** является обязательным.  <br/> |
|IsTruncated  <br/> |Указывает, что содержимое текста быть усечен. Текстовое значение **false** для атрибута **IsTruncated** указывает, что содержимое текста не были сокращены. Нормализованный body усекаются, если длина body текст больше, чем значение, установленное в элементе [MaximumBodySize](maximumbodysize.md) .  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

[Элемент](item.md) | [контакт](contact.md) | [сообщение](message-ex15websvcsotherref.md) | [DistributionList](distributionlist.md) | [элемента календаря, имеющего](calendaritem.md) | [PostItem](postitem.md) | [задач](task.md)
  
## <a name="text-value"></a>Текстовое значение

Текстовое значение элемента **TextBody** является текста элемента. 
  
## <a name="remarks"></a>Замечания

Этот элемент появился в Exchange Server 2013.
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> ||
   

