---
title: RetentionAction
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 3bdf5955-1212-48a1-b3b5-743086866c91
description: Элемент RetentionAction указывает действие, выполняемое с элементами с помощью тега хранения.
ms.openlocfilehash: 54a1038f2e56aad66f89522423ccfbd69dc44a80
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835215"
---
# <a name="retentionaction"></a>RetentionAction

Элемент **RetentionAction** указывает действие, выполняемое с элементами с помощью тега хранения. 
  
```XML
<RetentionAction> None | MoveToDeletedItems | MoveToFolder | DeleteAndAllowRecovery | PermanentlyDelete | MarkAsPastRetentionLimit | MoveToArchive <RetentionAction>
```

 **ретентионактионтипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

[Retentionpolicytag используется](retentionpolicytag.md)
  
## <a name="text-value"></a>Текстовое значение

Текстовое значение элемента **RetentionAction** — это действие, выполняемое над элементами. Следующий список содержит текстовые значения для элемента **RetentionAction** . 
  
> **None** — для элемента не выполняется никаких действий. 
    
> **MoveToDeletedItems** — элемент перемещается в папку "Удаленные" по умолчанию. 
    
> **MoveToFolder** — элемент перемещается в указанную папку. 
    
> **Делетеандалловрековери** — элемент удален и помещен в корзину. 
    
> **PermanentlyDelete** — элемент безвозвратно удаляется из почтового ящика. 
    
> **Маркаспастретентионлимит** — элемент с пометкой о превышении предельного времени хранения. 
    
> **MoveToArchive** — элемент перемещается в архивный почтовый ящик. 
    
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
   

