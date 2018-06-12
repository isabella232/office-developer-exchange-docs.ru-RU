---
title: UnresolvedEntry
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UnresolvedEntry
api_type:
- schema
ms.assetid: 5ac6116a-3b24-40f8-a877-dbe9a6935919
description: Элемент UnresolvedEntry содержит имя контакта или список рассылки для разрешения.
ms.openlocfilehash: 98b447cd49685b49f73f75f12d921a65749be245
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19840300"
---
# <a name="unresolvedentry"></a>UnresolvedEntry

Элемент **UnresolvedEntry** содержит имя контакта или список рассылки для разрешения. 
  
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
|[ResolveNames](resolvenames.md) <br/> |Определяет запрос для разрешения неоднозначных имен.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение представляет имя общей списка рассылки или контактов. Минимальная длина строки — один символ.
  
## <a name="remarks"></a>Замечания

Текстовое значение этого элемента используется для разрешения имен для следующих полей:
  
- Имя
    
- Фамилия
    
- Отображаемое имя
    
- Полное имя
    
- Office
    
- Alias
    
- SMTP-адрес
    
Адреса электронной почты с с префиксами типов маршрутизации, например smtp или sip, сохраняются в нескольких значений массива. [Операция ResolveNames](resolvenames-operation.md) выполняет частичное соответствие каждого значения этого массива, при добавлении типа маршрутизации в начале неизвестное имя, например «sip:User1@Contoso.com». Если не указать тип маршрутизации, операция **ResolveNames** по умолчанию для типа маршрутизации smtp, соответствует свойству основной адрес SMTP и поиск нескольких значений массива. 
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операция ResolveNames](resolvenames-operation.md)


- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

