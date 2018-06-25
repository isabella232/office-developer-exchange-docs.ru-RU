---
title: FieldUri (правила)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: cecdea78-de9c-48be-ae31-03877feafeec
description: Элемент FieldURI указывает URI в поле правило, вызвавшей ошибку проверки.
ms.openlocfilehash: 88ba54994625d3a950b58e900f28c986c31eddac
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762527"
---
# <a name="fielduri-rule"></a><span data-ttu-id="d5e3d-103">FieldUri (правила)</span><span class="sxs-lookup"><span data-stu-id="d5e3d-103">FieldUri (Rule)</span></span>

<span data-ttu-id="d5e3d-104">Элемент **FieldURI** указывает URI в поле правило, вызвавшей ошибку проверки.</span><span class="sxs-lookup"><span data-stu-id="d5e3d-104">The **FieldURI** element specifies the URI to the rule field that caused the validation error.</span></span> 
  
```XML
<FieldURI/>
```

 <span data-ttu-id="d5e3d-105">**RuleFieldURIType**</span><span class="sxs-lookup"><span data-stu-id="d5e3d-105">**RuleFieldURIType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d5e3d-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="d5e3d-106">Attributes and elements</span></span>

<span data-ttu-id="d5e3d-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="d5e3d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d5e3d-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="d5e3d-108">Attributes</span></span>

<span data-ttu-id="d5e3d-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="d5e3d-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d5e3d-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="d5e3d-110">Child elements</span></span>

<span data-ttu-id="d5e3d-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="d5e3d-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="d5e3d-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="d5e3d-112">Parent elements</span></span>

|<span data-ttu-id="d5e3d-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="d5e3d-113">**Element**</span></span>|<span data-ttu-id="d5e3d-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d5e3d-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d5e3d-115">Error</span><span class="sxs-lookup"><span data-stu-id="d5e3d-115">Error</span></span>](error.md) <br/> |<span data-ttu-id="d5e3d-116">Представляет ошибку одной проверки на значение свойства определенное правило, значение свойства предиката или значение свойства действия.</span><span class="sxs-lookup"><span data-stu-id="d5e3d-116">Represents a single validation error on a particular rule property value, predicate property value, or action property value.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="d5e3d-117">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="d5e3d-117">Text value</span></span>

<span data-ttu-id="d5e3d-118">Текстовое значение для этого элемента есть только один из следующих строк:</span><span class="sxs-lookup"><span data-stu-id="d5e3d-118">The text value for this element is restricted to one of the following strings:</span></span>
  
- <span data-ttu-id="d5e3d-119">RuleId</span><span class="sxs-lookup"><span data-stu-id="d5e3d-119">RuleId</span></span>
    
- <span data-ttu-id="d5e3d-120">DisplayName</span><span class="sxs-lookup"><span data-stu-id="d5e3d-120">DisplayName</span></span>
    
- <span data-ttu-id="d5e3d-121">Priority</span><span class="sxs-lookup"><span data-stu-id="d5e3d-121">Priority</span></span>
    
- <span data-ttu-id="d5e3d-122">IsNotSupported</span><span class="sxs-lookup"><span data-stu-id="d5e3d-122">IsNotSupported</span></span>
    
- <span data-ttu-id="d5e3d-123">Действия</span><span class="sxs-lookup"><span data-stu-id="d5e3d-123">Actions</span></span>
    
- <span data-ttu-id="d5e3d-124">Условие: категории</span><span class="sxs-lookup"><span data-stu-id="d5e3d-124">Condition:Categories</span></span>
    
- <span data-ttu-id="d5e3d-125">Условие: ContainsBodyStrings</span><span class="sxs-lookup"><span data-stu-id="d5e3d-125">Condition:ContainsBodyStrings</span></span>
    
- <span data-ttu-id="d5e3d-126">Условие: ContainsHeaderStrings</span><span class="sxs-lookup"><span data-stu-id="d5e3d-126">Condition:ContainsHeaderStrings</span></span>
    
- <span data-ttu-id="d5e3d-127">Условие: ContainsRecipientStrings</span><span class="sxs-lookup"><span data-stu-id="d5e3d-127">Condition:ContainsRecipientStrings</span></span>
    
- <span data-ttu-id="d5e3d-128">Условие: ContainsSenderStrings</span><span class="sxs-lookup"><span data-stu-id="d5e3d-128">Condition:ContainsSenderStrings</span></span>
    
