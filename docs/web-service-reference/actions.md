---
title: Действия
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Actions
api_type:
- schema
ms.assetid: c5aa96b1-2d8b-422f-8c2f-f118572ab23f
description: Элемент Actions представляет набор действий, которые доступны для выполнения на сообщение при условия будут выполнены.
ms.openlocfilehash: 093d2f28135c6077b6cea488591573af0182934b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761330"
---
# <a name="actions"></a><span data-ttu-id="c2bd7-103">Действия</span><span class="sxs-lookup"><span data-stu-id="c2bd7-103">Actions</span></span>

<span data-ttu-id="c2bd7-104">Элемент **Actions** представляет набор действий, которые доступны для выполнения на сообщение при условия будут выполнены.</span><span class="sxs-lookup"><span data-stu-id="c2bd7-104">The **Actions** element represents the set of actions that are available to be taken on a message when the conditions are fulfilled.</span></span> 
  
[<span data-ttu-id="c2bd7-105">Правило (RuleType)</span><span class="sxs-lookup"><span data-stu-id="c2bd7-105">Rule (RuleType)</span></span>](rule-ruletype.md)
  
```XML
<Actions>
    <AssignCategories>
    <CopyToFolder>
    <Delete>
    <ForwardAsAttachmentToRecipients>
    <ForwardToRecipients>
    <MarkImportance>
    <MarkAsRead>
    <MoveToFolder>
    <PermanentDelete>
    <RedirectToRecipients>
    <SendSMSAlertToRecipients>
    <ServerReplyWithMessage>
    <StopProcessingRules>
</Actions>
```

 <span data-ttu-id="c2bd7-106">**RuleActionsType**</span><span class="sxs-lookup"><span data-stu-id="c2bd7-106">**RuleActionsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c2bd7-107">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="c2bd7-107">Attributes and elements</span></span>

<span data-ttu-id="c2bd7-108">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="c2bd7-108">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c2bd7-109">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="c2bd7-109">Attributes</span></span>

<span data-ttu-id="c2bd7-110">Нет.</span><span class="sxs-lookup"><span data-stu-id="c2bd7-110">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c2bd7-111">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="c2bd7-111">Child elements</span></span>

