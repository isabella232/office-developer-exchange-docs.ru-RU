---
title: Фиелдури (правило)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: cecdea78-de9c-48be-ae31-03877feafeec
description: Элемент Фиелдури указывает универсальный код ресурса (URI) для поля правила, вызвавшего ошибку проверки.
ms.openlocfilehash: 3d88efdf951af580f81b5e2e7a544dcdf70ea830
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44461249"
---
# <a name="fielduri-rule"></a><span data-ttu-id="dec0c-103">Фиелдури (правило)</span><span class="sxs-lookup"><span data-stu-id="dec0c-103">FieldUri (Rule)</span></span>

<span data-ttu-id="dec0c-104">Элемент **фиелдури** указывает универсальный код ресурса (URI) для поля правила, вызвавшего ошибку проверки.</span><span class="sxs-lookup"><span data-stu-id="dec0c-104">The **FieldURI** element specifies the URI to the rule field that caused the validation error.</span></span> 
  
```XML
<FieldURI/>
```

 <span data-ttu-id="dec0c-105">**рулефиелдуритипе**</span><span class="sxs-lookup"><span data-stu-id="dec0c-105">**RuleFieldURIType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="dec0c-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="dec0c-106">Attributes and elements</span></span>

<span data-ttu-id="dec0c-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="dec0c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="dec0c-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="dec0c-108">Attributes</span></span>

<span data-ttu-id="dec0c-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="dec0c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="dec0c-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="dec0c-110">Child elements</span></span>

<span data-ttu-id="dec0c-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="dec0c-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="dec0c-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="dec0c-112">Parent elements</span></span>

|<span data-ttu-id="dec0c-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="dec0c-113">**Element**</span></span>|<span data-ttu-id="dec0c-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="dec0c-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="dec0c-115">Error</span><span class="sxs-lookup"><span data-stu-id="dec0c-115">Error</span></span>](error.md) <br/> |<span data-ttu-id="dec0c-116">Представляет одну ошибку проверки для определенного значения свойства правила, значения свойства предиката или значения свойства Action.</span><span class="sxs-lookup"><span data-stu-id="dec0c-116">Represents a single validation error on a particular rule property value, predicate property value, or action property value.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="dec0c-117">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="dec0c-117">Text value</span></span>

<span data-ttu-id="dec0c-118">Текстовое значение для этого элемента ограничено одной из следующих строк:</span><span class="sxs-lookup"><span data-stu-id="dec0c-118">The text value for this element is restricted to one of the following strings:</span></span>
  
- <span data-ttu-id="dec0c-119">RuleId</span><span class="sxs-lookup"><span data-stu-id="dec0c-119">RuleId</span></span>
    
- <span data-ttu-id="dec0c-120">DisplayName</span><span class="sxs-lookup"><span data-stu-id="dec0c-120">DisplayName</span></span>
    
- <span data-ttu-id="dec0c-121">Priority</span><span class="sxs-lookup"><span data-stu-id="dec0c-121">Priority</span></span>
    
- <span data-ttu-id="dec0c-122">иснотсуппортед</span><span class="sxs-lookup"><span data-stu-id="dec0c-122">IsNotSupported</span></span>
    
- <span data-ttu-id="dec0c-123">Действия</span><span class="sxs-lookup"><span data-stu-id="dec0c-123">Actions</span></span>
    
- <span data-ttu-id="dec0c-124">Условие: категории</span><span class="sxs-lookup"><span data-stu-id="dec0c-124">Condition:Categories</span></span>
    
- <span data-ttu-id="dec0c-125">Условие: Контаинсбодистрингс</span><span class="sxs-lookup"><span data-stu-id="dec0c-125">Condition:ContainsBodyStrings</span></span>
    
- <span data-ttu-id="dec0c-126">Условие: Контаиншеадерстрингс</span><span class="sxs-lookup"><span data-stu-id="dec0c-126">Condition:ContainsHeaderStrings</span></span>
    
- <span data-ttu-id="dec0c-127">Условие: КонтаинсреЦипиентстрингс</span><span class="sxs-lookup"><span data-stu-id="dec0c-127">Condition:ContainsRecipientStrings</span></span>
    
- <span data-ttu-id="dec0c-128">Условие: Контаинссендерстрингс</span><span class="sxs-lookup"><span data-stu-id="dec0c-128">Condition:ContainsSenderStrings</span></span>
    
