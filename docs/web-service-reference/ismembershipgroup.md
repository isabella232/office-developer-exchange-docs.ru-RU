---
title: IsMembershipGroup
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 0dc3e285-8f49-48ad-b844-37041c0d782b
description: Элемент IsMembershipGroup задает логическое значение, указывающее, является ли объект группы рассылки или почтового ящика.
ms.openlocfilehash: 03ab0dc75d2c798b7f2afeef85aa45f0349be70a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834050"
---
# <a name="ismembershipgroup"></a>IsMembershipGroup

Элемент **IsMembershipGroup** задает логическое значение, указывающее, является ли объект группы рассылки или почтового ящика. 
  
```XML
<IsMembershipGroup>true | false</IsMembershipGroup>
```

 **Boolean**
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

Текстовое значение **true** для элемента **IsMembershipGroup** указывает, что сущность является группу рассылки или почтового ящика. Значение false указывает, что объект не является группу рассылки или почтового ящика. 
  
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

