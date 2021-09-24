---
title: SuggestionsViewOptions
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- SuggestionsViewOptions
api_type:
- schema
ms.assetid: bb04ae38-e62d-4a69-a479-8ff326ca726e
description: Элемент SuggestionsViewOptions содержит параметры получения сведений о предложении собрания.
ms.openlocfilehash: ba3591b88e581d45c811100a53b0a74e4bb8e010
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59522616"
---
# <a name="suggestionsviewoptions"></a>SuggestionsViewOptions

Элемент **SuggestionsViewOptions содержит** параметры получения сведений о предложении собрания. 
  
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
|[GoodThreshold](goodthreshold.md) <br/> |Указывает процент участников, которые должны иметь период времени, открытый для периода времени, чтобы квалифицироваться как хорошее предложенное время собрания.  <br/> |
|[MaximumResultsByDay](maximumresultsbyday.md) <br/> |Указывает количество рекомендуемого времени собрания в день, возвращаемого в ответе.  <br/> |
|[MaximumNonWorkHourResultsByDay](maximumnonworkhourresultsbyday.md) <br/> |Указывает количество предлагаемых результатов для времени собраний за пределами обычных рабочих часов в день.  <br/> |
|[MeetingDurationInMinutes](meetingdurationinminutes.md) <br/> |Указывает продолжительность предложенного собрания.  <br/> |
|[MinimumSuggestionQuality](minimumsuggestionquality.md) <br/> |Указывает качество предложений собрания, которые будут возвращены в ответе.  <br/> |
|[DetailedSuggestionsWindow](detailedsuggestionswindow.md) <br/> |Определяет период времени, запрашиваемой для получения подробных сведений о рекомендуемом времени собраний.  <br/> |
|[CurrentMeetingTime](currentmeetingtime.md) <br/> |Представляет время начала собрания, которое необходимо обновить с предложенными результатами времени собрания.  <br/> |
|[GlobalObjectId](globalobjectid.md) <br/> |Этот элемент не используется.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[GetUserAvailabilityRequest](getuseravailabilityrequest.md) <br/> |Содержит аргументы, используемые для получения сведений о доступности пользователей. Это корневой элемент.  <br/> XPath для этого элемента:  <br/>  `/GetUserAvailabilityRequest` <br/> |
   
## <a name="remarks"></a>Заметки

Этот элемент не требуется и может возникать только один раз, если используется. Это значение может быть null, если значение элемента [FreeBusyViewOptions](freebusyviewoptions.md) не является null. 
  
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