- <span data-ttu-id="d5e3d-129">Условие: ContainsSubjectOrBodyStrings</span><span class="sxs-lookup"><span data-stu-id="d5e3d-129">Condition:ContainsSubjectOrBodyStrings</span></span>
    
- <span data-ttu-id="d5e3d-130">Условие: ContainsSubjectStrings</span><span class="sxs-lookup"><span data-stu-id="d5e3d-130">Condition:ContainsSubjectStrings</span></span>
    
- <span data-ttu-id="d5e3d-131">Условие: FlaggedForAction</span><span class="sxs-lookup"><span data-stu-id="d5e3d-131">Condition:FlaggedForAction</span></span>
    
- <span data-ttu-id="d5e3d-132">Условие: FromAddresses</span><span class="sxs-lookup"><span data-stu-id="d5e3d-132">Condition:FromAddresses</span></span>
    
- <span data-ttu-id="d5e3d-133">Условие: FromConnectedAccounts</span><span class="sxs-lookup"><span data-stu-id="d5e3d-133">Condition:FromConnectedAccounts</span></span>
    
- <span data-ttu-id="d5e3d-134">Условие: HasAttachments</span><span class="sxs-lookup"><span data-stu-id="d5e3d-134">Condition:HasAttachments</span></span>
    
- <span data-ttu-id="d5e3d-135">Условие: важность</span><span class="sxs-lookup"><span data-stu-id="d5e3d-135">Condition:Importance</span></span>
    
- <span data-ttu-id="d5e3d-136">Условие: IsApprovalRequest</span><span class="sxs-lookup"><span data-stu-id="d5e3d-136">Condition:IsApprovalRequest</span></span>
    
- <span data-ttu-id="d5e3d-137">Условие: IsAutomaticForward</span><span class="sxs-lookup"><span data-stu-id="d5e3d-137">Condition:IsAutomaticForward</span></span>
    
- <span data-ttu-id="d5e3d-138">Условие: IsAutomaticReply</span><span class="sxs-lookup"><span data-stu-id="d5e3d-138">Condition:IsAutomaticReply</span></span>
    
- <span data-ttu-id="d5e3d-139">Условие: IsEncrypted</span><span class="sxs-lookup"><span data-stu-id="d5e3d-139">Condition:IsEncrypted</span></span>
    
- <span data-ttu-id="d5e3d-140">Условие: IsMeetingRequest</span><span class="sxs-lookup"><span data-stu-id="d5e3d-140">Condition:IsMeetingRequest</span></span>
    
- <span data-ttu-id="d5e3d-141">Условие: IsMeetingResponse</span><span class="sxs-lookup"><span data-stu-id="d5e3d-141">Condition:IsMeetingResponse</span></span>
    
- <span data-ttu-id="d5e3d-142">Условие: IsNDR</span><span class="sxs-lookup"><span data-stu-id="d5e3d-142">Condition:IsNDR</span></span>
    
- <span data-ttu-id="d5e3d-143">Условие: IsPermissionControlled</span><span class="sxs-lookup"><span data-stu-id="d5e3d-143">Condition:IsPermissionControlled</span></span>
    
- <span data-ttu-id="d5e3d-144">Условие: IsReadReceipt</span><span class="sxs-lookup"><span data-stu-id="d5e3d-144">Condition:IsReadReceipt</span></span>
    
- <span data-ttu-id="d5e3d-145">Условие: IsSigned</span><span class="sxs-lookup"><span data-stu-id="d5e3d-145">Condition:IsSigned</span></span>
    
- <span data-ttu-id="d5e3d-146">Условие: IsVoicemail</span><span class="sxs-lookup"><span data-stu-id="d5e3d-146">Condition:IsVoicemail</span></span>
    
- <span data-ttu-id="d5e3d-147">Условие: ItemClasses</span><span class="sxs-lookup"><span data-stu-id="d5e3d-147">Condition:ItemClasses</span></span>
    
- <span data-ttu-id="d5e3d-148">Условие: MessageClassifications</span><span class="sxs-lookup"><span data-stu-id="d5e3d-148">Condition:MessageClassifications</span></span>
    
- <span data-ttu-id="d5e3d-149">Условие: NotSentToMe</span><span class="sxs-lookup"><span data-stu-id="d5e3d-149">Condition:NotSentToMe</span></span>
    
