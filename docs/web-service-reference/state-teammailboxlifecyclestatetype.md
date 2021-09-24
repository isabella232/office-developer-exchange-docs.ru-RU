---
title: State (TeamMailboxLifecycleStateType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 3b1bc531-6988-41c3-9aad-3f5ad5b732a9
description: Элемент State содержит состояние жизненного цикла, за набором на почтовом ящике сайта.
ms.openlocfilehash: 5189ee8573fd33d2265fd60c47bb40d17b16b8fe
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59538970"
---
# <a name="state-teammailboxlifecyclestatetype"></a>State (TeamMailboxLifecycleStateType)

Элемент **State** содержит состояние жизненного цикла, за набором на почтовом ящике сайта. 
  
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

Текстовое значение элемента **State** — это состояние жизненного цикла, за набором на почтовом ящике сайта. Текстовое значение **Active** указывает на активное использование почтового ящика сайта. Текстовое значение **Closed** указывает, что почтовый ящик сайта закрыт и не используется. Текстовое значение **Unlinked указывает,** что почтовый ящик сайта не связан с веб-средой совместной работы. Значения **Active,** **Closed** и **PendingDelete** являются взаимоисключающими, но значение **Unlinked** не является взаимоисключающими другими значениями. Текстовое значение **PendingDelete** указывает, что почтовый ящик сайта находится в ожидании удаления. Почтовый ящик сайта должен быть закрыт, прежде чем его можно задать **как PendingDelete.**
  
## <a name="remarks"></a>Заметки

Этот элемент появился в Exchange Server 2013.
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> ||
   

