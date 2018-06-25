---
title: GlobalUniqueSenders
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GlobalUniqueSenders
api_type:
- schema
ms.assetid: 6bd9e9cb-19c8-45af-b211-dfb8a6003b1b
description: Элемент GlobalUniqueSender содержит список всех отправителей беседы элементов в почтовом ящике.
ms.openlocfilehash: 72dec056880c41ac9e79235dddb3c82102580a31
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833751"
---
# <a name="globaluniquesenders"></a><span data-ttu-id="d3882-103">GlobalUniqueSenders</span><span class="sxs-lookup"><span data-stu-id="d3882-103">GlobalUniqueSenders</span></span>

<span data-ttu-id="d3882-104">Элемент **GlobalUniqueSender** содержит список всех отправителей беседы элементов в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="d3882-104">The **GlobalUniqueSender** element contains a list of all the senders of conversation items in the mailbox.</span></span> 
  
[<span data-ttu-id="d3882-105">FindConversationResponse</span><span class="sxs-lookup"><span data-stu-id="d3882-105">FindConversationResponse</span></span>](findconversationresponse.md)
  
[<span data-ttu-id="d3882-106">Conversations</span><span class="sxs-lookup"><span data-stu-id="d3882-106">Conversations</span></span>](conversations-ex15websvcsotherref.md)
  
[<span data-ttu-id="d3882-107">Беседы (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="d3882-107">Conversation (ConversationType)</span></span>](conversation-conversationtype.md)
  
[<span data-ttu-id="d3882-108">GlobalUniqueSenders</span><span class="sxs-lookup"><span data-stu-id="d3882-108">GlobalUniqueSenders</span></span>](globaluniquesenders.md)
  
```XML
<GlobalUniqueSender>
   <String/>
</GlobalUniqueSender>
```

 <span data-ttu-id="d3882-109">**ArrayOfStringsType**</span><span class="sxs-lookup"><span data-stu-id="d3882-109">**ArrayOfStringsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d3882-110">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="d3882-110">Attributes and elements</span></span>

<span data-ttu-id="d3882-111">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="d3882-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d3882-112">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="d3882-112">Attributes</span></span>

<span data-ttu-id="d3882-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="d3882-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d3882-114">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="d3882-114">Child elements</span></span>

|<span data-ttu-id="d3882-115">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="d3882-115">**Element**</span></span>|<span data-ttu-id="d3882-116">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d3882-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d3882-117">Строка</span><span class="sxs-lookup"><span data-stu-id="d3882-117">String</span></span>](string.md) <br/> |<span data-ttu-id="d3882-118">Содержит отправителя разговора.</span><span class="sxs-lookup"><span data-stu-id="d3882-118">Contains a single conversation sender.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d3882-119">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="d3882-119">Parent elements</span></span>

|<span data-ttu-id="d3882-120">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="d3882-120">**Element**</span></span>|<span data-ttu-id="d3882-121">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d3882-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d3882-122">Беседы (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="d3882-122">Conversation (ConversationType)</span></span>](conversation-conversationtype.md) <br/> |<span data-ttu-id="d3882-123">Представляет одну беседу.</span><span class="sxs-lookup"><span data-stu-id="d3882-123">Represents a single conversation.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="d3882-124">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="d3882-124">Text value</span></span>

<span data-ttu-id="d3882-125">Нет.</span><span class="sxs-lookup"><span data-stu-id="d3882-125">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="d3882-126">Замечания</span><span class="sxs-lookup"><span data-stu-id="d3882-126">Remarks</span></span>

<span data-ttu-id="d3882-127">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.Этот элемент появился в Exchange Server 2010 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="d3882-127">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d3882-128">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="d3882-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d3882-129">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="d3882-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d3882-130">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="d3882-130">Schema name</span></span>  <br/> |<span data-ttu-id="d3882-131">Схема Types</span><span class="sxs-lookup"><span data-stu-id="d3882-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="d3882-132">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="d3882-132">Validation file</span></span>  <br/> |<span data-ttu-id="d3882-133">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="d3882-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d3882-134">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="d3882-134">Can be empty</span></span>  <br/> |<span data-ttu-id="d3882-135">False</span><span class="sxs-lookup"><span data-stu-id="d3882-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d3882-136">См. также</span><span class="sxs-lookup"><span data-stu-id="d3882-136">See also</span></span>



[<span data-ttu-id="d3882-137">FindConversation Operation</span><span class="sxs-lookup"><span data-stu-id="d3882-137">FindConversation operation</span></span>](findconversation-operation.md)
  
[<span data-ttu-id="d3882-138">Операция ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="d3882-138">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)


[<span data-ttu-id="d3882-139">Conversations in EWS</span><span class="sxs-lookup"><span data-stu-id="d3882-139">Conversations in EWS</span></span>](http://msdn.microsoft.com/library/91e64629-db6c-4c94-9dcb-d386232e8467%28Office.15%29.aspx)