- <span data-ttu-id="dec0c-129">Условие: Контаинссубжекторбодистрингс</span><span class="sxs-lookup"><span data-stu-id="dec0c-129">Condition:ContainsSubjectOrBodyStrings</span></span>
    
- <span data-ttu-id="dec0c-130">Условие: Контаинссубжектстрингс</span><span class="sxs-lookup"><span data-stu-id="dec0c-130">Condition:ContainsSubjectStrings</span></span>
    
- <span data-ttu-id="dec0c-131">Условие: Флагжедфорактион</span><span class="sxs-lookup"><span data-stu-id="dec0c-131">Condition:FlaggedForAction</span></span>
    
- <span data-ttu-id="dec0c-132">Условие: Фромаддрессес</span><span class="sxs-lookup"><span data-stu-id="dec0c-132">Condition:FromAddresses</span></span>
    
- <span data-ttu-id="dec0c-133">Условие: Фромконнектедаккаунтс</span><span class="sxs-lookup"><span data-stu-id="dec0c-133">Condition:FromConnectedAccounts</span></span>
    
- <span data-ttu-id="dec0c-134">Условие: HasAttachments</span><span class="sxs-lookup"><span data-stu-id="dec0c-134">Condition:HasAttachments</span></span>
    
- <span data-ttu-id="dec0c-135">Условие: важно!</span><span class="sxs-lookup"><span data-stu-id="dec0c-135">Condition:Importance</span></span>
    
- <span data-ttu-id="dec0c-136">Условие: Исаппровалрекуест</span><span class="sxs-lookup"><span data-stu-id="dec0c-136">Condition:IsApprovalRequest</span></span>
    
- <span data-ttu-id="dec0c-137">Условие: Исаутоматикфорвард</span><span class="sxs-lookup"><span data-stu-id="dec0c-137">Condition:IsAutomaticForward</span></span>
    
- <span data-ttu-id="dec0c-138">Условие: Исаутоматикрепли</span><span class="sxs-lookup"><span data-stu-id="dec0c-138">Condition:IsAutomaticReply</span></span>
    
- <span data-ttu-id="dec0c-139">Условие: "с шифрованием"</span><span class="sxs-lookup"><span data-stu-id="dec0c-139">Condition:IsEncrypted</span></span>
    
- <span data-ttu-id="dec0c-140">Условие: Исмитингрекуест</span><span class="sxs-lookup"><span data-stu-id="dec0c-140">Condition:IsMeetingRequest</span></span>
    
- <span data-ttu-id="dec0c-141">Условие: Исмитингреспонсе</span><span class="sxs-lookup"><span data-stu-id="dec0c-141">Condition:IsMeetingResponse</span></span>
    
- <span data-ttu-id="dec0c-142">Условие: Исндр</span><span class="sxs-lookup"><span data-stu-id="dec0c-142">Condition:IsNDR</span></span>
    
- <span data-ttu-id="dec0c-143">Условие: Испермиссионконтроллед</span><span class="sxs-lookup"><span data-stu-id="dec0c-143">Condition:IsPermissionControlled</span></span>
    
- <span data-ttu-id="dec0c-144">Условие: Исреадрецеипт</span><span class="sxs-lookup"><span data-stu-id="dec0c-144">Condition:IsReadReceipt</span></span>
    
- <span data-ttu-id="dec0c-145">Условие: с подписью</span><span class="sxs-lookup"><span data-stu-id="dec0c-145">Condition:IsSigned</span></span>
    
- <span data-ttu-id="dec0c-146">Условие: Голосовая почта</span><span class="sxs-lookup"><span data-stu-id="dec0c-146">Condition:IsVoicemail</span></span>
    
- <span data-ttu-id="dec0c-147">Условие: Итемклассес</span><span class="sxs-lookup"><span data-stu-id="dec0c-147">Condition:ItemClasses</span></span>
    
- <span data-ttu-id="dec0c-148">Условие: Мессажеклассификатионс</span><span class="sxs-lookup"><span data-stu-id="dec0c-148">Condition:MessageClassifications</span></span>
    
- <span data-ttu-id="dec0c-149">Условие: Нотсенттоме</span><span class="sxs-lookup"><span data-stu-id="dec0c-149">Condition:NotSentToMe</span></span>
    
