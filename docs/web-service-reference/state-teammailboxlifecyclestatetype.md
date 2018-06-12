---
title: Состояние (TeamMailboxLifecycleStateType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 3b1bc531-6988-41c3-9aad-3f5ad5b732a9
description: Элемент состояния содержит состояния жизненного цикла, заданное для почтового ящика сайта.
ms.openlocfilehash: accd70d36cc34e7364387b98a2e94c56b91f012f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19835571"
---
# <a name="state-teammailboxlifecyclestatetype"></a>Состояние (TeamMailboxLifecycleStateType)

Элемент **состояния** содержит состояния жизненного цикла, заданное для почтового ящика сайта. 
  
```XML
<State> Active | Closed | Unlinked | PendingDelete </State>
```

**TeamMailboxLifecycleStateType**

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

[SetTeamMailbox](setteammailbox.md)
  
## <a name="text-value"></a>Текстовое значение

Текстовое значение элемента **состояние** является состояния жизненного цикла, заданное для почтового ящика сайта. Текстовое значение **Active** указывает почтовый ящик сайта в активном использовании. Текстовое значение **Закрыто** указывает, что почтовый ящик сайта был закрыт и не находится в активном использовании. Текстовое значение **Несвязанные** указывает, что почтовый ящик сайта не связаны в среде совместной работы в Интернете. Значения **Active**, **Закрыто**и **PendingDelete** являются взаимоисключающими, но значение **Несвязанные** не взаимно без учета расходов на другие значения. Текстовое значение **PendingDelete** указывает, что почтовый ящик сайта — это процесс удаления. Почтового ящика сайта должен быть закрыты перед его можно задать как **PendingDelete**.
  
## <a name="remarks"></a>Замечания

Этот элемент появился в Exchange Server 2013.
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> ||
   

