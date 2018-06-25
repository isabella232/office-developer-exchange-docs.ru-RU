---
title: SuggestionsViewOptions
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
description: Элемент SuggestionsViewOptions содержит параметры для получения сведения о предложения о собрании.
ms.openlocfilehash: 09ff317ae0b2ebf1eadc89dc3bb1cf5b3ae19dcb
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19840115"
---
# <a name="suggestionsviewoptions"></a>SuggestionsViewOptions

Элемент **SuggestionsViewOptions** содержит параметры для получения сведения о предложения о собрании. 
  
[GetUserAvailabilityRequest](getuseravailabilityrequest.md)
  
[SuggestionsViewOptions](suggestionsviewoptions.md)
  
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

 **SuggestionsViewOptionsType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[GoodThreshold](goodthreshold.md) <br/> |Указывает процент участников, которые необходимо открыть для периода времени, в рамках программы как хороший предложенного собрания период времени.  <br/> |
|[MaximumResultsByDay](maximumresultsbyday.md) <br/> |Указывает, сколько раз предложенного собрания в день, возвращаемого в ответе.  <br/> |
|[MaximumNonWorkHourResultsByDay](maximumnonworkhourresultsbyday.md) <br/> |Указывает количество предложенного результатов время за пределами обычных рабочих часов в день собрания.  <br/> |
|[MeetingDurationInMinutes](meetingdurationinminutes.md) <br/> |Определяет продолжительность собрания предлагаются.  <br/> |
|[MinimumSuggestionQuality](minimumsuggestionquality.md) <br/> |Определяет качество предложения о собрании должно быть возвращено в ответе.  <br/> |
|[DetailedSuggestionsWindow](detailedsuggestionswindow.md) <br/> |Определяет период времени, который будет опрошен на наличие подробные сведения о времени предложенного собрания.  <br/> |
|[CurrentMeetingTime](currentmeetingtime.md) <br/> |Представляет время начала собрания, который нужно обновить с предложенного собрания время результаты.  <br/> |
|[GlobalObjectId](globalobjectid.md) <br/> |Этот элемент не используется.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[GetUserAvailabilityRequest](getuseravailabilityrequest.md) <br/> |Содержит аргументы, используемые для получения сведений о доступности пользователя. Это корневой элемент.  <br/> XPath для этого элемента:  <br/>  `/GetUserAvailabilityRequest` <br/> |
   
## <a name="remarks"></a>Замечания

Этот элемент не является обязательным и можно только один раз при использовании. Это значение может быть null, если значение элемента [FreeBusyViewOptions](freebusyviewoptions.md) не равно null. 
  
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

