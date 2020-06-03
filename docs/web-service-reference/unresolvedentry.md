---
title: унресолведентри
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
description: Элемент Унресолведентри содержит имя контакта или списка рассылки, которые требуется разрешить.
ms.openlocfilehash: 0f157c1be6c327187456a795c4c1000b8c35b620
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459842"
---
# <a name="unresolvedentry"></a>унресолведентри

Элемент **унресолведентри** содержит имя контакта или списка рассылки, которые требуется разрешить. 
  
[ResolveNames](resolvenames.md)
  
[унресолведентри](unresolvedentry.md)
  
```xml
<UnresolvedEntry/>
```

 **нонемптистрингтипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

Отсутствуют.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[ResolveNames](resolvenames.md) <br/> |Определяет запрос на разрешение неоднозначных имен.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение представляет имя общедоступного контакта или списка рассылки. Минимальная длина строки — один символ.
  
## <a name="remarks"></a>Примечания

Текстовое значение этого элемента используется для сопоставления имен со следующими полями:
  
- Имя
    
- Фамилия
    
- Различающееся имя (DN)
    
- Полное имя
    
- Office
    
- Alias
    
- SMTP-адрес
    
Адреса электронной почты с предфиксированными типами маршрутизации, такими как SMTP или SIP, сохраняются в массиве с несколькими значениями. [Операция ResolveNames](resolvenames-operation.md) выполняет частичное соответствие с каждым значением этого массива при добавлении типа маршрутизации в начале неизвестного имени, например "SIP:user1@Contoso.com". Если не указать тип маршрутизации, операция **ResolveNames** по умолчанию будет иметь тип маршрутизации SMTP, сопоставлять его с основным СВОЙСТВОМ SMTP-адреса, а не выполнять поиск по многозначному массиву. 
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операция ResolveNames](resolvenames-operation.md)


- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

