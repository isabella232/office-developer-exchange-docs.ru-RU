---
title: рулеоператионеррорс
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f15c7b9e-a670-4a11-bb62-2a298c91f142
description: Элемент Рулеоператионеррорс представляет массив ошибок проверки правил для каждого поля правила, которое содержит ошибку.
ms.openlocfilehash: d547155f3cbf9eedd0f9bfac7bf3768b3630b50e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44464954"
---
# <a name="ruleoperationerrors"></a>рулеоператионеррорс

Элемент **рулеоператионеррорс** представляет массив ошибок проверки правил для каждого поля правила, которое содержит ошибку. 
  
[упдатеинбоксрулесреспонсе](updateinboxrulesresponse.md)
  
[рулеоператионеррорс](ruleoperationerrors.md)
  
```XML
<RuleOperationErrors>
    <RuleOperationError>
</RuleOperationErrors>
```

 **аррайофрулеоператионеррорстипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[рулеоператионеррор](ruleoperationerror.md) <br/> |Представляет ошибку операции с правилом.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[упдатеинбоксрулесреспонсе](updateinboxrulesresponse.md) <br/> |Определяет ответ на запрос [UpdateInboxRules](updateinboxrules.md) .  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Нет.
  
## <a name="remarks"></a>Примечания

Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages. xsd  <br/> |
|Может быть пустым  <br/> |Верно.  <br/> |
   
## <a name="see-also"></a>См. также



[UpdateInboxRules](updateinboxrules.md)


- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

