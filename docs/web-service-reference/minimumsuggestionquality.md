---
title: минимумсугжестионкуалити
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MinimumSuggestionQuality
api_type:
- schema
ms.assetid: 3725cbd4-9bc1-4f7d-8929-b2c68cb46114
description: Элемент Минимумсугжестионкуалити определяет качество предложений о встречах, возвращаемых в ответе.
ms.openlocfilehash: c85cbf65a63ac0b09408c14e01889f97a05b27b0
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44467482"
---
# <a name="minimumsuggestionquality"></a>минимумсугжестионкуалити

Элемент **минимумсугжестионкуалити** определяет качество предложений о встречах, возвращаемых в ответе. 
  
[жетусераваилабилитирекуест](getuseravailabilityrequest.md)
  
[сугжестионсвиевоптионс](suggestionsviewoptions.md)
  
[минимумсугжестионкуалити](minimumsuggestionquality.md)
  
```xml
<MinimumSuggestionQuality>...</MinimumSuggestionQuality>
```

 **сугжестионкуалити**
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

Необходимо указать текстовое значение. В следующей таблице приведены возможные значения для этого элемента:
  
|**Значение**|**Описание**|
|:-----|:-----|
|**Отличная** <br/> |0% участников конфликтуют с предложенным временем собрания.  <br/> |
|**Good** <br/> |Процент, который считается хорошим, задается с помощью элемента [гудсрешолд](goodthreshold.md) .  <br/> |
|**Честно** <br/> |Процент, который считается честным, задается с помощью элемента [гудсрешолд](goodthreshold.md) .  <br/> |
|**Плохо** <br/> |50% или несколько участников конфликтуют с предложенным временем собрания.  <br/> |
   
## <a name="remarks"></a>Примечания

Этот элемент является обязательным, если используется элемент [сугжестионсвиевоптионс](suggestionsviewoptions.md) . 
  
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

