---
title: сендердепартментс
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
description: Элемент Сендердепартментс указывает, что отдел отправителя соответствует любой из указанных отделов в дочерних элементах value (Протектионрулевалуетипе).
ms.openlocfilehash: cf15b974b9c0cfb09767661f17334defc4041e43
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530347"
---
# <a name="senderdepartments"></a>сендердепартментс

Элемент **сендердепартментс** указывает, что отдел отправителя соответствует любой из указанных отделов в дочерних элементах [value (протектионрулевалуетипе)](value-protectionrulevaluetype.md) . 
  
```XML
<SenderDepartments>
   <Value/>
</SenderDepartments>
```

 **протектионрулесендердепартментстипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Значение (Протектионрулевалуетипе)](value-protectionrulevaluetype.md) <br/> |Определяет один отдел отправителя.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Условие](condition.md) <br/> |Определяет условие, которое должно быть удовлетворено для части действия правила, которое необходимо выполнить.  <br/> |
|[И (Протектионрулеандтипе)](and-protectionruleandtype.md) <br/> |Указывает, что все дочерние элементы должны сопоставляться со значением **true**. Указывает, что должно быть больше одного дочернего условия правила защиты.  <br/> |
   
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

