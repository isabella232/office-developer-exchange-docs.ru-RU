---
title: текстбоди
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: bd0c0bce-3e7c-47c7-af7f-5ee5f5ad9820
description: Элемент Текстбоди указывает текст текста.
ms.openlocfilehash: 78b18b27891d571605d2eeeeffb5c252cc790c11
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19840152"
---
# <a name="textbody"></a>текстбоди

Элемент **текстбоди** указывает текст текста. 
  
```XML
<TextBody BodyTypeType=" HTML | Text" IsTruncated=" true | false"></TextBody>
```

 **BodyType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|бодитипетипе  <br/> |Указывает тип тела. Значение **Text** для атрибута **бодитипетипе** указывает на то, что текст отображается в виде обычного текста. Значение **HTML** для атрибута **бодитипетипе** указывает на то, что текст находится в HTML-форме. Атрибут **бодитипетипе** является обязательным.  <br/> |
|Усечено  <br/> |Указывает, что содержимое тела было усечено. Текстовое значение **false** для атрибута **Truncate** указывает на то, что содержимое основного текста не было усечено. Нормализованный текст будет усечен, если длина текста текста превышает значение, заданное в элементе [максимумбодисизе](maximumbodysize.md) .  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

[Item](item.md) |  | [Сообщение](message-ex15websvcsotherref.md) | [PostItem](postitem.md) | [Task](task.md) [DistributionList](distributionlist.md) | [CalendarItem](calendaritem.md)[Contact](contact.md)с контактами для элемента дистрибутионлист календаритем i i Item Task | 
  
## <a name="text-value"></a>Текстовое значение

Текстовое значение элемента **текстбоди** — основной текст элемента. 
  
## <a name="remarks"></a>Примечания

Этот элемент появился в Exchange Server 2013.
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> ||
   

