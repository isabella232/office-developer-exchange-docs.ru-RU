---
title: PolicyTag
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: fa4b1447-dc7b-47ad-a677-78fcee443dc6
description: Элемент PolicyTag указывает идентификатор хранения в элементе или папке.
ms.openlocfilehash: 16759748dded6978e68450a6b8d504dd378c04be
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59519256"
---
# <a name="policytag"></a>PolicyTag

Элемент **PolicyTag** указывает идентификатор хранения в элементе или папке. 
  
```xml
<PolicyTag IsExplicit="true | false"></PolicyTag>
```

 **RetentionTagType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|IsExplicit  <br/> |Указывает, был ли метка политики явно установлена на элементе или папке.  <br/> Текстовое **значение, истинное** для атрибута **IsExplicit,** указывает на то, что тег политики был явно за установлен на элементе или папке. Текстовое значение **false** указывает на то, что тег политики был неявно установлен на элементе или папке на основе тега политики родительской папки.  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

[SearchPreviewItem](searchpreviewitem.md)  |  [Item](item.md)  |  [Контакт](contact.md)  |  [Сообщение](message-ex15websvcsotherref.md)  |  [DistributionList](distributionlist.md)  |  [CalendarItem](calendaritem.md)  |  [PostItem](postitem.md)  |  [Задача](task.md)
  
## <a name="text-value"></a>Текстовое значение

Текстовое значение элемента **PolicyTag** — идентификатор тега политики. Идентификатор тега политики — GUID. 
  
## <a name="remarks"></a>Заметки

Этот элемент появился в Exchange Server 2013.
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> ||
   

