---
title: MailTipsRequested
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MailTipsRequested
api_type:
- schema
ms.assetid: 8037bbe5-a37f-4f77-8209-27a94f9095ef
description: Элемент MailTipsRequested содержит типы, запрашивается из службы почтовые подсказки.
ms.openlocfilehash: fa2bef394ea8473aa65bdc2f1d39c0794186fdc6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19834348"
---
# <a name="mailtipsrequested"></a><span data-ttu-id="1256b-103">MailTipsRequested</span><span class="sxs-lookup"><span data-stu-id="1256b-103">MailTipsRequested</span></span>

<span data-ttu-id="1256b-104">Элемент **MailTipsRequested** содержит типы, запрашивается из службы почтовые подсказки.</span><span class="sxs-lookup"><span data-stu-id="1256b-104">The **MailTipsRequested** element contains the types of mail tips requested from the service.</span></span> 
  
```XML
<MailTipsRequested/>
```

 <span data-ttu-id="1256b-105">**MailTipTypes**</span><span class="sxs-lookup"><span data-stu-id="1256b-105">**MailTipTypes**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1256b-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="1256b-106">Attributes and elements</span></span>

<span data-ttu-id="1256b-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="1256b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1256b-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="1256b-108">Attributes</span></span>

<span data-ttu-id="1256b-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="1256b-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1256b-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="1256b-110">Child elements</span></span>

<span data-ttu-id="1256b-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="1256b-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="1256b-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="1256b-112">Parent elements</span></span>

|<span data-ttu-id="1256b-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="1256b-113">**Element**</span></span>|<span data-ttu-id="1256b-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="1256b-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1256b-115">GetMailTips</span><span class="sxs-lookup"><span data-stu-id="1256b-115">GetMailTips</span></span>](getmailtips.md) <br/> |<span data-ttu-id="1256b-116">Содержит получателей и типы почтовые подсказки для извлечения.</span><span class="sxs-lookup"><span data-stu-id="1256b-116">Contains the recipients and types of mail tips to retrieve.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="1256b-117">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="1256b-117">Text value</span></span>

<span data-ttu-id="1256b-118">В следующей таблице приведены возможные значения для элемента **MailTipsRequested** .</span><span class="sxs-lookup"><span data-stu-id="1256b-118">The following table lists the possible values for the **MailTipsRequested** element.</span></span> 
  
