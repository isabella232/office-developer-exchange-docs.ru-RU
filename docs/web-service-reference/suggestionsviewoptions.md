---
title: сугжестионсвиевоптионс
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SuggestionsViewOptions
api_type:
- schema
ms.assetid: bb04ae38-e62d-4a69-a479-8ff326ca726e
description: Элемент Сугжестионсвиевоптионс содержит параметры для получения сведений о предложении о собрании.
ms.openlocfilehash: 09ff317ae0b2ebf1eadc89dc3bb1cf5b3ae19dcb
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19840115"
---
# <a name="suggestionsviewoptions"></a>сугжестионсвиевоптионс

Элемент **сугжестионсвиевоптионс** содержит параметры для получения сведений о предложении о собрании. 
  
[жетусераваилабилитирекуест](getuseravailabilityrequest.md)
  
[сугжестионсвиевоптионс](suggestionsviewoptions.md)
  
```xml
<SuggestionsViewOptions>
   <GoodThreshold>...</GoodThreshold>
   <MaximumResultsByDay>...</MaximumResultsByDay>
   <MaximumNonWorkingHourResultsByDay>...</MaximumNonWorkingHourResultsByDay>
   <MeetingDurationInMinutes>...</MeetingDurationInMinutes>
   <MinimumSuggestionQuality>...</MinimumSuggestionQuality>
   <SuggestionIntervalInMinutes>...</SuggestionIntervalInMinutes>
   <DetailedSuggestionsWindow>...</DetailedSuggestionsWindow>
   <CurrentMeetingTime>...</CurrentMeetingTime>
   <GlobalObjectId>...</GlobalObjectId>
</SuggestionsViewOptions>
```

 **сугжестионсвиевоптионстипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[гудсрешолд](goodthreshold.md) <br/> |Указывает процент участников, которые должны иметь период времени, который должен быть указан в качестве приемлемого времени проведения собрания.  <br/> |
|[максимумресултсбидай](maximumresultsbyday.md) <br/> |Указывает количество предложенных собраний в день, возвращаемых в ответе.  <br/> |
|[максимумнонворкхаурресултсбидай](maximumnonworkhourresultsbyday.md) <br/> |Указывает количество предполагаемых результатов для времени проведения собрания, не входящих в число обычных рабочих часов в день.  <br/> |
|[митингдуратионинминутес](meetingdurationinminutes.md) <br/> |Указывает предполагаемую длину собрания.  <br/> |
|[минимумсугжестионкуалити](minimumsuggestionquality.md) <br/> |Указывает качество предложений собраний, возвращаемых в ответе.  <br/> |
|[детаиледсугжестионсвиндов](detailedsuggestionswindow.md) <br/> |Определяет интервал времени, на который запрашивается подробная информация о предложенном времени проведения собрания.  <br/> |
|[куррентмитингтиме](currentmeetingtime.md) <br/> |Представляет время начала собрания, которое вы хотите обновить с учетом предложенного времени проведения собрания.  <br/> |
|[глобалобжектид](globalobjectid.md) <br/> |Этот элемент не используется.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[жетусераваилабилитирекуест](getuseravailabilityrequest.md) <br/> |Содержит аргументы, используемые для получения сведений о доступности пользователя. Это корневой элемент.  <br/> XPath для этого элемента:  <br/>  `/GetUserAvailabilityRequest` <br/> |
   
## <a name="remarks"></a>Примечания

Этот элемент не является обязательным и может быть использован только один раз. Это значение может быть равно null, если значение элемента [фрибусивиевоптионс](freebusyviewoptions.md) отлично от NULL. 
  
> [!NOTE]
> Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа. 
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операция GetUserAvailability](getuseravailability-operation.md)


[Getting User Availability](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

