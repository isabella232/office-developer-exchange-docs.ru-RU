---
title: GroupAttendeeConflictData
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
description: Элемент GroupAttendeeConflictData содержит конфликта статистические сведения о количество пользователей, которые доступны, количество пользователей, конфликтов и количество пользователей, у которых нет сведений о доступности в рассылки списка для Предлагаемое время собрания.
ms.openlocfilehash: 382b4d866c95de98bd444cd6226d71813889d4f4
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833757"
---
# <a name="groupattendeeconflictdata"></a>GroupAttendeeConflictData

Элемент **GroupAttendeeConflictData** содержит конфликта статистические сведения о количество пользователей, которые доступны, количество пользователей, конфликтов и количество пользователей, у которых нет сведений о доступности в список рассылки для предложенного собрания. 
  
- [GetUserAvailabilityResponse](getuseravailabilityresponse.md)
- [SuggestionsResponse](suggestionsresponse.md)
- [SuggestionDayResultArray](suggestiondayresultarray.md)
- [SuggestionDayResult](suggestiondayresult.md)
- [SuggestionArray](suggestionarray.md)
- [Предложения](suggestion.md)
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
|[NumberOfMembers](numberofmembers.md) <br/> |Представляет число пользователей, ресурсов и помещения в список рассылки.  <br/> |
|[NumberOfMembersAvailable](numberofmembersavailable.md) <br/> |Представляет число членов списка рассылки, которые доступны для предложенного собрания. Этот элемент представляет элементы, для которых состояние — **бесплатными**.  <br/> |
|[NumberOfMembersWithConflict](numberofmemberswithconflict.md) <br/> |Представляет число членов списка рассылки, конфликт с временем предложенного собрания. Этот элемент представляет работников, которые имеют состояние **«занят»**, **об отсутствии на работе**или **под вопросом** .  <br/> |
|[NumberOfMembersWithNoData](numberofmemberswithnodata.md) <br/> |Представляет число членов группы, у которых нет опубликованных данных о доступности для сравнения для предложенного собрания. Этот элемент представляет членов списка рассылки слишком большого размера или участники, которые имеют состояние **Нет данных** .  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[AttendeeConflictDataArray](attendeeconflictdataarray.md) <br/> |Содержит массив данных конфликта запрашиваемого участников, определенный в [операция GetUserAvailability](getuseravailability-operation.md).  <br/> Ниже приведен выражение XPath для этого элемента.  <br/>  `/GetUserAvailabilityResponse/SuggestionsResponse/SuggestionDayResultArray/SuggestionDayResult[i]/SuggestionArray/Suggestion[i]/AttendeeConflictDataArray` <br/> |
   
## <a name="remarks"></a>Замечания

Элемент **GroupAttendeeConflictData** присутствует в ответе, когда участник в [GetUserAvailabilityRequest](getuseravailabilityrequest.md) разрешена в список рассылки. Элемент **GroupAttendeeConflictData** определяет три состояния для членов списка рассылки: доступны, конфликта, или без данных. Раскрытие списка рассылки будет поддерживает до 100 элементов. Таким образом элемент [NumberOfMembers](numberofmembers.md) может содержать не более 100 участников. Раскрытие списка рассылки — это рекурсивный. Если список рассылки содержит список рассылки дочерним, которая расширяет членства общий родительский более 100 членов, списка рассылки дочерним не развернуто и будет считаться одной операции из [NumberOfMembersWithNoData](numberofmemberswithnodata.md) счетчик элементов. Если членства общий родительский не разворачивается до более 100 членов списка рассылки дочерним могут быть развернуты, принадлежность развертывается, и число элементов добавляются дочерние элементы элемента **GroupAttendeeConflictData** . 
  
Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Операция GetUserAvailability](getuseravailability-operation.md)
- [GetUserAvailabilityResponse](getuseravailabilityresponse.md)
- [Getting User Availability](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

