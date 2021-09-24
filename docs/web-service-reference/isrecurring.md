---
title: IsRecurring
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- IsRecurring
api_type:
- schema
ms.assetid: f4df6997-8d5b-4893-a4a5-fc7047e0a9c3
description: Элемент IsRecurring указывает, является ли элемент календаря, запрос собрания или задача частью повторяющегося элемента. Этот элемент доступен только для чтения.
ms.openlocfilehash: ea910b78e962906285a73c869e394147c324372c
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59532728"
---
# <a name="isrecurring"></a>IsRecurring

Элемент **IsRecurring указывает,** является ли элемент календаря, запрос собрания или задача частью повторяющегося элемента. Этот элемент доступен только для чтения. 
  
```xml
<IsRecurring/>
```

 **Boolean**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[CalendarItem](calendaritem.md) <br/> |Представляет элемент календаря Exchange.  <br/> |
|[MeetingRequest](meetingrequest.md) <br/> |Представляет приглашение на собрание в хранилище Exchange.  <br/> |
|[Задача](task.md) <br/> |Представляет задачу в хранилище Exchange.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение, представляющее логическое значение является обязательным.
  
## <a name="remarks"></a>Заметки

В следующей таблице показано, как заказано свойство **IsRecurring** для различных типов элементов календаря для организаторов и участников, а также для запросов и обновлений собраний. 
  
|**Тип CalendarItem**|**Организатор  <br/> (IsRecurring)**|**Участник  <br/> (IsRecurring)**|**Запрос на собрание/обновление  <br/> (IsRecurring)**|
|:-----|:-----|:-----|:-----|
|Единое возникновение  <br/> |**FALSE** <br/> |**FALSE** <br/> |**FALSE** <br/> |
|Повторяющийся мастер  <br/> |**FALSE** <br/> |**TRUE** <br/> |**TRUE** <br/> |
|Повторяющееся исключение  <br/> |**TRUE** <br/> |**TRUE** <br/> |**TRUE** <br/> |
   
Значение **свойства IsRecurring,** за набором для повторяющихся элементов календаря для организатора, неверно; это значение должно быть заданной значение **TRUE**. 
  
> [!NOTE]
> Операция GetUserAvailability также имеет элемент [IsRecurring (CalendarEventDetails).](isrecurring-calendareventdetails.md) 
  
Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[TaskType.IsRecurring](https://msdn.microsoft.com/library/ExchangeWebServices.TaskType.IsRecurring.aspx)
  
[CalendarEventDetails.IsRecurring](https://msdn.microsoft.com/library/ExchangeWebServices.CalendarEventDetails.IsRecurring.aspx)
  
[CalendarItemType.IsRecurring](https://msdn.microsoft.com/library/ExchangeWebServices.CalendarItemType.IsRecurring.aspx)
  
[MeetingRequestMessageType.IsRecurring](https://msdn.microsoft.com/library/ExchangeWebServices.MeetingRequestMessageType.IsRecurring.aspx)
  
[CalendarItemType.IsRecurringSpecified](https://msdn.microsoft.com/library/ExchangeWebServices.CalendarItemType.IsRecurringSpecified.aspx)
  
[MeetingRequestMessageType.IsRecurringSpecified](https://msdn.microsoft.com/library/ExchangeWebServices.MeetingRequestMessageType.IsRecurringSpecified.aspx)
  
[TaskType.IsRecurringSpecified](https://msdn.microsoft.com/library/ExchangeWebServices.TaskType.IsRecurringSpecified.aspx)


- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

