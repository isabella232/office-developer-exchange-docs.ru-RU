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
description: Элемент Actions представляет набор действий, которые могут быть выполнены над сообщением при выполнении условий.
ms.openlocfilehash: 2ac53778b583595fa8be07f2c5110a9e2df16eca
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465067"
---
# <a name="actions"></a><span data-ttu-id="9250c-103">Действия</span><span class="sxs-lookup"><span data-stu-id="9250c-103">Actions</span></span>

<span data-ttu-id="9250c-104">Элемент **Actions** представляет набор действий, которые могут быть выполнены над сообщением при выполнении условий.</span><span class="sxs-lookup"><span data-stu-id="9250c-104">The **Actions** element represents the set of actions that are available to be taken on a message when the conditions are fulfilled.</span></span> 
  
[<span data-ttu-id="9250c-105">Правило (RuleType)</span><span class="sxs-lookup"><span data-stu-id="9250c-105">Rule (RuleType)</span></span>](rule-ruletype.md)
  
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

 <span data-ttu-id="9250c-106">**рулеактионстипе**</span><span class="sxs-lookup"><span data-stu-id="9250c-106">**RuleActionsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9250c-107">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="9250c-107">Attributes and elements</span></span>

<span data-ttu-id="9250c-108">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="9250c-108">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9250c-109">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="9250c-109">Attributes</span></span>

<span data-ttu-id="9250c-110">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="9250c-110">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9250c-111">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="9250c-111">Child elements</span></span>

|<span data-ttu-id="9250c-112">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="9250c-112">**Element**</span></span>|<span data-ttu-id="9250c-113">**Описание**</span><span class="sxs-lookup"><span data-stu-id="9250c-113">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9250c-114">ассигнкатегориес</span><span class="sxs-lookup"><span data-stu-id="9250c-114">AssignCategories</span></span>](assigncategories.md) <br/> |<span data-ttu-id="9250c-115">Представляет категории, помеченные в сообщениях электронной почты.</span><span class="sxs-lookup"><span data-stu-id="9250c-115">Represents the categories that are stamped on e-mail messages.</span></span>  <br/> |
|[<span data-ttu-id="9250c-116">CopyToFolder</span><span class="sxs-lookup"><span data-stu-id="9250c-116">CopyToFolder</span></span>](copytofolder.md) <br/> |<span data-ttu-id="9250c-117">Определяет идентификатор папки, в которую будут скопированы элементы электронной почты.</span><span class="sxs-lookup"><span data-stu-id="9250c-117">Identifies the ID of the folder that e-mail items will be copied to.</span></span>  <br/> |
|[<span data-ttu-id="9250c-118">Удаление</span><span class="sxs-lookup"><span data-stu-id="9250c-118">Delete</span></span>](delete.md) <br/> |<span data-ttu-id="9250c-119">Указывает, следует ли перемещать сообщения в папку "Удаленные".</span><span class="sxs-lookup"><span data-stu-id="9250c-119">Indicates whether messages are to be moved to the Deleted Items folder.</span></span>  <br/> |
|[<span data-ttu-id="9250c-120">форвардасаттачменттореЦипиентс</span><span class="sxs-lookup"><span data-stu-id="9250c-120">ForwardAsAttachmentToRecipients</span></span>](forwardasattachmenttorecipients.md) <br/> |<span data-ttu-id="9250c-121">Указывает адреса электронной почты, на которые будут пересылаться сообщения в виде вложений.</span><span class="sxs-lookup"><span data-stu-id="9250c-121">Indicates the e-mail addresses to which messages are to be forwarded as attachments.</span></span>  <br/> |
|[<span data-ttu-id="9250c-122">форвардтореЦипиентс</span><span class="sxs-lookup"><span data-stu-id="9250c-122">ForwardToRecipients</span></span>](forwardtorecipients.md) <br/> |<span data-ttu-id="9250c-123">Указывает адреса электронной почты, на которые пересылаются сообщения.</span><span class="sxs-lookup"><span data-stu-id="9250c-123">Indicates the e-mail addresses to which messages are to be forwarded.</span></span>  <br/> |
|[<span data-ttu-id="9250c-124">маркимпортанце</span><span class="sxs-lookup"><span data-stu-id="9250c-124">MarkImportance</span></span>](markimportance.md) <br/> |<span data-ttu-id="9250c-125">Указывает важность, с которой будут отмечаться сообщения.</span><span class="sxs-lookup"><span data-stu-id="9250c-125">Specifies the importance that is to be stamped on messages.</span></span>  <br/> |
|[<span data-ttu-id="9250c-126">MarkAsRead</span><span class="sxs-lookup"><span data-stu-id="9250c-126">MarkAsRead</span></span>](markasread.md) <br/> |<span data-ttu-id="9250c-127">Указывает, следует ли помечать сообщения как прочтенные.</span><span class="sxs-lookup"><span data-stu-id="9250c-127">Indicates whether messages are to be marked as read.</span></span>  <br/> |
|[<span data-ttu-id="9250c-128">MoveToFolder</span><span class="sxs-lookup"><span data-stu-id="9250c-128">MoveToFolder</span></span>](movetofolder.md) <br/> |<span data-ttu-id="9250c-129">Определяет идентификатор папки, в которую будут перемещены элементы электронной почты.</span><span class="sxs-lookup"><span data-stu-id="9250c-129">Identifies the ID of the folder that e-mail items will be moved to.</span></span>  <br/> |
|[<span data-ttu-id="9250c-130">перманентделете</span><span class="sxs-lookup"><span data-stu-id="9250c-130">PermanentDelete</span></span>](permanentdelete.md) <br/> |<span data-ttu-id="9250c-131">Указывает, следует ли окончательно удалять сообщения и не сохранять их в папке "Удаленные".</span><span class="sxs-lookup"><span data-stu-id="9250c-131">Indicates whether messages are to be permanently deleted and not saved to the Deleted Items folder.</span></span>  <br/> |
|[<span data-ttu-id="9250c-132">RedirectToRecipients</span><span class="sxs-lookup"><span data-stu-id="9250c-132">RedirectToRecipients</span></span>](redirecttorecipients.md) <br/> |<span data-ttu-id="9250c-133">Указывает адреса электронной почты, на которые перенаправляются сообщения.</span><span class="sxs-lookup"><span data-stu-id="9250c-133">Indicates the e-mail addresses to which messages are to be redirected.</span></span>  <br/> |
|[<span data-ttu-id="9250c-134">сендсмсалерттореЦипиентс</span><span class="sxs-lookup"><span data-stu-id="9250c-134">SendSMSAlertToRecipients</span></span>](sendsmsalerttorecipients.md) <br/> |<span data-ttu-id="9250c-135">Указывает номера мобильных телефонов, к которым отправляется оповещение в службе коротких сообщений (SMS).</span><span class="sxs-lookup"><span data-stu-id="9250c-135">Indicates the mobile phone numbers to which a Short Message Service (SMS) alert is to be sent.</span></span>  <br/> |
|[<span data-ttu-id="9250c-136">серверрепливисмессаже</span><span class="sxs-lookup"><span data-stu-id="9250c-136">ServerReplyWithMessage</span></span>](serverreplywithmessage.md) <br/> |<span data-ttu-id="9250c-137">Указывает.</span><span class="sxs-lookup"><span data-stu-id="9250c-137">Indicates.</span></span> <span data-ttu-id="9250c-138">Идентификатор сообщения шаблона, отправляемого в качестве ответа на входящие сообщения.</span><span class="sxs-lookup"><span data-stu-id="9250c-138">the ID of the template message that is to be sent as a reply to incoming messages.</span></span>  <br/> |
|[<span data-ttu-id="9250c-139">StopProcessingRules</span><span class="sxs-lookup"><span data-stu-id="9250c-139">StopProcessingRules</span></span>](stopprocessingrules.md) <br/> |<span data-ttu-id="9250c-140">Указывает, следует ли оценивать последующие правила.</span><span class="sxs-lookup"><span data-stu-id="9250c-140">Indicates whether subsequent rules are to be evaluated.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="9250c-141">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="9250c-141">Parent elements</span></span>