- <span data-ttu-id="dec0c-150">Условие: Сентккме</span><span class="sxs-lookup"><span data-stu-id="dec0c-150">Condition:SentCcMe</span></span>
    
- <span data-ttu-id="dec0c-151">Условие: Сентонлитоме</span><span class="sxs-lookup"><span data-stu-id="dec0c-151">Condition:SentOnlyToMe</span></span>
    
- <span data-ttu-id="dec0c-152">Условие: Сенттоаддрессес</span><span class="sxs-lookup"><span data-stu-id="dec0c-152">Condition:SentToAddresses</span></span>
    
- <span data-ttu-id="dec0c-153">Условие: Сенттоме</span><span class="sxs-lookup"><span data-stu-id="dec0c-153">Condition:SentToMe</span></span>
    
- <span data-ttu-id="dec0c-154">Условие: Сенттурккме</span><span class="sxs-lookup"><span data-stu-id="dec0c-154">Condition:SentToOrCcMe</span></span>
    
- <span data-ttu-id="dec0c-155">Условие: чувствительность</span><span class="sxs-lookup"><span data-stu-id="dec0c-155">Condition:Sensitivity</span></span>
    
- <span data-ttu-id="dec0c-156">Условие: Висиндатеранже</span><span class="sxs-lookup"><span data-stu-id="dec0c-156">Condition:WithinDateRange</span></span>
    
- <span data-ttu-id="dec0c-157">Условие: Висинсизеранже</span><span class="sxs-lookup"><span data-stu-id="dec0c-157">Condition:WithinSizeRange</span></span>
    
- <span data-ttu-id="dec0c-158">Исключение: категории</span><span class="sxs-lookup"><span data-stu-id="dec0c-158">Exception:Categories</span></span>
    
- <span data-ttu-id="dec0c-159">Исключение: Контаинсбодистрингс</span><span class="sxs-lookup"><span data-stu-id="dec0c-159">Exception:ContainsBodyStrings</span></span>
    
- <span data-ttu-id="dec0c-160">Исключение: Контаиншеадерстрингс</span><span class="sxs-lookup"><span data-stu-id="dec0c-160">Exception:ContainsHeaderStrings</span></span>
    
- <span data-ttu-id="dec0c-161">Исключение: КонтаинсреЦипиентстрингс</span><span class="sxs-lookup"><span data-stu-id="dec0c-161">Exception:ContainsRecipientStrings</span></span>
    
- <span data-ttu-id="dec0c-162">Исключение: Контаинссендерстрингс</span><span class="sxs-lookup"><span data-stu-id="dec0c-162">Exception:ContainsSenderStrings</span></span>
    
- <span data-ttu-id="dec0c-163">Исключение: Контаинссубжекторбодистрингс</span><span class="sxs-lookup"><span data-stu-id="dec0c-163">Exception:ContainsSubjectOrBodyStrings</span></span>
    
- <span data-ttu-id="dec0c-164">Исключение: Контаинссубжектстрингс</span><span class="sxs-lookup"><span data-stu-id="dec0c-164">Exception:ContainsSubjectStrings</span></span>
    
- <span data-ttu-id="dec0c-165">Исключение: Флагжедфорактион</span><span class="sxs-lookup"><span data-stu-id="dec0c-165">Exception:FlaggedForAction</span></span>
    
- <span data-ttu-id="dec0c-166">Исключение: Фромаддрессес</span><span class="sxs-lookup"><span data-stu-id="dec0c-166">Exception:FromAddresses</span></span>
    
- <span data-ttu-id="dec0c-167">Исключение: Фромконнектедаккаунтс</span><span class="sxs-lookup"><span data-stu-id="dec0c-167">Exception:FromConnectedAccounts</span></span>
    
- <span data-ttu-id="dec0c-168">Исключение: HasAttachments</span><span class="sxs-lookup"><span data-stu-id="dec0c-168">Exception:HasAttachments</span></span>
    
- <span data-ttu-id="dec0c-169">Исключение: важность</span><span class="sxs-lookup"><span data-stu-id="dec0c-169">Exception:Importance</span></span>
    
- <span data-ttu-id="dec0c-170">Исключение: Исаппровалрекуест</span><span class="sxs-lookup"><span data-stu-id="dec0c-170">Exception:IsApprovalRequest</span></span>
    
