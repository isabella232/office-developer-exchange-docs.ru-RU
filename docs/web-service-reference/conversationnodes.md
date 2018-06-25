---
title: ConversationNodes
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 5c8a35b8-a940-4b3e-8768-9ba95766fd79
description: Элемент ConversationNodes указывает коллекцию узлов беседы.
ms.openlocfilehash: 62ec061f6d03abb9db7e511722e5570e70d65772
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761830"
---
# <a name="conversationnodes"></a><span data-ttu-id="718d9-103">ConversationNodes</span><span class="sxs-lookup"><span data-stu-id="718d9-103">ConversationNodes</span></span>

<span data-ttu-id="718d9-104">Элемент **ConversationNodes** указывает коллекцию узлов беседы.</span><span class="sxs-lookup"><span data-stu-id="718d9-104">The **ConversationNodes** element specifies a collection of conversation nodes.</span></span> 
  
```XML
<ConversationNodes>
    <ConversationNode></ConversationNode>
</ConversationNodes>
```

 <span data-ttu-id="718d9-105">**ArrayOfConversationNodesType**</span><span class="sxs-lookup"><span data-stu-id="718d9-105">**ArrayOfConversationNodesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="718d9-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="718d9-106">Attributes and elements</span></span>

<span data-ttu-id="718d9-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="718d9-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="718d9-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="718d9-108">Attributes</span></span>

<span data-ttu-id="718d9-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="718d9-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="718d9-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="718d9-110">Child elements</span></span>

|<span data-ttu-id="718d9-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="718d9-111">**Element**</span></span>|<span data-ttu-id="718d9-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="718d9-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="718d9-113">ConversationNode</span><span class="sxs-lookup"><span data-stu-id="718d9-113">ConversationNode</span></span>](conversationnode.md) <br/> |<span data-ttu-id="718d9-114">Определяет узел в беседе.</span><span class="sxs-lookup"><span data-stu-id="718d9-114">Specifies a node in a conversation.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="718d9-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="718d9-115">Parent elements</span></span>

|<span data-ttu-id="718d9-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="718d9-116">**Element**</span></span>|<span data-ttu-id="718d9-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="718d9-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="718d9-118">Беседы (ConversationResponseType)</span><span class="sxs-lookup"><span data-stu-id="718d9-118">Conversation (ConversationResponseType)</span></span>](conversation-conversationresponsetype.md) <br/> |<span data-ttu-id="718d9-119">Представляет один беседы, возвращаемых в ответе **GetConversationItems** .</span><span class="sxs-lookup"><span data-stu-id="718d9-119">Represents a single conversation returned in a **GetConversationItems** response.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="718d9-120">Замечания</span><span class="sxs-lookup"><span data-stu-id="718d9-120">Remarks</span></span>

<span data-ttu-id="718d9-121">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="718d9-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="718d9-122">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="718d9-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="718d9-123">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="718d9-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="718d9-124">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="718d9-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="718d9-125">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="718d9-125">Schema Name</span></span>  <br/> |<span data-ttu-id="718d9-126">Схема типа</span><span class="sxs-lookup"><span data-stu-id="718d9-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="718d9-127">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="718d9-127">Validation File</span></span>  <br/> |<span data-ttu-id="718d9-128">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="718d9-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="718d9-129">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="718d9-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="718d9-130">См. также</span><span class="sxs-lookup"><span data-stu-id="718d9-130">See also</span></span>



- [<span data-ttu-id="718d9-131">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="718d9-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

