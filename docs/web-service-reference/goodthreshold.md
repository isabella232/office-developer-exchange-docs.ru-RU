---
title: гудсрешолд
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GoodThreshold
api_type:
- schema
ms.assetid: 68f607f5-7271-46a6-8ffc-91878185a683
description: Элемент Гудсрешолд указывает процент участников, для которых должен быть открыт период времени, чтобы определить, какой период времени должен быть приемлемым для предполагаемого времени проведения собрания.
ms.openlocfilehash: 34ea433ad7315d61df8cf8e22bae1166d3210af3
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457314"
---
# <a name="goodthreshold"></a>гудсрешолд

Элемент **гудсрешолд** указывает процент участников, для которых должен быть открыт период времени, чтобы определить, какой период времени должен быть приемлемым для предполагаемого времени проведения собрания. 
  
[жетусераваилабилитирекуест](getuseravailabilityrequest.md)
  
[сугжестионсвиевоптионс](suggestionsviewoptions.md)
  
[гудсрешолд](goodthreshold.md)
  
```xml
<GoodThreshold>...</GoodThreshold>
```

 **int**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

Отсутствуют.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[сугжестионсвиевоптионс](suggestionsviewoptions.md) <br/> |Содержит параметры для получения сведений о предложении собрания.  <br/> XPath для этого элемента:  <br/>  `/GetUserAvailabilityRequest/SuggestionViewOptions` <br/> |
   
## <a name="text-value"></a>Текстовое значение

Необходимо указать текстовое значение. Ожидаемые целые значения находятся в диапазоне от 0 до 50.
  
## <a name="remarks"></a>Примечания

Этот элемент является обязательным, если используется элемент [сугжестионсвиевоптионс](suggestionsviewoptions.md) . Элемент **гудсрешолд** также определяет, что встречами считается удовлетворительно. В процентах от участников с конфликтами меньше, чем на 50 процентов, рекомендуемое время проведения собрания определено как справедливое. Хорошее пороговое значение плюс 50 соответствует проценту, определяющему хорошее/приемлемое пороговое значение. 
  
> [!NOTE]
> Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа. 
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операция GetUserAvailability](getuseravailability-operation.md)


[Getting User Availability](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

