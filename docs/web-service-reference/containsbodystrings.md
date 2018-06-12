---
title: ContainsBodyStrings
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ContainsBodyStrings
api_type:
- schema
ms.assetid: 70639472-64bb-456a-8b40-dce727542443
description: Элемент ContainsBodyStrings указывает строк, которые должны встречаться в теле входящих сообщений в порядке для условие или исключение для применения.
ms.openlocfilehash: 5993bd4061298e82a2393768eccb051326564e98
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761757"
---
# <a name="containsbodystrings"></a>ContainsBodyStrings

Элемент **ContainsBodyStrings** указывает строк, которые должны встречаться в теле входящих сообщений в порядке для условие или исключение для применения. 
  
```XML
<ContainsBodyStrings>
    <String/>
</ContainsBodyStrings>
```

 **ArrayOfStringsType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Строка](string.md) <br/> |Представляет строку, которые должны встречаться в теле входящих сообщений в порядке для условие или исключение для применения.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Условия](conditions.md) <br/> |Представляет условия, которые, если удовлетворены, запускают действия правила для правила.  <br/> |
|[Исключения](exceptions.md) <br/> |Представляет исключения, которые представляют все доступные правила условия исключений для правила папки «Входящие».  <br/> |
   
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

