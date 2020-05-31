---
title: IsRecurring
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsRecurring
api_type:
- schema
ms.assetid: f4df6997-8d5b-4893-a4a5-fc7047e0a9c3
description: Элемент IsRecurring указывает, является ли элемент календаря, приглашение на собрание или задача частью повторяющегося элемента. Этот элемент доступен только для чтения.
ms.openlocfilehash: dfb0c28fe225792c7128409a8cf010627c624fe0
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834104"
---
# <a name="isrecurring"></a>IsRecurring

Элемент **IsRecurring** указывает, является ли элемент календаря, приглашение на собрание или задача частью повторяющегося элемента. Этот элемент доступен только для чтения. 
  
```xml
<IsRecurring/>
```

 **Boolean**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[календаритем](calendaritem.md) <br/> |Представляет элемент календаря Exchange.  <br/> |
|[Свойство meetingrequest](meetingrequest.md) <br/> |Представляет приглашение на собрание в хранилище Exchange.  <br/> |
|[Задача](task.md) <br/> |Представляет задачу в хранилище Exchange.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение, представляющее логическое значение является обязательным.
  
## <a name="remarks"></a>Примечания

В следующей таблице показано, как свойство **IsRecurring** задано для различных типов элементов календаря для организаторов и участников, а также для приглашений на собрания и обновлений. 
  
|**Тип Календаритем**|**Органайзер <br/> (IsRecurring)**|**Участник <br/> (IsRecurring)**|**Приглашение на собрание или <br/> обновление (IsRecurring)**|
|:-----|:-----|:-----|:-----|
|Один экземпляр  <br/> |**ЗНАЧЕНИЯ** <br/> |**ЗНАЧЕНИЯ** <br/> |**ЗНАЧЕНИЯ** <br/> |
|Повторяющаяся основная реплика  <br/> |**ЗНАЧЕНИЯ** <br/> |**ОТНОСИТСЯ** <br/> |**ОТНОСИТСЯ** <br/> |
|Повторяющееся исключение  <br/> |**ОТНОСИТСЯ** <br/> |**ОТНОСИТСЯ** <br/> |**ОТНОСИТСЯ** <br/> |
   
Значение свойства **IsRecurring** , заданное для повторяющихся элементов основного календаря для организатора, является неправильным; Это значение должно быть равно **true**. 
  
> [!NOTE]
> Операция GetUserAvailability также содержит элемент [IsRecurring (календаревентдетаилс)](isrecurring-calendareventdetails.md) . 
  
Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Тасктипе. IsRecurring](https://msdn.microsoft.com/library/ExchangeWebServices.TaskType.IsRecurring.aspx)
  
[Календаревентдетаилс. IsRecurring](https://msdn.microsoft.com/library/ExchangeWebServices.CalendarEventDetails.IsRecurring.aspx)
  
[Календаритемтипе. IsRecurring](https://msdn.microsoft.com/library/ExchangeWebServices.CalendarItemType.IsRecurring.aspx)
  
[Митингрекуестмессажетипе. IsRecurring](https://msdn.microsoft.com/library/ExchangeWebServices.MeetingRequestMessageType.IsRecurring.aspx)
  
[Календаритемтипе. ИсрекуррингспеЦифиед](https://msdn.microsoft.com/library/ExchangeWebServices.CalendarItemType.IsRecurringSpecified.aspx)
  
[Митингрекуестмессажетипе. ИсрекуррингспеЦифиед](https://msdn.microsoft.com/library/ExchangeWebServices.MeetingRequestMessageType.IsRecurringSpecified.aspx)
  
[Тасктипе. ИсрекуррингспеЦифиед](https://msdn.microsoft.com/library/ExchangeWebServices.TaskType.IsRecurringSpecified.aspx)


- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

