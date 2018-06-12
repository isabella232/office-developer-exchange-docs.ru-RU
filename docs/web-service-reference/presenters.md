---
title: Докладчики
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 01057872-4f1a-4246-86ba-73d10ef854a0
description: Элемент выступающие указывает докладчики в собрании по сети.
ms.openlocfilehash: f62b458759e0d8199c98827602d6c3fe16aebeea
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19834875"
---
# <a name="presenters"></a>Докладчики

Элемент **выступающие** указывает докладчики в собрании по сети. 
  
```XML
<Presenters> Disabled | Internal | Everyone </Presenters>
```

 **PresentersType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

[OnlineMeetingSettings](onlinemeetingsettings.md)
  
## <a name="text-value"></a>Текстовое значение

Текстовое значение элемента **выступающие** — тип пользователей, которые могут быть выступающим собрания по сети. Текстовые значения для элемента **выступающие** описаны в следующей таблице. 
  
**Докладчики элемент текстовые значения**

|**Значение**|**Описание**|
|:-----|:-----|
|Отключена  <br/> |Докладчики отключены.  <br/> |
|Внутренний  <br/> |Только внутренние участников может быть выступающим.  <br/> |
|Всем пользователям  <br/> |Любой участник может быть выступающим.  <br/> |
   
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
   

