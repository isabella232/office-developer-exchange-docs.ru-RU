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
description: Элемент исключения определяет исключения, которые представляют все доступные правила условия исключений для правила папки «Входящие».
ms.openlocfilehash: b875b4dc0029bb9e0bc2bb50c41569fb72ef9268
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762417"
---
# <a name="exceptions"></a><span data-ttu-id="c1cbc-103">Исключения</span><span class="sxs-lookup"><span data-stu-id="c1cbc-103">Exceptions</span></span>

<span data-ttu-id="c1cbc-104">Элемент **исключения** определяет исключения, которые представляют все доступные правила условия исключений для правила папки «Входящие».</span><span class="sxs-lookup"><span data-stu-id="c1cbc-104">The **Exceptions** element identifies the exceptions that represent all the available rule exception conditions for an Inbox rule.</span></span> 
  
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

 <span data-ttu-id="c1cbc-105">**RulePredicatesType**</span><span class="sxs-lookup"><span data-stu-id="c1cbc-105">**RulePredicatesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c1cbc-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="c1cbc-106">Attributes and elements</span></span>

<span data-ttu-id="c1cbc-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="c1cbc-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c1cbc-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="c1cbc-108">Attributes</span></span>

<span data-ttu-id="c1cbc-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="c1cbc-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c1cbc-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="c1cbc-110">Child elements</span></span>

