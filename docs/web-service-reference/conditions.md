---
title: Условия
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Conditions
api_type:
- schema
ms.assetid: f049a48c-9585-43f7-8549-0b8cb19a5eea
description: Элемент Conditions указывает условия, при выполнении которых будут запускаться действия правил для правила.
ms.openlocfilehash: 2c6b4794a87cca79b4c723197b57360ad0ff973d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463204"
---
# <a name="conditions"></a><span data-ttu-id="76873-103">Условия</span><span class="sxs-lookup"><span data-stu-id="76873-103">Conditions</span></span>

<span data-ttu-id="76873-104">Элемент **Conditions** указывает условия, при выполнении которых будут запускаться действия правил для правила.</span><span class="sxs-lookup"><span data-stu-id="76873-104">The **Conditions** element identifies the conditions that, when fulfilled, will trigger the rule actions for a rule.</span></span> 
  
```XML
<Conditions>
   <Categories/>
   <ContainsBodyStrings/>
   <ContainsHeaderStrings/>
   <ContainsRecipientStrings/>
   <ContainsSenderStrings/>
   <ContainsSubjectOrBodyStrings/>
   <ContainsSubjectStrings/>
   <FlaggedForAction/>
   <FromAddresses/>
   <FromConnectedAccounts/>
   <HasAttachments/>
   <Importance/>
   <IsApprovalRequest/>
   <IsAutomaticForward/>
   <IsAutomaticReply/>
   <IsEncrypted/>
   <IsMeetingRequest/>
   <IsMeetingResponse/>
   <IsNDR/>
   <IsPermissionControlled/>
   <IsReadReceipt/>
   <IsSigned/>
   <IsVoicemail/>
   <ItemClasses/>
   <MessageClassifications/>
   <NotSentToMe/>
   <SentCcMe/>
   <SentOnlyToMe/>
   <SentToAddresses/>
   <SentToMe/>
   <SentToOrCcMe/>
   <Sensitivity/>
   <WithinDateRange/>
   <WithinSizeRange/>
</Conditions>
```

 <span data-ttu-id="76873-105">**рулепредикатестипе**</span><span class="sxs-lookup"><span data-stu-id="76873-105">**RulePredicatesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="76873-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="76873-106">Attributes and elements</span></span>

<span data-ttu-id="76873-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="76873-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="76873-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="76873-108">Attributes</span></span>

<span data-ttu-id="76873-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="76873-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="76873-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="76873-110">Child elements</span></span>

