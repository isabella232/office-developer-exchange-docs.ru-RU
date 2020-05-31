---
title: Исключения
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Exceptions
api_type:
- schema
ms.assetid: 7cd63ac2-3441-4ed4-915b-6f90af4b28fc
description: Элемент Exceptions определяет исключения, которые представляют все доступные условия исключения правила для правила папки "Входящие".
ms.openlocfilehash: b875b4dc0029bb9e0bc2bb50c41569fb72ef9268
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762417"
---
# <a name="exceptions"></a><span data-ttu-id="57a1f-103">Исключения</span><span class="sxs-lookup"><span data-stu-id="57a1f-103">Exceptions</span></span>

<span data-ttu-id="57a1f-104">Элемент **exceptions** определяет исключения, которые представляют все доступные условия исключения правила для правила папки "Входящие".</span><span class="sxs-lookup"><span data-stu-id="57a1f-104">The **Exceptions** element identifies the exceptions that represent all the available rule exception conditions for an Inbox rule.</span></span> 
  
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

 <span data-ttu-id="57a1f-105">**рулепредикатестипе**</span><span class="sxs-lookup"><span data-stu-id="57a1f-105">**RulePredicatesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="57a1f-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="57a1f-106">Attributes and elements</span></span>

<span data-ttu-id="57a1f-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="57a1f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="57a1f-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="57a1f-108">Attributes</span></span>

<span data-ttu-id="57a1f-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="57a1f-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="57a1f-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="57a1f-110">Child elements</span></span>

