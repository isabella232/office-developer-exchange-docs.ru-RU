---
title: NormalizedBody
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: bfb813e4-642d-4f1b-9e91-1fee89dbd083
description: Элемент NormalizedBody указывает HTML-представление свойства body элемента как фрагмента, который можно вставить в другое HTML-тело.
ms.openlocfilehash: 9ce7a745cfbe2e08afbe4c83873cb670b6afa571
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59515434"
---
# <a name="normalizedbody"></a>NormalizedBody

Элемент **NormalizedBody** указывает HTML-представление свойства **body** элемента как фрагмента, который можно вставить в другое HTML-тело. 
  
```XML
<NormalizedBody BodyType="Text | HTML" IsTruncated="true | false"></NormalizedBody>
```

 **BodyType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|BodyType  <br/> |Указывает тип тела. Значение текста **для** **атрибута BodyType** указывает на то, что тело находится в обычной текстовой форме. Значение **HTML для** **атрибута BodyType** указывает на то, что тело находится в HTML-форме. Атрибут **BodyType** необходим.  <br/> |
|IsTruncated  <br/> |Указывает, что содержимое тела было усечено. Текстовое значение **false для** **атрибута IsTruncated** указывает на то, что содержимое тела не было усечено. Нормализуемое тело будет усечено, если нормализуемая длина тела больше значения, задатого в [элементе MaximumBodySize.](maximumbodysize.md)  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

[Item](item.md)  |  [Сообщение](message-ex15websvcsotherref.md)  |  [MeetingMessage](meetingmessage.md)  |  [MeetingRequest](meetingrequest.md)  |  [MeetingResponse](meetingresponse.md)  |  [MeetingCancellation](meetingcancellation.md)  |  [Задача](task.md)  |  [PostItem](postitem.md)  |  [CalendarItem](calendaritem.md)  |  [Контакт](contact.md)  |  [DistributionList](distributionlist.md)
  
## <a name="text-value"></a>Текстовое значение

Текстовое значение элемента **NormalizedBody** — это нормализуемое тело элемента. 
  
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
   

