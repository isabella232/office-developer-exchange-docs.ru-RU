---
title: GlobalImportance
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GlobalImportance
api_type:
- schema
ms.assetid: 8bcec699-e771-4f38-b7d9-61f324af1b4e
description: Элемент GlobalImportance содержит объединенные важности для всех элементов беседы в почтовом ящике.
ms.openlocfilehash: c9cdcf20fd3e6eca9ab501cbc747544a4d7b7ded
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833731"
---
# <a name="globalimportance"></a><span data-ttu-id="022e0-103">GlobalImportance</span><span class="sxs-lookup"><span data-stu-id="022e0-103">GlobalImportance</span></span>

<span data-ttu-id="022e0-104">Элемент **GlobalImportance** содержит объединенные важности для всех элементов беседы в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="022e0-104">The **GlobalImportance** element contains the aggregated importance for all conversation items in a mailbox.</span></span> 
  
[<span data-ttu-id="022e0-105">FindConversationResponse</span><span class="sxs-lookup"><span data-stu-id="022e0-105">FindConversationResponse</span></span>](findconversationresponse.md)
  
[<span data-ttu-id="022e0-106">Conversations</span><span class="sxs-lookup"><span data-stu-id="022e0-106">Conversations</span></span>](conversations-ex15websvcsotherref.md)
  
[<span data-ttu-id="022e0-107">Беседы (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="022e0-107">Conversation (ConversationType)</span></span>](conversation-conversationtype.md)
  
[<span data-ttu-id="022e0-108">GlobalImportance</span><span class="sxs-lookup"><span data-stu-id="022e0-108">GlobalImportance</span></span>](globalimportance.md)
  
```XML
<GlobalImportance> Low | Normal | High </GlobalImportance>
```

 <span data-ttu-id="022e0-109">**ImportanceChoicesType**</span><span class="sxs-lookup"><span data-stu-id="022e0-109">**ImportanceChoicesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="022e0-110">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="022e0-110">Attributes and elements</span></span>

<span data-ttu-id="022e0-111">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="022e0-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="022e0-112">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="022e0-112">Attributes</span></span>

<span data-ttu-id="022e0-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="022e0-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="022e0-114">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="022e0-114">Child elements</span></span>

<span data-ttu-id="022e0-115">Нет.</span><span class="sxs-lookup"><span data-stu-id="022e0-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="022e0-116">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="022e0-116">Parent elements</span></span>

|<span data-ttu-id="022e0-117">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="022e0-117">**Element**</span></span>|<span data-ttu-id="022e0-118">**Описание**</span><span class="sxs-lookup"><span data-stu-id="022e0-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="022e0-119">Беседы (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="022e0-119">Conversation (ConversationType)</span></span>](conversation-conversationtype.md) <br/> |<span data-ttu-id="022e0-120">Представляет одну беседу.</span><span class="sxs-lookup"><span data-stu-id="022e0-120">Represents a single conversation.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="022e0-121">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="022e0-121">Text value</span></span>

<span data-ttu-id="022e0-122">Текстовое значение является обязательным.</span><span class="sxs-lookup"><span data-stu-id="022e0-122">A text value is required.</span></span> <span data-ttu-id="022e0-123">Ниже приведены возможные значения для этого элемента:</span><span class="sxs-lookup"><span data-stu-id="022e0-123">The following are the possible values for this element:</span></span>
  
- <span data-ttu-id="022e0-124">Low</span><span class="sxs-lookup"><span data-stu-id="022e0-124">Low</span></span>
    
- <span data-ttu-id="022e0-125">Обычный</span><span class="sxs-lookup"><span data-stu-id="022e0-125">Normal</span></span>
    
- <span data-ttu-id="022e0-126">High</span><span class="sxs-lookup"><span data-stu-id="022e0-126">High</span></span>
    
## <a name="remarks"></a><span data-ttu-id="022e0-127">Замечания</span><span class="sxs-lookup"><span data-stu-id="022e0-127">Remarks</span></span>

<span data-ttu-id="022e0-128">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.Этот элемент появился в Exchange Server 2010 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="022e0-128">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="022e0-129">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="022e0-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="022e0-130">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="022e0-130">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="022e0-131">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="022e0-131">Schema name</span></span>  <br/> |<span data-ttu-id="022e0-132">Схема Types</span><span class="sxs-lookup"><span data-stu-id="022e0-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="022e0-133">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="022e0-133">Validation file</span></span>  <br/> |<span data-ttu-id="022e0-134">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="022e0-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="022e0-135">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="022e0-135">Can be empty</span></span>  <br/> |<span data-ttu-id="022e0-136">False</span><span class="sxs-lookup"><span data-stu-id="022e0-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="022e0-137">См. также</span><span class="sxs-lookup"><span data-stu-id="022e0-137">See also</span></span>



[<span data-ttu-id="022e0-138">FindConversation Operation</span><span class="sxs-lookup"><span data-stu-id="022e0-138">FindConversation operation</span></span>](findconversation-operation.md)
  
[<span data-ttu-id="022e0-139">Операция ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="022e0-139">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)


[<span data-ttu-id="022e0-140">Conversations in EWS</span><span class="sxs-lookup"><span data-stu-id="022e0-140">Conversations in EWS</span></span>](http://msdn.microsoft.com/library/91e64629-db6c-4c94-9dcb-d386232e8467%28Office.15%29.aspx)

