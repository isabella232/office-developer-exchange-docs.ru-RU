---
title: Правило (RuleType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Rule
api_type:
- schema
ms.assetid: 259a1f62-b235-4964-88bf-2d1f1c05a563
description: Элемент Rule содержит одно правило и представляет правило в почтовом ящике пользователя.
ms.openlocfilehash: b1f9f058213543633335db11f03729964baf98ad
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835259"
---
# <a name="rule-ruletype"></a>Правило (RuleType)

Элемент **Rule** содержит одно правило и представляет правило в почтовом ящике пользователя. 
  
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
|[Отображаемое имя (строка)](displayname-string.md) <br/> |Содержит отображаемое имя правила.  <br/> |
|[Приоритет](priority.md) <br/> |Указывает порядок, в котором будет выполняться правило.  <br/> |
|[Свойства IsEnabled](isenabled.md) <br/> |Указывает, включена ли правило.  <br/> |
|[IsNotSupported](isnotsupported.md) <br/> |Указывает ли правило не могут быть изменены с управляемым кодом API-интерфейсы.  <br/> |
|[IsInError](isinerror.md) <br/> |Указывает, является ли правило ошибкой.  <br/> |
|[Условия](conditions.md) <br/> |Определяет условия, если выполнены, запустит действия правил для правила.  <br/> |
|[Исключения](exceptions.md) <br/> |Определяет исключения, которые представляют все доступные правила условия исключений для правила папки «Входящие».  <br/> |
|[Действия](actions.md) <br/> |Представляет действия, которые необходимо выполнить на сообщение, если будут выполнены условия.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[CreateRuleOperation](createruleoperation.md) <br/> |Представляет операцию, чтобы создать новое правило.  <br/> |
|[InboxRules](inboxrules.md) <br/> |Представляет собой массив из правил в почтовом ящике пользователя.  <br/> |
|[SetRuleOperation](setruleoperation.md) <br/> |Представляет операцию для обновления существующего правила.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Нет.
  
## <a name="remarks"></a>Замечания

Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |True  <br/> |
   
## <a name="see-also"></a>См. также



[UpdateInboxRules](updateinboxrules.md)
  
[SetRuleOperation](setruleoperation.md)
  
[CreateRuleOperation](createruleoperation.md)


- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