- <span data-ttu-id="d5e3d-150">Условие: SentCcMe</span><span class="sxs-lookup"><span data-stu-id="d5e3d-150">Condition:SentCcMe</span></span>
    
- <span data-ttu-id="d5e3d-151">Условие: SentOnlyToMe</span><span class="sxs-lookup"><span data-stu-id="d5e3d-151">Condition:SentOnlyToMe</span></span>
    
- <span data-ttu-id="d5e3d-152">Условие: SentToAddresses</span><span class="sxs-lookup"><span data-stu-id="d5e3d-152">Condition:SentToAddresses</span></span>
    
- <span data-ttu-id="d5e3d-153">Условие: SentToMe</span><span class="sxs-lookup"><span data-stu-id="d5e3d-153">Condition:SentToMe</span></span>
    
- <span data-ttu-id="d5e3d-154">Условие: SentToOrCcMe</span><span class="sxs-lookup"><span data-stu-id="d5e3d-154">Condition:SentToOrCcMe</span></span>
    
- <span data-ttu-id="d5e3d-155">Условие: уровень конфиденциальности сообщения</span><span class="sxs-lookup"><span data-stu-id="d5e3d-155">Condition:Sensitivity</span></span>
    
- <span data-ttu-id="d5e3d-156">Условие: WithinDateRange</span><span class="sxs-lookup"><span data-stu-id="d5e3d-156">Condition:WithinDateRange</span></span>
    
- <span data-ttu-id="d5e3d-157">Условие: WithinSizeRange</span><span class="sxs-lookup"><span data-stu-id="d5e3d-157">Condition:WithinSizeRange</span></span>
    
- <span data-ttu-id="d5e3d-158">Исключение: категории</span><span class="sxs-lookup"><span data-stu-id="d5e3d-158">Exception:Categories</span></span>
    
- <span data-ttu-id="d5e3d-159">Исключение: ContainsBodyStrings</span><span class="sxs-lookup"><span data-stu-id="d5e3d-159">Exception:ContainsBodyStrings</span></span>
    
- <span data-ttu-id="d5e3d-160">Исключение: ContainsHeaderStrings</span><span class="sxs-lookup"><span data-stu-id="d5e3d-160">Exception:ContainsHeaderStrings</span></span>
    
- <span data-ttu-id="d5e3d-161">Исключение: ContainsRecipientStrings</span><span class="sxs-lookup"><span data-stu-id="d5e3d-161">Exception:ContainsRecipientStrings</span></span>
    
- <span data-ttu-id="d5e3d-162">Исключение: ContainsSenderStrings</span><span class="sxs-lookup"><span data-stu-id="d5e3d-162">Exception:ContainsSenderStrings</span></span>
    
- <span data-ttu-id="d5e3d-163">Исключение: ContainsSubjectOrBodyStrings</span><span class="sxs-lookup"><span data-stu-id="d5e3d-163">Exception:ContainsSubjectOrBodyStrings</span></span>
    
- <span data-ttu-id="d5e3d-164">Исключение: ContainsSubjectStrings</span><span class="sxs-lookup"><span data-stu-id="d5e3d-164">Exception:ContainsSubjectStrings</span></span>
    
- <span data-ttu-id="d5e3d-165">Исключение: FlaggedForAction</span><span class="sxs-lookup"><span data-stu-id="d5e3d-165">Exception:FlaggedForAction</span></span>
    
- <span data-ttu-id="d5e3d-166">Исключение: FromAddresses</span><span class="sxs-lookup"><span data-stu-id="d5e3d-166">Exception:FromAddresses</span></span>
    
- <span data-ttu-id="d5e3d-167">Исключение: FromConnectedAccounts</span><span class="sxs-lookup"><span data-stu-id="d5e3d-167">Exception:FromConnectedAccounts</span></span>
    
- <span data-ttu-id="d5e3d-168">Исключение: HasAttachments</span><span class="sxs-lookup"><span data-stu-id="d5e3d-168">Exception:HasAttachments</span></span>
    
- <span data-ttu-id="d5e3d-169">Исключение: важность</span><span class="sxs-lookup"><span data-stu-id="d5e3d-169">Exception:Importance</span></span>
    
- <span data-ttu-id="d5e3d-170">Исключение: IsApprovalRequest</span><span class="sxs-lookup"><span data-stu-id="d5e3d-170">Exception:IsApprovalRequest</span></span>
    
