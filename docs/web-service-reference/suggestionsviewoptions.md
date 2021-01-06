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
description: Элемент SuggestionsViewOptions содержит параметры для получения сведений о предложении собрания.
ms.openlocfilehash: f584b19997f98760bd4e438dcd48a5c18cc63e4b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44433996"
---
# <a name="suggestionsviewoptions"></a>SuggestionsViewOptions

Элемент **SuggestionsViewOptions** содержит параметры для получения сведений о предложении собрания. 
  
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
|[GoodThreshold](goodthreshold.md) <br/> |Указывает процент участников, которые должны иметь период времени, открытый для периода времени, чтобы квалифицироваться как рекомендуемый период собрания.  <br/> |
|[MaximumResultsByDay](maximumresultsbyday.md) <br/> |Указывает число рекомендуемого времени собрания в день, возвращаемого в ответе.  <br/> |
|[MaximumNonWorkHourResultsByDay](maximumnonworkhourresultsbyday.md) <br/> |Указывает количество предлагаемых результатов для времени собрания вне обычного рабочего времени в день.  <br/> |
|[MeetingDurationInMinutes](meetingdurationinminutes.md) <br/> |Указывает длительность предложенного собрания.  <br/> |
|[MinimumSuggestionQuality](minimumsuggestionquality.md) <br/> |Указывает качество предложений собрания, возвращаемого в ответе.  <br/> |
|[DetailedSuggestionsWindow](detailedsuggestionswindow.md) <br/> |Определяет промежуток времени, в течение который запрашивается подробная информация о рекомендуемом времени собрания.  <br/> |
|[CurrentMeetingTime](currentmeetingtime.md) <br/> |Представляет время начала собрания, которое вы хотите обновить с помощью предложенных результатов.  <br/> |
|[GlobalObjectId](globalobjectid.md) <br/> |Этот элемент не используется.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[GetUserAvailabilityRequest](getuseravailabilityrequest.md) <br/> |Содержит аргументы, используемые для получения сведений о доступности пользователей. Это корневой элемент.  <br/> XPath для этого элемента:  <br/>  `/GetUserAvailabilityRequest` <br/> |
   
## <a name="remarks"></a>Примечания

Этот элемент не требуется и может возникать только один раз, если он используется. Это значение может иметь значение null, если значение элемента [FreeBusyViewOptions](freebusyviewoptions.md) не null. 
  
> [!NOTE]
> Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа. 
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операция GetUserAvailability](getuseravailability-operation.md)


[Getting User Availability](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

