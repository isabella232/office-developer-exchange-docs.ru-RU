---
title: Почтовые подсказки
manager: sethgros
ms.date: 09/17/2015
ms.audience: ITPro
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MailTips
api_type:
- schema
ms.assetid: c1cba493-bccc-4b8e-be8e-bfa8a8b10882
description: Элемент подсказки представляет значения для различных типов почтовые подсказки.
ms.openlocfilehash: 3a2e95225b09fd2d81db32f821ea3069ab7e7852
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19834311"
---
# <a name="mailtips"></a><span data-ttu-id="62024-103">Почтовые подсказки</span><span class="sxs-lookup"><span data-stu-id="62024-103">MailTips</span></span>

<span data-ttu-id="62024-104">Элемент **подсказки** представляет значения для различных типов почтовые подсказки.</span><span class="sxs-lookup"><span data-stu-id="62024-104">The **MailTips** element represents values for various types of mail tips.</span></span> 
  
```XML
<MailTips>
   <RecipientAddress/>
   <PendingMailTips/>
   <OutOfOffice/>
   <MailboxFull/>
   <CustomMailTip/>
   <TotalMemberCount/>
   <ExternalMemberCount/>
   <MaxMessageSize/>
   <DeliveryRestricted/>
   <IsModerated/>
   <InvalidRecipient/>
</MailTips>
```

 <span data-ttu-id="62024-105">**Почтовые подсказки**</span><span class="sxs-lookup"><span data-stu-id="62024-105">**MailTips**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="62024-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="62024-106">Attributes and elements</span></span>

<span data-ttu-id="62024-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="62024-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="62024-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="62024-108">Attributes</span></span>

<span data-ttu-id="62024-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="62024-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="62024-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="62024-110">Child elements</span></span>

