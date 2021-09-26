---
title: Value (ProtectionRuleValueType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Value
api_type:
- schema
ms.assetid: b039bd6e-2198-47cf-9c78-a5e8b9d51c98
description: Элемент Value идентифицирует одного получателя или отправитель отдела.
ms.openlocfilehash: 2c4bbdcb3364f0ef8f608469f0dc1b289c4eeaf6
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59541625"
---
# <a name="value-protectionrulevaluetype"></a>Value (ProtectionRuleValueType)

Элемент **Value** идентифицирует одного получателя или отправитель отдела. 
  
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
|[RecipientIs](recipientis.md) <br/> |Указывает, что любой получатель сообщения электронной почты соответствует любому из указанных получателей в элементах **значение** ребенка.  <br/> |
|[SenderDepartments](senderdepartments.md) <br/> |Указывает, что отдел отправитель соответствует любому из указанных отделов в элементах **значение** ребенка.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Этот элемент должен содержать несущестовую строку.
  
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

