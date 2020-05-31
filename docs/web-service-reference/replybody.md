---
title: реплибоди
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ReplyBody
api_type:
- schema
ms.assetid: bb184144-3e4b-4419-a883-cc9fab1085e6
description: Элемент Реплибоди содержит сообщение об отсутствии на работе (отсутствие на работе) и язык, используемый для сообщения.
ms.openlocfilehash: 8400dda1ee810781e129fcc44fd3cd5d6c15cbbe
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835116"
---
# <a name="replybody"></a>реплибоди

Элемент **реплибоди** содержит сообщение об отсутствии на работе (отсутствие на работе) и язык, используемый для сообщения. 
  
```XML
<ReplyBody xml:lang="">
   <Message/>
</ReplyBody>
```

 **реплибоди**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|XML: lang  <br/> |Указывает язык, используемый в содержимом **реплибоди** . Этот атрибут является необязательным. Возможные значения этого атрибута определены в документе IETF RFC 3066.  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Сообщение (доступность)](message-availability.md) <br/> |Содержит ответ "нет на месте" (отсутствие на работе).  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[аутофоффице](outofoffice.md) <br/> |Определяет ответное сообщение об отсутствии на работе и продолжительность отправки ответного сообщения для почтового ящика.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Нет.
  
## <a name="remarks"></a>Примечания

Этот элемент обязательный.
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

