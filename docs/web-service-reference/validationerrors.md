---
title: валидатионеррорс
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ValidationErrors
api_type:
- schema
ms.assetid: 009526aa-22e7-4f5c-be88-079175aa9122
description: Элемент Валидатионеррорс представляет массив ошибок проверки правил для каждого поля правила, которое содержит ошибку.
ms.openlocfilehash: 0861425b04e03a3e2e54a47a5027d0a11264392d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530277"
---
# <a name="validationerrors"></a>валидатионеррорс

Элемент **валидатионеррорс** представляет массив ошибок проверки правил для каждого поля правила, которое содержит ошибку. 
  
```XML
<VaidationErrors>
   <Error/>
</ValidationErrors>
```

 **аррайофрулевалидатионеррорстипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Error](error.md) <br/> |Представляет одну ошибку проверки для определенного значения свойства правила, значения свойства предиката или значения свойства Action  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[рулеоператионеррор](ruleoperationerror.md) <br/> |Представляет ошибку операции с правилом.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Нет.
  
## <a name="remarks"></a>Примечания

Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages. xsd  <br/> |
|Может быть пустым  <br/> |True  <br/> |
   
## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

