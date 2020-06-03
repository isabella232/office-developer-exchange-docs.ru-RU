---
title: конверсатионластсинктиме
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ConversationLastSyncTime
api_type:
- schema
ms.assetid: 90f8f9e3-5fc6-4a6a-bdfb-fc91fa51f8a2
description: Элемент Конверсатионластсинктиме содержит дату и время последней синхронизации беседы. Этот элемент должен присутствовать при попытке удалить все элементы в беседе, полученные до указанного времени.
ms.openlocfilehash: f7cc6e205ab9936685d7b8c1f34129b799a53021
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461431"
---
# <a name="conversationlastsynctime"></a>конверсатионластсинктиме

Элемент **конверсатионластсинктиме** содержит дату и время последней синхронизации беседы. Этот элемент должен присутствовать при попытке удалить все элементы в беседе, полученные до указанного времени. 
  
[ApplyConversationAction](applyconversationaction.md)
  
[конверсатионактионс](conversationactions.md)
  
[конверсатионактион](conversationaction.md)
  
[конверсатионластсинктиме](conversationlastsynctime.md)
  
```XML
<ConversationLastSyncTime/>
```

 **xs: dateTime**
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

Текстовое значение **конверсатионластсинктиме** указывает время последней синхронизации диалога. 
  
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

