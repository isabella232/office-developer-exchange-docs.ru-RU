---
title: Состояние (HoldStatusType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: fee3f1f9-e868-49fa-a554-7ff096964718
description: Элемент Status указывает состояние удержания почтового ящика.
ms.openlocfilehash: c40dc865d2b305ac86fa40d536e2d516a14260ab
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19835579"
---
# <a name="status-holdstatustype"></a>Состояние (HoldStatusType)

Элемент **Status** указывает состояние удержания почтового ящика. 
  
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

Текстовое значение элемента **состояние** — это состояние удержания почтового ящика. Элемент **Status** может иметь значения в приведенном ниже списке. 
  
> NotOnHold - почтового ящика не на удержание.
    
> Ожидание - почтовый ящик ожидает выполнившим или выпущен на удержание. 
    
> Удержании - удержание успешно применена к почтовому ящику. 
    
> PartialHold - удержание успешно применена некоторые почтовые ящики, но не ко всем почтовым ящикам.
    
> Ошибка — удержания не удается применить к почтовому ящику.
    
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
   

