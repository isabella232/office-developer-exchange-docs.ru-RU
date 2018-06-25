---
title: GlobalItemClasses
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GlobalItemClasses
api_type:
- schema
ms.assetid: 72634700-6d75-44c0-80b7-8c31743c04d6
description: Элемент GlobalItemClasses содержит список классов элементов, представляющий все классы элементов беседы элементов в почтовом ящике.
ms.openlocfilehash: a8f947d37c1335f1eaba5550a2b3a0aece0246ee
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833735"
---
# <a name="globalitemclasses"></a><span data-ttu-id="7d376-103">GlobalItemClasses</span><span class="sxs-lookup"><span data-stu-id="7d376-103">GlobalItemClasses</span></span>

<span data-ttu-id="7d376-104">Элемент **GlobalItemClasses** содержит список классов элементов, представляющий все классы элементов беседы элементов в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="7d376-104">The **GlobalItemClasses** element contains a list of item classes that represents all the item classes of the conversation items in a mailbox.</span></span> 
  
[<span data-ttu-id="7d376-105">FindConversationResponse</span><span class="sxs-lookup"><span data-stu-id="7d376-105">FindConversationResponse</span></span>](findconversationresponse.md)
  
[<span data-ttu-id="7d376-106">Conversations</span><span class="sxs-lookup"><span data-stu-id="7d376-106">Conversations</span></span>](conversations-ex15websvcsotherref.md)
  
[<span data-ttu-id="7d376-107">Беседы (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="7d376-107">Conversation (ConversationType)</span></span>](conversation-conversationtype.md)
  
[<span data-ttu-id="7d376-108">GlobalItemClasses</span><span class="sxs-lookup"><span data-stu-id="7d376-108">GlobalItemClasses</span></span>](globalitemclasses.md)
  
```XML
<GlobalItemClasses>
    <String/>
</GlobalItemClasses>
```

 <span data-ttu-id="7d376-109">**ArrayOfItemClassType**</span><span class="sxs-lookup"><span data-stu-id="7d376-109">**ArrayOfItemClassType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7d376-110">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="7d376-110">Attributes and elements</span></span>

<span data-ttu-id="7d376-111">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="7d376-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7d376-112">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="7d376-112">Attributes</span></span>

<span data-ttu-id="7d376-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="7d376-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7d376-114">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="7d376-114">Child elements</span></span>

|<span data-ttu-id="7d376-115">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="7d376-115">**Element**</span></span>|<span data-ttu-id="7d376-116">**Описание**</span><span class="sxs-lookup"><span data-stu-id="7d376-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7d376-117">ItemClass</span><span class="sxs-lookup"><span data-stu-id="7d376-117">ItemClass</span></span>](itemclass.md) <br/> |<span data-ttu-id="7d376-118">Представляет класс сообщения элемента.</span><span class="sxs-lookup"><span data-stu-id="7d376-118">Represents the message class of an item.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="7d376-119">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="7d376-119">Parent elements</span></span>

|<span data-ttu-id="7d376-120">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="7d376-120">**Element**</span></span>|<span data-ttu-id="7d376-121">**Описание**</span><span class="sxs-lookup"><span data-stu-id="7d376-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7d376-122">Беседы (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="7d376-122">Conversation (ConversationType)</span></span>](conversation-conversationtype.md) <br/> |<span data-ttu-id="7d376-123">Представляет одну беседу.</span><span class="sxs-lookup"><span data-stu-id="7d376-123">Represents a single conversation.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="7d376-124">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="7d376-124">Text value</span></span>

<span data-ttu-id="7d376-125">Нет.</span><span class="sxs-lookup"><span data-stu-id="7d376-125">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="7d376-126">Замечания</span><span class="sxs-lookup"><span data-stu-id="7d376-126">Remarks</span></span>

<span data-ttu-id="7d376-127">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.Этот элемент появился в Exchange Server 2010 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="7d376-127">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7d376-128">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="7d376-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7d376-129">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="7d376-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="7d376-130">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="7d376-130">Schema name</span></span>  <br/> |<span data-ttu-id="7d376-131">Схема Types</span><span class="sxs-lookup"><span data-stu-id="7d376-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="7d376-132">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="7d376-132">Validation file</span></span>  <br/> |<span data-ttu-id="7d376-133">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="7d376-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="7d376-134">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="7d376-134">Can be empty</span></span>  <br/> |<span data-ttu-id="7d376-135">False</span><span class="sxs-lookup"><span data-stu-id="7d376-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7d376-136">См. также</span><span class="sxs-lookup"><span data-stu-id="7d376-136">See also</span></span>



[<span data-ttu-id="7d376-137">FindConversation Operation</span><span class="sxs-lookup"><span data-stu-id="7d376-137">FindConversation operation</span></span>](findconversation-operation.md)
  
[<span data-ttu-id="7d376-138">Операция ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="7d376-138">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)


[<span data-ttu-id="7d376-139">Conversations in EWS</span><span class="sxs-lookup"><span data-stu-id="7d376-139">Conversations in EWS</span></span>](http://msdn.microsoft.com/library/91e64629-db6c-4c94-9dcb-d386232e8467%28Office.15%29.aspx)