|<span data-ttu-id="76873-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="76873-111">**Element**</span></span>|<span data-ttu-id="76873-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="76873-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="76873-113">Категории</span><span class="sxs-lookup"><span data-stu-id="76873-113">Categories</span></span>](categories-ex15websvcsotherref.md) <br/> |<span data-ttu-id="76873-114">Содержит категории, которые необходимо применить к входящему сообщению, чтобы применить условие или исключение.</span><span class="sxs-lookup"><span data-stu-id="76873-114">Contains the categories that must be applied to an incoming message in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="76873-115">контаинсбодистрингс</span><span class="sxs-lookup"><span data-stu-id="76873-115">ContainsBodyStrings</span></span>](containsbodystrings.md) <br/> |<span data-ttu-id="76873-116">Указывает строки, которые должны присутствовать в теле входящих сообщений, чтобы применить условие или исключение.</span><span class="sxs-lookup"><span data-stu-id="76873-116">Indicates the strings that must appear in the body of incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="76873-117">контаиншеадерстрингс</span><span class="sxs-lookup"><span data-stu-id="76873-117">ContainsHeaderStrings</span></span>](containsheaderstrings.md) <br/> |<span data-ttu-id="76873-118">Указывает строки, которые должны отображаться в заголовках входящих сообщений, чтобы применялось условие или исключение.</span><span class="sxs-lookup"><span data-stu-id="76873-118">Indicates the strings that must appear in the headers of incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="76873-119">контаинсреЦипиентстрингс</span><span class="sxs-lookup"><span data-stu-id="76873-119">ContainsRecipientStrings</span></span>](containsrecipientstrings.md) <br/> |<span data-ttu-id="76873-120">Указывает строки, которые должны присутствовать в свойствах **ToRecipients** или **CcRecipients** входящих сообщений, чтобы применялось условие или исключение.</span><span class="sxs-lookup"><span data-stu-id="76873-120">Indicates the strings that must appear in either the **ToRecipients** or **CcRecipients** properties of incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="76873-121">контаинссендерстрингс</span><span class="sxs-lookup"><span data-stu-id="76873-121">ContainsSenderStrings</span></span>](containssenderstrings.md) <br/> |<span data-ttu-id="76873-122">Указывает строки, которые должны присутствовать в свойстве **from** входящих сообщений, чтобы применялось условие или исключение.</span><span class="sxs-lookup"><span data-stu-id="76873-122">Indicates the strings that must appear in the **From** property of incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="76873-123">контаинссубжекторбодистрингс</span><span class="sxs-lookup"><span data-stu-id="76873-123">ContainsSubjectOrBodyStrings</span></span>](containssubjectorbodystrings.md) <br/> |<span data-ttu-id="76873-124">Указывает строки, которые должны присутствовать в тексте или теме входящих сообщений, чтобы применялось условие или исключение.</span><span class="sxs-lookup"><span data-stu-id="76873-124">Indicates the strings that must appear in either the body or the subject of incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="76873-125">контаинссубжектстрингс</span><span class="sxs-lookup"><span data-stu-id="76873-125">ContainsSubjectStrings</span></span>](containssubjectstrings.md) <br/> |<span data-ttu-id="76873-126">Указывает строки, которые должны присутствовать в теме входящих сообщений, чтобы применить условие или исключение.</span><span class="sxs-lookup"><span data-stu-id="76873-126">Indicates the strings that must appear in the subject of incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="76873-127">флагжедфорактион</span><span class="sxs-lookup"><span data-stu-id="76873-127">FlaggedForAction</span></span>](flaggedforaction.md) <br/> |<span data-ttu-id="76873-128">Указывает флаг для значения действия, который должен отображаться в входящих сообщениях, чтобы применить условие или исключение.</span><span class="sxs-lookup"><span data-stu-id="76873-128">Specifies the flag for action value that must appear on incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="76873-129">фромаддрессес</span><span class="sxs-lookup"><span data-stu-id="76873-129">FromAddresses</span></span>](fromaddresses.md) <br/> |<span data-ttu-id="76873-130">Указывает адреса электронной почты, из которых должны отправляться входящие сообщения, чтобы применялось условие или исключение.</span><span class="sxs-lookup"><span data-stu-id="76873-130">Indicates the e-mail addresses from which incoming messages must be sent in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="76873-131">фромконнектедаккаунтс</span><span class="sxs-lookup"><span data-stu-id="76873-131">FromConnectedAccounts</span></span>](fromconnectedaccounts.md) <br/> |<span data-ttu-id="76873-132">Представляет имена учетных записей электронной почты, для которых необходимо выполнить статистическую обработку входящих сообщений для того, чтобы применить условие или исключение.</span><span class="sxs-lookup"><span data-stu-id="76873-132">Represents the e-mail account names from which incoming messages have to have been aggregated in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="76873-133">HasAttachments</span><span class="sxs-lookup"><span data-stu-id="76873-133">HasAttachments</span></span>](hasattachments.md) <br/> |<span data-ttu-id="76873-134">Указывает, должны ли входящие сообщения иметь вложения, чтобы применялось условие или исключение.</span><span class="sxs-lookup"><span data-stu-id="76873-134">Indicates whether incoming messages have to have attachments in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="76873-135">Importance</span><span class="sxs-lookup"><span data-stu-id="76873-135">Importance</span></span>](importance.md) <br/> |<span data-ttu-id="76873-136">Указывает важность, которая отмечается на входящих сообщениях, чтобы применялось условие или исключение.</span><span class="sxs-lookup"><span data-stu-id="76873-136">Specifies the importance that is stamped on incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="76873-137">исаппровалрекуест</span><span class="sxs-lookup"><span data-stu-id="76873-137">IsApprovalRequest</span></span>](isapprovalrequest.md) <br/> |<span data-ttu-id="76873-138">Указывает, должны ли входящие сообщения быть запросами на утверждение, чтобы применялось условие или исключение.</span><span class="sxs-lookup"><span data-stu-id="76873-138">Indicates whether incoming messages must be approval requests in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="76873-139">исаутоматикфорвард</span><span class="sxs-lookup"><span data-stu-id="76873-139">IsAutomaticForward</span></span>](isautomaticforward.md) <br/> |<span data-ttu-id="76873-140">Указывает, должны ли входящие сообщения быть автоматически пересылаться, чтобы применялось условие или исключение.</span><span class="sxs-lookup"><span data-stu-id="76873-140">Indicates whether incoming messages must be automatic forwards in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="76873-141">исаутоматикрепли</span><span class="sxs-lookup"><span data-stu-id="76873-141">IsAutomaticReply</span></span>](isautomaticreply.md) <br/> |<span data-ttu-id="76873-142">Указывает, должны ли входящие сообщения быть автоматическими ответами, чтобы применялось условие или исключение.</span><span class="sxs-lookup"><span data-stu-id="76873-142">Indicates whether incoming messages must be automatic replies in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="76873-143">IsEncrypted</span><span class="sxs-lookup"><span data-stu-id="76873-143">IsEncrypted</span></span>](isencrypted.md) <br/> |<span data-ttu-id="76873-144">Указывает, должны ли входящие сообщения шифроваться с шифрованием S/MIME, чтобы применить условие или исключение.</span><span class="sxs-lookup"><span data-stu-id="76873-144">Indicates whether incoming messages must be S/MIME encrypted in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="76873-145">исмитингрекуест</span><span class="sxs-lookup"><span data-stu-id="76873-145">IsMeetingRequest</span></span>](ismeetingrequest.md) <br/> |<span data-ttu-id="76873-146">Указывает, должны ли входящие сообщения быть приглашениями на собрание, чтобы применялось условие или исключение.</span><span class="sxs-lookup"><span data-stu-id="76873-146">Indicates whether incoming messages must be meeting requests in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="76873-147">исмитингреспонсе</span><span class="sxs-lookup"><span data-stu-id="76873-147">IsMeetingResponse</span></span>](ismeetingresponse.md) <br/> |<span data-ttu-id="76873-148">Указывает, должны ли входящие сообщения отвечать на приглашения на собрания, чтобы применялось условие или исключение.</span><span class="sxs-lookup"><span data-stu-id="76873-148">Indicates whether incoming messages must be meeting responses in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="76873-149">исндр</span><span class="sxs-lookup"><span data-stu-id="76873-149">IsNDR</span></span>](isndr.md) <br/> |<span data-ttu-id="76873-150">Указывает, должны ли входящие сообщения относиться к отчетам о недоставке (NDR), чтобы применялось условие или исключение.</span><span class="sxs-lookup"><span data-stu-id="76873-150">Indicates whether incoming messages must be non-delivery reports (NDRs) in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="76873-151">испермиссионконтроллед</span><span class="sxs-lookup"><span data-stu-id="76873-151">IsPermissionControlled</span></span>](ispermissioncontrolled.md) <br/> |<span data-ttu-id="76873-152">Указывает, должны ли входящие сообщения управляться разрешениями (RMS protected), чтобы применялось условие или исключение.</span><span class="sxs-lookup"><span data-stu-id="76873-152">Indicates whether incoming messages must be permission controlled (RMS protected) in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="76873-153">исреадрецеипт</span><span class="sxs-lookup"><span data-stu-id="76873-153">IsReadReceipt</span></span>](isreadreceipt.md) <br/> |<span data-ttu-id="76873-154">Указывает, должны ли входящие сообщения принимать уведомления о прочтении, чтобы применялось условие или исключение.</span><span class="sxs-lookup"><span data-stu-id="76873-154">Indicates whether incoming messages must be read receipts in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="76873-155">IsSigned</span><span class="sxs-lookup"><span data-stu-id="76873-155">IsSigned</span></span>](issigned.md) <br/> |<span data-ttu-id="76873-156">Указывает, должны ли входящие сообщения быть подписаны на S/MIME, чтобы применялось условие или исключение.</span><span class="sxs-lookup"><span data-stu-id="76873-156">Indicates whether incoming messages must be S/MIME signed in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="76873-157">Голосовая почта</span><span class="sxs-lookup"><span data-stu-id="76873-157">IsVoicemail</span></span>](isvoicemail.md) <br/> |<span data-ttu-id="76873-158">Указывает, должны ли входящие сообщения быть сообщениями голосовой почты, чтобы применялось условие или исключение.</span><span class="sxs-lookup"><span data-stu-id="76873-158">Indicates whether incoming messages must be voice mail messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="76873-159">итемклассес</span><span class="sxs-lookup"><span data-stu-id="76873-159">ItemClasses</span></span>](itemclasses.md) <br/> |<span data-ttu-id="76873-160">Представляет классы элементов, которые должны быть помечены для входящих сообщений, чтобы применить условие или исключение.</span><span class="sxs-lookup"><span data-stu-id="76873-160">Represents the item classes that must be stamped on incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="76873-161">мессажеклассификатионс</span><span class="sxs-lookup"><span data-stu-id="76873-161">MessageClassifications</span></span>](messageclassifications.md) <br/> |<span data-ttu-id="76873-162">Представляет классификации сообщений, которые должны быть помечены для входящих сообщений, чтобы применить условие или исключение.</span><span class="sxs-lookup"><span data-stu-id="76873-162">Represents the message classifications that must be stamped on incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="76873-163">нотсенттоме</span><span class="sxs-lookup"><span data-stu-id="76873-163">NotSentToMe</span></span>](notsenttome.md) <br/> |<span data-ttu-id="76873-164">Указывает, должно ли владелец почтового ящика отсутствовать в свойстве **ToRecipients** входящих сообщений, чтобы применить условие или исключение.</span><span class="sxs-lookup"><span data-stu-id="76873-164">Indicates whether the owner of the mailbox must not be in the **ToRecipients** property of the incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="76873-165">сентккме</span><span class="sxs-lookup"><span data-stu-id="76873-165">SentCcMe</span></span>](sentccme.md) <br/> |<span data-ttu-id="76873-166">Указывает, должно ли владелец почтового ящика находиться в свойстве **CcRecipients** входящих сообщений, чтобы применялось условие или исключение.</span><span class="sxs-lookup"><span data-stu-id="76873-166">Indicates whether the owner of the mailbox has to be in the **CcRecipients** property of incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="76873-167">сентонлитоме</span><span class="sxs-lookup"><span data-stu-id="76873-167">SentOnlyToMe</span></span>](sentonlytome.md) <br/> |<span data-ttu-id="76873-168">Указывает, должен ли владелец почтового ящика быть единственным в свойстве **ToRecipients** входящих сообщений, чтобы применялось условие или исключение.</span><span class="sxs-lookup"><span data-stu-id="76873-168">Indicates whether the owner of the mailbox has to be the only one in the **ToRecipients** property of incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="76873-169">сенттоаддрессес</span><span class="sxs-lookup"><span data-stu-id="76873-169">SentToAddresses</span></span>](senttoaddresses.md) <br/> |<span data-ttu-id="76873-170">Указывает адреса электронной почты, на которые должны быть отправлены входящие сообщения, чтобы применялось условие или исключение.</span><span class="sxs-lookup"><span data-stu-id="76873-170">Indicates the e-mail addresses that incoming messages have to have been sent to in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="76873-171">сенттоме</span><span class="sxs-lookup"><span data-stu-id="76873-171">SentToMe</span></span>](senttome.md) <br/> |<span data-ttu-id="76873-172">Указывает, должно ли владелец почтового ящика находиться в свойстве **ToRecipients** входящих сообщений, чтобы применялось условие или исключение.</span><span class="sxs-lookup"><span data-stu-id="76873-172">Indicates whether the owner of the mailbox has to be in the **ToRecipients** property of incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="76873-173">сенттурккме</span><span class="sxs-lookup"><span data-stu-id="76873-173">SentToOrCcMe</span></span>](senttoorccme.md) <br/> |<span data-ttu-id="76873-174">Указывает, должен ли владелец почтового ящика находиться в свойстве **ToRecipients** или **CcRecipients** входящих сообщений, чтобы применить условие или исключение.</span><span class="sxs-lookup"><span data-stu-id="76873-174">Indicates whether the owner of the mailbox has to be in either a **ToRecipients** or **CcRecipients** property of incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="76873-175">Sensitivity</span><span class="sxs-lookup"><span data-stu-id="76873-175">Sensitivity</span></span>](sensitivity.md) <br/> |<span data-ttu-id="76873-176">Указывает чувствительность, которая должна быть отмечена для входящих сообщений, чтобы применить условие или исключение.</span><span class="sxs-lookup"><span data-stu-id="76873-176">Indicates the sensitivity that must be stamped on incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="76873-177">висиндатеранже</span><span class="sxs-lookup"><span data-stu-id="76873-177">WithinDateRange</span></span>](withindaterange.md) <br/> |<span data-ttu-id="76873-178">Указывает диапазон дат, в течение которого должны быть получены входящие сообщения, чтобы применялось условие или исключение.</span><span class="sxs-lookup"><span data-stu-id="76873-178">Specifies the date range within which incoming messages have to have been received in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="76873-179">висинсизеранже</span><span class="sxs-lookup"><span data-stu-id="76873-179">WithinSizeRange</span></span>](withinsizerange.md) <br/> |<span data-ttu-id="76873-180">Указывает минимальный и максимальный размеры для входящих сообщений, для которых необходимо применить условие или исключение.</span><span class="sxs-lookup"><span data-stu-id="76873-180">Specifies the minimum and maximum sizes that incoming messages must be in order for the condition or exception to apply.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="76873-181">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="76873-181">Parent elements</span></span>

