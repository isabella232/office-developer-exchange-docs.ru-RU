---
title: сугжестионсреспонсе
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SuggestionsResponse
api_type:
- schema
ms.assetid: d25ca143-f80c-4458-b669-346fda29a5a7
description: Элемент Сугжестионсреспонсе содержит сведения о состоянии ответа и данные предложения для запрошенных предложений о собрании.
ms.openlocfilehash: 614b58a1df8e340c6be468ccddd3b37537d32591
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19840114"
---
# <a name="suggestionsresponse"></a>сугжестионсреспонсе

Элемент **сугжестионсреспонсе** содержит сведения о состоянии ответа и данные предложения для запрошенных предложений о собрании. 
  
[жетусераваилабилитиреспонсе](getuseravailabilityresponse.md)
  
[сугжестионсреспонсе](suggestionsresponse.md)
  
```xml
<SuggestionsResponse>
   <ResponseMessage>...</ResponseMessage>
   <SuggestionDayResultArray>...</SuggestionDayResultArray>
</SuggestionsResponse>
```

 **сугжестионсреспонсетипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[респонсемессаже](responsemessage.md) <br/> |Предоставляет описательные сведения о состоянии отклика.  <br/> |
|[сугжестиондайресултаррай](suggestiondayresultarray.md) <br/> |Содержит массив предложений собраний, организованных по дате.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[жетусераваилабилитиреспонсе](getuseravailabilityresponse.md) <br/> |Содержит сведения о доступности запрошенных пользователей.  <br/> Ниже приведено выражение XPath для этого элемента:  <br/>  `/GetUserAvailabilityResponse` <br/> |
   
## <a name="remarks"></a>Примечания

Этот элемент не включается в ответ GetUserAvailability, если [сугжестионсвиевоптионс](suggestionsviewoptions.md) не задан в сообщении запроса GetUserAvailability. 
  
Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операция GetUserAvailability](getuseravailability-operation.md)
  
[жетусераваилабилитиреспонсе](getuseravailabilityresponse.md)


[Getting User Availability](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

