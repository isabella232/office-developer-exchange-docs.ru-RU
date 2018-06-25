---
title: ConversationNode
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: b7f7acd3-ed65-441e-9976-8b4ed5f12c0b
description: Элемент ConversationNode указывает узел в беседе.
ms.openlocfilehash: c8289e5f30bfd25eb12d54e3be0c561786308dc6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761821"
---
# <a name="conversationnode"></a><span data-ttu-id="59ac4-103">ConversationNode</span><span class="sxs-lookup"><span data-stu-id="59ac4-103">ConversationNode</span></span>

<span data-ttu-id="59ac4-104">Элемент **ConversationNode** указывает узел в беседе.</span><span class="sxs-lookup"><span data-stu-id="59ac4-104">The **ConversationNode** element specifies a node in a conversation.</span></span> 
  
```XML
<ConversationNode>
    <InternetMessageId></InternetMessageId>
    <ParentInternetMessageId></ParentInternetMessageId>
    <Items></Items>
</ConversationNode>
```

 <span data-ttu-id="59ac4-105">**ConversationNodeType**</span><span class="sxs-lookup"><span data-stu-id="59ac4-105">**ConversationNodeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="59ac4-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="59ac4-106">Attributes and elements</span></span>

<span data-ttu-id="59ac4-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="59ac4-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="59ac4-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="59ac4-108">Attributes</span></span>

<span data-ttu-id="59ac4-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="59ac4-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="59ac4-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="59ac4-110">Child elements</span></span>

|<span data-ttu-id="59ac4-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="59ac4-111">**Element**</span></span>|<span data-ttu-id="59ac4-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="59ac4-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="59ac4-113">InternetMessageId</span><span class="sxs-lookup"><span data-stu-id="59ac4-113">InternetMessageId</span></span>](internetmessageid.md) <br/> |<span data-ttu-id="59ac4-114">Представляет идентификатор сообщения Интернета элемента.</span><span class="sxs-lookup"><span data-stu-id="59ac4-114">Represents the Internet message identifier of an item.</span></span>  <br/> |
|[<span data-ttu-id="59ac4-115">ParentInternetMessageId</span><span class="sxs-lookup"><span data-stu-id="59ac4-115">ParentInternetMessageId</span></span>](parentinternetmessageid.md) <br/> |<span data-ttu-id="59ac4-116">Задает идентификатор сообщения Интернета родительского.</span><span class="sxs-lookup"><span data-stu-id="59ac4-116">Specifies the identifier of the parent Internet message.</span></span>  <br/> |
|[<span data-ttu-id="59ac4-117">Что ItemID (NonEmptyArrayOfItemIdsType)</span><span class="sxs-lookup"><span data-stu-id="59ac4-117">ItemIds (NonEmptyArrayOfItemIdsType)</span></span>](itemids-nonemptyarrayofitemidstype.md) <br/> |<span data-ttu-id="59ac4-118">Указывает все элементы в узле беседы.</span><span class="sxs-lookup"><span data-stu-id="59ac4-118">Specifies all the items in the conversation node.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="59ac4-119">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="59ac4-119">Parent elements</span></span>

|<span data-ttu-id="59ac4-120">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="59ac4-120">**Element**</span></span>|<span data-ttu-id="59ac4-121">**Описание**</span><span class="sxs-lookup"><span data-stu-id="59ac4-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="59ac4-122">ConversationNodes</span><span class="sxs-lookup"><span data-stu-id="59ac4-122">ConversationNodes</span></span>](conversationnodes.md) <br/> |<span data-ttu-id="59ac4-123">Задает семейство узлов беседы.</span><span class="sxs-lookup"><span data-stu-id="59ac4-123">Specifies a collection of conversation nodes.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="59ac4-124">Замечания</span><span class="sxs-lookup"><span data-stu-id="59ac4-124">Remarks</span></span>

<span data-ttu-id="59ac4-125">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="59ac4-125">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="59ac4-126">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="59ac4-126">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="59ac4-127">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="59ac4-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="59ac4-128">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="59ac4-128">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="59ac4-129">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="59ac4-129">Schema Name</span></span>  <br/> |<span data-ttu-id="59ac4-130">Схема типа</span><span class="sxs-lookup"><span data-stu-id="59ac4-130">Type schema</span></span>  <br/> |
|<span data-ttu-id="59ac4-131">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="59ac4-131">Validation File</span></span>  <br/> |<span data-ttu-id="59ac4-132">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="59ac4-132">types.xsd</span></span>  <br/> |
|<span data-ttu-id="59ac4-133">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="59ac4-133">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="59ac4-134">См. также</span><span class="sxs-lookup"><span data-stu-id="59ac4-134">See also</span></span>



- [<span data-ttu-id="59ac4-135">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="59ac4-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

