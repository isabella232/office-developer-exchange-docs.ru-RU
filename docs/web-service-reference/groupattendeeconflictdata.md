---
title: GroupAttendeeConflictData
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- GroupAttendeeConflictData
api_type:
- schema
ms.assetid: fd8bf19a-298b-4135-93e8-ead3db7e1142
description: Элемент GroupAttendeeConflictData содержит сводную конфликтную информацию о количестве доступных пользователей, количестве пользователей, имеющих конфликты, и количестве пользователей, не имеющих сведений о доступности в списке рассылки в течение предложенного времени собрания.
ms.openlocfilehash: 19ac366da5ad48cbc6c9e2aaa710a8c5f00e1151
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59519557"
---
# <a name="groupattendeeconflictdata"></a>GroupAttendeeConflictData

Элемент **GroupAttendeeConflictData** содержит сводную конфликтную информацию о количестве доступных пользователей, количестве пользователей, имеющих конфликты, и количестве пользователей, не имеющих сведений о доступности в списке рассылки в течение предложенного времени собрания. 
  
- [GetUserAvailabilityResponse](getuseravailabilityresponse.md)
- [SuggestionsResponse](suggestionsresponse.md)
- [SuggestionDayResultArray](suggestiondayresultarray.md)
- [SuggestionDayResult](suggestiondayresult.md)
- [SuggestionArray](suggestionarray.md)
- [Предложение](suggestion.md)
- [AttendeeConflictDataArray](attendeeconflictdataarray.md)
- [GroupAttendeeConflictData](groupattendeeconflictdata.md)
  
```xml
<GroupAttendeeConflictData>
   <NumberOfMembers>...</NumberOfMembers>
   <NumberOfMembersAvailable>...</NumberOfMembersAvailable>
   <NumberOfMembersWithConflict>...</NumberOfMembersWithConflict>
   <NumberOfMembersWithNoData>...</NumberOfMembersWithNoData>
</GroupAttendeeConflictData>
```

**GroupAttendeeConflictData**

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[NumberOfMembers](numberofmembers.md) <br/> |Представляет число пользователей, ресурсов и комнат в списке рассылки.  <br/> |
|[NumberOfMembersAvailable](numberofmembersavailable.md) <br/> |Представляет число участников списка рассылки, доступных в течение предложенного времени собрания. Этот элемент представляет участников, для которых состояние **является бесплатным.**  <br/> |
|[NumberOfMembersWithConflict](numberofmemberswithconflict.md) <br/> |Представляет число участников списка рассылки, у которых возник конфликт с предложенным временем собрания. Этот элемент представляет участников, которые имеют статус **Busy,** **OOF** или **Tentative.**  <br/> |
|[NumberOfMembersWithNoData](numberofmemberswithnodata.md) <br/> |Представляет число участников группы, которые не опубликовали бесплатные или загруженные данные для сравнения с предложенным временем собрания. Этот элемент представляет членов слишком большого списка рассылки или членов, не в которых **нет данных.**  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[AttendeeConflictDataArray](attendeeconflictdataarray.md) <br/> |Содержит массив конфликтных данных для запрашиваемого участника, выявленного в операции [GetUserAvailability.](getuseravailability-operation.md)  <br/> Ниже приводится выражение XPath к этому элементу:  <br/>  `/GetUserAvailabilityResponse/SuggestionsResponse/SuggestionDayResultArray/SuggestionDayResult[i]/SuggestionArray/Suggestion[i]/AttendeeConflictDataArray` <br/> |
   
## <a name="remarks"></a>Заметки

Элемент **GroupAttendeeConflictData** присутствует в ответе, когда участник [GetUserAvailabilityRequest](getuseravailabilityrequest.md) будет разрешен в список рассылки. Элемент **GroupAttendeeConflictData** определяет три состояния для участников списка рассылки: доступные, противоречивые или нет данных. Расширение списка рассылки будет поддерживать до 100 участников. Таким образом, элемент [NumberOfMembers](numberofmembers.md) может содержать не более 100 участников. Расширение списка рассылки является повторяемым. Если список рассылки содержит список распространения детей, который расширяет общее число родительских членов более чем до 100 членов, список распространения детей не будет расширен и будет считаться одним входом в число элементов [NumberOfMembersWithNoData.](numberofmemberswithnodata.md) Если список распространения детей может быть расширен, а общее родительское членство не расширяется до более 100 членов, его членство расширяется, а количество участников добавляется к детским элементам элемента **GroupAttendeeConflictData.** 
  
Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Операция GetUserAvailability](getuseravailability-operation.md)
- [GetUserAvailabilityResponse](getuseravailabilityresponse.md)
- [Getting User Availability](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

