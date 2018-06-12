---
title: Body
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 7851ea9b-9f87-4adc-a26f-7a27df4a9bca
description: Элемент Body указывает тела элемента.
ms.openlocfilehash: a4803c0e5ac3b027396983a5524241590eac35f6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761583"
---
# <a name="body"></a>Body

Элемент **Body** указывает тела элемента. 
  
```XML
<Body> BodyType="" IsTruncated="" </Body>
```

 **BodyType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|BodyType  <br/> |Указывает тип текста.  <br/> |
|IsTruncated  <br/> |Логическое значение, указывающее, является ли текст усекается.  <br/> |
   
#### <a name="bodytype"></a>BodyType

|**Значение**|**Описание**|
|:-----|:-----|
|HTML  <br/> |Указывает, что текст в формате HTML.  <br/> |
|Text  <br/> |Указывает, что текст в текст.  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Элемента календаря, имеющего](calendaritem.md) <br/> |Представляет элемент календаря Exchange.  <br/> |
|[Контакт](contact.md) <br/> |Представляет контакт в хранилище Exchange.  <br/> |
|[DistributionList](distributionlist.md) <br/> |Представляет список рассылки.  <br/> |
|[Элемент](item.md) <br/> |Представляет универсальный элемент в хранилище Exchange.  <br/> |
|[Message](message-ex15websvcsotherref.md) <br/> |Представляет сообщение электронной почты Microsoft Exchange.  <br/> |
|[PostItem](postitem.md) <br/> |Представляет элемент post в хранилище Exchange.  <br/> |
|[Задача](task.md) <br/> |Представляет задачу в хранилище Exchange.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение элемента **Body** является тела элемента. 
  
## <a name="remarks"></a>Замечания

Этот элемент появился в Exchange Server 2013.
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема типа  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> ||
   
## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

