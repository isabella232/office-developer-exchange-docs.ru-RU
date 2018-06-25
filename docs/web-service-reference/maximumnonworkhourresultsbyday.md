---
title: MaximumNonWorkHourResultsByDay
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MaximumNonWorkHourResultsByDay
api_type:
- schema
ms.assetid: 9fb7314d-779c-4b1f-9d7c-b5cb092ed134
description: Элемент MaximumNonWorkHourResultsByDay указывает количество предложенного результатов время за пределами обычных рабочих часов в день собрания.
ms.openlocfilehash: f931dcaabda222e1579a0a4c0e0e6e49d88c6342
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834382"
---
# <a name="maximumnonworkhourresultsbyday"></a>MaximumNonWorkHourResultsByDay

Элемент **MaximumNonWorkHourResultsByDay** указывает количество предложенного результатов время за пределами обычных рабочих часов в день собрания. 
  
[GetUserAvailabilityRequest](getuseravailabilityrequest.md)
  
[SuggestionsViewOptions](suggestionsviewoptions.md)
  
[MaximumNonWorkHourResultsByDay](maximumnonworkhourresultsbyday.md)
  
```xml
<MaximumNonWorkHourResultsByDay>...</MaximumNonWorkHourResultsByDay>
```

 **int**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[SuggestionsViewOptions](suggestionsviewoptions.md) <br/> |Содержит параметры для получения сведения о предложения о собрании.  <br/> XPath для этого элемента:  <br/>  `/GetUserAvailabilityRequest/SuggestionViewOptions` <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение является обязательным. Текстовое значение представляет собой целое число.
  
## <a name="remarks"></a>Замечания

Этот элемент является обязательным, если используется элемент [SuggestionsViewOptions](suggestionsviewoptions.md) . 
  
> [!NOTE]
> Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа. 
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операция GetUserAvailability](getuseravailability-operation.md)


[Getting User Availability](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

