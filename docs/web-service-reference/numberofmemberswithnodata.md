---
title: нумберофмемберсвиснодата
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- NumberOfMembersWithNoData
api_type:
- schema
ms.assetid: 7ca9c57c-9519-442c-a9f4-dca2b0309716
description: Элемент Нумберофмемберсвиснодата представляет количество участников списка рассылки, у которых нет опубликованных данных о занятости для сравнения с предложенным временем собрания. Этот элемент представляет слишком большое количество элементов списка рассылки или членов, у которых нет состояния данных.
ms.openlocfilehash: f73978df47bd8240dd5dabfbbf74523525e3270f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834637"
---
# <a name="numberofmemberswithnodata"></a>нумберофмемберсвиснодата

Элемент **нумберофмемберсвиснодата** представляет количество участников списка рассылки, у которых нет опубликованных данных о занятости для сравнения с предложенным временем собрания. Этот элемент представляет слишком большое количество элементов списка рассылки или членов, у которых нет состояния **данных** . 
  
[жетусераваилабилитиреспонсе](getuseravailabilityresponse.md)
  
[сугжестионсреспонсе](suggestionsresponse.md)
  
[сугжестиондайресултаррай](suggestiondayresultarray.md)
  
[сугжестиондайресулт](suggestiondayresult.md)
  
[сугжестионаррай](suggestionarray.md)
  
[Предложение](suggestion.md)
  
[аттендиконфликтдатааррай](attendeeconflictdataarray.md)
  
[граупаттендиконфликтдата](groupattendeeconflictdata.md)
  
[нумберофмемберсвиснодата](numberofmemberswithnodata.md)
  
```xml
<NumberOfMembersWithNoData>...</NumberOfMembersWithNoData>
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
|[граупаттендиконфликтдата](groupattendeeconflictdata.md) <br/> |Содержит статистические сведения о количестве доступных пользователей, количестве пользователей с конфликтами и количестве пользователей, не имеющих сведений о доступности, в списке рассылки для предполагаемого времени проведения собрания.  <br/> Ниже приведено выражение XPath для этого элемента:  <br/>  `/GetUserAvailabilityResponse/SuggestionsResponse/SuggestionDayResultArray/SuggestionDayResult[i]/SuggestionArray/Suggestion[i]/AttendeeConflictDataArray/GroupAttendeeConflictData` <br/> |
   
## <a name="remarks"></a>Примечания

Контакт в группе, у которого нет почтового ящика, это пример элемента списка рассылки, у которого нет данных календаря. Контакт может также не иметь состояния **данных** по следующим причинам: 
  
- Недостаточно разрешений.
    
- Слишком большой список рассылки для расширения.
    
- Служба каталогов Active Directory недоступна.
    
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