|<span data-ttu-id="76873-182">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="76873-182">**Element**</span></span>|<span data-ttu-id="76873-183">**Описание**</span><span class="sxs-lookup"><span data-stu-id="76873-183">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="76873-184">Правило (RuleType)</span><span class="sxs-lookup"><span data-stu-id="76873-184">Rule (RuleType)</span></span>](rule-ruletype.md) <br/> |<span data-ttu-id="76873-185">Содержит одно правило и представляет правило в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="76873-185">Contains a single rule and represents a rule in a user's mailbox.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="76873-186">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="76873-186">Text value</span></span>

<span data-ttu-id="76873-187">Нет.</span><span class="sxs-lookup"><span data-stu-id="76873-187">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="76873-188">Примечания</span><span class="sxs-lookup"><span data-stu-id="76873-188">Remarks</span></span>

<span data-ttu-id="76873-189">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="76873-189">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="76873-190">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="76873-190">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="76873-191">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="76873-191">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="76873-192">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="76873-192">Schema Name</span></span>  <br/> |<span data-ttu-id="76873-193">Схема Types</span><span class="sxs-lookup"><span data-stu-id="76873-193">Types schema</span></span>  <br/> |
|<span data-ttu-id="76873-194">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="76873-194">Validation File</span></span>  <br/> |<span data-ttu-id="76873-195">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="76873-195">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="76873-196">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="76873-196">Can be Empty</span></span>  <br/> |<span data-ttu-id="76873-197">True</span><span class="sxs-lookup"><span data-stu-id="76873-197">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="76873-198">См. также</span><span class="sxs-lookup"><span data-stu-id="76873-198">See also</span></span>



[<span data-ttu-id="76873-199">Exceptions</span><span class="sxs-lookup"><span data-stu-id="76873-199">Exceptions</span></span>](exceptions.md)


- [<span data-ttu-id="76873-200">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="76873-200">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

