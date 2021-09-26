---
title: ActionType (HoldActionType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: f50449b9-e73b-43c5-af96-6433bf434dce
description: Элемент ActionType указывает тип действия для удержания.
ms.openlocfilehash: 30028da4df2a53a4cd0066823872de5e586020f1
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59546842"
---
# <a name="actiontype-holdactiontype"></a>ActionType (HoldActionType)

Элемент **ActionType** указывает тип действия для удержания. 
  
```XML
<ActionType> Create | Update | Remove </ActionType>
```

 **HoldActionType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

[SetHoldOnMailboxes](setholdonmailboxes.md)
  
## <a name="text-value"></a>Текстовое значение

Текстовое значение элемента **ActionType** — это тип удержания на почтовом ящике. Текстовое значение **Create** указывает на создание удержания почтовых ящиков. Текстовое значение **Update** указывает, что удержание почтовых ящиков будет обновлено. Текстовое значение **Remove** указывает, что удержание почтового ящика будет удалено. 
  
## <a name="remarks"></a>Заметки

Этот элемент появился в Exchange Server 2013.
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |false  <br/> |
   

