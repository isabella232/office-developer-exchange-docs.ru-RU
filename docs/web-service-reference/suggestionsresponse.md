---
title: SuggestionsResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- SuggestionsResponse
api_type:
- schema
ms.assetid: d25ca143-f80c-4458-b669-346fda29a5a7
description: Элемент SuggestionsResponse содержит сведения о состоянии отклика и сведения о предложениях для запрашиваемого предложения собрания.
ms.openlocfilehash: 92dfac3cc0a6ddce9485a8cb266f072795b18bd5
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59544530"
---
# <a name="suggestionsresponse"></a>SuggestionsResponse

Элемент **SuggestionsResponse содержит** сведения о состоянии отклика и сведения о предложениях для запрашиваемого предложения собрания. 
  
[GetUserAvailabilityResponse](getuseravailabilityresponse.md)
  
[SuggestionsResponse](suggestionsresponse.md)
  
```xml
<SuggestionsResponse>
   <ResponseMessage>...</ResponseMessage>
   <SuggestionDayResultArray>...</SuggestionDayResultArray>
</SuggestionsResponse>
```

 **SuggestionsResponseType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[ResponseMessage](responsemessage.md) <br/> |Предоставляет описательные сведения о состоянии ответа.  <br/> |
|[SuggestionDayResultArray](suggestiondayresultarray.md) <br/> |Содержит массив предложений по собраниям, организованных по дате.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[GetUserAvailabilityResponse](getuseravailabilityresponse.md) <br/> |Содержит сведения о доступности запрашиваемой информации пользователей.  <br/> Ниже приводится выражение XPath к этому элементу:  <br/>  `/GetUserAvailabilityResponse` <br/> |
   
## <a name="remarks"></a>Заметки

Этот элемент не входит в ответ GetUserAvailability, если в сообщении запроса GetUserAvailability не задаваются [предложенияViewOptions.](suggestionsviewoptions.md) 
  
Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операция GetUserAvailability](getuseravailability-operation.md)
  
[GetUserAvailabilityResponse](getuseravailabilityresponse.md)


[Getting User Availability](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

