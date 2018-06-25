---
title: PendingMailTips
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- PendingMailTips
api_type:
- schema
ms.assetid: 0cd70eea-8d36-4b1b-bf80-5edf359e7ba7
description: Элемент PendingMailTips указывает, что почтовые подсказки в этот элемент не удалось вычислить до истечения времени ожидания обработки на сервере.
ms.openlocfilehash: 73d597f6534ea29f7d26d6526c48631251521ae5
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834704"
---
# <a name="pendingmailtips"></a><span data-ttu-id="dfced-103">PendingMailTips</span><span class="sxs-lookup"><span data-stu-id="dfced-103">PendingMailTips</span></span>

<span data-ttu-id="dfced-104">Элемент **PendingMailTips** указывает, что почтовые подсказки в этот элемент не удалось вычислить до истечения времени ожидания обработки на сервере.</span><span class="sxs-lookup"><span data-stu-id="dfced-104">The **PendingMailTips** element indicates that the mail tips in this element could not be evaluated before the server's processing timeout expired.</span></span> 
  
```XML
<PendingMailTips>All | OutOfOfficeMessage | MailboxFullStatus | CustomMailTip | ExternalMemberCount | TotalMemberCount | MaxMessageSize | DeliveryRestriction | ModerateStatus | InvalidRecipient</PendingMailTips>
```

 <span data-ttu-id="dfced-105">**MailTipTypes**</span><span class="sxs-lookup"><span data-stu-id="dfced-105">**MailTipTypes**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="dfced-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="dfced-106">Attributes and elements</span></span>

<span data-ttu-id="dfced-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="dfced-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="dfced-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="dfced-108">Attributes</span></span>

<span data-ttu-id="dfced-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="dfced-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="dfced-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="dfced-110">Child elements</span></span>

<span data-ttu-id="dfced-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="dfced-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="dfced-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="dfced-112">Parent elements</span></span>

|<span data-ttu-id="dfced-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="dfced-113">**Element**</span></span>|<span data-ttu-id="dfced-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="dfced-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="dfced-115">Почтовые подсказки</span><span class="sxs-lookup"><span data-stu-id="dfced-115">MailTips</span></span>](mailtips.md) <br/> |<span data-ttu-id="dfced-116">Представляет значения для различных типов почтовые подсказки.</span><span class="sxs-lookup"><span data-stu-id="dfced-116">Represents values for various types of mail tips.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="dfced-117">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="dfced-117">Text value</span></span>

<span data-ttu-id="dfced-118">В следующей таблице приведены возможные значения для элемента **PendingMailTips** .</span><span class="sxs-lookup"><span data-stu-id="dfced-118">The following table lists the possible values for the **PendingMailTips** element.</span></span> 
  
