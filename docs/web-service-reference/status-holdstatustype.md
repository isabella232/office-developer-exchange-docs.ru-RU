---
title: Status (HoldStatusType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: fee3f1f9-e868-49fa-a554-7ff096964718
description: Элемент Status указывает состояние удержания для почтового ящика.
ms.openlocfilehash: a055dde61ae52c266f2349036c881d2b00557171
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59521237"
---
# <a name="status-holdstatustype"></a>Status (HoldStatusType)

Элемент **Status** указывает состояние удержания для почтового ящика. 
  
```XML
<Status> NotOnHold | Pending | OnHold | PartialHold | Failed </Status>
```

 **HoldStatusType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

[MailboxHoldStatus](mailboxholdstatus.md)
  
## <a name="text-value"></a>Текстовое значение

Текстовое значение элемента **Status** — состояние удержания почтового ящика. Элемент **Status** может иметь значения в следующем списке. 
  
> NotOnHold — почтовый ящик не находится на удержании.
    
> Ожидание — почтовый ящик находится в ожидании, если его помещают или выпускают на удержание. 
    
> OnHold . Удержание было успешно применено к почтовому ящику. 
    
> PartialHold . Удержание было успешно применено к некоторым почтовым ящикам, но не для всех почтовых ящиков.
    
> Не удалось . Удержание не удалось применить к почтовому ящику.
    
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
   

