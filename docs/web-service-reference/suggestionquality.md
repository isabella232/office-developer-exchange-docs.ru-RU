---
title: сугжестионкуалити
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
description: Элемент Сугжестионкуалити представляет качество предполагаемого времени проведения собрания.
ms.openlocfilehash: 3f8c15ccabd03687dc386a0328020cbc0bc802c4
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457979"
---
# <a name="suggestionquality"></a>сугжестионкуалити

Элемент **сугжестионкуалити** представляет качество предполагаемого времени проведения собрания. 
  
[жетусераваилабилитиреспонсе](getuseravailabilityresponse.md)
  
[сугжестионсреспонсе](suggestionsresponse.md)
  
[сугжестиондайресултаррай](suggestiondayresultarray.md)
  
[сугжестиондайресулт](suggestiondayresult.md)
  
[сугжестионаррай](suggestionarray.md)
  
[Предложение](suggestion.md)
  
[сугжестионкуалити](suggestionquality.md)
  
```xml
<SuggestionQuality>Excellent or Good or Fair or Poor</SuggestionQuality>
```

 **сугжестионкуалити**
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

Текстовое значение, представляющее значение **сугжестионкуалити** , является обязательным. Ниже перечислены возможные значения. 
  
- Для предложенного времени собраний доступно **отличное** 100 процентов пользователей и ресурсов. 
    
- **Хороший** Минимальный процент доступных пользователей и ресурсов равен или больше значения элемента [гудсрешолд](goodthreshold.md) плюс 50. 
    
- **Справедливо** Максимальный процент пользователей и ресурсов, доступных для предполагаемого времени проведения собрания, равен значению элемента [гудсрешолд](goodthreshold.md) плюс 50. Минимальное значение времени проведения собрания **Fair** составляет 50 процентов. 
    
- **Плохое качество** Для предполагаемого времени проведения собрания доступно менее 50 процентов пользователей и ресурсов. 
    
## <a name="remarks"></a>Примечания

Тип **сугжестионкуалити** также является типом для элементов [дайкуалити](dayquality.md) и [минимумсугжестионкуалити](minimumsuggestionquality.md) . 
  
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

