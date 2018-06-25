---
title: SuggestionQuality
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SuggestionQuality
api_type:
- schema
ms.assetid: 734f1a58-adda-4830-973e-e84bf7b870d5
description: Элемент SuggestionQuality представляет качества предложенного собрания.
ms.openlocfilehash: e67e0149226b36c22cdd00acd78f6582f826dd3e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19840112"
---
# <a name="suggestionquality"></a>SuggestionQuality

Элемент **SuggestionQuality** представляет качества предложенного собрания. 
  
[GetUserAvailabilityResponse](getuseravailabilityresponse.md)
  
[SuggestionsResponse](suggestionsresponse.md)
  
[SuggestionDayResultArray](suggestiondayresultarray.md)
  
[SuggestionDayResult](suggestiondayresult.md)
  
[SuggestionArray](suggestionarray.md)
  
[Предложения](suggestion.md)
  
[SuggestionQuality](suggestionquality.md)
  
```xml
<SuggestionQuality>Excellent or Good or Fair or Poor</SuggestionQuality>
```

 **SuggestionQuality**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Предложения](suggestion.md) <br/> |Представляет один предложения о времени на собрания.  <br/> Ниже приведен выражение XPath для этого элемента.  <br/>  `/GetUserAvailabilityResponse/SuggestionsResponse/SuggestionDayResultArray/SuggestionDayResult[i]/SuggestionArray/Suggestion[i]` <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение, представляющее значение **SuggestionQuality** является обязательным. Ниже перечислены возможные значения. 
  
- **Отличное** 100 процентов пользователей и ресурсов, доступных для предложенного собрания. 
    
- **Хороший** Минимальный процент пользователей и ресурсы, доступные равно или больше, чем значение элемента [GoodThreshold](goodthreshold.md) плюс 50. 
    
- **Обычное** Максимальный процент пользователей и ресурсы, доступные для предложенного собрания равно значение элемента [GoodThreshold](goodthreshold.md) плюс 50. Минимальное значение для **Обычное** время собрания качества — 50 процентов. 
    
- **Низкий** Меньше 50% пользователей и ресурсов, доступных для предложенного собрания. 
    
## <a name="remarks"></a>Замечания

Тип **SuggestionQuality** также является типом для [DayQuality](dayquality.md) и [MinimumSuggestionQuality](minimumsuggestionquality.md) элементов. 
  
Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операция GetUserAvailability](getuseravailability-operation.md)
  
[GetUserAvailabilityResponse](getuseravailabilityresponse.md)


[Getting User Availability](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