- <span data-ttu-id="d5e3d-171">Исключение: IsAutomaticForward</span><span class="sxs-lookup"><span data-stu-id="d5e3d-171">Exception:IsAutomaticForward</span></span>
    
- <span data-ttu-id="d5e3d-172">Исключение: IsAutomaticReply</span><span class="sxs-lookup"><span data-stu-id="d5e3d-172">Exception:IsAutomaticReply</span></span>
    
- <span data-ttu-id="d5e3d-173">Исключение: IsEncrypted</span><span class="sxs-lookup"><span data-stu-id="d5e3d-173">Exception:IsEncrypted</span></span>
    
- <span data-ttu-id="d5e3d-174">Исключение: IsMeetingRequest</span><span class="sxs-lookup"><span data-stu-id="d5e3d-174">Exception:IsMeetingRequest</span></span>
    
- <span data-ttu-id="d5e3d-175">Исключение: IsMeetingResponse</span><span class="sxs-lookup"><span data-stu-id="d5e3d-175">Exception:IsMeetingResponse</span></span>
    
- <span data-ttu-id="d5e3d-176">Исключение: IsNDR</span><span class="sxs-lookup"><span data-stu-id="d5e3d-176">Exception:IsNDR</span></span>
    
- <span data-ttu-id="d5e3d-177">Исключение: IsPermissionControlled</span><span class="sxs-lookup"><span data-stu-id="d5e3d-177">Exception:IsPermissionControlled</span></span>
    
- <span data-ttu-id="d5e3d-178">Исключение: IsReadReceipt</span><span class="sxs-lookup"><span data-stu-id="d5e3d-178">Exception:IsReadReceipt</span></span>
    
- <span data-ttu-id="d5e3d-179">Исключение: IsSigned</span><span class="sxs-lookup"><span data-stu-id="d5e3d-179">Exception:IsSigned</span></span>
    
- <span data-ttu-id="d5e3d-180">Исключение: IsVoicemail</span><span class="sxs-lookup"><span data-stu-id="d5e3d-180">Exception:IsVoicemail</span></span>
    
- <span data-ttu-id="d5e3d-181">Исключение: ItemClasses</span><span class="sxs-lookup"><span data-stu-id="d5e3d-181">Exception:ItemClasses</span></span>
    
- <span data-ttu-id="d5e3d-182">Исключение: MessageClassifications</span><span class="sxs-lookup"><span data-stu-id="d5e3d-182">Exception:MessageClassifications</span></span>
    
- <span data-ttu-id="d5e3d-183">Исключение: NotSentToMe</span><span class="sxs-lookup"><span data-stu-id="d5e3d-183">Exception:NotSentToMe</span></span>
    
- <span data-ttu-id="d5e3d-184">Исключение: SentCcMe</span><span class="sxs-lookup"><span data-stu-id="d5e3d-184">Exception:SentCcMe</span></span>
    
- <span data-ttu-id="d5e3d-185">Исключение: SentOnlyToMe</span><span class="sxs-lookup"><span data-stu-id="d5e3d-185">Exception:SentOnlyToMe</span></span>
    
- <span data-ttu-id="d5e3d-186">Исключение: SentToAddresses</span><span class="sxs-lookup"><span data-stu-id="d5e3d-186">Exception:SentToAddresses</span></span>
    
- <span data-ttu-id="d5e3d-187">Исключение: SentToMe</span><span class="sxs-lookup"><span data-stu-id="d5e3d-187">Exception:SentToMe</span></span>
    
- <span data-ttu-id="d5e3d-188">Исключение: SentToOrCcMe</span><span class="sxs-lookup"><span data-stu-id="d5e3d-188">Exception:SentToOrCcMe</span></span>
    
- <span data-ttu-id="d5e3d-189">Исключение: уровень конфиденциальности сообщения</span><span class="sxs-lookup"><span data-stu-id="d5e3d-189">Exception:Sensitivity</span></span>
    
- <span data-ttu-id="d5e3d-190">Исключение: WithinDateRange</span><span class="sxs-lookup"><span data-stu-id="d5e3d-190">Exception:WithinDateRange</span></span>
    
- <span data-ttu-id="d5e3d-191">Исключение: WithinSizeRange</span><span class="sxs-lookup"><span data-stu-id="d5e3d-191">Exception:WithinSizeRange</span></span>
    
- <span data-ttu-id="d5e3d-192">Действие: AssignCategories</span><span class="sxs-lookup"><span data-stu-id="d5e3d-192">Action:AssignCategories</span></span>
    
