---
title: DeleteType
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DeleteType
api_type:
- schema
ms.assetid: 6e3136cd-9cb4-493a-aa85-9678f719002d
description: Элемент DeleteType указывает способ удаления элементов в беседе.
ms.openlocfilehash: abaa0c3d8b7001b2f42a38d1c82475edba32d2c5
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762046"
---
# <a name="deletetype"></a><span data-ttu-id="e9b64-103">DeleteType</span><span class="sxs-lookup"><span data-stu-id="e9b64-103">DeleteType</span></span>

<span data-ttu-id="e9b64-104">Элемент **DeleteType** указывает способ удаления элементов в беседе.</span><span class="sxs-lookup"><span data-stu-id="e9b64-104">The **DeleteType** element indicates how items in a conversation are deleted.</span></span> 
  
- [<span data-ttu-id="e9b64-105">ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="e9b64-105">ApplyConversationAction</span></span>](applyconversationaction.md)  
- [<span data-ttu-id="e9b64-106">ConversationActions</span><span class="sxs-lookup"><span data-stu-id="e9b64-106">ConversationActions</span></span>](conversationactions.md)  
- [<span data-ttu-id="e9b64-107">ConversationAction</span><span class="sxs-lookup"><span data-stu-id="e9b64-107">ConversationAction</span></span>](conversationaction.md)  
- [<span data-ttu-id="e9b64-108">DeleteType</span><span class="sxs-lookup"><span data-stu-id="e9b64-108">DeleteType</span></span>](deletetype.md)
  
```XML
<DeleteType> HardDelete | MoveToDeletedItems | SoftDelete </DeleteType>
```

 <span data-ttu-id="e9b64-109">**DisposalType**</span><span class="sxs-lookup"><span data-stu-id="e9b64-109">**DisposalType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e9b64-110">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="e9b64-110">Attributes and elements</span></span>

<span data-ttu-id="e9b64-111">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="e9b64-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e9b64-112">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="e9b64-112">Attributes</span></span>

<span data-ttu-id="e9b64-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="e9b64-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e9b64-114">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="e9b64-114">Child elements</span></span>

<span data-ttu-id="e9b64-115">Нет.</span><span class="sxs-lookup"><span data-stu-id="e9b64-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="e9b64-116">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="e9b64-116">Parent elements</span></span>

|<span data-ttu-id="e9b64-117">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="e9b64-117">**Element**</span></span>|<span data-ttu-id="e9b64-118">**Описание**</span><span class="sxs-lookup"><span data-stu-id="e9b64-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e9b64-119">ConversationAction</span><span class="sxs-lookup"><span data-stu-id="e9b64-119">ConversationAction</span></span>](conversationaction.md) <br/> |<span data-ttu-id="e9b64-120">Содержит одно действие должен применяться к разговора.</span><span class="sxs-lookup"><span data-stu-id="e9b64-120">Contains a single action to be applied to a single conversation.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="e9b64-121">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="e9b64-121">Text value</span></span>

<span data-ttu-id="e9b64-122">Текстовое значение элемента **DeleteType** указывает способ удаления элементов в беседе.</span><span class="sxs-lookup"><span data-stu-id="e9b64-122">The text value of the **DeleteType** element indicates how items in a conversation are deleted.</span></span> <span data-ttu-id="e9b64-123">Ниже приведены возможные текстовые значения.</span><span class="sxs-lookup"><span data-stu-id="e9b64-123">The following are the possible text values:</span></span> 
  
- <span data-ttu-id="e9b64-124">HardDelete — указывает, что элементы в беседе будут окончательно удалены из базы данных почтовых ящиков.</span><span class="sxs-lookup"><span data-stu-id="e9b64-124">HardDelete - Indicates that items in a conversation are permanently removed from the mailbox database.</span></span>
    
- <span data-ttu-id="e9b64-125">MoveToDeleteItems — указывает, что элементы в беседе перемещаются в папку «Удаленные».</span><span class="sxs-lookup"><span data-stu-id="e9b64-125">MoveToDeleteItems - Indicates that items in a conversation are moved to the Deleted Items folder.</span></span>
    
- <span data-ttu-id="e9b64-126">SoftDelete — указывает, что элементы в беседе перемещаются в корзину Если корзина включена.</span><span class="sxs-lookup"><span data-stu-id="e9b64-126">SoftDelete - Indicates that items in a conversation are moved to the dumpster if the dumpster is enabled.</span></span>
    
## <a name="remarks"></a><span data-ttu-id="e9b64-127">Замечания</span><span class="sxs-lookup"><span data-stu-id="e9b64-127">Remarks</span></span>

<span data-ttu-id="e9b64-128">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.Этот элемент появился в Exchange Server 2010 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="e9b64-128">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e9b64-129">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="e9b64-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e9b64-130">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="e9b64-130">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="e9b64-131">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="e9b64-131">Schema Name</span></span>  <br/> |<span data-ttu-id="e9b64-132">Схема Types</span><span class="sxs-lookup"><span data-stu-id="e9b64-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="e9b64-133">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="e9b64-133">Validation File</span></span>  <br/> |<span data-ttu-id="e9b64-134">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="e9b64-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="e9b64-135">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="e9b64-135">Can be Empty</span></span>  <br/> |<span data-ttu-id="e9b64-136">False</span><span class="sxs-lookup"><span data-stu-id="e9b64-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e9b64-137">См. также</span><span class="sxs-lookup"><span data-stu-id="e9b64-137">See also</span></span>

- [<span data-ttu-id="e9b64-138">Операция ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="e9b64-138">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)
- [<span data-ttu-id="e9b64-139">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="e9b64-139">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

