---
title: Message
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Message
api_type:
- schema
ms.assetid: 2400b33c-43b2-4fc2-b6fb-275a99e0e810
description: Элемент сообщения представляет сообщения электронной почты Microsoft Exchange.
ms.openlocfilehash: 388b944cfa16899cb2376320882f5087396d7b82
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834474"
---
# <a name="message"></a><span data-ttu-id="17ac1-103">Message</span><span class="sxs-lookup"><span data-stu-id="17ac1-103">Message</span></span>

<span data-ttu-id="17ac1-104">Элемент **сообщения** представляет сообщения электронной почты Microsoft Exchange.</span><span class="sxs-lookup"><span data-stu-id="17ac1-104">The **Message** element represents a Microsoft Exchange e-mail message.</span></span> 
  
```xml
<Message>
   <MimeContent/>
   <ItemId/>
   <ParentFolderId/>
   <ItemClass/>
   <Subject/>
   <Sensitivity/>
   <Body/>
   <Attachments/>
   <DateTimeReceived/>
   <Size/>
   <Categories/>
   <Importance/>
   <InReplyTo/>
   <IsSubmitted/>
   <IsDraft/>
   <IsFromMe/>
   <IsResend/>
   <IsUnmodified/>
   <InternetMessageHeaders/>
   <DateTimeSent/>
   <DateTimeCreated/>
   <ResponseObjects/>
   <ReminderDueBy/>
   <ReminderIsSet/>
   <ReminderMinutesBeforeStart/>
   <DisplayCc/>
   <DisplayTo/>
   <HasAttachments/>
   <ExtendedProperty/>
   <Culture/>
   <Sender/>
   <ToRecipients/>
   <CcRecipients/>
   <BccRecipients/>
   <IsReadReceiptRequested/>
   <IsDeliveryReceiptRequested/>
   <ConversationIndex/>
   <ConversationTopic/>
   <From/>
   <InternetMessageId/>
   <IsRead/>
   <IsResponseRequested/>
   <References/>
   <ReplyTo/>
   <EffectiveRights/>
   <ReceivedBy/>
   <ReceivedRepresenting/>
   <LastModifiedName/>
   <LastModifiedTime/>
   <IsAssociated/>
   <WebClientReadFormQueryString/>
   <WebClientEditFormQueryString/>
   <ConversationId/>
   <UniqueBody/>
   <ReminderMessageData/>
</Message>
```

 <span data-ttu-id="17ac1-105">**MessageType**</span><span class="sxs-lookup"><span data-stu-id="17ac1-105">**MessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="17ac1-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="17ac1-106">Attributes and elements</span></span>

<span data-ttu-id="17ac1-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="17ac1-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="17ac1-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="17ac1-108">Attributes</span></span>

<span data-ttu-id="17ac1-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="17ac1-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="17ac1-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="17ac1-110">Child elements</span></span>

