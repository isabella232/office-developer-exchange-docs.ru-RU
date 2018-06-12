---
title: AttendeeConflictDataArray
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
description: Элемент AttendeeConflictDataArray содержит массив данных конфликта запрашиваемого участников, определенный в операция GetUserAvailability.
ms.openlocfilehash: 169312b8a3d37c014ba58fbfe094d786b134fc90
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761517"
---
# <a name="attendeeconflictdataarray"></a>AttendeeConflictDataArray

Элемент **AttendeeConflictDataArray** содержит массив данных конфликта запрашиваемого участников, определенный в [операция GetUserAvailability](getuseravailability-operation.md).
  
- [GetUserAvailabilityResponse](getuseravailabilityresponse.md)
  
- [SuggestionsResponse](suggestionsresponse.md)
  
- [SuggestionDayResultArray](suggestiondayresultarray.md)
  
- [SuggestionDayResult](suggestiondayresult.md)
  
- [SuggestionArray](suggestionarray.md)
  
- [Предложения](suggestion.md)
  
- [AttendeeConflictDataArray](attendeeconflictdataarray.md)
  
```xml
<ArrayOfAttendeeConflictData>
   <UnknownAttendeeConflictData>...</UnknownAttendeeConflictData>
   <IndividualAttendeeConflictData>...</IndividualAttendeeConflictData>
   <TooBigGroupAttendeeConflictData>...</TooBigGroupAttendeeConflictData>
   <GroupAttendeeConflictData>...</GroupAttendeeConflictData>
</ArrayOfAttendeeConflictData>
```

 **ArrayOfAttendeeConflictData**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[UnknownAttendeeConflictData](unknownattendeeconflictdata.md) <br/> |Представляет неразрешимые участника или участника, который не является пользователем, список рассылки или контактов.  <br/> |
|[IndividualAttendeeConflictData](individualattendeeconflictdata.md) <br/> |Содержит пользователя или контакта состояния занятости для временной интервал, что происходит в то же время согласно предложениям время, обнаруженных в элементе [предложение](suggestion.md) собрания.  <br/> |
|[TooBigGroupAttendeeConflictData](toobiggroupattendeeconflictdata.md) <br/> |Представляет участника, которая разрешается в качестве список рассылки, который был слишком велик для разверните узел.  <br/> |
|[GroupAttendeeConflictData](groupattendeeconflictdata.md) <br/> |Содержит конфликта статистические сведения об число доступных пользователей, число пользователей, имеющих конфликтов и количество пользователей, у которых нет сведений о доступности в списке рассылки для предложенного собрания.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Предложения](suggestion.md) <br/> |Представляет один предложения о времени на собрания.  <br/> Ниже приведен выражение XPath для этого элемента.  <br/>  `/GetUserAvailabilityResponse/SuggestionsResponse/SuggestionDayResultArray/SuggestionDayResult[i]/SuggestionArray/Suggestion[i]` <br/> |
   
## <a name="remarks"></a>Замечания

Положение каждого элемента в **AttendeeConflictDataArray** соответствует положение запрошенного участников в элементе [MailboxDataArray](mailboxdataarray.md) . Каждого запроса участника должен соответствовать одному из **AttendeeConflictDataArray** дочерние элементы. Эти элементы представляют отдельного конфликта с временем предложенного собрания, обнаруженных в элементе [предложения](suggestion.md) . 
  
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