- <span data-ttu-id="d5e3d-193">Действие: CopyToFolder</span><span class="sxs-lookup"><span data-stu-id="d5e3d-193">Action:CopyToFolder</span></span>
    
- <span data-ttu-id="d5e3d-194">Действие: удаление</span><span class="sxs-lookup"><span data-stu-id="d5e3d-194">Action:Delete</span></span>
    
- <span data-ttu-id="d5e3d-195">Действие: ForwardAsAttachmentToRecipients</span><span class="sxs-lookup"><span data-stu-id="d5e3d-195">Action:ForwardAsAttachmentToRecipients</span></span>
    
- <span data-ttu-id="d5e3d-196">Действие: ForwardToRecipients</span><span class="sxs-lookup"><span data-stu-id="d5e3d-196">Action:ForwardToRecipients</span></span>
    
- <span data-ttu-id="d5e3d-197">Действие: MarkImportance</span><span class="sxs-lookup"><span data-stu-id="d5e3d-197">Action:MarkImportance</span></span>
    
- <span data-ttu-id="d5e3d-198">Действие: MarkAsRead</span><span class="sxs-lookup"><span data-stu-id="d5e3d-198">Action:MarkAsRead</span></span>
    
- <span data-ttu-id="d5e3d-199">Действие: MoveToFolder</span><span class="sxs-lookup"><span data-stu-id="d5e3d-199">Action:MoveToFolder</span></span>
    
- <span data-ttu-id="d5e3d-200">Действие: PermanentDelete</span><span class="sxs-lookup"><span data-stu-id="d5e3d-200">Action:PermanentDelete</span></span>
    
- <span data-ttu-id="d5e3d-201">Действие: RedirectToRecipients</span><span class="sxs-lookup"><span data-stu-id="d5e3d-201">Action:RedirectToRecipients</span></span>
    
- <span data-ttu-id="d5e3d-202">Действие: SendSMSAlertToRecipients</span><span class="sxs-lookup"><span data-stu-id="d5e3d-202">Action:SendSMSAlertToRecipients</span></span>
    
- <span data-ttu-id="d5e3d-203">Действие: ServerReplyWithMessage</span><span class="sxs-lookup"><span data-stu-id="d5e3d-203">Action:ServerReplyWithMessage</span></span>
    
- <span data-ttu-id="d5e3d-204">Действие: StopProcessingRules</span><span class="sxs-lookup"><span data-stu-id="d5e3d-204">Action:StopProcessingRules</span></span>
    
- <span data-ttu-id="d5e3d-205">Свойства IsEnabled</span><span class="sxs-lookup"><span data-stu-id="d5e3d-205">IsEnabled</span></span>
    
- <span data-ttu-id="d5e3d-206">IsInError</span><span class="sxs-lookup"><span data-stu-id="d5e3d-206">IsInError</span></span>
    
- <span data-ttu-id="d5e3d-207">Условия</span><span class="sxs-lookup"><span data-stu-id="d5e3d-207">Conditions</span></span>
    
- <span data-ttu-id="d5e3d-208">Исключения</span><span class="sxs-lookup"><span data-stu-id="d5e3d-208">Exceptions</span></span>
    
## <a name="remarks"></a><span data-ttu-id="d5e3d-209">Замечания</span><span class="sxs-lookup"><span data-stu-id="d5e3d-209">Remarks</span></span>

<span data-ttu-id="d5e3d-210">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="d5e3d-210">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d5e3d-211">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="d5e3d-211">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d5e3d-212">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="d5e3d-212">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="d5e3d-213">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="d5e3d-213">Schema Name</span></span>  <br/> |<span data-ttu-id="d5e3d-214">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="d5e3d-214">Messages schema</span></span>  <br/> |
|<span data-ttu-id="d5e3d-215">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="d5e3d-215">Validation File</span></span>  <br/> |<span data-ttu-id="d5e3d-216">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="d5e3d-216">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="d5e3d-217">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="d5e3d-217">Can be Empty</span></span>  <br/> |<span data-ttu-id="d5e3d-218">False</span><span class="sxs-lookup"><span data-stu-id="d5e3d-218">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d5e3d-219">См. также</span><span class="sxs-lookup"><span data-stu-id="d5e3d-219">See also</span></span>



- [<span data-ttu-id="d5e3d-220">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="d5e3d-220">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

