---
title: митингтиме
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MeetingTime
api_type:
- schema
ms.assetid: 6e6d2d8b-e8a2-43e6-a715-0fc7d6dd44b9
description: Элемент Митингтиме представляет предполагаемое время проведения собрания.
ms.openlocfilehash: 3a7031e70eb8b22adc8030c1cec09d33399332ee
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530452"
---
# <a name="meetingtime"></a>митингтиме

Элемент **митингтиме** представляет предполагаемое время проведения собрания. 
  
[жетусераваилабилитиреспонсе](getuseravailabilityresponse.md)
  
[сугжестионсреспонсе](suggestionsresponse.md)
  
[сугжестиондайресултаррай](suggestiondayresultarray.md)
  
[сугжестиондайресулт](suggestiondayresult.md)
  
[сугжестионаррай](suggestionarray.md)
  
[Предложение](suggestion.md)
  
[митингтиме](meetingtime.md)
  
```xml
<MeetingTime>...</MeetingTime
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
|[Предложение](suggestion.md) <br/> |Представляет один вариант времени собрания.  <br/> Ниже приведено выражение XPath для этого элемента:  <br/>  `/GetUserAvailabilityResponse/SuggestionsResponse/SuggestionDayResultArray/SuggestionDayResult[i]/SuggestionArray/Suggestion[i]` <br/> |
   
## <a name="text-value"></a>Текстовое значение

Необходимо указать текстовое значение, представляющее значение **DateTime** . 
  
## <a name="remarks"></a>Примечания

Элемент [митингтиме](meetingtime.md) является обязательным дочерним элементом элемента [предложения](suggestion.md) . 
  
Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операция GetUserAvailability](getuseravailability-operation.md)
  
[жетусераваилабилитиреспонсе](getuseravailabilityresponse.md)


[Getting User Availability](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

