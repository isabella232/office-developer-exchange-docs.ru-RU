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
ms.openlocfilehash: cdbd21df235a62a9e201e1eaae1d82a8ac10cdd2
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465081"
---
# <a name="rule-ruletype"></a>Правило (RuleType)

Элемент **rule** содержит одно правило и представляет правило в почтовом ящике пользователя. 
  
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

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[RuleId](ruleid.md) <br/> |Задает идентификатор правила.  <br/> |
|[DisplayName (строка)](displayname-string.md) <br/> |Содержит отображаемое имя правила.  <br/> |
|[Priority](priority.md) <br/> |Указывает порядок запуска правила.  <br/> |
|[IsEnabled](isenabled.md) <br/> |Указывает, включено ли правило.  <br/> |
|[иснотсуппортед](isnotsupported.md) <br/> |Указывает, может ли правило измениться с помощью API управляемого кода.  <br/> |
|[исинеррор](isinerror.md) <br/> |Указывает, является ли правило ошибкой.  <br/> |
|[Conditions](conditions.md) <br/> |Определяет условия, при выполнении которых будут запускаться действия правил для правила.  <br/> |
|[Exceptions](exceptions.md) <br/> |Определяет исключения, которые представляют все доступные условия исключения правила для правила папки "Входящие".  <br/> |
|[Actions](actions.md) <br/> |Представляет действия, выполняемые над сообщением при выполнении условий.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[креатерулеоператион](createruleoperation.md) <br/> |Представляет операцию для создания нового правила.  <br/> |
|[инбоксрулес](inboxrules.md) <br/> |Представляет массив правил в почтовом ящике пользователя.  <br/> |
|[сетрулеоператион](setruleoperation.md) <br/> |Представляет операцию для обновления существующего правила.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Нет.
  
## <a name="remarks"></a>Примечания

Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> |True  <br/> |
   
## <a name="see-also"></a>См. также



[UpdateInboxRules](updateinboxrules.md)
  
[сетрулеоператион](setruleoperation.md)
  
[креатерулеоператион](createruleoperation.md)


- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

