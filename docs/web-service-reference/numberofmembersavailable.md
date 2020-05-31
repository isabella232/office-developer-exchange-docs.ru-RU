---
title: нумберофмемберсаваилабле
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- NumberOfMembersAvailable
api_type:
- schema
ms.assetid: e367a278-1622-4b65-955f-2d4b2fc6e4d7
description: Элемент Нумберофмемберсаваилабле представляет количество участников списка рассылки, доступных для предложенного времени проведения собрания. Этот элемент представляет элементы, состояние которых свободно.
ms.openlocfilehash: 8669f61fbd640c160ad54739c5a15407b3dd470a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834641"
---
# <a name="numberofmembersavailable"></a>нумберофмемберсаваилабле

Элемент **нумберофмемберсаваилабле** представляет количество участников списка рассылки, доступных для предложенного времени проведения собрания. Этот элемент представляет элементы, состояние которых **свободно**.
  
[жетусераваилабилитиреспонсе](getuseravailabilityresponse.md)
  
[сугжестионсреспонсе](suggestionsresponse.md)
  
[сугжестиондайресултаррай](suggestiondayresultarray.md)
  
[сугжестиондайресулт](suggestiondayresult.md)
  
[сугжестионаррай](suggestionarray.md)
  
[Предложение](suggestion.md)
  
[аттендиконфликтдатааррай](attendeeconflictdataarray.md)
  
[граупаттендиконфликтдата](groupattendeeconflictdata.md)
  
[нумберофмемберсаваилабле](numberofmembersavailable.md)
  
```xml
<NumberOfMembersAvailable>...</NumberOfMembersAvailable>
```

 **int**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[граупаттендиконфликтдата](groupattendeeconflictdata.md) <br/> |Содержит статистические сведения о количестве доступных пользователей, количестве пользователей с конфликтами и количестве пользователей, не имеющих сведений о доступности, в списке рассылки для предполагаемого времени проведения собрания.  <br/> Ниже приведено выражение XPath для этого элемента:  <br/>  `/GetUserAvailabilityResponse/SuggestionsResponse/SuggestionDayResultArray/SuggestionDayResult[i]/SuggestionArray/Suggestion[i]/AttendeeConflictDataArray/GroupAttendeeConflictData[i]` <br/> |
   
## <a name="remarks"></a>Примечания

Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операция GetUserAvailability](getuseravailability-operation.md)
  
[жетусераваилабилитиреспонсе](getuseravailabilityresponse.md)


[Getting User Availability](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