|<span data-ttu-id="17ac1-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="17ac1-111">**Element**</span></span>|<span data-ttu-id="17ac1-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="17ac1-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="17ac1-113">MimeContent</span><span class="sxs-lookup"><span data-stu-id="17ac1-113">MimeContent</span></span>](mimecontent.md) <br/> |<span data-ttu-id="17ac1-114">Содержит собственный поток Multipurpose Internet Mail Extensions (MIME), представленного в формате base64Binary объекта.</span><span class="sxs-lookup"><span data-stu-id="17ac1-114">Contains the native Multipurpose Internet Mail Extensions (MIME) stream of an object that is represented in base64Binary format.</span></span>  <br/> |
|[<span data-ttu-id="17ac1-115">Идентификатор элемента</span><span class="sxs-lookup"><span data-stu-id="17ac1-115">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="17ac1-116">Содержит уникальный идентификатор и меняет ключ элемента в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="17ac1-116">Contains the unique identifier and change key of an item in the Exchange store.</span></span> <span data-ttu-id="17ac1-117">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="17ac1-117">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="17ac1-118">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="17ac1-118">ParentFolderId</span></span>](parentfolderid.md) <br/> |<span data-ttu-id="17ac1-119">Представляет идентификатор родительской папки, содержащей элемент или папку.</span><span class="sxs-lookup"><span data-stu-id="17ac1-119">Represents the identifier of the parent folder that contains the item or folder.</span></span> <span data-ttu-id="17ac1-120">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="17ac1-120">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="17ac1-121">ItemClass</span><span class="sxs-lookup"><span data-stu-id="17ac1-121">ItemClass</span></span>](itemclass.md) <br/> |<span data-ttu-id="17ac1-122">Представляет класс сообщения элемента.</span><span class="sxs-lookup"><span data-stu-id="17ac1-122">Represents the message class of an item.</span></span>  <br/> |
|[<span data-ttu-id="17ac1-123">Subject</span><span class="sxs-lookup"><span data-stu-id="17ac1-123">Subject</span></span>](subject.md) <br/> |<span data-ttu-id="17ac1-124">Представляет тему для элементов хранилища Exchange и объекты ответа.</span><span class="sxs-lookup"><span data-stu-id="17ac1-124">Represents the subject for Exchange store items and response objects.</span></span> <span data-ttu-id="17ac1-125">Тема ограничена 255 символов.</span><span class="sxs-lookup"><span data-stu-id="17ac1-125">The subject is limited to 255 characters.</span></span>  <br/> |
|[<span data-ttu-id="17ac1-126">Уровень конфиденциальности сообщения</span><span class="sxs-lookup"><span data-stu-id="17ac1-126">Sensitivity</span></span>](sensitivity.md) <br/> |<span data-ttu-id="17ac1-127">Указывает уровень конфиденциальности для элемента.</span><span class="sxs-lookup"><span data-stu-id="17ac1-127">Indicates the sensitivity level of an item.</span></span>  <br/> |
|[<span data-ttu-id="17ac1-128">Body</span><span class="sxs-lookup"><span data-stu-id="17ac1-128">Body</span></span>](body.md) <br/> |<span data-ttu-id="17ac1-129">Представляет фактическое содержимое основного текста сообщения.</span><span class="sxs-lookup"><span data-stu-id="17ac1-129">Represents the actual body content of a message.</span></span>  <br/> |
|[<span data-ttu-id="17ac1-130">Вложения</span><span class="sxs-lookup"><span data-stu-id="17ac1-130">Attachments</span></span>](attachments-ex15websvcsotherref.md) <br/> |<span data-ttu-id="17ac1-131">Содержит элементы или файлы, подключенные к элементу в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="17ac1-131">Contains the items or files that are attached to an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="17ac1-132">DateTimeReceived</span><span class="sxs-lookup"><span data-stu-id="17ac1-132">DateTimeReceived</span></span>](datetimereceived.md) <br/> |<span data-ttu-id="17ac1-133">Представляет дату и время получения элемента в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="17ac1-133">Represents the date and time that an item in a mailbox was received.</span></span>  <br/> |
|[<span data-ttu-id="17ac1-134">Размер</span><span class="sxs-lookup"><span data-stu-id="17ac1-134">Size</span></span>](size.md) <br/> |<span data-ttu-id="17ac1-135">Представляет размер в байтах элемента.</span><span class="sxs-lookup"><span data-stu-id="17ac1-135">Represents the size in bytes of an item.</span></span> <span data-ttu-id="17ac1-136">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="17ac1-136">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="17ac1-137">Категории</span><span class="sxs-lookup"><span data-stu-id="17ac1-137">Categories</span></span>](categories-ex15websvcsotherref.md) <br/> |<span data-ttu-id="17ac1-138">Представляет набор строк, чтобы указать, к какой категории относится элемент в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="17ac1-138">Represents a collection of strings that identify to which categories an item in the mailbox belongs.</span></span>  <br/> |
|[<span data-ttu-id="17ac1-139">Важность</span><span class="sxs-lookup"><span data-stu-id="17ac1-139">Importance</span></span>](importance.md) <br/> |<span data-ttu-id="17ac1-140">Описывает важность элемента.</span><span class="sxs-lookup"><span data-stu-id="17ac1-140">Describes the importance of an item.</span></span>  <br/> |
|[<span data-ttu-id="17ac1-141">InReplyTo</span><span class="sxs-lookup"><span data-stu-id="17ac1-141">InReplyTo</span></span>](inreplyto.md) <br/> |<span data-ttu-id="17ac1-142">Представляет идентификатор элемента, к которому этот элемент является ее в ответ.</span><span class="sxs-lookup"><span data-stu-id="17ac1-142">Represents the identifier of the item to which this item is a reply.</span></span>  <br/> |
|[<span data-ttu-id="17ac1-143">IsSubmitted</span><span class="sxs-lookup"><span data-stu-id="17ac1-143">IsSubmitted</span></span>](issubmitted.md) <br/> |<span data-ttu-id="17ac1-144">Указывает, является ли элемент был отправлен исходящие папке по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="17ac1-144">Indicates whether an item has been submitted to the Outbox default folder.</span></span>  <br/> |
|[<span data-ttu-id="17ac1-145">IsDraft</span><span class="sxs-lookup"><span data-stu-id="17ac1-145">IsDraft</span></span>](isdraft.md) <br/> |<span data-ttu-id="17ac1-146">Представляет ли элемент еще не были отправлены.</span><span class="sxs-lookup"><span data-stu-id="17ac1-146">Represents whether an item has not yet been sent.</span></span>  <br/> |
|[<span data-ttu-id="17ac1-147">IsFromMe</span><span class="sxs-lookup"><span data-stu-id="17ac1-147">IsFromMe</span></span>](isfromme.md) <br/> |<span data-ttu-id="17ac1-148">Указывает, отправил ли пользователь элемента для его сами себя.</span><span class="sxs-lookup"><span data-stu-id="17ac1-148">Indicates whether a user sent an item to him or herself.</span></span>  <br/> |
|[<span data-ttu-id="17ac1-149">IsResend</span><span class="sxs-lookup"><span data-stu-id="17ac1-149">IsResend</span></span>](isresend.md) <br/> |<span data-ttu-id="17ac1-150">Указывает, является ли элемент ранее еще был отправлен.</span><span class="sxs-lookup"><span data-stu-id="17ac1-150">Indicates whether the item had previously been sent.</span></span>  <br/> |
|[<span data-ttu-id="17ac1-151">IsUnmodified</span><span class="sxs-lookup"><span data-stu-id="17ac1-151">IsUnmodified</span></span>](isunmodified.md) <br/> |<span data-ttu-id="17ac1-152">Указывает, были ли изменены элемента.</span><span class="sxs-lookup"><span data-stu-id="17ac1-152">Indicates whether the item has been modified.</span></span>  <br/> |
|[<span data-ttu-id="17ac1-153">InternetMessageHeaders</span><span class="sxs-lookup"><span data-stu-id="17ac1-153">InternetMessageHeaders</span></span>](internetmessageheaders.md) <br/> |<span data-ttu-id="17ac1-154">Представляет коллекцию всех заголовков сообщений Интернета, находящихся внутри элемента в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="17ac1-154">Represents the collection of all Internet message headers that are contained within an item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="17ac1-155">DateTimeSent</span><span class="sxs-lookup"><span data-stu-id="17ac1-155">DateTimeSent</span></span>](datetimesent.md) <br/> |<span data-ttu-id="17ac1-156">Представляет дату и время отправки элемента в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="17ac1-156">Represents the date and time that an item in a mailbox was sent.</span></span>  <br/> |
|[<span data-ttu-id="17ac1-157">DateTimeCreated</span><span class="sxs-lookup"><span data-stu-id="17ac1-157">DateTimeCreated</span></span>](datetimecreated.md) <br/> |<span data-ttu-id="17ac1-158">Представляет дату и время создания данного элемента в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="17ac1-158">Represents the date and time that a given item in the mailbox was created.</span></span>  <br/> |
|[<span data-ttu-id="17ac1-159">ResponseObjects</span><span class="sxs-lookup"><span data-stu-id="17ac1-159">ResponseObjects</span></span>](responseobjects.md) <br/> |<span data-ttu-id="17ac1-160">Содержит коллекцию всех объектов ответа, которые связаны с элемента в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="17ac1-160">Contains a collection of all the response objects that are associated with an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="17ac1-161">ReminderDueBy</span><span class="sxs-lookup"><span data-stu-id="17ac1-161">ReminderDueBy</span></span>](reminderdueby.md) <br/> |<span data-ttu-id="17ac1-162">Представляет дату и время, когда происходит событие.</span><span class="sxs-lookup"><span data-stu-id="17ac1-162">Represents the date and time when the event occurs.</span></span> <span data-ttu-id="17ac1-163">Используется в элементе [ReminderMinutesBeforeStart](reminderminutesbeforestart.md) определить, когда отображается оповещение.</span><span class="sxs-lookup"><span data-stu-id="17ac1-163">This is used by the [ReminderMinutesBeforeStart](reminderminutesbeforestart.md) element to determine when the reminder is displayed.</span></span>  <br/> |
|[<span data-ttu-id="17ac1-164">ReminderIsSet</span><span class="sxs-lookup"><span data-stu-id="17ac1-164">ReminderIsSet</span></span>](reminderisset.md) <br/> |<span data-ttu-id="17ac1-165">Указывает, установлен ли напоминания для элемента в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="17ac1-165">Indicates whether a reminder has been set for an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="17ac1-166">ReminderMinutesBeforeStart</span><span class="sxs-lookup"><span data-stu-id="17ac1-166">ReminderMinutesBeforeStart</span></span>](reminderminutesbeforestart.md) <br/> |<span data-ttu-id="17ac1-167">Представляет число минут и только потом событие, когда отображается напоминание.</span><span class="sxs-lookup"><span data-stu-id="17ac1-167">Represents the number of minutes before an event when a reminder is displayed.</span></span>  <br/> |
|[<span data-ttu-id="17ac1-168">DisplayCc</span><span class="sxs-lookup"><span data-stu-id="17ac1-168">DisplayCc</span></span>](displaycc.md) <br/> |<span data-ttu-id="17ac1-169">Строка отображения, который используется для содержимого строку "Копия".</span><span class="sxs-lookup"><span data-stu-id="17ac1-169">Represents the display string that is used for the contents of the CC line.</span></span> <span data-ttu-id="17ac1-170">Это составное строка всех получателей отображаемые имена «копия».</span><span class="sxs-lookup"><span data-stu-id="17ac1-170">This is the concatenated string of all CC recipient display names.</span></span>  <br/> |
|[<span data-ttu-id="17ac1-171">DisplayTo</span><span class="sxs-lookup"><span data-stu-id="17ac1-171">DisplayTo</span></span>](displayto.md) <br/> |<span data-ttu-id="17ac1-172">Строка отображения, который используется для содержимого в поле «Кому».</span><span class="sxs-lookup"><span data-stu-id="17ac1-172">Represents the display string that is used for the contents of the To box.</span></span> <span data-ttu-id="17ac1-173">Это составное строка всех для получателей отображаемые имена.</span><span class="sxs-lookup"><span data-stu-id="17ac1-173">This is the concatenated string of all To recipient display names.</span></span>  <br/> |
|[<span data-ttu-id="17ac1-174">HasAttachments</span><span class="sxs-lookup"><span data-stu-id="17ac1-174">HasAttachments</span></span>](hasattachments.md) <br/> |<span data-ttu-id="17ac1-175">Представляет свойство, которое задано значение **true,** Если у элемента есть по крайней мере один видимым вложения.</span><span class="sxs-lookup"><span data-stu-id="17ac1-175">Represents a property that is set to **true** if an item has at least one visible attachment.</span></span> <span data-ttu-id="17ac1-176">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="17ac1-176">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="17ac1-177">ExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="17ac1-177">ExtendedProperty</span></span>](extendedproperty.md) <br/> |<span data-ttu-id="17ac1-178">Определяет расширенные свойства для папок и элементов.</span><span class="sxs-lookup"><span data-stu-id="17ac1-178">Identifies extended properties on folders and items.</span></span>  <br/> |
|[<span data-ttu-id="17ac1-179">Язык и региональные параметры</span><span class="sxs-lookup"><span data-stu-id="17ac1-179">Culture</span></span>](culture.md) <br/> |<span data-ttu-id="17ac1-180">Представляет язык и региональные параметры для заданного элемента в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="17ac1-180">Represents the culture for a given item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="17ac1-181">Отправитель</span><span class="sxs-lookup"><span data-stu-id="17ac1-181">Sender</span></span>](sender.md) <br/> |<span data-ttu-id="17ac1-182">Идентифицирует отправителя элемента.</span><span class="sxs-lookup"><span data-stu-id="17ac1-182">Identifies the sender of an item.</span></span>  <br/> |
|[<span data-ttu-id="17ac1-183">ToRecipients</span><span class="sxs-lookup"><span data-stu-id="17ac1-183">ToRecipients</span></span>](torecipients.md) <br/> |<span data-ttu-id="17ac1-184">Содержит список получателей сообщения.</span><span class="sxs-lookup"><span data-stu-id="17ac1-184">Contains a set of recipients of a message.</span></span>  <br/> |
|[<span data-ttu-id="17ac1-185">CcRecipients</span><span class="sxs-lookup"><span data-stu-id="17ac1-185">CcRecipients</span></span>](ccrecipients.md) <br/> |<span data-ttu-id="17ac1-186">Представляет коллекцию получателей, которые будут получать копии сообщения.</span><span class="sxs-lookup"><span data-stu-id="17ac1-186">Represents a collection of recipients that will receive a copy of the message.</span></span>  <br/> |
|[<span data-ttu-id="17ac1-187">BccRecipients</span><span class="sxs-lookup"><span data-stu-id="17ac1-187">BccRecipients</span></span>](bccrecipients.md) <br/> |<span data-ttu-id="17ac1-188">Представляет коллекцию получателей скрытой копии (СК) сообщения электронной почты.</span><span class="sxs-lookup"><span data-stu-id="17ac1-188">Represents a collection of recipients to receive a blind carbon copy (Bcc) of an e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="17ac1-189">IsReadReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="17ac1-189">IsReadReceiptRequested</span></span>](isreadreceiptrequested.md) <br/> |<span data-ttu-id="17ac1-190">Указывает, будет ли отправителя элемента о прочтении.</span><span class="sxs-lookup"><span data-stu-id="17ac1-190">Indicates whether the sender of an item requests a read receipt.</span></span>  <br/> |
|[<span data-ttu-id="17ac1-191">IsDeliveryReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="17ac1-191">IsDeliveryReceiptRequested</span></span>](isdeliveryreceiptrequested.md) <br/> |<span data-ttu-id="17ac1-192">Указывает, требует ли отправитель элемента уведомление о доставке.</span><span class="sxs-lookup"><span data-stu-id="17ac1-192">Indicates whether the sender of an item requests a delivery receipt.</span></span>  <br/> |
|[<span data-ttu-id="17ac1-193">ConversationIndex</span><span class="sxs-lookup"><span data-stu-id="17ac1-193">ConversationIndex</span></span>](conversationindex.md) <br/> |<span data-ttu-id="17ac1-194">Содержит двоичные идентификатор, представляющий поток, к которой принадлежит это сообщение.</span><span class="sxs-lookup"><span data-stu-id="17ac1-194">Contains a binary ID that represents the thread to which this message belongs.</span></span>  <br/> |
|[<span data-ttu-id="17ac1-195">ConversationTopic</span><span class="sxs-lookup"><span data-stu-id="17ac1-195">ConversationTopic</span></span>](conversationtopic.md) <br/> |<span data-ttu-id="17ac1-196">Представляет идентификатор беседы.</span><span class="sxs-lookup"><span data-stu-id="17ac1-196">Represents the conversation identifier.</span></span>  <br/> |
|[<span data-ttu-id="17ac1-197">From</span><span class="sxs-lookup"><span data-stu-id="17ac1-197">From</span></span>](from.md) <br/> |<span data-ttu-id="17ac1-198">Представляет получателя, у которого было отправлено сообщение.</span><span class="sxs-lookup"><span data-stu-id="17ac1-198">Represents the addressee from whom the message was sent.</span></span>  <br/> |
|[<span data-ttu-id="17ac1-199">InternetMessageId</span><span class="sxs-lookup"><span data-stu-id="17ac1-199">InternetMessageId</span></span>](internetmessageid.md) <br/> |<span data-ttu-id="17ac1-200">Представляет идентификатор сообщения Интернета элемента.</span><span class="sxs-lookup"><span data-stu-id="17ac1-200">Represents the Internet message identifier of an item.</span></span>  <br/> |
|[<span data-ttu-id="17ac1-201">IsRead</span><span class="sxs-lookup"><span data-stu-id="17ac1-201">IsRead</span></span>](isread.md) <br/> |<span data-ttu-id="17ac1-202">Указывает, имеет ли чтение сообщения.</span><span class="sxs-lookup"><span data-stu-id="17ac1-202">Indicates whether a message has been read.</span></span>  <br/> |
|[<span data-ttu-id="17ac1-203">IsResponseRequested</span><span class="sxs-lookup"><span data-stu-id="17ac1-203">IsResponseRequested</span></span>](isresponserequested.md) <br/> |<span data-ttu-id="17ac1-204">Указывает, запрашивается ли ответ на сообщение электронной почты.</span><span class="sxs-lookup"><span data-stu-id="17ac1-204">Indicates whether a response to an e-mail message is requested.</span></span>  <br/> |
|[<span data-ttu-id="17ac1-205">Справочные материалы</span><span class="sxs-lookup"><span data-stu-id="17ac1-205">References</span></span>](references.md) <br/> |<span data-ttu-id="17ac1-206">Представляет заголовок групп, используемый для сопоставления ответов с исходными сообщениями.</span><span class="sxs-lookup"><span data-stu-id="17ac1-206">Represents the Usenet header that is used to correlate replies with their original messages.</span></span>  <br/> |
|[<span data-ttu-id="17ac1-207">ReplyTo</span><span class="sxs-lookup"><span data-stu-id="17ac1-207">ReplyTo</span></span>](replyto.md) <br/> |<span data-ttu-id="17ac1-208">Определяет набор адресов, к которым будут отправляться ответы.</span><span class="sxs-lookup"><span data-stu-id="17ac1-208">Identifies a set of addresses to which replies should be sent.</span></span>  <br/> |
|[<span data-ttu-id="17ac1-209">EffectiveRights</span><span class="sxs-lookup"><span data-stu-id="17ac1-209">EffectiveRights</span></span>](effectiverights.md) <br/> |<span data-ttu-id="17ac1-210">Содержит права клиента на основании параметров разрешений для элемента или папки.</span><span class="sxs-lookup"><span data-stu-id="17ac1-210">Contains the client's rights based on the permission settings for the item or folder.</span></span> <span data-ttu-id="17ac1-211">Этот элемент доступен только для чтения.</span><span class="sxs-lookup"><span data-stu-id="17ac1-211">This element is read-only.</span></span>  <br/> |
|[<span data-ttu-id="17ac1-212">Получил</span><span class="sxs-lookup"><span data-stu-id="17ac1-212">ReceivedBy</span></span>](receivedby.md) <br/> |<span data-ttu-id="17ac1-213">Определяет делегат в сценарии доступа делегата.</span><span class="sxs-lookup"><span data-stu-id="17ac1-213">Identifies the delegate in a delegate access scenario.</span></span>  <br/> |
|[<span data-ttu-id="17ac1-214">ReceivedRepresenting</span><span class="sxs-lookup"><span data-stu-id="17ac1-214">ReceivedRepresenting</span></span>](receivedrepresenting.md) <br/> |<span data-ttu-id="17ac1-215">Идентифицирует участника в сценарии доступа делегата.</span><span class="sxs-lookup"><span data-stu-id="17ac1-215">Identifies the principal in a delegate access scenario.</span></span>  <br/> |
|[<span data-ttu-id="17ac1-216">LastModifiedName</span><span class="sxs-lookup"><span data-stu-id="17ac1-216">LastModifiedName</span></span>](lastmodifiedname.md) <br/> |<span data-ttu-id="17ac1-217">Содержит отображаемое имя последнего пользователя, чтобы изменить элемент.</span><span class="sxs-lookup"><span data-stu-id="17ac1-217">Contains the display name of the last user to modify an item.</span></span>  <br/> |
|[<span data-ttu-id="17ac1-218">LastModifiedTime</span><span class="sxs-lookup"><span data-stu-id="17ac1-218">LastModifiedTime</span></span>](lastmodifiedtime.md) <br/> |<span data-ttu-id="17ac1-219">Указывает время последнего изменения элемента.</span><span class="sxs-lookup"><span data-stu-id="17ac1-219">Indicates when an item was last modified.</span></span>  <br/> |
|[<span data-ttu-id="17ac1-220">IsAssociated</span><span class="sxs-lookup"><span data-stu-id="17ac1-220">IsAssociated</span></span>](isassociated.md) <br/> |<span data-ttu-id="17ac1-221">Указывает, является ли элемент связан с папкой.</span><span class="sxs-lookup"><span data-stu-id="17ac1-221">Indicates whether the item is associated with a folder.</span></span>  <br/> |
|[<span data-ttu-id="17ac1-222">WebClientReadFormQueryString</span><span class="sxs-lookup"><span data-stu-id="17ac1-222">WebClientReadFormQueryString</span></span>](webclientreadformquerystring.md) <br/> |<span data-ttu-id="17ac1-223">Представляет URL-адрес для присоединения к конечной точке Microsoft Office Outlook Web App для чтения элемента в Outlook Web App.</span><span class="sxs-lookup"><span data-stu-id="17ac1-223">Represents a URL to concatenate to the Microsoft Office Outlook Web App endpoint to read an item in Outlook Web App.</span></span>  <br/> |
|[<span data-ttu-id="17ac1-224">WebClientEditFormQueryString</span><span class="sxs-lookup"><span data-stu-id="17ac1-224">WebClientEditFormQueryString</span></span>](webclienteditformquerystring.md) <br/> |<span data-ttu-id="17ac1-225">Представляет URL-адрес для объединения в конечную точку Outlook Web App для редактирования элемента в Outlook Web App.</span><span class="sxs-lookup"><span data-stu-id="17ac1-225">Represents a URL to concatenate to the Outlook Web App endpoint to edit an item in Outlook Web App.</span></span>  <br/> |
|[<span data-ttu-id="17ac1-226">ConversationId</span><span class="sxs-lookup"><span data-stu-id="17ac1-226">ConversationId</span></span>](conversationid.md) <br/> |<span data-ttu-id="17ac1-227">Содержит идентификатор элемента или беседы.</span><span class="sxs-lookup"><span data-stu-id="17ac1-227">Contains the identifier of an item or conversation.</span></span>  <br/> |
|[<span data-ttu-id="17ac1-228">UniqueBody</span><span class="sxs-lookup"><span data-stu-id="17ac1-228">UniqueBody</span></span>](uniquebody.md) <br/> |<span data-ttu-id="17ac1-229">Представляет фрагмент HTML или обычный текст, который представляет уникальное body эту беседу.</span><span class="sxs-lookup"><span data-stu-id="17ac1-229">Represents an HTML fragment or plain text which represents the unique body of this conversation.</span></span>  <br/> |
|[<span data-ttu-id="17ac1-230">ReminderMessageData</span><span class="sxs-lookup"><span data-stu-id="17ac1-230">ReminderMessageData</span></span>](remindermessagedata.md) <br/> |<span data-ttu-id="17ac1-231">Содержит данные для напоминания о сообщении.</span><span class="sxs-lookup"><span data-stu-id="17ac1-231">Contains the data for a reminder message.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="17ac1-232">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="17ac1-232">Parent elements</span></span>

