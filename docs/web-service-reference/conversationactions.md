---
title: ConversationActions
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ConversationActions
api_type:
- schema
ms.assetid: 3d6c663d-4bd9-4eec-b95a-cd683f592672
description: Элемент ConversationActions содержит коллекцию бесед и действий для применения к ним.
ms.openlocfilehash: 3dff7ff66f758f1cd2eb3cd7b8126294d2799fc0
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761815"
---
# <a name="conversationactions"></a>ConversationActions

Элемент **ConversationActions** содержит коллекцию бесед и действий для применения к ним. 
  
[ApplyConversationAction](applyconversationaction.md)
  
[ConversationActions](conversationactions.md)
  
```XML
<ConversationActions>
   <ConversationAction/>
</ConversationActions>
```

 **NonEmptyArrayOfApplyConversationActionType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[ConversationAction](conversationaction.md) <br/> |Содержит одно действие должен применяться к разговора.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[ApplyConversationAction](applyconversationaction.md) <br/> |Определяет запрос для выполнения определенных действий к элементам в беседе.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Нет.
  
## <a name="remarks"></a>Замечания

Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.Этот элемент появился в Exchange Server 2010 с пакетом обновления 1 (SP1).
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операция ApplyConversationAction](applyconversationaction-operation.md)