|<span data-ttu-id="57a1f-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="57a1f-111">**Element**</span></span>|<span data-ttu-id="57a1f-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="57a1f-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="57a1f-113">Категории</span><span class="sxs-lookup"><span data-stu-id="57a1f-113">Categories</span></span>](categories-ex15websvcsotherref.md) <br/> |<span data-ttu-id="57a1f-114">Содержит категории, которые необходимо применить к входящему сообщению, чтобы применить условие или исключение.</span><span class="sxs-lookup"><span data-stu-id="57a1f-114">Contains the categories that must be applied to an incoming message in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="57a1f-115">контаинсбодистрингс</span><span class="sxs-lookup"><span data-stu-id="57a1f-115">ContainsBodyStrings</span></span>](containsbodystrings.md) <br/> |<span data-ttu-id="57a1f-116">Указывает строки, которые должны присутствовать в теле входящих сообщений, чтобы применить условие или исключение.</span><span class="sxs-lookup"><span data-stu-id="57a1f-116">Indicates the strings that must appear in the body of incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="57a1f-117">контаиншеадерстрингс</span><span class="sxs-lookup"><span data-stu-id="57a1f-117">ContainsHeaderStrings</span></span>](containsheaderstrings.md) <br/> |<span data-ttu-id="57a1f-118">Индикактес строки, которые должны отображаться в заголовках входящих сообщений, чтобы применить условие или исключение.</span><span class="sxs-lookup"><span data-stu-id="57a1f-118">Indicaqtes the strings that must appear in the headers of incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="57a1f-119">контаинсреЦипиентстрингс</span><span class="sxs-lookup"><span data-stu-id="57a1f-119">ContainsRecipientStrings</span></span>](containsrecipientstrings.md) <br/> |<span data-ttu-id="57a1f-120">Указывает строки, которые должны присутствовать в свойствах **ToRecipients** или **CcRecipients** входящих сообщений, чтобы применялось условие или исключение.</span><span class="sxs-lookup"><span data-stu-id="57a1f-120">Indicates the strings that must appear in either the **ToRecipients** or **CcRecipients** properties of incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="57a1f-121">контаинссендерстрингс</span><span class="sxs-lookup"><span data-stu-id="57a1f-121">ContainsSenderStrings</span></span>](containssenderstrings.md) <br/> |<span data-ttu-id="57a1f-122">Указывает строки, которые должны присутствовать в свойстве **from** входящих сообщений, чтобы применялось условие или исключение.</span><span class="sxs-lookup"><span data-stu-id="57a1f-122">Indicates the strings that must appear in the **From** property of incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="57a1f-123">контаинссубжекторбодистрингс</span><span class="sxs-lookup"><span data-stu-id="57a1f-123">ContainsSubjectOrBodyStrings</span></span>](containssubjectorbodystrings.md) <br/> |<span data-ttu-id="57a1f-124">Указывает строки, которые должны присутствовать в тексте или теме входящих сообщений, чтобы применялось условие или исключение.</span><span class="sxs-lookup"><span data-stu-id="57a1f-124">Indicates the strings that must appear in either the body or the subject of incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="57a1f-125">контаинссубжектстрингс</span><span class="sxs-lookup"><span data-stu-id="57a1f-125">ContainsSubjectStrings</span></span>](containssubjectstrings.md) <br/> |<span data-ttu-id="57a1f-126">Указывает строки, которые должны присутствовать в теме входящих сообщений, чтобы применить условие или исключение.</span><span class="sxs-lookup"><span data-stu-id="57a1f-126">Indicates the strings that must appear in the subject of incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="57a1f-127">флагжедфорактион</span><span class="sxs-lookup"><span data-stu-id="57a1f-127">FlaggedForAction</span></span>](flaggedforaction.md) <br/> |<span data-ttu-id="57a1f-128">Указывает флаг для значения действия, который должен отображаться в входящих сообщениях, чтобы применить условие или исключение.</span><span class="sxs-lookup"><span data-stu-id="57a1f-128">Specifies the flag for action value that must appear on incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="57a1f-129">фромаддрессес</span><span class="sxs-lookup"><span data-stu-id="57a1f-129">FromAddresses</span></span>](fromaddresses.md) <br/> |<span data-ttu-id="57a1f-130">Указывает адреса электронной почты, из которых должны отправляться входящие сообщения, чтобы применялось условие или исключение.</span><span class="sxs-lookup"><span data-stu-id="57a1f-130">Indicates the e-mail addresses from which incoming messages must be sent in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="57a1f-131">фромконнектедаккаунтс</span><span class="sxs-lookup"><span data-stu-id="57a1f-131">FromConnectedAccounts</span></span>](fromconnectedaccounts.md) <br/> |<span data-ttu-id="57a1f-132">Представляет имена учетных записей электронной почты, для которых необходимо выполнить статистическую обработку входящих сообщений для того, чтобы применить условие или исключение.</span><span class="sxs-lookup"><span data-stu-id="57a1f-132">Represents the e-mail account names from which incoming messages have to have been aggregated in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="57a1f-133">HasAttachments</span><span class="sxs-lookup"><span data-stu-id="57a1f-133">HasAttachments</span></span>](hasattachments.md) <br/> |<span data-ttu-id="57a1f-134">Указывает, должны ли входящие сообщения иметь вложения, чтобы применялось условие или исключение.</span><span class="sxs-lookup"><span data-stu-id="57a1f-134">Indicates whether incoming messages have to have attachments in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="57a1f-135">Importance</span><span class="sxs-lookup"><span data-stu-id="57a1f-135">Importance</span></span>](importance.md) <br/> |<span data-ttu-id="57a1f-136">Указывает важность, которая отмечается на входящих сообщениях, чтобы применялось условие или исключение.</span><span class="sxs-lookup"><span data-stu-id="57a1f-136">Specifies the importance that is stamped on incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="57a1f-137">исаппровалрекуест</span><span class="sxs-lookup"><span data-stu-id="57a1f-137">IsApprovalRequest</span></span>](isapprovalrequest.md) <br/> |<span data-ttu-id="57a1f-138">Указывает, должны ли входящие сообщения быть запросами на утверждение, чтобы применялось условие или исключение.</span><span class="sxs-lookup"><span data-stu-id="57a1f-138">Indicates whether incoming messages must be approval requests in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="57a1f-139">исаутоматикфорвард</span><span class="sxs-lookup"><span data-stu-id="57a1f-139">IsAutomaticForward</span></span>](isautomaticforward.md) <br/> |<span data-ttu-id="57a1f-140">Указывает, должны ли входящие сообщения быть автоматически пересылаться, чтобы применялось условие или исключение.</span><span class="sxs-lookup"><span data-stu-id="57a1f-140">Indicates whether incoming messages must be automatic forwards in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="57a1f-141">исаутоматикрепли</span><span class="sxs-lookup"><span data-stu-id="57a1f-141">IsAutomaticReply</span></span>](isautomaticreply.md) <br/> |<span data-ttu-id="57a1f-142">Указывает, должны ли входящие сообщения быть автоматическими ответами, чтобы применялось условие или исключение.</span><span class="sxs-lookup"><span data-stu-id="57a1f-142">Indicates whether incoming messages must be automatic replies in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="57a1f-143">IsEncrypted</span><span class="sxs-lookup"><span data-stu-id="57a1f-143">IsEncrypted</span></span>](isencrypted.md) <br/> |<span data-ttu-id="57a1f-144">Указывает, должны ли входящие сообщения шифроваться с шифрованием S/MIME, чтобы применить условие или исключение.</span><span class="sxs-lookup"><span data-stu-id="57a1f-144">Indicates whether incoming messages must be S/MIME encrypted in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="57a1f-145">исмитингрекуест</span><span class="sxs-lookup"><span data-stu-id="57a1f-145">IsMeetingRequest</span></span>](ismeetingrequest.md) <br/> |<span data-ttu-id="57a1f-146">Указывает, должны ли входящие сообщения быть приглашениями на собрание, чтобы применялось условие или исключение.</span><span class="sxs-lookup"><span data-stu-id="57a1f-146">Indicates whether incoming messages must be meeting requests in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="57a1f-147">исмитингреспонсе</span><span class="sxs-lookup"><span data-stu-id="57a1f-147">IsMeetingResponse</span></span>](ismeetingresponse.md) <br/> |<span data-ttu-id="57a1f-148">Указывает, должны ли входящие сообщения отвечать на приглашения на собрания, чтобы применялось условие или исключение.</span><span class="sxs-lookup"><span data-stu-id="57a1f-148">Indicates whether incoming messages must be meeting responses in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="57a1f-149">исндр</span><span class="sxs-lookup"><span data-stu-id="57a1f-149">IsNDR</span></span>](isndr.md) <br/> |<span data-ttu-id="57a1f-150">Указывает, должны ли входящие сообщения относиться к отчетам о недоставке (NDR), чтобы применялось условие или исключение.</span><span class="sxs-lookup"><span data-stu-id="57a1f-150">Indicates whether incoming messages must be non-delivery reports (NDRs) in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="57a1f-151">испермиссионконтроллед</span><span class="sxs-lookup"><span data-stu-id="57a1f-151">IsPermissionControlled</span></span>](ispermissioncontrolled.md) <br/> |<span data-ttu-id="57a1f-152">Указывает, должны ли входящие сообщения управляться с помощью управления разрешениями (RMS protected), чтобы применить условие или исключение.</span><span class="sxs-lookup"><span data-stu-id="57a1f-152">Indicates whether incoming messages must be permission controlled (RMS protected) in order for the condition or exception to apply</span></span>  <br/> |
|[<span data-ttu-id="57a1f-153">исреадрецеипт</span><span class="sxs-lookup"><span data-stu-id="57a1f-153">IsReadReceipt</span></span>](isreadreceipt.md) <br/> |<span data-ttu-id="57a1f-154">Указывает, должны ли входящие сообщения принимать уведомления о прочтении, чтобы применялось условие или исключение.</span><span class="sxs-lookup"><span data-stu-id="57a1f-154">Indicates whether incoming messages must be read receipts in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="57a1f-155">IsSigned</span><span class="sxs-lookup"><span data-stu-id="57a1f-155">IsSigned</span></span>](issigned.md) <br/> |<span data-ttu-id="57a1f-156">Указывает, должны ли входящие сообщения быть подписаны на S/MIME, чтобы применялось условие или исключение.</span><span class="sxs-lookup"><span data-stu-id="57a1f-156">Indicates whether incoming messages must be S/MIME signed in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="57a1f-157">Голосовая почта</span><span class="sxs-lookup"><span data-stu-id="57a1f-157">IsVoicemail</span></span>](isvoicemail.md) <br/> |<span data-ttu-id="57a1f-158">Указывает, должны ли входящие сообщения быть сообщениями голосовой почты, чтобы применялось условие или исключение.</span><span class="sxs-lookup"><span data-stu-id="57a1f-158">Indicates whether incoming messages must be voice mail messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="57a1f-159">итемклассес</span><span class="sxs-lookup"><span data-stu-id="57a1f-159">ItemClasses</span></span>](itemclasses.md) <br/> |<span data-ttu-id="57a1f-160">Представляет классы элементов, которые должны быть помечены для входящих сообщений, чтобы применить условие или исключение.</span><span class="sxs-lookup"><span data-stu-id="57a1f-160">Represents the item classes that must be stamped on incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="57a1f-161">мессажеклассификатионс</span><span class="sxs-lookup"><span data-stu-id="57a1f-161">MessageClassifications</span></span>](messageclassifications.md) <br/> |<span data-ttu-id="57a1f-162">Представляет классификации сообщений, которые должны быть помечены для входящих сообщений, чтобы применить условие или исключение.</span><span class="sxs-lookup"><span data-stu-id="57a1f-162">Represents the message classifications that must be stamped on incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="57a1f-163">нотсенттоме</span><span class="sxs-lookup"><span data-stu-id="57a1f-163">NotSentToMe</span></span>](notsenttome.md) <br/> |<span data-ttu-id="57a1f-164">Указывает, должно ли владелец почтового ящика отсутствовать в свойстве **ToRecipients** входящих сообщений, чтобы применить условие или исключение.</span><span class="sxs-lookup"><span data-stu-id="57a1f-164">Indicates whether the owner of the mailbox must not be in the **ToRecipients** property of the incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="57a1f-165">сентккме</span><span class="sxs-lookup"><span data-stu-id="57a1f-165">SentCcMe</span></span>](sentccme.md) <br/> |<span data-ttu-id="57a1f-166">Указывает, должно ли владелец почтового ящика находиться в свойстве **CcRecipients** входящих сообщений, чтобы применялось условие или исключение.</span><span class="sxs-lookup"><span data-stu-id="57a1f-166">Indicates whether the owner of the mailbox has to be in the **CcRecipients** property of incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="57a1f-167">сентонлитоме</span><span class="sxs-lookup"><span data-stu-id="57a1f-167">SentOnlyToMe</span></span>](sentonlytome.md) <br/> |<span data-ttu-id="57a1f-168">Указывает, должен ли владелец почтового ящика быть единственным в свойстве **ToRecipients** входящих сообщений, чтобы применялось условие или исключение.</span><span class="sxs-lookup"><span data-stu-id="57a1f-168">Indicates whether the owner of the mailbox has to be the only one in the **ToRecipients** property of incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="57a1f-169">сенттоаддрессес</span><span class="sxs-lookup"><span data-stu-id="57a1f-169">SentToAddresses</span></span>](senttoaddresses.md) <br/> |<span data-ttu-id="57a1f-170">Указывает адреса электронной почты, на которые должны быть отправлены входящие сообщения, чтобы применялось условие или исключение.</span><span class="sxs-lookup"><span data-stu-id="57a1f-170">Indicates the e-mail addresses that incoming messages have to have been sent to in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="57a1f-171">сенттоме</span><span class="sxs-lookup"><span data-stu-id="57a1f-171">SentToMe</span></span>](senttome.md) <br/> |<span data-ttu-id="57a1f-172">Указывает, должно ли владелец почтового ящика находиться в свойстве **ToRecipients** входящих сообщений, чтобы применялось условие или исключение.</span><span class="sxs-lookup"><span data-stu-id="57a1f-172">Indicates whether the owner of the mailbox has to be in the **ToRecipients** property of incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="57a1f-173">сенттурккме</span><span class="sxs-lookup"><span data-stu-id="57a1f-173">SentToOrCcMe</span></span>](senttoorccme.md) <br/> |<span data-ttu-id="57a1f-174">Указывает, должен ли владелец почтового ящика находиться в свойстве **ToRecipients** или **CcRecipients** входящих сообщений, чтобы применить условие или исключение.</span><span class="sxs-lookup"><span data-stu-id="57a1f-174">Indicates whether the owner of the mailbox has to be in either a **ToRecipients** or **CcRecipients** property of incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="57a1f-175">Sensitivity</span><span class="sxs-lookup"><span data-stu-id="57a1f-175">Sensitivity</span></span>](sensitivity.md) <br/> |<span data-ttu-id="57a1f-176">Указывает чувствительность, которая должна быть отмечена для входящих сообщений, чтобы применить условие или исключение.</span><span class="sxs-lookup"><span data-stu-id="57a1f-176">Indicates the sensitivity that must be stamped on incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="57a1f-177">висиндатеранже</span><span class="sxs-lookup"><span data-stu-id="57a1f-177">WithinDateRange</span></span>](withindaterange.md) <br/> |<span data-ttu-id="57a1f-178">Указывает диапазон дат, в течение которого должны быть получены входящие сообщения, чтобы применялось условие или исключение.</span><span class="sxs-lookup"><span data-stu-id="57a1f-178">Specifies the date range within which incoming messages have to have been received in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="57a1f-179">висинсизеранже</span><span class="sxs-lookup"><span data-stu-id="57a1f-179">WithinSizeRange</span></span>](withinsizerange.md) <br/> |<span data-ttu-id="57a1f-180">Указывает минимальный и максимальный размеры для входящих сообщений, для которых необходимо применить условие или исключение.</span><span class="sxs-lookup"><span data-stu-id="57a1f-180">Specifies the minimum and maximum sizes that incoming messages must be in order for the condition or exception to apply.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="57a1f-181">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="57a1f-181">Parent elements</span></span>

