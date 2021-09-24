---
title: TextBody
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: bd0c0bce-3e7c-47c7-af7f-5ee5f5ad9820
description: Элемент TextBody указывает текстовое тело.
ms.openlocfilehash: 5dfc0aa76f0b0778d785e46fe12259c4a226b89f
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59515182"
---
# <a name="textbody"></a>TextBody

Элемент **TextBody** указывает текстовое тело. 
  
```XML
<TextBody BodyTypeType=" HTML | Text" IsTruncated=" true | false"></TextBody>
```

 **BodyType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|BodyTypeType  <br/> |Указывает тип тела. Значение текста **для** **атрибута BodyTypeType** указывает на то, что тело находится в обычной текстовой форме. Значение **HTML для** **атрибута BodyTypeType** указывает на то, что тело находится в HTML-форме. Атрибут **BodyTypeType** необходим.  <br/> |
|IsTruncated  <br/> |Указывает, что содержимое тела было усечено. Текстовое значение **false для** **атрибута IsTruncated** указывает на то, что содержимое тела не было усечено. Нормализуемое тело будет усечено, если длина текстового тела больше значения, задатого в [элементе MaximumBodySize.](maximumbodysize.md)  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

[Item](item.md)  |  [Контакт](contact.md)  |  [Сообщение](message-ex15websvcsotherref.md)  |  [DistributionList](distributionlist.md)  |  [CalendarItem](calendaritem.md)  |  [PostItem](postitem.md)  |  [Задача](task.md)
  
## <a name="text-value"></a>Текстовое значение

Текстовое значение элемента **TextBody** — текстовое тело элемента. 
  
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
   

