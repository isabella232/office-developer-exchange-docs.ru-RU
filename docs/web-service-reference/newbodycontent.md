---
title: NewBodyContent
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- NewBodyContent
api_type:
- schema
ms.assetid: 0303600d-16d8-4685-88f2-980c5ca7e9a6
description: Элемент NewBodyContent представляет новое содержимое тела сообщения.
ms.openlocfilehash: 48f6a12e0492249d239196ca3be19857e34e0099
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59509519"
---
# <a name="newbodycontent"></a>NewBodyContent

Элемент **NewBodyContent** представляет новое содержимое тела сообщения. 
  
```xml
<NewBodyContent BodyType=""/>
```

 **BodyType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|**BodyType** <br/> |Представляет фактическое содержимое тела сообщения.  <br/> |
   
#### <a name="bodytype-attribute"></a>Атрибут BodyType

|**Значение**|**Описание**|
|:-----|:-----|
|**HTML** <br/> |Преобразует все органы в HTML.  <br/> |
|**Text** <br/> |Преобразует все органы в обычный текст.  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[ReplyToItem](replytoitem.md) <br/> |Содержит ответ отправительу элемента в Exchange магазине.  <br/> |
|[ReplyAllToItem](replyalltoitem.md) <br/> |Содержит ответ отправительу и всем идентифицированным получателям элемента в Exchange магазине.  <br/> |
|[ForwardItem](forwarditem.md) <br/> |Содержит элемент хранилища Exchange переадресация получателям.  <br/> |
|[CancelCalendarItem](cancelcalendaritem.md) <br/> |Представляет объект ответа, которая используется для отмены собрания.  <br/> |
|[PostReplyItem](postreplyitem.md) <br/> |Содержит ответ на сообщение элемента. Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение представляет новое содержимое текста сообщения.
  
## <a name="remarks"></a>Заметки

Схема, описываемая этим элементом, расположена в виртуальном каталоге EWS сервера Exchange, на который установлена роль сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

