---
title: глобалфлагстатус
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GlobalFlagStatus
api_type:
- schema
ms.assetid: 3ba300f3-3355-4cab-9e77-0dcc2902e712
description: Элемент Глобалфлагстатус содержит сводный статус флага для всех элементов бесед в почтовом ящике.
ms.openlocfilehash: 0c560c065463b8b619f96ecef73d1120b216ca35
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833713"
---
# <a name="globalflagstatus"></a><span data-ttu-id="d8161-103">глобалфлагстатус</span><span class="sxs-lookup"><span data-stu-id="d8161-103">GlobalFlagStatus</span></span>

<span data-ttu-id="d8161-104">Элемент **глобалфлагстатус** содержит сводный статус флага для всех элементов бесед в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="d8161-104">The **GlobalFlagStatus** element contains the aggregated flag status for all conversation items in a mailbox.</span></span> 
  
[<span data-ttu-id="d8161-105">финдконверсатионреспонсе</span><span class="sxs-lookup"><span data-stu-id="d8161-105">FindConversationResponse</span></span>](findconversationresponse.md)
  
[<span data-ttu-id="d8161-106">Conversations</span><span class="sxs-lookup"><span data-stu-id="d8161-106">Conversations</span></span>](conversations-ex15websvcsotherref.md)
  
[<span data-ttu-id="d8161-107">Беседы (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="d8161-107">Conversation (ConversationType)</span></span>](conversation-conversationtype.md)
  
[<span data-ttu-id="d8161-108">глобалфлагстатус</span><span class="sxs-lookup"><span data-stu-id="d8161-108">GlobalFlagStatus</span></span>](globalflagstatus.md)
  
```XML
<GlobalFlagStatus> NotFlagged | Flagged | Complete </GlobalFlagStatus>
```

 <span data-ttu-id="d8161-109">**флагстатустипе**</span><span class="sxs-lookup"><span data-stu-id="d8161-109">**FlagStatusType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d8161-110">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="d8161-110">Attributes and elements</span></span>

<span data-ttu-id="d8161-111">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="d8161-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d8161-112">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="d8161-112">Attributes</span></span>

<span data-ttu-id="d8161-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="d8161-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d8161-114">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="d8161-114">Child elements</span></span>

<span data-ttu-id="d8161-115">Нет.</span><span class="sxs-lookup"><span data-stu-id="d8161-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="d8161-116">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="d8161-116">Parent elements</span></span>

|<span data-ttu-id="d8161-117">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="d8161-117">**Element**</span></span>|<span data-ttu-id="d8161-118">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d8161-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d8161-119">Беседы (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="d8161-119">Conversation (ConversationType)</span></span>](conversation-conversationtype.md) <br/> |<span data-ttu-id="d8161-120">Представляет одну беседу.</span><span class="sxs-lookup"><span data-stu-id="d8161-120">Represents a single conversation.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="d8161-121">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="d8161-121">Text value</span></span>

<span data-ttu-id="d8161-122">Текстовое значение элемента **глобалфлагстатус** — это сводный статус флага для элементов беседы в текущей папке.</span><span class="sxs-lookup"><span data-stu-id="d8161-122">The text value of the **GlobalFlagStatus** element is the aggregated flag status for conversation items in the current folder.</span></span> <span data-ttu-id="d8161-123">Ниже приведены возможные текстовые значения.</span><span class="sxs-lookup"><span data-stu-id="d8161-123">The following are the possible text values:</span></span> 
  
- <span data-ttu-id="d8161-124">**Нотфлагжед** — указывает состояние "без отметки".</span><span class="sxs-lookup"><span data-stu-id="d8161-124">**NotFlagged** - Indicates the not-flagged status.</span></span> 
    
- <span data-ttu-id="d8161-125">**Отмечено** — указывает на состояние помечено.</span><span class="sxs-lookup"><span data-stu-id="d8161-125">**Flagged** - Indicates the flagged status.</span></span> 
    
- <span data-ttu-id="d8161-126">**Complete** — полный статус флага.</span><span class="sxs-lookup"><span data-stu-id="d8161-126">**Complete** - Indicates the complete flag status.</span></span> 
    
## <a name="remarks"></a><span data-ttu-id="d8161-127">Примечания</span><span class="sxs-lookup"><span data-stu-id="d8161-127">Remarks</span></span>

<span data-ttu-id="d8161-128">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.Этот элемент появился в Exchange Server 2010 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="d8161-128">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d8161-129">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="d8161-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d8161-130">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="d8161-130">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d8161-131">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="d8161-131">Schema name</span></span>  <br/> |<span data-ttu-id="d8161-132">Схема Types</span><span class="sxs-lookup"><span data-stu-id="d8161-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="d8161-133">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="d8161-133">Validation file</span></span>  <br/> |<span data-ttu-id="d8161-134">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="d8161-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d8161-135">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="d8161-135">Can be empty</span></span>  <br/> |<span data-ttu-id="d8161-136">False</span><span class="sxs-lookup"><span data-stu-id="d8161-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d8161-137">См. также</span><span class="sxs-lookup"><span data-stu-id="d8161-137">See also</span></span>



[<span data-ttu-id="d8161-138">FindConversation Operation</span><span class="sxs-lookup"><span data-stu-id="d8161-138">FindConversation operation</span></span>](findconversation-operation.md)
  
[<span data-ttu-id="d8161-139">Операция ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="d8161-139">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)


[<span data-ttu-id="d8161-140">Conversations in EWS</span><span class="sxs-lookup"><span data-stu-id="d8161-140">Conversations in EWS</span></span>](http://msdn.microsoft.com/library/91e64629-db6c-4c94-9dcb-d386232e8467%28Office.15%29.aspx)