|<span data-ttu-id="c1cbc-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="c1cbc-111">**Element**</span></span>|<span data-ttu-id="c1cbc-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="c1cbc-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c1cbc-113">Категории</span><span class="sxs-lookup"><span data-stu-id="c1cbc-113">Categories</span></span>](categories-ex15websvcsotherref.md) <br/> |<span data-ttu-id="c1cbc-114">Содержит категории, которые должны применяться к входящего сообщения в порядке для условие или исключение для применения.</span><span class="sxs-lookup"><span data-stu-id="c1cbc-114">Contains the categories that must be applied to an incoming message in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="c1cbc-115">ContainsBodyStrings</span><span class="sxs-lookup"><span data-stu-id="c1cbc-115">ContainsBodyStrings</span></span>](containsbodystrings.md) <br/> |<span data-ttu-id="c1cbc-116">Указывает строк, которые должны встречаться в теле входящих сообщений в порядке для условие или исключение для применения.</span><span class="sxs-lookup"><span data-stu-id="c1cbc-116">Indicates the strings that must appear in the body of incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="c1cbc-117">ContainsHeaderStrings</span><span class="sxs-lookup"><span data-stu-id="c1cbc-117">ContainsHeaderStrings</span></span>](containsheaderstrings.md) <br/> |<span data-ttu-id="c1cbc-118">Indicaqtes строк, которые должны встречаться в заголовках входящих сообщений в порядке для условие или исключение для применения.</span><span class="sxs-lookup"><span data-stu-id="c1cbc-118">Indicaqtes the strings that must appear in the headers of incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="c1cbc-119">ContainsRecipientStrings</span><span class="sxs-lookup"><span data-stu-id="c1cbc-119">ContainsRecipientStrings</span></span>](containsrecipientstrings.md) <br/> |<span data-ttu-id="c1cbc-120">Указывает строк, которые должны встречаться в параметр **ToRecipients** или **CcRecipients** свойства входящих сообщений в порядке для условие или исключение для применения.</span><span class="sxs-lookup"><span data-stu-id="c1cbc-120">Indicates the strings that must appear in either the **ToRecipients** or **CcRecipients** properties of incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="c1cbc-121">ContainsSenderStrings</span><span class="sxs-lookup"><span data-stu-id="c1cbc-121">ContainsSenderStrings</span></span>](containssenderstrings.md) <br/> |<span data-ttu-id="c1cbc-122">Указывает строк, которые должны встречаться в свойстве **из** входящих сообщений в порядке для условие или исключение для применения.</span><span class="sxs-lookup"><span data-stu-id="c1cbc-122">Indicates the strings that must appear in the **From** property of incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="c1cbc-123">ContainsSubjectOrBodyStrings</span><span class="sxs-lookup"><span data-stu-id="c1cbc-123">ContainsSubjectOrBodyStrings</span></span>](containssubjectorbodystrings.md) <br/> |<span data-ttu-id="c1cbc-124">Указывает строк, которые должны встречаться в тексте или теме входящих сообщений в порядке для условие или исключение для применения.</span><span class="sxs-lookup"><span data-stu-id="c1cbc-124">Indicates the strings that must appear in either the body or the subject of incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="c1cbc-125">ContainsSubjectStrings</span><span class="sxs-lookup"><span data-stu-id="c1cbc-125">ContainsSubjectStrings</span></span>](containssubjectstrings.md) <br/> |<span data-ttu-id="c1cbc-126">Указывает строк, которые должны встречаться в теме входящих сообщений в порядке для условие или исключение для применения.</span><span class="sxs-lookup"><span data-stu-id="c1cbc-126">Indicates the strings that must appear in the subject of incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="c1cbc-127">FlaggedForAction</span><span class="sxs-lookup"><span data-stu-id="c1cbc-127">FlaggedForAction</span></span>](flaggedforaction.md) <br/> |<span data-ttu-id="c1cbc-128">Задает флаг, для которого действию задано значение, которое должно отображаться на входящих сообщений в порядке для условие или исключение для применения.</span><span class="sxs-lookup"><span data-stu-id="c1cbc-128">Specifies the flag for action value that must appear on incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="c1cbc-129">FromAddresses</span><span class="sxs-lookup"><span data-stu-id="c1cbc-129">FromAddresses</span></span>](fromaddresses.md) <br/> |<span data-ttu-id="c1cbc-130">Указывает адреса электронной почты, из которых необходимо отправить входящих сообщений в порядке для условие или исключение для применения.</span><span class="sxs-lookup"><span data-stu-id="c1cbc-130">Indicates the e-mail addresses from which incoming messages must be sent in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="c1cbc-131">FromConnectedAccounts</span><span class="sxs-lookup"><span data-stu-id="c1cbc-131">FromConnectedAccounts</span></span>](fromconnectedaccounts.md) <br/> |<span data-ttu-id="c1cbc-132">Представляет имена учетных записей электронной почты, из которых нужно были сводный в порядке для условие или исключение для применения входящих сообщений.</span><span class="sxs-lookup"><span data-stu-id="c1cbc-132">Represents the e-mail account names from which incoming messages have to have been aggregated in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="c1cbc-133">HasAttachments</span><span class="sxs-lookup"><span data-stu-id="c1cbc-133">HasAttachments</span></span>](hasattachments.md) <br/> |<span data-ttu-id="c1cbc-134">Указывает, будет ли входящих сообщений для получения вложений в порядке для условие или исключение для применения.</span><span class="sxs-lookup"><span data-stu-id="c1cbc-134">Indicates whether incoming messages have to have attachments in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="c1cbc-135">Важность</span><span class="sxs-lookup"><span data-stu-id="c1cbc-135">Importance</span></span>](importance.md) <br/> |<span data-ttu-id="c1cbc-136">Указывает важность, записывается во входящих сообщениях в порядке для условие или исключение для применения.</span><span class="sxs-lookup"><span data-stu-id="c1cbc-136">Specifies the importance that is stamped on incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="c1cbc-137">IsApprovalRequest</span><span class="sxs-lookup"><span data-stu-id="c1cbc-137">IsApprovalRequest</span></span>](isapprovalrequest.md) <br/> |<span data-ttu-id="c1cbc-138">Указывает, должен ли входящих сообщений запросов на утверждение в порядке для условие или исключение для применения.</span><span class="sxs-lookup"><span data-stu-id="c1cbc-138">Indicates whether incoming messages must be approval requests in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="c1cbc-139">IsAutomaticForward</span><span class="sxs-lookup"><span data-stu-id="c1cbc-139">IsAutomaticForward</span></span>](isautomaticforward.md) <br/> |<span data-ttu-id="c1cbc-140">Указывает, должен ли входящих сообщений автоматическая переадресация в порядке для условие или исключение для применения.</span><span class="sxs-lookup"><span data-stu-id="c1cbc-140">Indicates whether incoming messages must be automatic forwards in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="c1cbc-141">IsAutomaticReply</span><span class="sxs-lookup"><span data-stu-id="c1cbc-141">IsAutomaticReply</span></span>](isautomaticreply.md) <br/> |<span data-ttu-id="c1cbc-142">Указывает, должен ли входящих сообщений автоматических ответов в порядке для условие или исключение для применения.</span><span class="sxs-lookup"><span data-stu-id="c1cbc-142">Indicates whether incoming messages must be automatic replies in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="c1cbc-143">IsEncrypted</span><span class="sxs-lookup"><span data-stu-id="c1cbc-143">IsEncrypted</span></span>](isencrypted.md) <br/> |<span data-ttu-id="c1cbc-144">Указывает, будет ли входящих сообщений должен быть зашифрован в порядке для условие или исключение для применения S/MIME.</span><span class="sxs-lookup"><span data-stu-id="c1cbc-144">Indicates whether incoming messages must be S/MIME encrypted in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="c1cbc-145">IsMeetingRequest</span><span class="sxs-lookup"><span data-stu-id="c1cbc-145">IsMeetingRequest</span></span>](ismeetingrequest.md) <br/> |<span data-ttu-id="c1cbc-146">Указывает, будет ли входящих сообщений должны быть приглашений на собрания в порядке для условие или исключение для применения.</span><span class="sxs-lookup"><span data-stu-id="c1cbc-146">Indicates whether incoming messages must be meeting requests in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="c1cbc-147">IsMeetingResponse</span><span class="sxs-lookup"><span data-stu-id="c1cbc-147">IsMeetingResponse</span></span>](ismeetingresponse.md) <br/> |<span data-ttu-id="c1cbc-148">Указывает, должен ли собрания ответы в порядке для условие или исключение для применения входящих сообщений.</span><span class="sxs-lookup"><span data-stu-id="c1cbc-148">Indicates whether incoming messages must be meeting responses in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="c1cbc-149">IsNDR</span><span class="sxs-lookup"><span data-stu-id="c1cbc-149">IsNDR</span></span>](isndr.md) <br/> |<span data-ttu-id="c1cbc-150">Указывает, должен ли входящих сообщений отчеты о недоставке (NDR) в порядке для условие или исключение для применения.</span><span class="sxs-lookup"><span data-stu-id="c1cbc-150">Indicates whether incoming messages must be non-delivery reports (NDRs) in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="c1cbc-151">IsPermissionControlled</span><span class="sxs-lookup"><span data-stu-id="c1cbc-151">IsPermissionControlled</span></span>](ispermissioncontrolled.md) <br/> |<span data-ttu-id="c1cbc-152">Указывает, входящих сообщений должен ли разрешение управляются (защищенные RMS) в порядке для условие или исключение для применения</span><span class="sxs-lookup"><span data-stu-id="c1cbc-152">Indicates whether incoming messages must be permission controlled (RMS protected) in order for the condition or exception to apply</span></span>  <br/> |
|[<span data-ttu-id="c1cbc-153">IsReadReceipt</span><span class="sxs-lookup"><span data-stu-id="c1cbc-153">IsReadReceipt</span></span>](isreadreceipt.md) <br/> |<span data-ttu-id="c1cbc-154">Указывает, должны ли прочитать поступлений в порядке для условие или исключение для применения входящих сообщений.</span><span class="sxs-lookup"><span data-stu-id="c1cbc-154">Indicates whether incoming messages must be read receipts in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="c1cbc-155">IsSigned</span><span class="sxs-lookup"><span data-stu-id="c1cbc-155">IsSigned</span></span>](issigned.md) <br/> |<span data-ttu-id="c1cbc-156">Указывает, должен ли входящих сообщений в порядке для условие или исключение для применения подписью S/MIME.</span><span class="sxs-lookup"><span data-stu-id="c1cbc-156">Indicates whether incoming messages must be S/MIME signed in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="c1cbc-157">IsVoicemail</span><span class="sxs-lookup"><span data-stu-id="c1cbc-157">IsVoicemail</span></span>](isvoicemail.md) <br/> |<span data-ttu-id="c1cbc-158">Указывает, должен ли входящих сообщений сообщения голосовой почты в порядке для условие или исключение для применения.</span><span class="sxs-lookup"><span data-stu-id="c1cbc-158">Indicates whether incoming messages must be voice mail messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="c1cbc-159">ItemClasses</span><span class="sxs-lookup"><span data-stu-id="c1cbc-159">ItemClasses</span></span>](itemclasses.md) <br/> |<span data-ttu-id="c1cbc-160">Представляет элемент классы, которые необходимо ставится отметка для входящих сообщений в порядке для условие или исключение для применения.</span><span class="sxs-lookup"><span data-stu-id="c1cbc-160">Represents the item classes that must be stamped on incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="c1cbc-161">MessageClassifications</span><span class="sxs-lookup"><span data-stu-id="c1cbc-161">MessageClassifications</span></span>](messageclassifications.md) <br/> |<span data-ttu-id="c1cbc-162">Представляет классификации сообщений, которые необходимо ставится отметка для входящих сообщений в порядке для условие или исключение для применения.</span><span class="sxs-lookup"><span data-stu-id="c1cbc-162">Represents the message classifications that must be stamped on incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="c1cbc-163">NotSentToMe</span><span class="sxs-lookup"><span data-stu-id="c1cbc-163">NotSentToMe</span></span>](notsenttome.md) <br/> |<span data-ttu-id="c1cbc-164">Указывает, является ли владелец почтового ящика не должна быть в свойстве **ToRecipients** входящих сообщений в порядке для условие или исключение для применения.</span><span class="sxs-lookup"><span data-stu-id="c1cbc-164">Indicates whether the owner of the mailbox must not be in the **ToRecipients** property of the incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="c1cbc-165">SentCcMe</span><span class="sxs-lookup"><span data-stu-id="c1cbc-165">SentCcMe</span></span>](sentccme.md) <br/> |<span data-ttu-id="c1cbc-166">Указывает, имеет ли владельца почтового ящика в свойство **CcRecipients** входящих сообщений в порядке для условие или исключение для применения.</span><span class="sxs-lookup"><span data-stu-id="c1cbc-166">Indicates whether the owner of the mailbox has to be in the **CcRecipients** property of incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="c1cbc-167">SentOnlyToMe</span><span class="sxs-lookup"><span data-stu-id="c1cbc-167">SentOnlyToMe</span></span>](sentonlytome.md) <br/> |<span data-ttu-id="c1cbc-168">Указывает, является ли владелец почтового ящика должен быть только один в свойстве **ToRecipients** входящих сообщений в порядке для условие или исключение для применения.</span><span class="sxs-lookup"><span data-stu-id="c1cbc-168">Indicates whether the owner of the mailbox has to be the only one in the **ToRecipients** property of incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="c1cbc-169">SentToAddresses</span><span class="sxs-lookup"><span data-stu-id="c1cbc-169">SentToAddresses</span></span>](senttoaddresses.md) <br/> |<span data-ttu-id="c1cbc-170">Указывает адреса электронной почты, которые должны входящих сообщений, отправленных в порядке для условие или исключение для применения.</span><span class="sxs-lookup"><span data-stu-id="c1cbc-170">Indicates the e-mail addresses that incoming messages have to have been sent to in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="c1cbc-171">SentToMe</span><span class="sxs-lookup"><span data-stu-id="c1cbc-171">SentToMe</span></span>](senttome.md) <br/> |<span data-ttu-id="c1cbc-172">Указывает, имеет ли владельца почтового ящика в свойство **ToRecipients** входящих сообщений в порядке для условие или исключение для применения.</span><span class="sxs-lookup"><span data-stu-id="c1cbc-172">Indicates whether the owner of the mailbox has to be in the **ToRecipients** property of incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="c1cbc-173">SentToOrCcMe</span><span class="sxs-lookup"><span data-stu-id="c1cbc-173">SentToOrCcMe</span></span>](senttoorccme.md) <br/> |<span data-ttu-id="c1cbc-174">Указывает, имеет ли владельца почтового ящика в **CcRecipients** или в **ToRecipients** свойство входящих сообщений в порядке для условие или исключение для применения.</span><span class="sxs-lookup"><span data-stu-id="c1cbc-174">Indicates whether the owner of the mailbox has to be in either a **ToRecipients** or **CcRecipients** property of incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="c1cbc-175">Уровень конфиденциальности сообщения</span><span class="sxs-lookup"><span data-stu-id="c1cbc-175">Sensitivity</span></span>](sensitivity.md) <br/> |<span data-ttu-id="c1cbc-176">Указывает уровень конфиденциальности сообщения, которое необходимо ставится отметка для входящих сообщений в порядке для условие или исключение для применения.</span><span class="sxs-lookup"><span data-stu-id="c1cbc-176">Indicates the sensitivity that must be stamped on incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="c1cbc-177">WithinDateRange</span><span class="sxs-lookup"><span data-stu-id="c1cbc-177">WithinDateRange</span></span>](withindaterange.md) <br/> |<span data-ttu-id="c1cbc-178">Указывает диапазон дат, в течение которого нужно были получены в порядке для условие или исключение для применения входящих сообщений.</span><span class="sxs-lookup"><span data-stu-id="c1cbc-178">Specifies the date range within which incoming messages have to have been received in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="c1cbc-179">WithinSizeRange</span><span class="sxs-lookup"><span data-stu-id="c1cbc-179">WithinSizeRange</span></span>](withinsizerange.md) <br/> |<span data-ttu-id="c1cbc-180">Указывает минимальный и максимальный размеры, которые должны быть входящих сообщений в порядке для условие или исключение для применения.</span><span class="sxs-lookup"><span data-stu-id="c1cbc-180">Specifies the minimum and maximum sizes that incoming messages must be in order for the condition or exception to apply.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="c1cbc-181">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="c1cbc-181">Parent elements</span></span>

