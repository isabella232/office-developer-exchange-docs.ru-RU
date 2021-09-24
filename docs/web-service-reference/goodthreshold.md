---
title: GoodThreshold
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- GoodThreshold
api_type:
- schema
ms.assetid: 68f607f5-7271-46a6-8ffc-91878185a683
description: Элемент GoodThreshold указывает процент участников, которые должны иметь открытый период времени для того, чтобы период времени мог квалифицироваться как хорошее предложенное время собрания.
ms.openlocfilehash: bec5159b46a350cb01f8d573c68e1925aeb40ac9
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59533222"
---
# <a name="goodthreshold"></a>GoodThreshold

Элемент **GoodThreshold** указывает процент участников, которые должны иметь открытый период времени для того, чтобы период времени мог квалифицироваться как хорошее предложенное время собрания. 
  
[GetUserAvailabilityRequest](getuseravailabilityrequest.md)
  
[SuggestionsViewOptions](suggestionsviewoptions.md)
  
[GoodThreshold](goodthreshold.md)
  
```xml
<GoodThreshold>...</GoodThreshold>
```

 **int**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[SuggestionsViewOptions](suggestionsviewoptions.md) <br/> |Содержит параметры получения сведений о предложении собрания.  <br/> XPath для этого элемента:  <br/>  `/GetUserAvailabilityRequest/SuggestionViewOptions` <br/> |
   
## <a name="text-value"></a>Текстовое значение

Требуется текстовое значение. Ожидаемые значения в несколько раз от 0 до 50.
  
## <a name="remarks"></a>Заметки

Этот элемент необходим, если используется элемент [SuggestionsViewOptions.](suggestionsviewoptions.md) Элемент **GoodThreshold** также определяет, какие собрания считаются справедливыми. Это процент участников с конфликтами меньше, чем хороший порог и выше 50 процентов, предложенное время собрания квалифицируется как Справедливое. Хороший порог плюс 50 равняется проценту, который определяет пороговое значение Good/Fair. 
  
> [!NOTE]
> Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа. 
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операция GetUserAvailability](getuseravailability-operation.md)


[Getting User Availability](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

