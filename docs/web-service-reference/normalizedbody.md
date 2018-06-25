---
title: NormalizedBody
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: bfb813e4-642d-4f1b-9e91-1fee89dbd083
description: Элемент NormalizedBody указывает представлением HTML свойства тела элемента как фрагмент, который можно вставить в другой HTML-текста.
ms.openlocfilehash: 07c2176d2c8a7473c06b7e42f8bcbbe6670581ef
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834548"
---
# <a name="normalizedbody"></a>NormalizedBody

Элемент **NormalizedBody** указывает представлением HTML свойства **тела** элемента как фрагмент, который можно вставить в другой HTML-текста. 
  
```XML
<NormalizedBody BodyType="Text | HTML" IsTruncated="true | false"></NormalizedBody>
```

 **BodyType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|BodyType  <br/> |Указывает тип основного текста. Значение **текста** в атрибуте **BodyType** указывает текст в виде обычного текста. Значение **HTML-код** для атрибута **типа текста сообщения** указывает текст в формате HTML. Атрибут **типа текста сообщения** является обязательным.  <br/> |
|IsTruncated  <br/> |Указывает, что содержимое текста быть усечен. Текстовое значение **false** для атрибута **IsTruncated** указывает, что содержимое текста не были сокращены. Нормализованный body усекаются, если длина нормализованный body больше, чем значение, установленное в элементе [MaximumBodySize](maximumbodysize.md) .  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

[Элемент](item.md) | [сообщение](message-ex15websvcsotherref.md) | [MeetingMessage](meetingmessage.md) | [MeetingRequest](meetingrequest.md) | [MeetingResponse](meetingresponse.md) | [MeetingCancellation](meetingcancellation.md) | [задачи](task.md) | [PostItem ](postitem.md)  |  [Элемента календаря, имеющего](calendaritem.md) | [контакт](contact.md) | [DistributionList](distributionlist.md)
  
## <a name="text-value"></a>Текстовое значение

Текстовое значение элемента **NormalizedBody** является нормализованный тело элемента. 
  
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
   

