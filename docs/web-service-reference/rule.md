---
title: Rule
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
ms.assetid: c30f3851-bd56-4473-9106-dc85e9619486
description: Элемент Правила содержит одно правило защиты.
ms.openlocfilehash: 45fb13ae6e1aacb78e7e8520f8678097796e339f
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59517877"
---
# <a name="rule"></a>Rule

Элемент **Правила** содержит одно правило защиты. 
  
```XML
<Rule Name="" UserOverridable=="" Priority="">
   <Condition/>
   <Action/>
</Rule>
```

 **ProtectionRuleType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|**Name** <br/> |Определяет имя правила. Необходимый атрибут строки типа с минимальной длиной 1.  <br/> |
|**UserOverridable** <br/> |Указывает, является ли правило обязательным. Если правило является обязательным, это значение атрибута должно быть **ложным.** Необходимый атрибут типа Boolean.  <br/> |
|**Приоритет** <br/> |Указывает приоритет правила. Необходимый атрибут int типа с минимальным значением 1.  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Condition](condition.md) <br/> |Определяет условие, которое должно быть удовлетворено для исполняемой части правила действий.  <br/> |
|[Action (ProtectionRuleActionType)](action-protectionruleactiontype.md) <br/> |Определяет, какое действие должно быть выполнено, если условие соответствует части правила.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Правила ](rules-ex15websvcsotherref.md) <br/> |Содержит массив правил защиты.  <br/> |
   
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
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

