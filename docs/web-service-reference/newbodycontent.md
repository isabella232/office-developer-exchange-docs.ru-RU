---
title: NewBodyContent
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- NewBodyContent
api_type:
- schema
ms.assetid: 0303600d-16d8-4685-88f2-980c5ca7e9a6
description: Элемент NewBodyContent представляет новое содержимое текста сообщения.
ms.openlocfilehash: b87393e460b1eee1c13efebf38e898d17915bd71
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834516"
---
# <a name="newbodycontent"></a>NewBodyContent

Элемент **NewBodyContent** представляет новое содержимое текста сообщения. 
  
```xml
<NewBodyContent BodyType=""/>
```

 **BodyType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|**BodyType** <br/> |Представляет фактическое содержимое основного текста сообщения.  <br/> |
   
#### <a name="bodytype-attribute"></a>Атрибут типа текста сообщения

|**Значение**|**Описание**|
|:-----|:-----|
|**HTML-КОД** <br/> |Преобразует все тексты в HTML-код.  <br/> |
|**Text** <br/> |Преобразует все тексты в обычный текст.  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[ReplyToItem](replytoitem.md) <br/> |Содержит ответ отправителя элемента в хранилище Exchange.  <br/> |
|[ReplyAllToItem](replyalltoitem.md) <br/> |Содержит ответ для отправителя и всех указанных получателей элемента в хранилище Exchange.  <br/> |
|[ForwardItem](forwarditem.md) <br/> |Содержит элемент хранилища Exchange переадресация получателям.  <br/> |
|[CancelCalendarItem](cancelcalendaritem.md) <br/> |Представляет объект ответа, которая используется для отмены собрания.  <br/> |
|[PostReplyItem](postreplyitem.md) <br/> |Содержит ответ элемента записи. Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение представляет новое содержимое текста сообщения.
  
## <a name="remarks"></a>Замечания

Схема, описывающая этот элемент находится в виртуальном каталоге EWS сервера Exchange Server с установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

