---
title: граупаттендиконфликтдата
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GroupAttendeeConflictData
api_type:
- schema
ms.assetid: fd8bf19a-298b-4135-93e8-ead3db7e1142
description: Элемент Граупаттендиконфликтдата содержит статистические сведения о количестве доступных пользователей, количестве пользователей с конфликтами и числе пользователей, не имеющих сведений о доступности, в списке рассылки для предполагаемого времени проведения собрания.
ms.openlocfilehash: 382b4d866c95de98bd444cd6226d71813889d4f4
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833757"
---
# <a name="groupattendeeconflictdata"></a>граупаттендиконфликтдата

Элемент **граупаттендиконфликтдата** содержит статистические сведения о количестве доступных пользователей, количестве пользователей с конфликтами и числе пользователей, не имеющих сведений о доступности, в списке рассылки для предполагаемого времени проведения собрания. 
  
- [жетусераваилабилитиреспонсе](getuseravailabilityresponse.md)
- [сугжестионсреспонсе](suggestionsresponse.md)
- [сугжестиондайресултаррай](suggestiondayresultarray.md)
- [сугжестиондайресулт](suggestiondayresult.md)
- [сугжестионаррай](suggestionarray.md)
- [Предложение](suggestion.md)
- [аттендиконфликтдатааррай](attendeeconflictdataarray.md)
- [граупаттендиконфликтдата](groupattendeeconflictdata.md)
  
```xml
<GroupAttendeeConflictData>
   <NumberOfMembers>...</NumberOfMembers>
   <NumberOfMembersAvailable>...</NumberOfMembersAvailable>
   <NumberOfMembersWithConflict>...</NumberOfMembersWithConflict>
   <NumberOfMembersWithNoData>...</NumberOfMembersWithNoData>
</GroupAttendeeConflictData>
```

**граупаттендиконфликтдата**

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[нумберофмемберс](numberofmembers.md) <br/> |Представляет количество пользователей, ресурсов и комнат в списке рассылки.  <br/> |
|[нумберофмемберсаваилабле](numberofmembersavailable.md) <br/> |Представляет количество участников списка рассылки, доступных для предложенного времени проведения собрания. Этот элемент представляет элементы, состояние которых **свободно**.  <br/> |
|[нумберофмемберсвисконфликт](numberofmemberswithconflict.md) <br/> |Представляет количество участников списка рассылки, у которых возник конфликт с предложенным временем собрания. Этот элемент представляет элементы со статусом " **занято**", " **отсутствие**на работе" или " **под вопросом** ".  <br/> |
|[нумберофмемберсвиснодата](numberofmemberswithnodata.md) <br/> |Представляет количество участников группы, у которых нет опубликованных сведений о доступности, для сравнения с предложенным временем собрания. Этот элемент представляет слишком большое количество элементов списка рассылки или членов, у которых нет состояния **данных** .  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[аттендиконфликтдатааррай](attendeeconflictdataarray.md) <br/> |Содержит массив данных о конфликтах для запрашиваемых участников, идентифицированных в [операции GetUserAvailability](getuseravailability-operation.md).  <br/> Ниже приведено выражение XPath для этого элемента:  <br/>  `/GetUserAvailabilityResponse/SuggestionsResponse/SuggestionDayResultArray/SuggestionDayResult[i]/SuggestionArray/Suggestion[i]/AttendeeConflictDataArray` <br/> |
   
## <a name="remarks"></a>Примечания

Элемент **граупаттендиконфликтдата** присутствует в отклике, когда участник в [жетусераваилабилитирекуест](getuseravailabilityrequest.md) разрешается в список рассылки. Элемент **граупаттендиконфликтдата** определяет три состояния для членов списка рассылки: Available, конфликтовали или No Data. Расширение списка рассылки будет поддерживать до 100 членов. Таким образом, элемент [нумберофмемберс](numberofmembers.md) может содержать не более 100 элементов. Расширение списка рассылки является рекурсивным. Если список рассылки содержит дочерний список рассылки, расширяющий общее родительское членство на 100 элементов, дочерний список рассылки не будет расширен и будет считаться одной записью числа элементов [нумберофмемберсвиснодата](numberofmemberswithnodata.md) . Если дочерний список рассылки можно развернуть, а общее родительское членство не разворачивается до 100 элементов, его членство разворачивается, и счетчики элементов добавляются в дочерние элементы элемента **граупаттендиконфликтдата** . 
  
Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Операция GetUserAvailability](getuseravailability-operation.md)
- [жетусераваилабилитиреспонсе](getuseravailabilityresponse.md)
- [Getting User Availability](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

