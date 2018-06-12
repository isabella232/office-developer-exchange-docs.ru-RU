---
title: FlagStatus
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FlagStatus
api_type:
- schema
ms.assetid: d5907ec5-3a60-4d83-bf85-406c54f95eb7
description: Элемент FlagStatus содержит объединенные флаг состояния для элементов беседы в текущую папку.
ms.openlocfilehash: 59e071cbd402c49f4dcc4370059883f3f45409ae
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762612"
---
# <a name="flagstatus"></a><span data-ttu-id="5d6ac-103">FlagStatus</span><span class="sxs-lookup"><span data-stu-id="5d6ac-103">FlagStatus</span></span>

<span data-ttu-id="5d6ac-104">Элемент **FlagStatus** содержит объединенные флаг состояния для элементов беседы в текущую папку.</span><span class="sxs-lookup"><span data-stu-id="5d6ac-104">The **FlagStatus** element contains the aggregated flag status for conversation items in the current folder.</span></span> 
  
[<span data-ttu-id="5d6ac-105">FindConversationResponse</span><span class="sxs-lookup"><span data-stu-id="5d6ac-105">FindConversationResponse</span></span>](findconversationresponse.md)
  
[<span data-ttu-id="5d6ac-106">Conversations</span><span class="sxs-lookup"><span data-stu-id="5d6ac-106">Conversations</span></span>](conversations-ex15websvcsotherref.md)
  
[<span data-ttu-id="5d6ac-107">Беседы (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="5d6ac-107">Conversation (ConversationType)</span></span>](conversation-conversationtype.md)
  
[<span data-ttu-id="5d6ac-108">FlagStatus</span><span class="sxs-lookup"><span data-stu-id="5d6ac-108">FlagStatus</span></span>](flagstatus.md)
  
```XML
<FlagStatus> NotFlagged | Flagged | Complete </FlagStatus>
```

 <span data-ttu-id="5d6ac-109">**FlagStatusType**</span><span class="sxs-lookup"><span data-stu-id="5d6ac-109">**FlagStatusType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5d6ac-110">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="5d6ac-110">Attributes and elements</span></span>

<span data-ttu-id="5d6ac-111">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="5d6ac-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5d6ac-112">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="5d6ac-112">Attributes</span></span>

<span data-ttu-id="5d6ac-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="5d6ac-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5d6ac-114">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="5d6ac-114">Child elements</span></span>

<span data-ttu-id="5d6ac-115">Нет.</span><span class="sxs-lookup"><span data-stu-id="5d6ac-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="5d6ac-116">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="5d6ac-116">Parent elements</span></span>

|<span data-ttu-id="5d6ac-117">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="5d6ac-117">**Element**</span></span>|<span data-ttu-id="5d6ac-118">**Описание**</span><span class="sxs-lookup"><span data-stu-id="5d6ac-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5d6ac-119">Беседы (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="5d6ac-119">Conversation (ConversationType)</span></span>](conversation-conversationtype.md) <br/> |<span data-ttu-id="5d6ac-120">Представляет одну беседу.</span><span class="sxs-lookup"><span data-stu-id="5d6ac-120">Represents a single conversation.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="5d6ac-121">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="5d6ac-121">Text value</span></span>

<span data-ttu-id="5d6ac-122">Текстовое значение элемента **FlagStatus** сводный флаг статус используется для элементов беседы в текущую папку.</span><span class="sxs-lookup"><span data-stu-id="5d6ac-122">The text value of the **FlagStatus** element is the aggregated flag status for conversation items in the current folder.</span></span> <span data-ttu-id="5d6ac-123">Ниже приведены возможные текстовые значения.</span><span class="sxs-lookup"><span data-stu-id="5d6ac-123">The following are the possible text values:</span></span> 
  
- <span data-ttu-id="5d6ac-124">**NotFlagged** - указывает состояние не отмеченные.</span><span class="sxs-lookup"><span data-stu-id="5d6ac-124">**NotFlagged** - Indicates the not-flagged status.</span></span> 
    
- <span data-ttu-id="5d6ac-125">**Пометкой** - указывает отмеченного состояния.</span><span class="sxs-lookup"><span data-stu-id="5d6ac-125">**Flagged** - Indicates the flagged status.</span></span> 
    
- <span data-ttu-id="5d6ac-126">**Полная** - указывает состояние флага завершена.</span><span class="sxs-lookup"><span data-stu-id="5d6ac-126">**Complete** - Indicates the complete flag status.</span></span> 
    
## <a name="remarks"></a><span data-ttu-id="5d6ac-127">Замечания</span><span class="sxs-lookup"><span data-stu-id="5d6ac-127">Remarks</span></span>

<span data-ttu-id="5d6ac-128">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.Этот элемент появился в Exchange Server 2010 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="5d6ac-128">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5d6ac-129">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="5d6ac-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5d6ac-130">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="5d6ac-130">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="5d6ac-131">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="5d6ac-131">Schema name</span></span>  <br/> |<span data-ttu-id="5d6ac-132">Схема Types</span><span class="sxs-lookup"><span data-stu-id="5d6ac-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="5d6ac-133">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="5d6ac-133">Validation file</span></span>  <br/> |<span data-ttu-id="5d6ac-134">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="5d6ac-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="5d6ac-135">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="5d6ac-135">Can be empty</span></span>  <br/> |<span data-ttu-id="5d6ac-136">False</span><span class="sxs-lookup"><span data-stu-id="5d6ac-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="5d6ac-137">См. также</span><span class="sxs-lookup"><span data-stu-id="5d6ac-137">See also</span></span>



[<span data-ttu-id="5d6ac-138">FindConversation Operation</span><span class="sxs-lookup"><span data-stu-id="5d6ac-138">FindConversation operation</span></span>](findconversation-operation.md)
  
[<span data-ttu-id="5d6ac-139">Операция ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="5d6ac-139">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)


[<span data-ttu-id="5d6ac-140">Conversations in EWS</span><span class="sxs-lookup"><span data-stu-id="5d6ac-140">Conversations in EWS</span></span>](http://msdn.microsoft.com/library/91e64629-db6c-4c94-9dcb-d386232e8467%28Office.15%29.aspx)

