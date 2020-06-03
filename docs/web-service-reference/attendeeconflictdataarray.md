---
title: аттендиконфликтдатааррай
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AttendeeConflictDataArray
api_type:
- schema
ms.assetid: 1d758547-28c5-4649-8334-427480c282d6
description: Элемент Аттендиконфликтдатааррай содержит массив данных о конфликтах для запрашиваемых участников, идентифицированных в операции GetUserAvailability.
ms.openlocfilehash: 770e8c00ca248ec3562180dc9d3626fd5b58f4d9
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44455802"
---
# <a name="attendeeconflictdataarray"></a>аттендиконфликтдатааррай

Элемент **аттендиконфликтдатааррай** содержит массив данных о конфликтах для запрашиваемых участников, идентифицированных в [операции GetUserAvailability](getuseravailability-operation.md).
  
- [жетусераваилабилитиреспонсе](getuseravailabilityresponse.md)
  
- [сугжестионсреспонсе](suggestionsresponse.md)
  
- [сугжестиондайресултаррай](suggestiondayresultarray.md)
  
- [сугжестиондайресулт](suggestiondayresult.md)
  
- [сугжестионаррай](suggestionarray.md)
  
- [Предложение](suggestion.md)
  
- [аттендиконфликтдатааррай](attendeeconflictdataarray.md)
  
```xml
<ArrayOfAttendeeConflictData>
   <UnknownAttendeeConflictData>...</UnknownAttendeeConflictData>
   <IndividualAttendeeConflictData>...</IndividualAttendeeConflictData>
   <TooBigGroupAttendeeConflictData>...</TooBigGroupAttendeeConflictData>
   <GroupAttendeeConflictData>...</GroupAttendeeConflictData>
</ArrayOfAttendeeConflictData>
```

 **аррайофаттендиконфликтдата**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[ункновнаттендиконфликтдата](unknownattendeeconflictdata.md) <br/> |Представляет неразрешимого участника или участника, который не является пользователем, списком рассылки или контактом.  <br/> |
|[индивидуалаттендиконфликтдата](individualattendeeconflictdata.md) <br/> |Содержит сведения о занятости пользователя или контакта для временного периода, выполняемого одновременно с указанным в элементе [предложение](suggestion.md) временем собрания.  <br/> |
|[тубигграупаттендиконфликтдата](toobiggroupattendeeconflictdata.md) <br/> |Представляет участника, которое разрешалось как список рассылки, который был слишком большим для расширения.  <br/> |
|[граупаттендиконфликтдата](groupattendeeconflictdata.md) <br/> |Содержит статистические сведения о количестве доступных пользователей, количестве пользователей с конфликтами и количестве пользователей, не имеющих сведений о доступности, в списке рассылки для предполагаемого времени проведения собрания.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Предложение](suggestion.md) <br/> |Представляет один вариант времени собрания.  <br/> Ниже приведено выражение XPath для этого элемента:  <br/>  `/GetUserAvailabilityResponse/SuggestionsResponse/SuggestionDayResultArray/SuggestionDayResult[i]/SuggestionArray/Suggestion[i]` <br/> |
   
## <a name="remarks"></a>Примечания

Положение каждого элемента в **аттендиконфликтдатааррай** соответствует положению запрашиваемых участников в элементе [маилбоксдатааррай](mailboxdataarray.md) . Каждый запрашиваемый Участник должен соответствовать одному из дочерних элементов **аттендиконфликтдатааррай** . Эти элементы представляют один конфликт с предложенным временем собрания, указанным в элементе " [предложение](suggestion.md) ". 
  
Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Операция GetUserAvailability](getuseravailability-operation.md) 
- [жетусераваилабилитиреспонсе](getuseravailabilityresponse.md)
- [Getting User Availability](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

