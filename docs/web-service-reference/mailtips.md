---
title: Подсказки
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
description: Элемент MailTips представляет значения для различных типов подсказок.
ms.openlocfilehash: 9bacdea7b4f3108f700ed102025445e01a73e69d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44447598"
---
# <a name="mailtips"></a><span data-ttu-id="3304b-103">Подсказки</span><span class="sxs-lookup"><span data-stu-id="3304b-103">MailTips</span></span>

<span data-ttu-id="3304b-104">Элемент **MailTips** представляет значения для различных типов подсказок.</span><span class="sxs-lookup"><span data-stu-id="3304b-104">The **MailTips** element represents values for various types of mail tips.</span></span> 
  
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

 <span data-ttu-id="3304b-105">**Подсказки**</span><span class="sxs-lookup"><span data-stu-id="3304b-105">**MailTips**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3304b-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="3304b-106">Attributes and elements</span></span>

<span data-ttu-id="3304b-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="3304b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3304b-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="3304b-108">Attributes</span></span>

<span data-ttu-id="3304b-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="3304b-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3304b-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="3304b-110">Child elements</span></span>

|<span data-ttu-id="3304b-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="3304b-111">**Element**</span></span>|<span data-ttu-id="3304b-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="3304b-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3304b-113">RecipientAddress</span><span class="sxs-lookup"><span data-stu-id="3304b-113">RecipientAddress</span></span>](recipientaddress.md) <br/> |<span data-ttu-id="3304b-114">Представляет почтовый ящик получателя.</span><span class="sxs-lookup"><span data-stu-id="3304b-114">Represents the mailbox of the recipient.</span></span>  <br/> |
|[<span data-ttu-id="3304b-115">PendingMailTips</span><span class="sxs-lookup"><span data-stu-id="3304b-115">PendingMailTips</span></span>](pendingmailtips.md) <br/> |<span data-ttu-id="3304b-116">Указывает, что подсказки электронной почты в этом элементе не удалось оценить до истечения времени действия обработки сервера.</span><span class="sxs-lookup"><span data-stu-id="3304b-116">Indicates that the mail tips in this element could not be evaluated before the server's processing timeout expired.</span></span>  <br/> |
|[<span data-ttu-id="3304b-117">OutOfOffice</span><span class="sxs-lookup"><span data-stu-id="3304b-117">OutOfOffice</span></span>](outofoffice.md) <br/> |<span data-ttu-id="3304b-118">Представляет ответное сообщение и продолжительность отправки сообщения.</span><span class="sxs-lookup"><span data-stu-id="3304b-118">Represents the response message and a duration time for sending the response message.</span></span>  <br/> |
|[<span data-ttu-id="3304b-119">MailboxFull</span><span class="sxs-lookup"><span data-stu-id="3304b-119">MailboxFull</span></span>](mailboxfull.md) <br/> |<span data-ttu-id="3304b-120">Указывает, заполнен ли почтовый ящик получателя.</span><span class="sxs-lookup"><span data-stu-id="3304b-120">Indicates whether the mailbox for the recipient is full.</span></span>  <br/> |
|[<span data-ttu-id="3304b-121">CustomMailTip</span><span class="sxs-lookup"><span data-stu-id="3304b-121">CustomMailTip</span></span>](custommailtip.md) <br/> |<span data-ttu-id="3304b-122">Представляет настроенное сообщение подсказки почты.</span><span class="sxs-lookup"><span data-stu-id="3304b-122">Represents a customized mail tip message.</span></span>  <br/> |
|[<span data-ttu-id="3304b-123">TotalMemberCount</span><span class="sxs-lookup"><span data-stu-id="3304b-123">TotalMemberCount</span></span>](totalmembercount.md) <br/> |<span data-ttu-id="3304b-124">Представляет количество всех членов группы.</span><span class="sxs-lookup"><span data-stu-id="3304b-124">Represents the count of all members in a group.</span></span>  <br/> |
|[<span data-ttu-id="3304b-125">ExternalMemberCount</span><span class="sxs-lookup"><span data-stu-id="3304b-125">ExternalMemberCount</span></span>](externalmembercount.md) <br/> |<span data-ttu-id="3304b-126">Представляет количество внешних участников в группе.</span><span class="sxs-lookup"><span data-stu-id="3304b-126">Represents the count of external members in a group.</span></span>  <br/> |
|[<span data-ttu-id="3304b-127">MaxMessageSize</span><span class="sxs-lookup"><span data-stu-id="3304b-127">MaxMessageSize</span></span>](maxmessagesize.md) <br/> |<span data-ttu-id="3304b-128">Представляет максимальный размер сообщения, который может принять получатель.</span><span class="sxs-lookup"><span data-stu-id="3304b-128">Represents the maximum message size the recipient can accept.</span></span>  <br/> |
|[<span data-ttu-id="3304b-129">DeliveryRestricted</span><span class="sxs-lookup"><span data-stu-id="3304b-129">DeliveryRestricted</span></span>](deliveryrestricted.md) <br/> |<span data-ttu-id="3304b-130">Указывает, будут ли ограничения доставки препятствовать доставке сообщения отправи мне.</span><span class="sxs-lookup"><span data-stu-id="3304b-130">Indicates whether delivery restrictions will prevent the sender's message from reaching the recipient.</span></span>  <br/> |
|[<span data-ttu-id="3304b-131">IsModerated</span><span class="sxs-lookup"><span data-stu-id="3304b-131">IsModerated</span></span>](ismoderated.md) <br/> |<span data-ttu-id="3304b-132">Указывает, является ли почтовый ящик получателя модером.</span><span class="sxs-lookup"><span data-stu-id="3304b-132">Indicates whether the recipient's mailbox is being moderated.</span></span>  <br/> |
|[<span data-ttu-id="3304b-133">InvalidRecipient (MailTips)</span><span class="sxs-lookup"><span data-stu-id="3304b-133">InvalidRecipient (MailTips)</span></span>](invalidrecipient-mailtips.md) <br/> |<span data-ttu-id="3304b-134">Указывает, является ли получатель недопустимым.</span><span class="sxs-lookup"><span data-stu-id="3304b-134">Indicates whether the recipient is invalid.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="3304b-135">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="3304b-135">Parent elements</span></span>