- <span data-ttu-id="dec0c-171">Исключение: Исаутоматикфорвард</span><span class="sxs-lookup"><span data-stu-id="dec0c-171">Exception:IsAutomaticForward</span></span>
    
- <span data-ttu-id="dec0c-172">Исключение: Исаутоматикрепли</span><span class="sxs-lookup"><span data-stu-id="dec0c-172">Exception:IsAutomaticReply</span></span>
    
- <span data-ttu-id="dec0c-173">Исключение: не зашифровано</span><span class="sxs-lookup"><span data-stu-id="dec0c-173">Exception:IsEncrypted</span></span>
    
- <span data-ttu-id="dec0c-174">Исключение: Исмитингрекуест</span><span class="sxs-lookup"><span data-stu-id="dec0c-174">Exception:IsMeetingRequest</span></span>
    
- <span data-ttu-id="dec0c-175">Исключение: Исмитингреспонсе</span><span class="sxs-lookup"><span data-stu-id="dec0c-175">Exception:IsMeetingResponse</span></span>
    
- <span data-ttu-id="dec0c-176">Исключение: Исндр</span><span class="sxs-lookup"><span data-stu-id="dec0c-176">Exception:IsNDR</span></span>
    
- <span data-ttu-id="dec0c-177">Исключение: Испермиссионконтроллед</span><span class="sxs-lookup"><span data-stu-id="dec0c-177">Exception:IsPermissionControlled</span></span>
    
- <span data-ttu-id="dec0c-178">Исключение: Исреадрецеипт</span><span class="sxs-lookup"><span data-stu-id="dec0c-178">Exception:IsReadReceipt</span></span>
    
- <span data-ttu-id="dec0c-179">Исключение: подпись</span><span class="sxs-lookup"><span data-stu-id="dec0c-179">Exception:IsSigned</span></span>
    
- <span data-ttu-id="dec0c-180">Исключение: Голосовая почта</span><span class="sxs-lookup"><span data-stu-id="dec0c-180">Exception:IsVoicemail</span></span>
    
- <span data-ttu-id="dec0c-181">Исключение: Итемклассес</span><span class="sxs-lookup"><span data-stu-id="dec0c-181">Exception:ItemClasses</span></span>
    
- <span data-ttu-id="dec0c-182">Исключение: Мессажеклассификатионс</span><span class="sxs-lookup"><span data-stu-id="dec0c-182">Exception:MessageClassifications</span></span>
    
- <span data-ttu-id="dec0c-183">Исключение: Нотсенттоме</span><span class="sxs-lookup"><span data-stu-id="dec0c-183">Exception:NotSentToMe</span></span>
    
- <span data-ttu-id="dec0c-184">Исключение: Сентккме</span><span class="sxs-lookup"><span data-stu-id="dec0c-184">Exception:SentCcMe</span></span>
    
- <span data-ttu-id="dec0c-185">Исключение: Сентонлитоме</span><span class="sxs-lookup"><span data-stu-id="dec0c-185">Exception:SentOnlyToMe</span></span>
    
- <span data-ttu-id="dec0c-186">Исключение: Сенттоаддрессес</span><span class="sxs-lookup"><span data-stu-id="dec0c-186">Exception:SentToAddresses</span></span>
    
- <span data-ttu-id="dec0c-187">Исключение: Сенттоме</span><span class="sxs-lookup"><span data-stu-id="dec0c-187">Exception:SentToMe</span></span>
    
- <span data-ttu-id="dec0c-188">Исключение: Сенттурккме</span><span class="sxs-lookup"><span data-stu-id="dec0c-188">Exception:SentToOrCcMe</span></span>
    
- <span data-ttu-id="dec0c-189">Исключение: чувствительность</span><span class="sxs-lookup"><span data-stu-id="dec0c-189">Exception:Sensitivity</span></span>
    
- <span data-ttu-id="dec0c-190">Исключение: Висиндатеранже</span><span class="sxs-lookup"><span data-stu-id="dec0c-190">Exception:WithinDateRange</span></span>
    
- <span data-ttu-id="dec0c-191">Исключение: Висинсизеранже</span><span class="sxs-lookup"><span data-stu-id="dec0c-191">Exception:WithinSizeRange</span></span>
    
