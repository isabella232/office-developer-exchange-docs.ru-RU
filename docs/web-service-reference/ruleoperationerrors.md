---
title: RuleOperationErrors
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: f15c7b9e-a670-4a11-bb62-2a298c91f142
description: Элемент RuleOperationErrors представляет массив ошибок проверки правил в каждом поле правил, в которых имеется ошибка.
ms.openlocfilehash: 2428d68719e7d9ef5d1fdf87ec94f1f9390bf631
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59524499"
---
# <a name="ruleoperationerrors"></a>RuleOperationErrors

Элемент **RuleOperationErrors** представляет массив ошибок проверки правил в каждом поле правил, в которых имеется ошибка. 
  
[UpdateInboxRulesResponse](updateinboxrulesresponse.md)
  
[RuleOperationErrors](ruleoperationerrors.md)
  
```XML
<RuleOperationErrors>
    <RuleOperationError>
</RuleOperationErrors>
```

 **ArrayOfRuleOperationErrorsType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[RuleOperationError](ruleoperationerror.md) <br/> |Представляет ошибку операции правила.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[UpdateInboxRulesResponse](updateinboxrulesresponse.md) <br/> |Определяет ответ на запрос [UpdateInboxRules.](updateinboxrules.md)  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Нет.
  
## <a name="remarks"></a>Заметки

Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |Верно  <br/> |
   
## <a name="see-also"></a>См. также



[UpdateInboxRules](updateinboxrules.md)


- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

