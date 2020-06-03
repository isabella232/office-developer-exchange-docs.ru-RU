---
title: Состояние (Холдстатустипе)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: fee3f1f9-e868-49fa-a554-7ff096964718
description: Элемент Status указывает состояние удержания для почтового ящика.
ms.openlocfilehash: cecfdfaf67b00b6f8cf02188e7a4df7062a732e4
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459989"
---
# <a name="status-holdstatustype"></a>Состояние (Холдстатустипе)

Элемент **Status** указывает состояние удержания для почтового ящика. 
  
```XML
<Status> NotOnHold | Pending | OnHold | PartialHold | Failed </Status>
```

 **холдстатустипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

Отсутствуют.
  
### <a name="parent-elements"></a>Родительские элементы

[маилбоксхолдстатус](mailboxholdstatus.md)
  
## <a name="text-value"></a>Текстовое значение

Текстовое значение элемента **Status** — это состояние удержания почтового ящика. Элемент **Status** может иметь значения из следующего списка. 
  
> Нотонхолд — почтовый ящик не находится на удержании.
    
> Ожидание — почтовый ящик находится в состоянии ожидания размещения или освобождения. 
    
> Onhold — удержание успешно применено к почтовому ящику. 
    
> Партиалхолд — удержание успешно применено к некоторым почтовым ящикам, но не ко всем почтовым ящикам.
    
> Сбой: не удалось применить удержание к почтовому ящику.
    
## <a name="remarks"></a>Примечания

Этот элемент появился в Exchange Server 2013.
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> ||
   

