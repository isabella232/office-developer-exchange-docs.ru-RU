---
title: Error
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Error
api_type:
- schema
ms.assetid: b1f54673-578a-496b-99f5-0fde2c669278
description: Элемент Error представляет одну ошибку проверки для определенного значения свойства правила, предикационного значения свойства или свойства действия.
ms.openlocfilehash: aeeda25ccc3e657e99bd6f2fea12322fdd3e720d
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59530863"
---
# <a name="error"></a>Error

Элемент **Error** представляет одну ошибку проверки для определенного значения свойства правила, предикационного значения свойства или свойства действия. 
  
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
|[FieldUri (Rule)](fielduri-rule.md) <br/> |Указывает URI в поле правил, которое вызвало ошибку проверки.  <br/> |
|[ErrorCode](errorcode.md) <br/> |Представляет код ошибки проверки правил, в который описывается, что не удалось проверки для каждого правила предиката или действия.  <br/> |
|[ErrorMessage](errormessage.md) <br/> |Представляет причину ошибки проверки.  <br/> |
|[FieldValue](fieldvalue.md) <br/> |Представляет значение поля, вызываемого ошибкой проверки.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[ValidationErrors](validationerrors.md) <br/> |Представляет массив ошибок проверки правил в каждом поле правил, в которых имеется ошибка.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Нет.
  
## <a name="remarks"></a>Заметки

Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |True  <br/> |
   
## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