|<span data-ttu-id="17ac1-233">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="17ac1-233">**Element**</span></span>|<span data-ttu-id="17ac1-234">**Описание**</span><span class="sxs-lookup"><span data-stu-id="17ac1-234">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="17ac1-235">AdjacentMeetings</span><span class="sxs-lookup"><span data-stu-id="17ac1-235">AdjacentMeetings</span></span>](adjacentmeetings.md) <br/> |<span data-ttu-id="17ac1-236">Описание всех элементов календаря, расположенных на время собрания.</span><span class="sxs-lookup"><span data-stu-id="17ac1-236">Describes all calendar items that are adjacent to a meeting time.</span></span>  <br/> |
|[<span data-ttu-id="17ac1-237">AppendToItemField</span><span class="sxs-lookup"><span data-stu-id="17ac1-237">AppendToItemField</span></span>](appendtoitemfield.md) <br/> |<span data-ttu-id="17ac1-238">Указывает данные для добавления к отдельное свойство элемента во время [операции UpdateItem](updateitem-operation.md).</span><span class="sxs-lookup"><span data-stu-id="17ac1-238">Identifies data to append to a single property of an item during an [UpdateItem operation](updateitem-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="17ac1-239">ConflictingMeetings</span><span class="sxs-lookup"><span data-stu-id="17ac1-239">ConflictingMeetings</span></span>](conflictingmeetings.md) <br/> |<span data-ttu-id="17ac1-240">Определяет все элементы, конфликтующие с время собрания.</span><span class="sxs-lookup"><span data-stu-id="17ac1-240">Identifies all items that conflict with a meeting time.</span></span>  <br/> |
|[<span data-ttu-id="17ac1-241">Создание (ItemSync)</span><span class="sxs-lookup"><span data-stu-id="17ac1-241">Create (ItemSync)</span></span>](create-itemsync.md) <br/> |<span data-ttu-id="17ac1-242">Определяет один элемент для создания в локальном хранилище клиента.</span><span class="sxs-lookup"><span data-stu-id="17ac1-242">Identifies a single item to create in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="17ac1-243">ItemAttachment</span><span class="sxs-lookup"><span data-stu-id="17ac1-243">ItemAttachment</span></span>](itemattachment.md) <br/> |<span data-ttu-id="17ac1-244">Представляет собой элемент Exchange, подключенный к другой элемент Exchange.</span><span class="sxs-lookup"><span data-stu-id="17ac1-244">Represents an Exchange item that is attached to another Exchange item.</span></span>  <br/> |
|[<span data-ttu-id="17ac1-245">Элементы</span><span class="sxs-lookup"><span data-stu-id="17ac1-245">Items</span></span>](items.md) <br/> |<span data-ttu-id="17ac1-246">Содержит массив элементов.</span><span class="sxs-lookup"><span data-stu-id="17ac1-246">Contains an array of items.</span></span>  <br/> |
|[<span data-ttu-id="17ac1-247">Элементы (NonEmptyArrayOfAllItemsType)</span><span class="sxs-lookup"><span data-stu-id="17ac1-247">Items (NonEmptyArrayOfAllItemsType)</span></span>](items-nonemptyarrayofallitemstype.md) <br/> |<span data-ttu-id="17ac1-248">Содержит массив элементов для создания в папке, указанной с помощью элемента [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) .</span><span class="sxs-lookup"><span data-stu-id="17ac1-248">Contains an array of items to create in the folder that is identified by the [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) element.</span></span>  <br/> |
|[<span data-ttu-id="17ac1-249">SetItemField</span><span class="sxs-lookup"><span data-stu-id="17ac1-249">SetItemField</span></span>](setitemfield.md) <br/> |<span data-ttu-id="17ac1-250">Представляет отдельное свойство элемента в [UpdateItem операции](updateitem-operation.md)обновления.</span><span class="sxs-lookup"><span data-stu-id="17ac1-250">Represents an update to a single property of an item in an [UpdateItem operation](updateitem-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="17ac1-251">Обновление (ItemSync)</span><span class="sxs-lookup"><span data-stu-id="17ac1-251">Update (ItemSync)</span></span>](update-itemsync.md) <br/> |<span data-ttu-id="17ac1-252">Определяет один элемент для обновления в локальном хранилище клиента.</span><span class="sxs-lookup"><span data-stu-id="17ac1-252">Identifies a single item to update in the local client store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="17ac1-253">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="17ac1-253">Text value</span></span>

