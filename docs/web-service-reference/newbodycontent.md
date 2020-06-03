---
title: невбодиконтент
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
description: Элемент Невбодиконтент представляет новое содержимое основного текста сообщения.
ms.openlocfilehash: dcfa927bb284ff00e510d8c7b4b31910a70b3cbb
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44466859"
---
# <a name="newbodycontent"></a>невбодиконтент

Элемент **невбодиконтент** представляет новое содержимое основного текста сообщения. 
  
```xml
<NewBodyContent BodyType=""/>
```

 **BodyType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|**BodyType** <br/> |Представляет реальное содержимое основного текста сообщения.  <br/> |
   
#### <a name="bodytype-attribute"></a>Атрибут BodyType

|**Значение**|**Описание**|
|:-----|:-----|
|**HTML** <br/> |Преобразует все тексты в HTML.  <br/> |
|**Text** <br/> |Преобразует все тексты в обычный текст.  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

Отсутствуют.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[реплитоитем](replytoitem.md) <br/> |Содержит ответ отправителю элемента в хранилище Exchange.  <br/> |
|[репляллтоитем](replyalltoitem.md) <br/> |Содержит ответ на отправителя и всех идентифицированных получателей элемента в хранилище Exchange.  <br/> |
|[форвардитем](forwarditem.md) <br/> |Содержит элемент хранилища Exchange переадресация получателям.  <br/> |
|[канцелкалендаритем](cancelcalendaritem.md) <br/> |Представляет объект ответа, которая используется для отмены собрания.  <br/> |
|[постреплитем](postreplyitem.md) <br/> |Содержит ответ на элемент POST. Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение представляет новое содержимое основного текста сообщения.
  
## <a name="remarks"></a>Примечания

Схема, описывающая этот элемент, находится в виртуальном каталоге EWS сервера Exchange, на котором установлена роль сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

