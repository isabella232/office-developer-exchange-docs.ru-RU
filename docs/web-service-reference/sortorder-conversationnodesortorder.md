---
title: SortOrder (ConversationNodeSortOrder)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f9c4295c-8089-4533-b92f-2051eae9afeb
description: Элемент SortOrder определяет порядок сортировки для результата запроса GetConversationItems.
ms.openlocfilehash: 397aead62d32e72f991af783bff02e79a6e4b0fb
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19835520"
---
# <a name="sortorder-conversationnodesortorder"></a><span data-ttu-id="4ea7e-103">SortOrder (ConversationNodeSortOrder)</span><span class="sxs-lookup"><span data-stu-id="4ea7e-103">SortOrder (ConversationNodeSortOrder)</span></span>

<span data-ttu-id="4ea7e-104">Элемент **SortOrder** определяет порядок сортировки для результата запроса **GetConversationItems** .</span><span class="sxs-lookup"><span data-stu-id="4ea7e-104">The **SortOrder** element specifies the sort order used for the result of a **GetConversationItems** request.</span></span> 
  
```XML
<SortOrder>TreeOrderAscending | TreeOrderDescending | DateOrderAscending | DateOrderDescending</SortOrder>
```

 <span data-ttu-id="4ea7e-105">**ConversationNodeSortOrder**</span><span class="sxs-lookup"><span data-stu-id="4ea7e-105">**ConversationNodeSortOrder**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4ea7e-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="4ea7e-106">Attributes and elements</span></span>

<span data-ttu-id="4ea7e-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="4ea7e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4ea7e-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="4ea7e-108">Attributes</span></span>

<span data-ttu-id="4ea7e-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="4ea7e-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4ea7e-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="4ea7e-110">Child elements</span></span>

<span data-ttu-id="4ea7e-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="4ea7e-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="4ea7e-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="4ea7e-112">Parent elements</span></span>

[<span data-ttu-id="4ea7e-113">GetConversationItems</span><span class="sxs-lookup"><span data-stu-id="4ea7e-113">GetConversationItems</span></span>](getconversationitems.md)
  
## <a name="text-value"></a><span data-ttu-id="4ea7e-114">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="4ea7e-114">Text value</span></span>

<span data-ttu-id="4ea7e-115">Текстовое значение элемента **SortOrder** является порядок, в котором упорядоченные бесед.</span><span class="sxs-lookup"><span data-stu-id="4ea7e-115">The text value of the **SortOrder** element is the order in which conversations ordered.</span></span> <span data-ttu-id="4ea7e-116">Текстовое значение **TreeOrderAscending** указывает, что бесед упорядочены в соответствии с дерева беседы в порядке возрастания.</span><span class="sxs-lookup"><span data-stu-id="4ea7e-116">A text value of **TreeOrderAscending** indicates that the conversations are ordered according to the conversation tree in ascending order.</span></span> <span data-ttu-id="4ea7e-117">Текстовое значение **TreeOrderDescending** указывает, что бесед упорядочены в соответствии с дерева беседы в убывающем порядке.</span><span class="sxs-lookup"><span data-stu-id="4ea7e-117">A text value of **TreeOrderDescending** indicates that the conversations are ordered according to the conversation tree in descending order.</span></span> <span data-ttu-id="4ea7e-118">Текстовое значение **DateOrderAscending** указывает, что бесед упорядочены в соответствии с датой беседы в порядке возрастания.</span><span class="sxs-lookup"><span data-stu-id="4ea7e-118">A text value of **DateOrderAscending** indicates that the conversations are ordered according to the conversation date in ascending order.</span></span> <span data-ttu-id="4ea7e-119">Текстовое значение **DateOrderDescending** указывает, что бесед упорядочены в соответствии с датой беседы в убывающем порядке.</span><span class="sxs-lookup"><span data-stu-id="4ea7e-119">A text value of **DateOrderDescending** indicates that the conversations are ordered according to the conversation date in descending order.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="4ea7e-120">Замечания</span><span class="sxs-lookup"><span data-stu-id="4ea7e-120">Remarks</span></span>

<span data-ttu-id="4ea7e-121">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="4ea7e-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="4ea7e-122">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="4ea7e-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4ea7e-123">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="4ea7e-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4ea7e-124">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="4ea7e-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="4ea7e-125">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="4ea7e-125">Schema name</span></span>  <br/> |<span data-ttu-id="4ea7e-126">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="4ea7e-126">Messages schema</span></span>  <br/> |
|<span data-ttu-id="4ea7e-127">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="4ea7e-127">Validation file</span></span>  <br/> |<span data-ttu-id="4ea7e-128">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="4ea7e-128">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="4ea7e-129">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="4ea7e-129">Can be empty</span></span>  <br/> ||
   

