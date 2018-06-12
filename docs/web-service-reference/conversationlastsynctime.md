---
title: ConversationLastSyncTime
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ConversationLastSyncTime
api_type:
- schema
ms.assetid: 90f8f9e3-5fc6-4a6a-bdfb-fc91fa51f8a2
description: Элемент ConversationLastSyncTime содержит дату и время последнего синхронизирована беседы. Этот элемент должен присутствовать при попытке удаления всех элементов в беседе, которые были получены до заданного времени.
ms.openlocfilehash: 3b086d69ac0ef307059df4902e65f796c63733d1
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761819"
---
# <a name="conversationlastsynctime"></a>ConversationLastSyncTime

Элемент **ConversationLastSyncTime** содержит дату и время последнего синхронизирована беседы. Этот элемент должен присутствовать при попытке удаления всех элементов в беседе, которые были получены до заданного времени. 
  
[ApplyConversationAction](applyconversationaction.md)
  
[ConversationActions](conversationactions.md)
  
[ConversationAction](conversationaction.md)
  
[ConversationLastSyncTime](conversationlastsynctime.md)
  
```XML
<ConversationLastSyncTime/>
```

 **xs: DateTime**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[ConversationAction](conversationaction.md) <br/> |Содержит одно действие должен применяться к разговора.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение **ConversationLastSyncTime** указывает время последнего синхронизации беседу. 
  
## <a name="remarks"></a>Замечания

Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.Этот элемент появился в Exchange Server 2010 с пакетом обновления 1 (SP1).
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операция ApplyConversationAction](applyconversationaction-operation.md)


- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

