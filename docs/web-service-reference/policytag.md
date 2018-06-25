---
title: PolicyTag
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: fa4b1447-dc7b-47ad-a677-78fcee443dc6
description: Элемент PolicyTag указывает идентификатор хранения для элемента или папки.
ms.openlocfilehash: d6cd5aab1145f6006912541c8f8c1d0a91d1e17e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834835"
---
# <a name="policytag"></a>PolicyTag

Элемент **PolicyTag** указывает идентификатор хранения для элемента или папки. 
  
```xml
<PolicyTag IsExplicit="true | false"></PolicyTag>
```

 **RetentionTagType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|IsExplicit  <br/> |Указывает, было ли явно задано тег политики на элемента или папки.  <br/> Текстовое значение **true** для атрибута **IsExplicit** указывает, что тег политики явно была установлена на элемент или папку. Текстовое значение **false** указывает, что тег политики неявно была установлена на элемент или папку на основании тег политики родительской папки.  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

[SearchPreviewItem](searchpreviewitem.md) | [элемента](item.md) | [контакт](contact.md) | [сообщение](message-ex15websvcsotherref.md) | [DistributionList](distributionlist.md) | [элемента календаря, имеющего](calendaritem.md) | [PostItem](postitem.md) | [задач](task.md)
  
## <a name="text-value"></a>Текстовое значение

Текстовое значение элемента **PolicyTag** является идентификатором тег политики. Идентификатор тега политики — это GUID. 
  
## <a name="remarks"></a>Замечания

Этот элемент появился в Exchange Server 2013.
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> ||
   