|<span data-ttu-id="9250c-142">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="9250c-142">**Element**</span></span>|<span data-ttu-id="9250c-143">**Описание**</span><span class="sxs-lookup"><span data-stu-id="9250c-143">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9250c-144">Правило (RuleType)</span><span class="sxs-lookup"><span data-stu-id="9250c-144">Rule (RuleType)</span></span>](rule-ruletype.md) <br/> |<span data-ttu-id="9250c-145">Представляет одно правило в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="9250c-145">Represents a single rule in a user's mailbox.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="9250c-146">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="9250c-146">Text value</span></span>

<span data-ttu-id="9250c-147">Нет.</span><span class="sxs-lookup"><span data-stu-id="9250c-147">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="9250c-148">Примечания</span><span class="sxs-lookup"><span data-stu-id="9250c-148">Remarks</span></span>

<span data-ttu-id="9250c-149">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="9250c-149">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9250c-150">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="9250c-150">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9250c-151">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="9250c-151">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="9250c-152">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="9250c-152">Schema Name</span></span>  <br/> |<span data-ttu-id="9250c-153">Схема Types</span><span class="sxs-lookup"><span data-stu-id="9250c-153">Types schema</span></span>  <br/> |
|<span data-ttu-id="9250c-154">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="9250c-154">Validation File</span></span>  <br/> |<span data-ttu-id="9250c-155">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="9250c-155">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="9250c-156">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="9250c-156">Can be Empty</span></span>  <br/> |<span data-ttu-id="9250c-157">True</span><span class="sxs-lookup"><span data-stu-id="9250c-157">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9250c-158">См. также</span><span class="sxs-lookup"><span data-stu-id="9250c-158">See also</span></span>

- [<span data-ttu-id="9250c-159">Conditions</span><span class="sxs-lookup"><span data-stu-id="9250c-159">Conditions</span></span>](conditions.md)
- [<span data-ttu-id="9250c-160">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="9250c-160">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

