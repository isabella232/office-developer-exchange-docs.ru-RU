---
title: И (ProtectionRuleAndType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- And
api_type:
- schema
ms.assetid: 7fafd1c8-cd29-43a0-b383-f6595f934f48
description: Элемент и указывает, что все дочерние элементы должен соответствовать для оценено как истинное.
ms.openlocfilehash: 9e0128ee3fa2b6ffdc5975946694475afec53c25
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761379"
---
# <a name="and-protectionruleandtype"></a>И (ProtectionRuleAndType)

Элемент **и** указывает, что все дочерние элементы должны соответствовать значение **true**.
  
```xml
<And>
   <AllInternal/>
   <And/>
   <RecipientIs/>
   <SenderDepartments/>
   <True/>
</And>
```

 **ProtectionRuleAndType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[AllInternal](allinternal.md) <br/> |Имеет значение **true** , если все получатели сообщения электронной почты являются внутренними относительно организации отправителя.  <br/> |
|**И** <br/> |Указывает, что все дочерние элементы должны соответствовать значение **true**.  <br/> |
|[RecipientIs](recipientis.md) <br/> |Указывает, что какого-либо получателя сообщения электронной почты, соответствует любому из заданных получателей в дочерних элементов [значение (ProtectionRuleValueType)](value-protectionrulevaluetype.md) .  <br/> |
|[SenderDepartments](senderdepartments.md) <br/> |Указывает, что отдела отправителя соответствует любому из указанного подразделения в дочерних элементов [значение (ProtectionRuleValueType)](value-protectionrulevaluetype.md) .  <br/> |
|[Значение true](true.md) <br/> |Указывает условие, которое всегда соответствует.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Условие](condition.md) <br/> |Определяет условие, которое должно выполняться для части действия правила для выполнения.  <br/> |
|**И** <br/> |Указывает, что все дочерние элементы должны соответствовать значение **true**.  <br/> |
   
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
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