|<span data-ttu-id="62024-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="62024-111">**Element**</span></span>|<span data-ttu-id="62024-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="62024-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="62024-113">RecipientAddress</span><span class="sxs-lookup"><span data-stu-id="62024-113">RecipientAddress</span></span>](recipientaddress.md) <br/> |<span data-ttu-id="62024-114">Представляет почтовый ящик получателя.</span><span class="sxs-lookup"><span data-stu-id="62024-114">Represents the mailbox of the recipient.</span></span>  <br/> |
|[<span data-ttu-id="62024-115">PendingMailTips</span><span class="sxs-lookup"><span data-stu-id="62024-115">PendingMailTips</span></span>](pendingmailtips.md) <br/> |<span data-ttu-id="62024-116">Указывает, что почтовые подсказки в этот элемент не удалось вычислить до истечения времени ожидания обработки на сервере.</span><span class="sxs-lookup"><span data-stu-id="62024-116">Indicates that the mail tips in this element could not be evaluated before the server's processing timeout expired.</span></span>  <br/> |
|[<span data-ttu-id="62024-117">Нет на месте</span><span class="sxs-lookup"><span data-stu-id="62024-117">OutOfOffice</span></span>](outofoffice.md) <br/> |<span data-ttu-id="62024-118">Представляет ответное сообщение и время для отправки сообщения ответа.</span><span class="sxs-lookup"><span data-stu-id="62024-118">Represents the response message and a duration time for sending the response message.</span></span>  <br/> |
|[<span data-ttu-id="62024-119">MailboxFull</span><span class="sxs-lookup"><span data-stu-id="62024-119">MailboxFull</span></span>](mailboxfull.md) <br/> |<span data-ttu-id="62024-120">Указывает, является ли полный почтовый ящик получателя.</span><span class="sxs-lookup"><span data-stu-id="62024-120">Indicates whether the mailbox for the recipient is full.</span></span>  <br/> |
|[<span data-ttu-id="62024-121">CustomMailTip</span><span class="sxs-lookup"><span data-stu-id="62024-121">CustomMailTip</span></span>](custommailtip.md) <br/> |<span data-ttu-id="62024-122">Представляет подсказку настроенного почтового сообщения.</span><span class="sxs-lookup"><span data-stu-id="62024-122">Represents a customized mail tip message.</span></span>  <br/> |
|[<span data-ttu-id="62024-123">TotalMemberCount</span><span class="sxs-lookup"><span data-stu-id="62024-123">TotalMemberCount</span></span>](totalmembercount.md) <br/> |<span data-ttu-id="62024-124">Представляет количество всех элементов в группе.</span><span class="sxs-lookup"><span data-stu-id="62024-124">Represents the count of all members in a group.</span></span>  <br/> |
|[<span data-ttu-id="62024-125">ExternalMemberCount</span><span class="sxs-lookup"><span data-stu-id="62024-125">ExternalMemberCount</span></span>](externalmembercount.md) <br/> |<span data-ttu-id="62024-126">Представляет количество внешних элементов в группе.</span><span class="sxs-lookup"><span data-stu-id="62024-126">Represents the count of external members in a group.</span></span>  <br/> |
|[<span data-ttu-id="62024-127">MaxMessageSize</span><span class="sxs-lookup"><span data-stu-id="62024-127">MaxMessageSize</span></span>](maxmessagesize.md) <br/> |<span data-ttu-id="62024-128">Представляет максимальный размер сообщения, можно принять получателя.</span><span class="sxs-lookup"><span data-stu-id="62024-128">Represents the maximum message size the recipient can accept.</span></span>  <br/> |
|[<span data-ttu-id="62024-129">DeliveryRestricted</span><span class="sxs-lookup"><span data-stu-id="62024-129">DeliveryRestricted</span></span>](deliveryrestricted.md) <br/> |<span data-ttu-id="62024-130">Указывает ли ограничения на доставку будет препятствовать сообщения достигает получателя.</span><span class="sxs-lookup"><span data-stu-id="62024-130">Indicates whether delivery restrictions will prevent the sender's message from reaching the recipient.</span></span>  <br/> |
|[<span data-ttu-id="62024-131">IsModerated</span><span class="sxs-lookup"><span data-stu-id="62024-131">IsModerated</span></span>](ismoderated.md) <br/> |<span data-ttu-id="62024-132">Указывает, является ли управляемым почтовый ящик получателя.</span><span class="sxs-lookup"><span data-stu-id="62024-132">Indicates whether the recipient's mailbox is being moderated.</span></span>  <br/> |
|[<span data-ttu-id="62024-133">InvalidRecipient (подсказки)</span><span class="sxs-lookup"><span data-stu-id="62024-133">InvalidRecipient (MailTips)</span></span>](invalidrecipient-mailtips.md) <br/> |<span data-ttu-id="62024-134">Указывает, является ли получатель является недопустимым.</span><span class="sxs-lookup"><span data-stu-id="62024-134">Indicates whether the recipient is invalid.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="62024-135">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="62024-135">Parent elements</span></span>

|<span data-ttu-id="62024-136">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="62024-136">**Element**</span></span>|<span data-ttu-id="62024-137">**Описание**</span><span class="sxs-lookup"><span data-stu-id="62024-137">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="62024-138">MailTipsResponseMessageType</span><span class="sxs-lookup"><span data-stu-id="62024-138">MailTipsResponseMessageType</span></span>](mailtipsresponsemessagetype.md) <br/> |<span data-ttu-id="62024-139">Представляет почтовые подсказки параметров.</span><span class="sxs-lookup"><span data-stu-id="62024-139">Represents mail tips settings.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="62024-140">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="62024-140">Text value</span></span>

<span data-ttu-id="62024-141">Нет.</span><span class="sxs-lookup"><span data-stu-id="62024-141">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="62024-142">Замечания</span><span class="sxs-lookup"><span data-stu-id="62024-142">Remarks</span></span>

<span data-ttu-id="62024-143">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="62024-143">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="62024-144">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="62024-144">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="62024-145">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="62024-145">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="62024-146">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="62024-146">Schema Name</span></span>  <br/> |<span data-ttu-id="62024-147">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="62024-147">Messages schema</span></span>  <br/> |
|<span data-ttu-id="62024-148">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="62024-148">Validation File</span></span>  <br/> |<span data-ttu-id="62024-149">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="62024-149">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="62024-150">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="62024-150">Can be Empty</span></span>  <br/> |<span data-ttu-id="62024-151">False</span><span class="sxs-lookup"><span data-stu-id="62024-151">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="62024-152">См. также</span><span class="sxs-lookup"><span data-stu-id="62024-152">See also</span></span>



- [<span data-ttu-id="62024-153">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="62024-153">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

