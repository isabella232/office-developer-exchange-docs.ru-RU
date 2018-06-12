---
title: RetentionAction
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 3bdf5955-1212-48a1-b3b5-743086866c91
description: Элемент RetentionAction указывает действие, выполняемое для элементов с помощью тега хранения.
ms.openlocfilehash: 54a1038f2e56aad66f89522423ccfbd69dc44a80
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19835215"
---
# <a name="retentionaction"></a>RetentionAction

Элемент **RetentionAction** указывает действие, выполняемое для элементов с помощью тега хранения. 
  
```XML
<RetentionAction> None | MoveToDeletedItems | MoveToFolder | DeleteAndAllowRecovery | PermanentlyDelete | MarkAsPastRetentionLimit | MoveToArchive <RetentionAction>
```

 **RetentionActionType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

[RetentionPolicyTag](retentionpolicytag.md)
  
## <a name="text-value"></a>Текстовое значение

Текстовое значение элемента **RetentionAction** — это действие, выполняемое для элементов. Следующий список содержит текстовые значения для элемента **RetentionAction** . 
  
> **None** - никаких действий выполняется для элемента. 
    
> **MoveToDeletedItems** - элемент перемещаются в папку Deleted Items по умолчанию. 
    
> **MoveToFolder** - элемент перемещается в указанную папку. 
    
> **DeleteAndAllowRecovery** - элемент удаляется и поместить в корзину. 
    
> **PermanentlyDelete** - элемент окончательно удаляется из почтового ящика. 
    
> **MarkAsPastRetentionLimit** - элемент отмечен как превышении ограничения времени хранения. 
    
> **MoveToArchive** - элемент перемещаются в архивный почтовый ящик. 
    
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
   

