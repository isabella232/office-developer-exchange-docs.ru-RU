---
title: Guid
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 49dcf69f-bf8d-4be6-a24c-03bbd13f4fe5
description: Элемент Guid указывает идентификатор почтового ящика.
ms.openlocfilehash: 35307a706523fc5c2916767c7508dec07deb8d09
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833799"
---
# <a name="guid"></a>Guid

Элемент **Guid** указывает идентификатор почтового ящика. 
  
```XML
<Guid></Guid>
```

 **GuidType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[SearchableMailbox](searchablemailbox.md) <br/> |Указывает почтового ящика возвращаются из **GetSearchableMailboxes** запроса.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение элемента **Guid** — это идентификатор GUID, который уникальным образом определяет почтовый ящик. 
  
## <a name="remarks"></a>Замечания

Этот элемент появился в Exchange Server 2013.
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема типа  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> ||
   
## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