|<span data-ttu-id="1256b-119">**Значение**</span><span class="sxs-lookup"><span data-stu-id="1256b-119">**Value**</span></span>|<span data-ttu-id="1256b-120">**Описание**</span><span class="sxs-lookup"><span data-stu-id="1256b-120">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="1256b-121">Все</span><span class="sxs-lookup"><span data-stu-id="1256b-121">All</span></span>  <br/> |<span data-ttu-id="1256b-122">Представляет все доступные почтовые подсказки.</span><span class="sxs-lookup"><span data-stu-id="1256b-122">Represents all available mail tips.</span></span>  <br/> |
|<span data-ttu-id="1256b-123">OutOfOfficeMessage</span><span class="sxs-lookup"><span data-stu-id="1256b-123">OutOfOfficeMessage</span></span>  <br/> |<span data-ttu-id="1256b-124">Представляет сообщение об отсутствии на работе Office (отсутствие на работе).</span><span class="sxs-lookup"><span data-stu-id="1256b-124">Represents the Out of Office (OOF) message.</span></span>  <br/> |
|<span data-ttu-id="1256b-125">MailboxFullStatus</span><span class="sxs-lookup"><span data-stu-id="1256b-125">MailboxFullStatus</span></span>  <br/> |<span data-ttu-id="1256b-126">Представляет состояние почтового ящика, заполнена.</span><span class="sxs-lookup"><span data-stu-id="1256b-126">Represents the status for a mailbox that is full.</span></span>  <br/> |
|<span data-ttu-id="1256b-127">CustomMailTip</span><span class="sxs-lookup"><span data-stu-id="1256b-127">CustomMailTip</span></span>  <br/> |<span data-ttu-id="1256b-128">Представляет подсказку настраиваемых почты.</span><span class="sxs-lookup"><span data-stu-id="1256b-128">Represents a custom mail tip.</span></span>  <br/> |
|<span data-ttu-id="1256b-129">ExternalMemberCount</span><span class="sxs-lookup"><span data-stu-id="1256b-129">ExternalMemberCount</span></span>  <br/> |<span data-ttu-id="1256b-130">Представляет количество внешних элементов.</span><span class="sxs-lookup"><span data-stu-id="1256b-130">Represents the count of external members.</span></span>  <br/> |
|<span data-ttu-id="1256b-131">TotalMemberCount</span><span class="sxs-lookup"><span data-stu-id="1256b-131">TotalMemberCount</span></span>  <br/> |<span data-ttu-id="1256b-132">Представляет количество всех элементов.</span><span class="sxs-lookup"><span data-stu-id="1256b-132">Represents the count of all members.</span></span>  <br/> |
|<span data-ttu-id="1256b-133">MaxMessageSize</span><span class="sxs-lookup"><span data-stu-id="1256b-133">MaxMessageSize</span></span>  <br/> |<span data-ttu-id="1256b-134">Представляет максимальный размер сообщения, можно принять получателя.</span><span class="sxs-lookup"><span data-stu-id="1256b-134">Represents the maximum message size a recipient can accept.</span></span>  <br/> |
|<span data-ttu-id="1256b-135">DeliveryRestriction</span><span class="sxs-lookup"><span data-stu-id="1256b-135">DeliveryRestriction</span></span>  <br/> |<span data-ttu-id="1256b-136">Указывает ли ограничения на доставку будет препятствовать сообщения достигает получателя.</span><span class="sxs-lookup"><span data-stu-id="1256b-136">Indicates whether delivery restrictions will prevent the sender's message from reaching the recipient.</span></span>  <br/> |
|<span data-ttu-id="1256b-137">ModerationStatus</span><span class="sxs-lookup"><span data-stu-id="1256b-137">ModerationStatus</span></span>  <br/> |<span data-ttu-id="1256b-138">Указывает, будет ли сообщения будут проверены модератором.</span><span class="sxs-lookup"><span data-stu-id="1256b-138">Indicates whether the sender's message will be reviewed by a moderator.</span></span>  <br/> |
|<span data-ttu-id="1256b-139">InvalidRecipient</span><span class="sxs-lookup"><span data-stu-id="1256b-139">InvalidRecipient</span></span>  <br/> |<span data-ttu-id="1256b-140">Указывает, является ли получатель является недопустимым.</span><span class="sxs-lookup"><span data-stu-id="1256b-140">Indicates whether the recipient is invalid.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="1256b-141">Замечания</span><span class="sxs-lookup"><span data-stu-id="1256b-141">Remarks</span></span>

<span data-ttu-id="1256b-142">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="1256b-142">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1256b-143">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="1256b-143">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1256b-144">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="1256b-144">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="1256b-145">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="1256b-145">Schema Name</span></span>  <br/> |<span data-ttu-id="1256b-146">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="1256b-146">Messages schema</span></span>  <br/> |
|<span data-ttu-id="1256b-147">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="1256b-147">Validation File</span></span>  <br/> |<span data-ttu-id="1256b-148">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="1256b-148">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="1256b-149">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="1256b-149">Can be Empty</span></span>  <br/> |<span data-ttu-id="1256b-150">False</span><span class="sxs-lookup"><span data-stu-id="1256b-150">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="1256b-151">См. также</span><span class="sxs-lookup"><span data-stu-id="1256b-151">See also</span></span>



- [<span data-ttu-id="1256b-152">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="1256b-152">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

