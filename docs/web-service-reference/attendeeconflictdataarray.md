---
title: AttendeeConflictDataArray
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- AttendeeConflictDataArray
api_type:
- schema
ms.assetid: 1d758547-28c5-4649-8334-427480c282d6
description: Элемент AttendeeConflictDataArray содержит массив конфликтных данных для запрашиваемого участника, выявленного в операции GetUserAvailability.
ms.openlocfilehash: 1054fba62c7e0746a13471433d6d619a304ff848
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59524364"
---
# <a name="attendeeconflictdataarray"></a>AttendeeConflictDataArray

Элемент **AttendeeConflictDataArray** содержит массив конфликтных данных для запрашиваемого участника, выявленного в операции [GetUserAvailability.](getuseravailability-operation.md)
  
- [GetUserAvailabilityResponse](getuseravailabilityresponse.md)
  
- [SuggestionsResponse](suggestionsresponse.md)
  
- [SuggestionDayResultArray](suggestiondayresultarray.md)
  
- [SuggestionDayResult](suggestiondayresult.md)
  
- [SuggestionArray](suggestionarray.md)
  
- [Предложение](suggestion.md)
  
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
|[UnknownAttendeeConflictData](unknownattendeeconflictdata.md) <br/> |Представляет нераспределяемого участника или участника, который не является пользователем, списком рассылки или контактом.  <br/> |
|[IndividualAttendeeConflictData](individualattendeeconflictdata.md) <br/> |Содержит состояние свободного или занятого пользователя или контакта для окне времени, которое происходит одновременно с предложенным временем собрания, идентифицированным в [элементе Предложение.](suggestion.md)  <br/> |
|[TooBigGroupAttendeeConflictData](toobiggroupattendeeconflictdata.md) <br/> |Представляет участника, который был разрешен в качестве списка рассылки, который был слишком велик для расширения.  <br/> |
|[GroupAttendeeConflictData](groupattendeeconflictdata.md) <br/> |Содержит сводную конфликтную информацию о количестве доступных пользователей, количестве пользователей, имеющих конфликты, и количестве пользователей, не имеющих сведений о доступности в списке рассылки в течение предложенного времени собрания.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Предложение](suggestion.md) <br/> |Представляет одно предложение о времени собрания.  <br/> Ниже приводится выражение XPath к этому элементу:  <br/>  `/GetUserAvailabilityResponse/SuggestionsResponse/SuggestionDayResultArray/SuggestionDayResult[i]/SuggestionArray/Suggestion[i]` <br/> |
   
## <a name="remarks"></a>Заметки

Положение каждого элемента **в элементе AttendeeConflictDataArray** соответствует позиции запрашиваемого участника элемента [MailboxDataArray.](mailboxdataarray.md) Каждый запрашиваемый участник должен соответствовать одному из детских элементов **AttendeeConflictDataArray.** Эти элементы представляют собой один конфликт с предложенным временем собрания, указанным в [элементе Предложение.](suggestion.md) 
  
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

