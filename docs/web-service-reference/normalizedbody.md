---
title: нормализедбоди
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: bfb813e4-642d-4f1b-9e91-1fee89dbd083
description: Элемент Нормализедбоди указывает HTML-представление свойства Body элемента в виде фрагмента, который можно вставить в другой HTML-текст.
ms.openlocfilehash: 07c2176d2c8a7473c06b7e42f8bcbbe6670581ef
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834548"
---
# <a name="normalizedbody"></a>нормализедбоди

Элемент **нормализедбоди** указывает HTML-представление свойства **Body** элемента в виде фрагмента, который можно вставить в другой HTML-текст. 
  
```XML
<NormalizedBody BodyType="Text | HTML" IsTruncated="true | false"></NormalizedBody>
```

 **BodyType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|BodyType  <br/> |Указывает тип тела. Значение **Text** для атрибута **BodyType** указывает на то, что текст отображается в виде обычного текста. Значение **HTML** для атрибута **BodyType** указывает на то, что текст находится в HTML-форме. Атрибут **BodyType** является обязательным.  <br/> |
|Усечено  <br/> |Указывает, что содержимое тела было усечено. Текстовое значение **false** для атрибута **Truncate** указывает на то, что содержимое основного текста не было усечено. Нормализованное тело будет усечено, если длина нормализованного текста превышает значение, заданное в элементе [максимумбодисизе](maximumbodysize.md) .  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

[Item](item.md) | [Сообщение](message-ex15websvcsotherref.md) | [MeetingResponse](meetingresponse.md) | [Contact](contact.md)[MeetingMessage](meetingmessage.md) | [MeetingCancellation](meetingcancellation.md)[MeetingRequest](meetingrequest.md) | [DistributionList](distributionlist.md) [Task](task.md)[PostItem](postitem.md)[CalendarItem](calendaritem.md)элемента митингмессаже | свойство meetingrequest митингреспонсе митингканцеллатион | Task | Item | календаритем Contact дистрибутионлист | 
  
## <a name="text-value"></a>Текстовое значение

Текстовое значение элемента **нормализедбоди** — это нормализованный текст элемента. 
  
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
   

