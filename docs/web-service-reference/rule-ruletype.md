---
title: Rule (RuleType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Rule
api_type:
- schema
ms.assetid: 259a1f62-b235-4964-88bf-2d1f1c05a563
description: Элемент Правила содержит одно правило и представляет правило в почтовом ящике пользователя.
ms.openlocfilehash: 0e7d7284d561ea374f66106072df0c4f850c590c
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59527518"
---
# <a name="rule-ruletype"></a>Rule (RuleType)

Элемент **Правила** содержит одно правило и представляет правило в почтовом ящике пользователя. 
  
```XML
<Rule>
    <RuleId>
    <DisplayName>
    <Priority>
    <IsEnabled>
    <IsNotSupported>
    <IsInError>
    <Conditions>
    <Exceptions>
    <Actions>
</Rule>
```

 **RuleType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[RuleId](ruleid.md) <br/> |Указывает идентификатор правила.  <br/> |
|[DisplayName (string)](displayname-string.md) <br/> |Содержит имя отображения правила.  <br/> |
|[Приоритет](priority.md) <br/> |Указывает порядок запуска правила.  <br/> |
|[IsEnabled](isenabled.md) <br/> |Указывает, включено ли правило.  <br/> |
|[IsNotSupported](isnotsupported.md) <br/> |Указывает, нельзя ли изменить правило с помощью API управляемого кода.  <br/> |
|[IsInError](isinerror.md) <br/> |Указывает, является ли правило ошибкой.  <br/> |
|[Conditions](conditions.md) <br/> |Определяет условия, которые при выполнении будут вызывать действия правила для правила.  <br/> |
|[Exceptions](exceptions.md) <br/> |Определяет исключения, которые представляют все доступные условия исключения правил для правила "Входящие".  <br/> |
|[Actions](actions.md) <br/> |Представляет действия, которые будут приняты в сообщении при выполнении условий.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[CreateRuleOperation](createruleoperation.md) <br/> |Представляет операцию по созданию нового правила.  <br/> |
|[InboxRules](inboxrules.md) <br/> |Представляет массив правил в почтовом ящике пользователя.  <br/> |
|[SetRuleOperation](setruleoperation.md) <br/> |Представляет операцию по обновлению существующего правила.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Нет.
  
## <a name="remarks"></a>Заметки

Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |True  <br/> |
   
## <a name="see-also"></a>См. также



[UpdateInboxRules](updateinboxrules.md)
  
[SetRuleOperation](setruleoperation.md)
  
[CreateRuleOperation](createruleoperation.md)


- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

