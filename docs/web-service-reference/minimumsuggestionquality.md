---
title: MinimumSuggestionQuality
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- MinimumSuggestionQuality
api_type:
- schema
ms.assetid: 3725cbd4-9bc1-4f7d-8929-b2c68cb46114
description: Элемент MinimumSuggestionQuality определяет качество предложений собрания, которые будут возвращены в ответе.
ms.openlocfilehash: c1126158f7a521fbefaf34fda906d60dd15c2af4
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59510934"
---
# <a name="minimumsuggestionquality"></a>MinimumSuggestionQuality

Элемент **MinimumSuggestionQuality** определяет качество предложений собрания, которые будут возвращены в ответе. 
  
[GetUserAvailabilityRequest](getuseravailabilityrequest.md)
  
[SuggestionsViewOptions](suggestionsviewoptions.md)
  
[MinimumSuggestionQuality](minimumsuggestionquality.md)
  
```xml
<MinimumSuggestionQuality>...</MinimumSuggestionQuality>
```

 **SuggestionQuality**
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

Требуется текстовое значение. В следующей таблице перечислены возможные значения для этого элемента:
  
|**Значение**|**Описание**|
|:-----|:-----|
|**Отличная** <br/> |0% участников имеют конфликт с предложенным временем собрания.  <br/> |
|**Good** <br/> |Процент, который считается хорошим, устанавливается с помощью элемента [GoodThreshold.](goodthreshold.md)  <br/> |
|**Ярмарка** <br/> |Процент, который считается справедливым, устанавливается с помощью элемента [GoodThreshold.](goodthreshold.md)  <br/> |
|**Плохо** <br/> |У 50% или более участников есть конфликт с предложенным временем собрания.  <br/> |
   
## <a name="remarks"></a>Заметки

Этот элемент необходим, если используется элемент [SuggestionsViewOptions.](suggestionsviewoptions.md) 
  
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

