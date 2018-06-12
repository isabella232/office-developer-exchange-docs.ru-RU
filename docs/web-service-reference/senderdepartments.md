---
title: SenderDepartments
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SenderDepartments
api_type:
- schema
ms.assetid: b016cdde-d597-40ac-87c4-63ca68bd539d
description: Элемент SenderDepartments указывает, что отдела отправителя соответствует любому из указанного подразделения в дочерних элементов значение (ProtectionRuleValueType).
ms.openlocfilehash: d40e6299bd46ede559cc2cce3bcc9d1611e96bd7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19835331"
---
# <a name="senderdepartments"></a>SenderDepartments

Элемент **SenderDepartments** указывает, что отдела отправителя соответствует любому из указанного подразделения в дочерних элементов [значение (ProtectionRuleValueType)](value-protectionrulevaluetype.md) . 
  
```XML
<SenderDepartments>
   <Value/>
</SenderDepartments>
```

 **ProtectionRuleSenderDepartmentsType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Значение (ProtectionRuleValueType)](value-protectionrulevaluetype.md) <br/> |Идентифицирует отдела одного отправителя.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Условие](condition.md) <br/> |Определяет условие, которое должно выполняться для части действия правила для выполнения.  <br/> |
|[И (ProtectionRuleAndType)](and-protectionruleandtype.md) <br/> |Указывает, что все дочерние элементы должны соответствовать значение **true**. Указывает, что должно быть более одного условия дочерних правила защиты.  <br/> |
   
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

