---
title: тубигграупаттендиконфликтдата
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- TooBigGroupAttendeeConflictData
api_type:
- schema
ms.assetid: 1512428d-ce22-4da9-b1c1-446b4bcd0a21
description: Элемент Тубигграупаттендиконфликтдата представляет участника, который был разрешен в качестве списка рассылки, но список рассылки слишком велик для расширения.
ms.openlocfilehash: 407a4a49e5f32c81439063f47df2e131dd663a4f
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44468602"
---
# <a name="toobiggroupattendeeconflictdata"></a>тубигграупаттендиконфликтдата

Элемент **тубигграупаттендиконфликтдата** представляет участника, который был разрешен в качестве списка рассылки, но список рассылки слишком велик для расширения. 
  
[жетусераваилабилитиреспонсе](getuseravailabilityresponse.md)
  
[сугжестионсреспонсе](suggestionsresponse.md)
  
[сугжестиондайресултаррай](suggestiondayresultarray.md)
  
[сугжестиондайресулт](suggestiondayresult.md)
  
[сугжестионаррай](suggestionarray.md)
  
[Предложение](suggestion.md)
  
[аттендиконфликтдатааррай](attendeeconflictdataarray.md)
  
[тубигграупаттендиконфликтдата](toobiggroupattendeeconflictdata.md)
  
```xml
<TooBigGroupAttendeeConflictData/>
```

 **тубигграупаттендиконфликтдата**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

Отсутствуют.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[аттендиконфликтдатааррай](attendeeconflictdataarray.md) <br/> |Содержит массив данных о конфликтах для участников, идентифицируемых в [жетусераваилабилитирекуест](getuseravailabilityrequest.md).  <br/> Ниже приведено выражение XPath для этого элемента:  <br/>  `/GetUserAvailabilityResponse/SuggestionsResponse/SuggestionDayResultArray/SuggestionDayResult[i]/SuggestionArray/Suggestion[i]/AttendeeConflictDataArray` <br/> |
   
## <a name="remarks"></a>Примечания

Списки рассылки, содержащие более 100 членов, не могут быть развернуты.
  
Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операция GetUserAvailability](getuseravailability-operation.md)
  
[жетусераваилабилитиреспонсе](getuseravailabilityresponse.md)


[Getting User Availability](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

