---
title: процессригхтавай
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ProcessRightAway
api_type:
- schema
ms.assetid: f6bba68b-ae4f-41c1-b3e7-c8a31cdb1b0c
description: Элемент Процессригхтавай указывает, отправляется ли ответ сразу после того, как действие начнет обработку на сервере или отправило ли ответ после завершения действия. Этот элемент должен присутствовать, чтобы ответ был асинхронно отправлен в запрошенное действие.
ms.openlocfilehash: 58d2b926c48db5e7395df64e1f8ee9d6a8f0e73c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44434073"
---
# <a name="processrightaway"></a>процессригхтавай

Элемент **процессригхтавай** указывает, отправляется ли ответ сразу после того, как действие начнет обработку на сервере или отправило ли ответ после завершения действия. Этот элемент должен присутствовать, чтобы ответ был асинхронно отправлен в запрошенное действие. 
  
[ApplyConversationAction](applyconversationaction.md)
  
[конверсатионактионс](conversationactions.md)
  
[конверсатионактион](conversationaction.md)
  
[процессригхтавай](processrightaway.md)
  
```XML
<ProcessRightAway/>
```

 **xs: Boolean**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

Отсутствуют.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[конверсатионактион](conversationaction.md) <br/> |Содержит одно действие, которое будет применено к одной беседе.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение **true** указывает на то, что ответ отправляется сразу после того, как действие начнет обработку на сервере. Текстовое значение **false** указывает, что ответ отправляется после выполнения действия. 
  
## <a name="remarks"></a>Примечания

Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.Этот элемент появился в Exchange Server 2010 с пакетом обновления 1 (SP1).
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операция ApplyConversationAction](applyconversationaction-operation.md)


- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

