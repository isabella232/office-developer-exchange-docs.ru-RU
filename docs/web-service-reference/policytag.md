---
title: полицитаг
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: fa4b1447-dc7b-47ad-a677-78fcee443dc6
description: Элемент Полицитаг указывает идентификатор хранения для элемента или папки.
ms.openlocfilehash: d6cd5aab1145f6006912541c8f8c1d0a91d1e17e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834835"
---
# <a name="policytag"></a>полицитаг

Элемент **полицитаг** указывает идентификатор хранения для элемента или папки. 
  
```xml
<PolicyTag IsExplicit="true | false"></PolicyTag>
```

 **ретентионтагтипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|Явный  <br/> |Указывает, был ли явно задан тег политики для элемента или папки.  <br/> Текстовое значение **true** для атрибута **explicit** указывает на то, что тег политики был явно задан для элемента или папки. Текстовое значение **false** указывает на то, что тег политики неявно задан для элемента или папки на основе тега политики родительской папки.  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

[SearchPreviewItem](searchpreviewitem.md) | [Item](item.md) | [Контактное](contact.md) | [CalendarItem](calendaritem.md)[Message](message-ex15websvcsotherref.md) | [PostItem](postitem.md)[DistributionList](distributionlist.md) | сообщение сеарчпревиевитем Item дистрибутионлист календаритем[Task](task.md) Item |  | 
  
## <a name="text-value"></a>Текстовое значение

Текстовое значение элемента **полицитаг** — идентификатор тега политики. Идентификатор тега политики — GUID. 
  
## <a name="remarks"></a>Примечания

Этот элемент появился в Exchange Server 2013.
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> ||
   

