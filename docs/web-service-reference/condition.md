---
title: Условие
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Condition
api_type:
- schema
ms.assetid: 0790a3f2-cb31-4036-a757-7821aa0722cb
description: Элемент Condition определяет условие, которое должно быть удовлетворено для части действия правила, которое необходимо выполнить.
ms.openlocfilehash: 2aea11197f072a4dbe21292bb47075d6f273d31b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463225"
---
# <a name="condition"></a>Условие

Элемент **Condition** определяет условие, которое должно быть удовлетворено для части действия правила, которое необходимо выполнить. 
  
```xml
<Condition>
   <AllInternal/>
</Condition>
```

```xml
<Condition> 
    <SenderDepartments/> 
</Condition>
```

```xml
<Condition> 
    <True/> 
</Condition>
```

```xml
<Condition> 
    <Recipients/> 
</Condition>
```

```xml
<Condition> 
    <And/> 
</Condition>
```

**протектионрулекондитионтипе**

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[аллинтернал](allinternal.md) <br/> |Возвращает **значение true** , если все получатели сообщения электронной почты являются внутренними для организации отправителя.  <br/> |
|[И (Протектионрулеандтипе)](and-protectionruleandtype.md) <br/> |Указывает, что все дочерние элементы должны сопоставляться со значением **true**. Указывает, что должно быть больше одного дочернего условия правила защиты.  <br/> |
|[Получательявляется](recipientis.md) <br/> |Указывает, что любой получатель сообщения электронной почты соответствует любому из указанных получателей в дочерних элементах [value (протектионрулевалуетипе)](value-protectionrulevaluetype.md) .  <br/> |
|[сендердепартментс](senderdepartments.md) <br/> |Указывает, что отдел отправителя соответствует любой из указанных отделов в дочерних элементах [value (протектионрулевалуетипе)](value-protectionrulevaluetype.md) .  <br/> |
|[True](true.md) <br/> |Задает условие, которое всегда соответствует.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Rule](rule.md) <br/> |Содержит одно правило защиты.  <br/> |
   
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
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