|<span data-ttu-id="c1cbc-182">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="c1cbc-182">**Element**</span></span>|<span data-ttu-id="c1cbc-183">**Описание**</span><span class="sxs-lookup"><span data-stu-id="c1cbc-183">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c1cbc-184">Правило (RuleType)</span><span class="sxs-lookup"><span data-stu-id="c1cbc-184">Rule (RuleType)</span></span>](rule-ruletype.md) <br/> |<span data-ttu-id="c1cbc-185">Содержит одно правило и представляет правило в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="c1cbc-185">Contains a single rule and represents a rule in a user's mailbox.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="c1cbc-186">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="c1cbc-186">Text value</span></span>

<span data-ttu-id="c1cbc-187">Нет.</span><span class="sxs-lookup"><span data-stu-id="c1cbc-187">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="c1cbc-188">Замечания</span><span class="sxs-lookup"><span data-stu-id="c1cbc-188">Remarks</span></span>

<span data-ttu-id="c1cbc-189">Предикаты правила используются как правила условий и исключений.</span><span class="sxs-lookup"><span data-stu-id="c1cbc-189">The rule predicates are used as rule conditions or exceptions.</span></span>
  
<span data-ttu-id="c1cbc-190">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="c1cbc-190">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c1cbc-191">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="c1cbc-191">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c1cbc-192">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="c1cbc-192">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="c1cbc-193">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="c1cbc-193">Schema Name</span></span>  <br/> |<span data-ttu-id="c1cbc-194">Схема Types</span><span class="sxs-lookup"><span data-stu-id="c1cbc-194">Types schema</span></span>  <br/> |
|<span data-ttu-id="c1cbc-195">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="c1cbc-195">Validation File</span></span>  <br/> |<span data-ttu-id="c1cbc-196">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="c1cbc-196">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="c1cbc-197">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="c1cbc-197">Can be Empty</span></span>  <br/> |<span data-ttu-id="c1cbc-198">True</span><span class="sxs-lookup"><span data-stu-id="c1cbc-198">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c1cbc-199">См. также</span><span class="sxs-lookup"><span data-stu-id="c1cbc-199">See also</span></span>



[<span data-ttu-id="c1cbc-200">Условия</span><span class="sxs-lookup"><span data-stu-id="c1cbc-200">Conditions</span></span>](conditions.md)


- [<span data-ttu-id="c1cbc-201">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="c1cbc-201">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