|<span data-ttu-id="3304b-136">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="3304b-136">**Element**</span></span>|<span data-ttu-id="3304b-137">**Описание**</span><span class="sxs-lookup"><span data-stu-id="3304b-137">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3304b-138">MailTipsResponseMessageType</span><span class="sxs-lookup"><span data-stu-id="3304b-138">MailTipsResponseMessageType</span></span>](mailtipsresponsemessagetype.md) <br/> |<span data-ttu-id="3304b-139">Представляет параметры подсказок почты.</span><span class="sxs-lookup"><span data-stu-id="3304b-139">Represents mail tips settings.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="3304b-140">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="3304b-140">Text value</span></span>

<span data-ttu-id="3304b-141">Нет.</span><span class="sxs-lookup"><span data-stu-id="3304b-141">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="3304b-142">Примечания</span><span class="sxs-lookup"><span data-stu-id="3304b-142">Remarks</span></span>

<span data-ttu-id="3304b-143">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="3304b-143">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3304b-144">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="3304b-144">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3304b-145">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="3304b-145">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="3304b-146">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="3304b-146">Schema Name</span></span>  <br/> |<span data-ttu-id="3304b-147">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="3304b-147">Messages schema</span></span>  <br/> |
|<span data-ttu-id="3304b-148">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="3304b-148">Validation File</span></span>  <br/> |<span data-ttu-id="3304b-149">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="3304b-149">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="3304b-150">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="3304b-150">Can be Empty</span></span>  <br/> |<span data-ttu-id="3304b-151">False</span><span class="sxs-lookup"><span data-stu-id="3304b-151">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3304b-152">См. также</span><span class="sxs-lookup"><span data-stu-id="3304b-152">See also</span></span>



- [<span data-ttu-id="3304b-153">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="3304b-153">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