|<span data-ttu-id="dfced-119">**Значение**</span><span class="sxs-lookup"><span data-stu-id="dfced-119">**Value**</span></span>|<span data-ttu-id="dfced-120">**Описание**</span><span class="sxs-lookup"><span data-stu-id="dfced-120">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="dfced-121">Все</span><span class="sxs-lookup"><span data-stu-id="dfced-121">All</span></span>  <br/> |<span data-ttu-id="dfced-122">Представляет все доступные почтовые подсказки.</span><span class="sxs-lookup"><span data-stu-id="dfced-122">Represents all available mail tips.</span></span>  <br/> |
|<span data-ttu-id="dfced-123">OutOfOfficeMessage</span><span class="sxs-lookup"><span data-stu-id="dfced-123">OutOfOfficeMessage</span></span>  <br/> |<span data-ttu-id="dfced-124">Представляет сообщение об отсутствии на работе Office (отсутствие на работе).</span><span class="sxs-lookup"><span data-stu-id="dfced-124">Represents the Out of Office (OOF) message.</span></span>  <br/> |
|<span data-ttu-id="dfced-125">MailboxFullStatus</span><span class="sxs-lookup"><span data-stu-id="dfced-125">MailboxFullStatus</span></span>  <br/> |<span data-ttu-id="dfced-126">Представляет сведения о состоянии, полный почтовый ящик.</span><span class="sxs-lookup"><span data-stu-id="dfced-126">Represents the status for a mailbox being full.</span></span>  <br/> |
|<span data-ttu-id="dfced-127">CustomMailTip</span><span class="sxs-lookup"><span data-stu-id="dfced-127">CustomMailTip</span></span>  <br/> |<span data-ttu-id="dfced-128">Представляет подсказку настраиваемых почты.</span><span class="sxs-lookup"><span data-stu-id="dfced-128">Represents a custom mail tip.</span></span>  <br/> |
|<span data-ttu-id="dfced-129">ExternalMemberCount</span><span class="sxs-lookup"><span data-stu-id="dfced-129">ExternalMemberCount</span></span>  <br/> |<span data-ttu-id="dfced-130">Представляет количество внешних элементов.</span><span class="sxs-lookup"><span data-stu-id="dfced-130">Represents the count of external members.</span></span>  <br/> |
|<span data-ttu-id="dfced-131">TotalMemberCount</span><span class="sxs-lookup"><span data-stu-id="dfced-131">TotalMemberCount</span></span>  <br/> |<span data-ttu-id="dfced-132">Представляет количество всех элементов.</span><span class="sxs-lookup"><span data-stu-id="dfced-132">Represents the count of all members.</span></span>  <br/> |
|<span data-ttu-id="dfced-133">MaxMessageSize</span><span class="sxs-lookup"><span data-stu-id="dfced-133">MaxMessageSize</span></span>  <br/> |<span data-ttu-id="dfced-134">Представляет максимальный размер сообщения, можно принять получателя.</span><span class="sxs-lookup"><span data-stu-id="dfced-134">Represents the maximum message size a recipient can accept.</span></span>  <br/> |
|<span data-ttu-id="dfced-135">DeliveryRestriction</span><span class="sxs-lookup"><span data-stu-id="dfced-135">DeliveryRestriction</span></span>  <br/> |<span data-ttu-id="dfced-136">Указывает ли ограничения на доставку будет препятствовать сообщения достигает получателя.</span><span class="sxs-lookup"><span data-stu-id="dfced-136">Indicates whether delivery restrictions will prevent the sender's message from reaching the recipient.</span></span>  <br/> |
|<span data-ttu-id="dfced-137">ModerationStatus</span><span class="sxs-lookup"><span data-stu-id="dfced-137">ModerationStatus</span></span>  <br/> |<span data-ttu-id="dfced-138">Указывает, будет ли сообщения будут проверены модератором.</span><span class="sxs-lookup"><span data-stu-id="dfced-138">Indicates whether the sender's message will be reviewed by a moderator.</span></span>  <br/> |
|<span data-ttu-id="dfced-139">InvalidRecipient</span><span class="sxs-lookup"><span data-stu-id="dfced-139">InvalidRecipient</span></span>  <br/> |<span data-ttu-id="dfced-140">Указывает, является ли получатель является недопустимым.</span><span class="sxs-lookup"><span data-stu-id="dfced-140">Indicates whether the recipient is invalid.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="dfced-141">Замечания</span><span class="sxs-lookup"><span data-stu-id="dfced-141">Remarks</span></span>

<span data-ttu-id="dfced-142">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="dfced-142">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="dfced-143">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="dfced-143">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="dfced-144">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="dfced-144">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="dfced-145">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="dfced-145">Schema Name</span></span>  <br/> |<span data-ttu-id="dfced-146">Схема Types</span><span class="sxs-lookup"><span data-stu-id="dfced-146">Types schema</span></span>  <br/> |
|<span data-ttu-id="dfced-147">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="dfced-147">Validation File</span></span>  <br/> |<span data-ttu-id="dfced-148">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="dfced-148">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="dfced-149">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="dfced-149">Can be Empty</span></span>  <br/> |<span data-ttu-id="dfced-150">False</span><span class="sxs-lookup"><span data-stu-id="dfced-150">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="dfced-151">См. также</span><span class="sxs-lookup"><span data-stu-id="dfced-151">See also</span></span>



- [<span data-ttu-id="dfced-152">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="dfced-152">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