- <span data-ttu-id="dec0c-192">Действие: Ассигнкатегориес</span><span class="sxs-lookup"><span data-stu-id="dec0c-192">Action:AssignCategories</span></span>
    
- <span data-ttu-id="dec0c-193">Действие: CopyToFolder</span><span class="sxs-lookup"><span data-stu-id="dec0c-193">Action:CopyToFolder</span></span>
    
- <span data-ttu-id="dec0c-194">Действие: Delete</span><span class="sxs-lookup"><span data-stu-id="dec0c-194">Action:Delete</span></span>
    
- <span data-ttu-id="dec0c-195">Действие: ФорвардасаттачменттореЦипиентс</span><span class="sxs-lookup"><span data-stu-id="dec0c-195">Action:ForwardAsAttachmentToRecipients</span></span>
    
- <span data-ttu-id="dec0c-196">Действие: ФорвардтореЦипиентс</span><span class="sxs-lookup"><span data-stu-id="dec0c-196">Action:ForwardToRecipients</span></span>
    
- <span data-ttu-id="dec0c-197">Действие: Маркимпортанце</span><span class="sxs-lookup"><span data-stu-id="dec0c-197">Action:MarkImportance</span></span>
    
- <span data-ttu-id="dec0c-198">Действие: Маркасреад</span><span class="sxs-lookup"><span data-stu-id="dec0c-198">Action:MarkAsRead</span></span>
    
- <span data-ttu-id="dec0c-199">Действие: MoveToFolder</span><span class="sxs-lookup"><span data-stu-id="dec0c-199">Action:MoveToFolder</span></span>
    
- <span data-ttu-id="dec0c-200">Действие: Перманентделете</span><span class="sxs-lookup"><span data-stu-id="dec0c-200">Action:PermanentDelete</span></span>
    
- <span data-ttu-id="dec0c-201">Действие: RedirectToRecipients</span><span class="sxs-lookup"><span data-stu-id="dec0c-201">Action:RedirectToRecipients</span></span>
    
- <span data-ttu-id="dec0c-202">Действие: СендсмсалерттореЦипиентс</span><span class="sxs-lookup"><span data-stu-id="dec0c-202">Action:SendSMSAlertToRecipients</span></span>
    
- <span data-ttu-id="dec0c-203">Действие: Серверрепливисмессаже</span><span class="sxs-lookup"><span data-stu-id="dec0c-203">Action:ServerReplyWithMessage</span></span>
    
- <span data-ttu-id="dec0c-204">Действие: StopProcessingRules</span><span class="sxs-lookup"><span data-stu-id="dec0c-204">Action:StopProcessingRules</span></span>
    
- <span data-ttu-id="dec0c-205">IsEnabled</span><span class="sxs-lookup"><span data-stu-id="dec0c-205">IsEnabled</span></span>
    
- <span data-ttu-id="dec0c-206">исинеррор</span><span class="sxs-lookup"><span data-stu-id="dec0c-206">IsInError</span></span>
    
- <span data-ttu-id="dec0c-207">Условия</span><span class="sxs-lookup"><span data-stu-id="dec0c-207">Conditions</span></span>
    
- <span data-ttu-id="dec0c-208">Исключения</span><span class="sxs-lookup"><span data-stu-id="dec0c-208">Exceptions</span></span>
    
## <a name="remarks"></a><span data-ttu-id="dec0c-209">Примечания</span><span class="sxs-lookup"><span data-stu-id="dec0c-209">Remarks</span></span>

<span data-ttu-id="dec0c-210">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="dec0c-210">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="dec0c-211">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="dec0c-211">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="dec0c-212">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="dec0c-212">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="dec0c-213">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="dec0c-213">Schema Name</span></span>  <br/> |<span data-ttu-id="dec0c-214">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="dec0c-214">Messages schema</span></span>  <br/> |
|<span data-ttu-id="dec0c-215">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="dec0c-215">Validation File</span></span>  <br/> |<span data-ttu-id="dec0c-216">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="dec0c-216">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="dec0c-217">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="dec0c-217">Can be Empty</span></span>  <br/> |<span data-ttu-id="dec0c-218">False</span><span class="sxs-lookup"><span data-stu-id="dec0c-218">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="dec0c-219">См. также</span><span class="sxs-lookup"><span data-stu-id="dec0c-219">See also</span></span>



- [<span data-ttu-id="dec0c-220">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="dec0c-220">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

