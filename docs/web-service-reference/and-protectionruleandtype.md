---
title: And (ProtectionRuleAndType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- And
api_type:
- schema
ms.assetid: 7fafd1c8-cd29-43a0-b383-f6595f934f48
description: Элемент And указывает, что все детские элементы должны соответствовать для оценки до true.
ms.openlocfilehash: 01721b460d87d3282a1a793966b0259e0f1342dd
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59518940"
---
# <a name="and-protectionruleandtype"></a>And (ProtectionRuleAndType)

Элемент **And** указывает, что все детские элементы должны соответствовать для оценки **true.**
  
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
|[AllInternal](allinternal.md) <br/> |Оценивается **до true,** если все получатели сообщения электронной почты являются внутренними в организации отправитель.  <br/> |
|**And** <br/> |Указывает, что все детские элементы должны соответствовать для оценки **true.**  <br/> |
|[RecipientIs](recipientis.md) <br/> |Указывает, что любой получатель сообщения электронной почты соответствует любому из указанных получателей в элементах [Child Value (ProtectionRuleValueType).](value-protectionrulevaluetype.md)  <br/> |
|[SenderDepartments](senderdepartments.md) <br/> |Указывает, что отдел отправитель соответствует любому из указанных отделов в элементах [child Value (ProtectionRuleValueType).](value-protectionrulevaluetype.md)  <br/> |
|[True](true.md) <br/> |Указывает условие, которое всегда совпадает.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Condition](condition.md) <br/> |Определяет условие, которое должно быть удовлетворено для исполняемой части правила действий.  <br/> |
|**And** <br/> |Указывает, что все детские элементы должны соответствовать для оценки **true.**  <br/> |
   
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

