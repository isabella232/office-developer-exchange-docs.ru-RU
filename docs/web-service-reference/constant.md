---
title: Константа
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Constant
api_type:
- schema
ms.assetid: 340af0cd-9f12-44ab-b8f1-21d107c8d0c9
description: Элемент Constant определяет константное значение в ограничении.
ms.openlocfilehash: 6cb2eaa4227a8fd0985e8ff5a15d647c3bb1cd6a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44461557"
---
# <a name="constant"></a>Константа

Элемент **Constant** определяет константное значение в ограничении. 
  
```xml
<Constant Value="" />
```

 **константвалуетипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|**Значение** <br/> |Указывает значение, которое требуется сравнить в ограничении.  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

Отсутствуют.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Contains](contains.md) <br/> |Представляет выражение поиска, которое определяет, содержит ли данное свойство предоставленное строковое значение константы.  <br/> |
|[фиелдуриорконстант](fielduriorconstant.md) <br/> |Представляет свойство или значение константы, которое будет использоваться при сравнении с другим свойством.  <br/> |
   
## <a name="remarks"></a>Примечания

Строковое значение в атрибуте **value** должно быть приводимым к типу, с которым выполняется сравнение. Например, если вы сравниваете свойство Date/Time со значением константы, строковое значение должно представлять дату и время. 
  
Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

