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
description: Элемент error представляет одну ошибку проверки для определенного значения свойства правила, значения свойства предиката или значения свойства Action.
ms.openlocfilehash: 9c28f63aa79446d89152868c81c85ffa7b3a8b39
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460682"
---
# <a name="error"></a>Ошибка

Элемент **Error** представляет одну ошибку проверки для определенного значения свойства правила, значения свойства предиката или значения свойства Action. 
  
```XML
<Error>
   <FieldUri/>
   <ErrorCode/>
   <ErrorMessage/>
   <FieldValue/>
</Error>
```

 **рулевалидатионеррортипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Фиелдури (правило)](fielduri-rule.md) <br/> |Задает универсальный код ресурса (URI) для поля правила, вызвавшего ошибку проверки.  <br/> |
|[ErrorCode](errorcode.md) <br/> |Представляет код ошибки проверки правила, указывающий, что не прошло проверку для каждого предиката правила или действия.  <br/> |
|[ErrorMessage](errormessage.md) <br/> |Представляет причину ошибки проверки.  <br/> |
|[FieldValue](fieldvalue.md) <br/> |Представляет значение поля, вызвавшего ошибку проверки.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[валидатионеррорс](validationerrors.md) <br/> |Представляет массив ошибок проверки правил для каждого поля правила, в котором возникла ошибка.  <br/> |
   
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

