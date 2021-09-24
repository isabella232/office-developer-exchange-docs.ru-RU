---
title: RetentionAction
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 3bdf5955-1212-48a1-b3b5-743086866c91
description: Элемент RetentionAction указывает действие, выполняемые на элементах с тегом хранения.
ms.openlocfilehash: ecea4326f0e50460635966991cd55badf8946993
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59517947"
---
# <a name="retentionaction"></a>RetentionAction

Элемент **RetentionAction** указывает действие, выполняемые на элементах с тегом хранения. 
  
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

Текстовое значение элемента **RetentionAction** — это действие, выполняемые на элементах. Следующий список содержит текстовые значения элемента **RetentionAction.** 
  
> **Нет** . Действие на элементе не выполняется. 
    
> **MoveToDeletedItems** — элемент перемещается в папку удаленных элементов по умолчанию. 
    
> **MoveToFolder** — элемент перемещается в указанную папку. 
    
> **DeleteAndAllowRecovery** — элемент удаляется и помещется в контейнер. 
    
> **PermanentlyDelete** — элемент постоянно удаляется из почтового ящика. 
    
> **MarkAsPastRetentionLimit** — элемент помечен как превышение срока хранения. 
    
> **MoveToArchive** — элемент перемещается в почтовый ящик архива. 
    
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
   

