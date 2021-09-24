---
title: UnresolvedEntry
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- UnresolvedEntry
api_type:
- schema
ms.assetid: 5ac6116a-3b24-40f8-a877-dbe9a6935919
description: Элемент UnresolvedEntry содержит имя списка контактов или рассылки для решения.
ms.openlocfilehash: 77074d5aed0a799d355fd176a8c9c06f2dffec5a
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59538669"
---
# <a name="unresolvedentry"></a>UnresolvedEntry

Элемент **UnresolvedEntry** содержит имя списка контактов или рассылки для решения. 
  
[ResolveNames](resolvenames.md)
  
[UnresolvedEntry](unresolvedentry.md)
  
```xml
<UnresolvedEntry/>
```

 **NonEmptyStringType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[ResolveNames](resolvenames.md) <br/> |Определяет запрос на разрешение неоднозначных имен.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение представляет имя общего контакта или списка рассылки. Минимальная длина строки — один символ.
  
## <a name="remarks"></a>Заметки

Текстовое значение этого элемента используется для решения имен в следующих полях:
  
- Имя
    
- Фамилия
    
- Отображаемое имя
    
- Полное имя
    
- Office
    
- Alias
    
- SMTP-адрес
    
Адреса электронной почты с префиксными типами маршрутиза, такими как smtp или sip, сохраняются в многоценном массиве. Операция [ResolveNames](resolvenames-operation.md) выполняет частичное соответствие каждому значению этого массива при добавлении типа маршрутизов в начале неурегулированного имени, например "sip:User1@Contoso.com". Если не указать тип маршрутизации, операция **ResolveNames** будет по умолчанию соответствовать типу smtp маршрутизации, соответствовать основному свойству адресов SMTP, а не искать многоценный массив. 
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операция ResolveNames](resolvenames-operation.md)


- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

