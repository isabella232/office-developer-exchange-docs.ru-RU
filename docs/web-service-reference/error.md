---
title: Ошибка
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Error
api_type:
- schema
ms.assetid: b1f54673-578a-496b-99f5-0fde2c669278
description: Элемент Error представляет ошибку одной проверки на значение свойства определенное правило, значение свойства предиката или значение свойства действия.
ms.openlocfilehash: adb2de56b7610aa92b5bf5b8d43ac22f35021b64
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762379"
---
# <a name="error"></a>Ошибка

Элемент **Error** представляет ошибку одной проверки на значение свойства определенное правило, значение свойства предиката или значение свойства действия. 
  
```XML
<Error>
   <FieldUri/>
   <ErrorCode/>
   <ErrorMessage/>
   <FieldValue/>
</Error>
```

 **RuleValidationErrorType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[FieldUri (правила)](fielduri-rule.md) <br/> |Задает URI в поле правило, вызвавшей ошибку проверки.  <br/> |
|[Код ошибки](errorcode.md) <br/> |Представляет код ошибки проверки правила, который описывает, что не удалось средства проверки для каждого правила предикат или действие.  <br/> |
|[Сообщение об ошибке](errormessage.md) <br/> |Представляет причину ошибки проверки.  <br/> |
|[FieldValue](fieldvalue.md) <br/> |Представляет значение поля, вызвавшей ошибку проверки.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[ValidationErrors](validationerrors.md) <br/> |Представляет массив ошибок проверки правил для каждого правила поля, имеющего ошибку.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Нет.
  
## <a name="remarks"></a>Замечания

Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |True  <br/> |
   
## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

