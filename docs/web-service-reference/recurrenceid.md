---
title: рекурренцеид
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RecurrenceId
api_type:
- schema
ms.assetid: 9ef3569d-ee56-4b22-b008-609fb3337da7
description: Элемент Рекурренцеид используется для определения конкретного экземпляра повторяющегося элемента календаря.
ms.openlocfilehash: 58a379f2cffa7ff37181e93ad1c45c9752e84f1d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461613"
---
# <a name="recurrenceid"></a>рекурренцеид

Элемент **рекурренцеид** используется для определения конкретного экземпляра повторяющегося элемента календаря. 
  
```xml
<RecurrenceId/>
```

 **дата и время**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

Отсутствуют.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[календаритем](calendaritem.md) <br/> |Представляет элемент календаря Exchange.  <br/> |
|[митингмессаже](meetingmessage.md) <br/> |Представляет сообщение о собрании.  <br/> |
|[Свойство meetingrequest](meetingrequest.md) <br/> |Представляет приглашение на собрание.  <br/> |
|[митингреспонсе](meetingresponse.md) <br/> |Представляет ответ на приглашение на собрание.  <br/> |
|[митингканцеллатион](meetingcancellation.md) <br/> |Представляет отмену собрания.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение представляет значение даты и времени, идентифицирующее вхождение календаря.
  
## <a name="remarks"></a>Примечания

Это свойство используется со свойством [UID](uid.md) для идентификации определенного экземпляра повторяющегося элемента календаря. 
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

