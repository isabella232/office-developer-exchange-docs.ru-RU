---
title: SortOrder (Конверсатионнодесортордер)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f9c4295c-8089-4533-b92f-2051eae9afeb
description: Элемент SortOrder указывает порядок сортировки, используемый для результатов запроса GetConversationItems.
ms.openlocfilehash: 397aead62d32e72f991af783bff02e79a6e4b0fb
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835520"
---
# <a name="sortorder-conversationnodesortorder"></a><span data-ttu-id="b0b85-103">SortOrder (Конверсатионнодесортордер)</span><span class="sxs-lookup"><span data-stu-id="b0b85-103">SortOrder (ConversationNodeSortOrder)</span></span>

<span data-ttu-id="b0b85-104">Элемент **SortOrder** указывает порядок сортировки, используемый для результатов запроса **GetConversationItems** .</span><span class="sxs-lookup"><span data-stu-id="b0b85-104">The **SortOrder** element specifies the sort order used for the result of a **GetConversationItems** request.</span></span> 
  
```XML
<SortOrder>TreeOrderAscending | TreeOrderDescending | DateOrderAscending | DateOrderDescending</SortOrder>
```

 <span data-ttu-id="b0b85-105">**конверсатионнодесортордер**</span><span class="sxs-lookup"><span data-stu-id="b0b85-105">**ConversationNodeSortOrder**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b0b85-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="b0b85-106">Attributes and elements</span></span>

<span data-ttu-id="b0b85-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="b0b85-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b0b85-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="b0b85-108">Attributes</span></span>

<span data-ttu-id="b0b85-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="b0b85-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b0b85-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="b0b85-110">Child elements</span></span>

<span data-ttu-id="b0b85-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="b0b85-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="b0b85-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="b0b85-112">Parent elements</span></span>

[<span data-ttu-id="b0b85-113">GetConversationItems</span><span class="sxs-lookup"><span data-stu-id="b0b85-113">GetConversationItems</span></span>](getconversationitems.md)
  
## <a name="text-value"></a><span data-ttu-id="b0b85-114">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="b0b85-114">Text value</span></span>

<span data-ttu-id="b0b85-115">Текстовое значение элемента **SortOrder** — это порядок, в котором упорядочиваются обсуждения.</span><span class="sxs-lookup"><span data-stu-id="b0b85-115">The text value of the **SortOrder** element is the order in which conversations ordered.</span></span> <span data-ttu-id="b0b85-116">Текстовое значение **триордерасцендинг** указывает, что беседы упорядочиваются в соответствии с деревом бесед в возрастающем порядке.</span><span class="sxs-lookup"><span data-stu-id="b0b85-116">A text value of **TreeOrderAscending** indicates that the conversations are ordered according to the conversation tree in ascending order.</span></span> <span data-ttu-id="b0b85-117">Текстовое значение **триордердесцендинг** указывает, что беседы упорядочиваются по дереву бесед в порядке убывания.</span><span class="sxs-lookup"><span data-stu-id="b0b85-117">A text value of **TreeOrderDescending** indicates that the conversations are ordered according to the conversation tree in descending order.</span></span> <span data-ttu-id="b0b85-118">Текстовое значение **датеордерасцендинг** указывает, что беседы упорядочиваются в соответствии с датой беседы в возрастающем порядке.</span><span class="sxs-lookup"><span data-stu-id="b0b85-118">A text value of **DateOrderAscending** indicates that the conversations are ordered according to the conversation date in ascending order.</span></span> <span data-ttu-id="b0b85-119">Текстовое значение **датеордердесцендинг** указывает, что беседы упорядочиваются в соответствии с датой беседы в убывающем порядке.</span><span class="sxs-lookup"><span data-stu-id="b0b85-119">A text value of **DateOrderDescending** indicates that the conversations are ordered according to the conversation date in descending order.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="b0b85-120">Примечания</span><span class="sxs-lookup"><span data-stu-id="b0b85-120">Remarks</span></span>

<span data-ttu-id="b0b85-121">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="b0b85-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="b0b85-122">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="b0b85-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b0b85-123">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="b0b85-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b0b85-124">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="b0b85-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="b0b85-125">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="b0b85-125">Schema name</span></span>  <br/> |<span data-ttu-id="b0b85-126">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="b0b85-126">Messages schema</span></span>  <br/> |
|<span data-ttu-id="b0b85-127">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="b0b85-127">Validation file</span></span>  <br/> |<span data-ttu-id="b0b85-128">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="b0b85-128">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="b0b85-129">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="b0b85-129">Can be empty</span></span>  <br/> ||
   