|<span data-ttu-id="57a1f-182">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="57a1f-182">**Element**</span></span>|<span data-ttu-id="57a1f-183">**Описание**</span><span class="sxs-lookup"><span data-stu-id="57a1f-183">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="57a1f-184">Правило (RuleType)</span><span class="sxs-lookup"><span data-stu-id="57a1f-184">Rule (RuleType)</span></span>](rule-ruletype.md) <br/> |<span data-ttu-id="57a1f-185">Содержит одно правило и представляет правило в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="57a1f-185">Contains a single rule and represents a rule in a user's mailbox.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="57a1f-186">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="57a1f-186">Text value</span></span>

<span data-ttu-id="57a1f-187">Нет.</span><span class="sxs-lookup"><span data-stu-id="57a1f-187">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="57a1f-188">Примечания</span><span class="sxs-lookup"><span data-stu-id="57a1f-188">Remarks</span></span>

<span data-ttu-id="57a1f-189">Предикаты правил используются в качестве условий правил или исключений.</span><span class="sxs-lookup"><span data-stu-id="57a1f-189">The rule predicates are used as rule conditions or exceptions.</span></span>
  
<span data-ttu-id="57a1f-190">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="57a1f-190">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="57a1f-191">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="57a1f-191">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="57a1f-192">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="57a1f-192">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="57a1f-193">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="57a1f-193">Schema Name</span></span>  <br/> |<span data-ttu-id="57a1f-194">Схема Types</span><span class="sxs-lookup"><span data-stu-id="57a1f-194">Types schema</span></span>  <br/> |
|<span data-ttu-id="57a1f-195">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="57a1f-195">Validation File</span></span>  <br/> |<span data-ttu-id="57a1f-196">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="57a1f-196">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="57a1f-197">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="57a1f-197">Can be Empty</span></span>  <br/> |<span data-ttu-id="57a1f-198">True</span><span class="sxs-lookup"><span data-stu-id="57a1f-198">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="57a1f-199">См. также</span><span class="sxs-lookup"><span data-stu-id="57a1f-199">See also</span></span>



[<span data-ttu-id="57a1f-200">Conditions</span><span class="sxs-lookup"><span data-stu-id="57a1f-200">Conditions</span></span>](conditions.md)


- [<span data-ttu-id="57a1f-201">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="57a1f-201">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

