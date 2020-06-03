---
title: Дата
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Date
api_type:
- schema
ms.assetid: 2f6bc090-fff4-45b1-8d7e-8fd6e060cce2
description: Элемент Date представляет дату, которая содержит предложенное время проведения собрания.
ms.openlocfilehash: bcc152ed6aba94907189b5579b998815be45db16
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44443790"
---
# <a name="date"></a>Дата

Элемент **Date** представляет дату, которая содержит предложенное время проведения собрания. 
  
- [жетусераваилабилитиреспонсе](getuseravailabilityresponse.md) 
- [сугжестионсреспонсе](suggestionsresponse.md) 
- [сугжестиондайресултаррай](suggestiondayresultarray.md)  
- [сугжестиондайресулт](suggestiondayresult.md)  
- [Date](date.md)
  
```xml
<Date>...</Date>
```

**дата и время**

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

Отсутствуют.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[сугжестиондайресулт](suggestiondayresult.md) <br/> |Представляет один день, который содержит предложенное время проведения собрания.  <br/><br/>Ниже приведено выражение XPath 2,0 для этого элемента:<br/><br/>  `/GetUserAvailabilityResponse/SuggestionsResponse/SuggestionDayResultArray/SuggestionDayResult[i]` <br/> |
   
## <a name="text-value"></a>Текстовое значение

Необходимо указать текстовое значение. Изучите рекомендации консорциума типов данных схемы консорциума W3C для формата данных примитива dateTime.
  
## <a name="remarks"></a>Примечания

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