<span data-ttu-id="17ac1-254">Нет.</span><span class="sxs-lookup"><span data-stu-id="17ac1-254">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="17ac1-255">Замечания</span><span class="sxs-lookup"><span data-stu-id="17ac1-255">Remarks</span></span>

<span data-ttu-id="17ac1-256">Другой элемент **сообщения** , [сообщение (доступность)](message-availability.md) используется операции доступности для возврата сообщения об отсутствии на работе.</span><span class="sxs-lookup"><span data-stu-id="17ac1-256">Another **Message** element, [Message (Availability)](message-availability.md) is used by the Availability operations to return OOF messages.</span></span> 
  
<span data-ttu-id="17ac1-257">Элементы [сообщения](message-ex15websvcsotherref.md) представляют сообщения электронной почты и другие элементы, которые не строго типизированные схемой веб-служб Exchange (EWS).</span><span class="sxs-lookup"><span data-stu-id="17ac1-257">[Message](message-ex15websvcsotherref.md) elements represent e-mail messages and all other items that are not strongly typed by the Exchange Web Services (EWS) schema.</span></span> <span data-ttu-id="17ac1-258">Элементы, такие как IPM. Общий доступ и IPM.InfoPath возвращаются в виде элементы **сообщения** .</span><span class="sxs-lookup"><span data-stu-id="17ac1-258">Items such as IPM.Sharing and IPM.InfoPath are returned as **Message** elements.</span></span> <span data-ttu-id="17ac1-259">Exchange 2010 не возвращает **базовый элемент** в ответы.</span><span class="sxs-lookup"><span data-stu-id="17ac1-259">Exchange 2010 does not return the base **Item** element in responses.</span></span> 
  
<span data-ttu-id="17ac1-260">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="17ac1-260">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="17ac1-261">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="17ac1-261">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="17ac1-262">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="17ac1-262">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="17ac1-263">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="17ac1-263">Schema Name</span></span>  <br/> |<span data-ttu-id="17ac1-264">Схема Types</span><span class="sxs-lookup"><span data-stu-id="17ac1-264">Types schema</span></span>  <br/> |
|<span data-ttu-id="17ac1-265">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="17ac1-265">Validation File</span></span>  <br/> |<span data-ttu-id="17ac1-266">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="17ac1-266">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="17ac1-267">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="17ac1-267">Can be Empty</span></span>  <br/> |<span data-ttu-id="17ac1-268">False</span><span class="sxs-lookup"><span data-stu-id="17ac1-268">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="17ac1-269">См. также</span><span class="sxs-lookup"><span data-stu-id="17ac1-269">See also</span></span>



- [<span data-ttu-id="17ac1-270">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="17ac1-270">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