|<span data-ttu-id="c2bd7-112">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="c2bd7-112">**Element**</span></span>|<span data-ttu-id="c2bd7-113">**Описание**</span><span class="sxs-lookup"><span data-stu-id="c2bd7-113">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c2bd7-114">AssignCategories</span><span class="sxs-lookup"><span data-stu-id="c2bd7-114">AssignCategories</span></span>](assigncategories.md) <br/> |<span data-ttu-id="c2bd7-115">Представляет категории, которые имеют на сообщения электронной почты.</span><span class="sxs-lookup"><span data-stu-id="c2bd7-115">Represents the categories that are stamped on e-mail messages.</span></span>  <br/> |
|[<span data-ttu-id="c2bd7-116">CopyToFolder</span><span class="sxs-lookup"><span data-stu-id="c2bd7-116">CopyToFolder</span></span>](copytofolder.md) <br/> |<span data-ttu-id="c2bd7-117">Определение идентификатора к папке, где будет скопировано элементов электронной почты.</span><span class="sxs-lookup"><span data-stu-id="c2bd7-117">Identifies the ID of the folder that e-mail items will be copied to.</span></span>  <br/> |
|<span data-ttu-id="c2bd7-118">[удаление](delete.md);</span><span class="sxs-lookup"><span data-stu-id="c2bd7-118">[Delete](delete.md)</span></span> <br/> |<span data-ttu-id="c2bd7-119">Указывает, будет ли сообщений перемещаются в папку «Удаленные».</span><span class="sxs-lookup"><span data-stu-id="c2bd7-119">Indicates whether messages are to be moved to the Deleted Items folder.</span></span>  <br/> |
|[<span data-ttu-id="c2bd7-120">ForwardAsAttachmentToRecipients</span><span class="sxs-lookup"><span data-stu-id="c2bd7-120">ForwardAsAttachmentToRecipients</span></span>](forwardasattachmenttorecipients.md) <br/> |<span data-ttu-id="c2bd7-121">Указывает адреса электронной почты, к которым сообщения, пересылаемые в виде вложений.</span><span class="sxs-lookup"><span data-stu-id="c2bd7-121">Indicates the e-mail addresses to which messages are to be forwarded as attachments.</span></span>  <br/> |
|[<span data-ttu-id="c2bd7-122">ForwardToRecipients</span><span class="sxs-lookup"><span data-stu-id="c2bd7-122">ForwardToRecipients</span></span>](forwardtorecipients.md) <br/> |<span data-ttu-id="c2bd7-123">Указывает адреса электронной почты, к которым сообщения, для перенаправления.</span><span class="sxs-lookup"><span data-stu-id="c2bd7-123">Indicates the e-mail addresses to which messages are to be forwarded.</span></span>  <br/> |
|[<span data-ttu-id="c2bd7-124">MarkImportance</span><span class="sxs-lookup"><span data-stu-id="c2bd7-124">MarkImportance</span></span>](markimportance.md) <br/> |<span data-ttu-id="c2bd7-125">Задает важность, ставится отметка в сообщениях.</span><span class="sxs-lookup"><span data-stu-id="c2bd7-125">Specifies the importance that is to be stamped on messages.</span></span>  <br/> |
|[<span data-ttu-id="c2bd7-126">MarkAsRead</span><span class="sxs-lookup"><span data-stu-id="c2bd7-126">MarkAsRead</span></span>](markasread.md) <br/> |<span data-ttu-id="c2bd7-127">Указывает, будет ли сообщений помечена как прочтенные.</span><span class="sxs-lookup"><span data-stu-id="c2bd7-127">Indicates whether messages are to be marked as read.</span></span>  <br/> |
|[<span data-ttu-id="c2bd7-128">MoveToFolder</span><span class="sxs-lookup"><span data-stu-id="c2bd7-128">MoveToFolder</span></span>](movetofolder.md) <br/> |<span data-ttu-id="c2bd7-129">Определение идентификатора к папке, где планируется переместить сообщения электронной почты.</span><span class="sxs-lookup"><span data-stu-id="c2bd7-129">Identifies the ID of the folder that e-mail items will be moved to.</span></span>  <br/> |
|[<span data-ttu-id="c2bd7-130">PermanentDelete</span><span class="sxs-lookup"><span data-stu-id="c2bd7-130">PermanentDelete</span></span>](permanentdelete.md) <br/> |<span data-ttu-id="c2bd7-131">Указывает, являются ли сообщения для окончательного удаления и не сохраняются в папку «Удаленные».</span><span class="sxs-lookup"><span data-stu-id="c2bd7-131">Indicates whether messages are to be permanently deleted and not saved to the Deleted Items folder.</span></span>  <br/> |
|[<span data-ttu-id="c2bd7-132">RedirectToRecipients</span><span class="sxs-lookup"><span data-stu-id="c2bd7-132">RedirectToRecipients</span></span>](redirecttorecipients.md) <br/> |<span data-ttu-id="c2bd7-133">Указывает адреса электронной почты, к которым должны перенаправляться сообщения.</span><span class="sxs-lookup"><span data-stu-id="c2bd7-133">Indicates the e-mail addresses to which messages are to be redirected.</span></span>  <br/> |
|[<span data-ttu-id="c2bd7-134">SendSMSAlertToRecipients</span><span class="sxs-lookup"><span data-stu-id="c2bd7-134">SendSMSAlertToRecipients</span></span>](sendsmsalerttorecipients.md) <br/> |<span data-ttu-id="c2bd7-135">Указывает, номера мобильного телефона, к которым будет отправляться уведомление службы коротких сообщений (SMS).</span><span class="sxs-lookup"><span data-stu-id="c2bd7-135">Indicates the mobile phone numbers to which a Short Message Service (SMS) alert is to be sent.</span></span>  <br/> |
|[<span data-ttu-id="c2bd7-136">ServerReplyWithMessage</span><span class="sxs-lookup"><span data-stu-id="c2bd7-136">ServerReplyWithMessage</span></span>](serverreplywithmessage.md) <br/> |<span data-ttu-id="c2bd7-137">Указывает.</span><span class="sxs-lookup"><span data-stu-id="c2bd7-137">Indicates.</span></span> <span data-ttu-id="c2bd7-138">Идентификатор шаблона сообщения, которые отправляются в виде ответа на входящие сообщения.</span><span class="sxs-lookup"><span data-stu-id="c2bd7-138">the ID of the template message that is to be sent as a reply to incoming messages.</span></span>  <br/> |
|[<span data-ttu-id="c2bd7-139">StopProcessingRules</span><span class="sxs-lookup"><span data-stu-id="c2bd7-139">StopProcessingRules</span></span>](stopprocessingrules.md) <br/> |<span data-ttu-id="c2bd7-140">Указывает, являются ли последующих правил для оценки.</span><span class="sxs-lookup"><span data-stu-id="c2bd7-140">Indicates whether subsequent rules are to be evaluated.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="c2bd7-141">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="c2bd7-141">Parent elements</span></span>

|<span data-ttu-id="c2bd7-142">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="c2bd7-142">**Element**</span></span>|<span data-ttu-id="c2bd7-143">**Описание**</span><span class="sxs-lookup"><span data-stu-id="c2bd7-143">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c2bd7-144">Правило (RuleType)</span><span class="sxs-lookup"><span data-stu-id="c2bd7-144">Rule (RuleType)</span></span>](rule-ruletype.md) <br/> |<span data-ttu-id="c2bd7-145">Представляет одно правило в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="c2bd7-145">Represents a single rule in a user's mailbox.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="c2bd7-146">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="c2bd7-146">Text value</span></span>

<span data-ttu-id="c2bd7-147">Нет.</span><span class="sxs-lookup"><span data-stu-id="c2bd7-147">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="c2bd7-148">Замечания</span><span class="sxs-lookup"><span data-stu-id="c2bd7-148">Remarks</span></span>

<span data-ttu-id="c2bd7-149">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="c2bd7-149">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c2bd7-150">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="c2bd7-150">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c2bd7-151">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="c2bd7-151">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="c2bd7-152">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="c2bd7-152">Schema Name</span></span>  <br/> |<span data-ttu-id="c2bd7-153">Схема Types</span><span class="sxs-lookup"><span data-stu-id="c2bd7-153">Types schema</span></span>  <br/> |
|<span data-ttu-id="c2bd7-154">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="c2bd7-154">Validation File</span></span>  <br/> |<span data-ttu-id="c2bd7-155">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="c2bd7-155">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="c2bd7-156">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="c2bd7-156">Can be Empty</span></span>  <br/> |<span data-ttu-id="c2bd7-157">True</span><span class="sxs-lookup"><span data-stu-id="c2bd7-157">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c2bd7-158">См. также</span><span class="sxs-lookup"><span data-stu-id="c2bd7-158">See also</span></span>

- [<span data-ttu-id="c2bd7-159">Условия</span><span class="sxs-lookup"><span data-stu-id="c2bd7-159">Conditions</span></span>](conditions.md)
- [<span data-ttu-id="c2bd7-160">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="c2bd7-160">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

