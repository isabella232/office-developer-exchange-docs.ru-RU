---
title: ConversationActions
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ConversationActions
api_type:
- schema
ms.assetid: 3d6c663d-4bd9-4eec-b95a-cd683f592672
description: Элемент ConversationActions содержит коллекцию бесед и действий для применения к ним.
ms.openlocfilehash: 3dff7ff66f758f1cd2eb3cd7b8126294d2799fc0
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761815"
---
# <a name="conversationactions"></a><span data-ttu-id="9c401-103">ConversationActions</span><span class="sxs-lookup"><span data-stu-id="9c401-103">ConversationActions</span></span>

<span data-ttu-id="9c401-104">Элемент **ConversationActions** содержит коллекцию бесед и действий для применения к ним.</span><span class="sxs-lookup"><span data-stu-id="9c401-104">The **ConversationActions** element contains a collection of conversations and the actions to apply to them.</span></span> 
  
[<span data-ttu-id="9c401-105">ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="9c401-105">ApplyConversationAction</span></span>](applyconversationaction.md)
  
[<span data-ttu-id="9c401-106">ConversationActions</span><span class="sxs-lookup"><span data-stu-id="9c401-106">ConversationActions</span></span>](conversationactions.md)
  
```XML
<ConversationActions>
   <ConversationAction/>
</ConversationActions>
```

 <span data-ttu-id="9c401-107">**NonEmptyArrayOfApplyConversationActionType**</span><span class="sxs-lookup"><span data-stu-id="9c401-107">**NonEmptyArrayOfApplyConversationActionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9c401-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="9c401-108">Attributes and elements</span></span>

<span data-ttu-id="9c401-109">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="9c401-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9c401-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="9c401-110">Attributes</span></span>

<span data-ttu-id="9c401-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="9c401-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9c401-112">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="9c401-112">Child elements</span></span>

|<span data-ttu-id="9c401-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="9c401-113">**Element**</span></span>|<span data-ttu-id="9c401-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="9c401-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9c401-115">ConversationAction</span><span class="sxs-lookup"><span data-stu-id="9c401-115">ConversationAction</span></span>](conversationaction.md) <br/> |<span data-ttu-id="9c401-116">Содержит одно действие должен применяться к разговора.</span><span class="sxs-lookup"><span data-stu-id="9c401-116">Contains a single action to be applied to a single conversation.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="9c401-117">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="9c401-117">Parent elements</span></span>

|<span data-ttu-id="9c401-118">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="9c401-118">**Element**</span></span>|<span data-ttu-id="9c401-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="9c401-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9c401-120">ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="9c401-120">ApplyConversationAction</span></span>](applyconversationaction.md) <br/> |<span data-ttu-id="9c401-121">Определяет запрос для выполнения определенных действий к элементам в беседе.</span><span class="sxs-lookup"><span data-stu-id="9c401-121">Defines a request to apply actions to items in a conversation.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="9c401-122">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="9c401-122">Text value</span></span>

<span data-ttu-id="9c401-123">Нет.</span><span class="sxs-lookup"><span data-stu-id="9c401-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="9c401-124">Замечания</span><span class="sxs-lookup"><span data-stu-id="9c401-124">Remarks</span></span>

<span data-ttu-id="9c401-125">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.Этот элемент появился в Exchange Server 2010 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="9c401-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9c401-126">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="9c401-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9c401-127">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="9c401-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="9c401-128">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="9c401-128">Schema Name</span></span>  <br/> |<span data-ttu-id="9c401-129">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="9c401-129">Messages schema</span></span>  <br/> |
|<span data-ttu-id="9c401-130">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="9c401-130">Validation File</span></span>  <br/> |<span data-ttu-id="9c401-131">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="9c401-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="9c401-132">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="9c401-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="9c401-133">False</span><span class="sxs-lookup"><span data-stu-id="9c401-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9c401-134">См. также</span><span class="sxs-lookup"><span data-stu-id="9c401-134">See also</span></span>



[<span data-ttu-id="9c401-135">Операция ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="9c401-135">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)

