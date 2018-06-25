---
title: Значение (ProtectionRuleValueType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Value
api_type:
- schema
ms.assetid: b039bd6e-2198-47cf-9c78-a5e8b9d51c98
description: Элемент Value определяет одного подразделения получателю и отправителю.
ms.openlocfilehash: 6173f94dcfb83eafd62e35f185a5e8c669d50f6c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19840463"
---
# <a name="value-protectionrulevaluetype"></a>Значение (ProtectionRuleValueType)

Элемент **Value** определяет одного подразделения получателю и отправителю. 
  
```XML
<Value/>
```

**ProtectionRuleValueType**

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[RecipientIs](recipientis.md) <br/> |Указывает, что какого-либо получателя сообщения электронной почты соответствует любому из заданных получателей в **значение** дочерние элементы.  <br/> |
|[SenderDepartments](senderdepartments.md) <br/> |Указывает, что отдела отправителя соответствует любому из указанного подразделения в **значение** дочерние элементы.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Этот элемент должен содержать значение пустая строка.
  
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

