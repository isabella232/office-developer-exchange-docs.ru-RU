---
title: MeetingMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MeetingMessage
api_type:
- schema
ms.assetid: c95956a8-7505-44b4-bea4-11d1f5182796
description: Элемент MeetingMessage представляет собрания в хранилище Exchange.
ms.openlocfilehash: a2e87bc9800ee1dc66c1a3110df76745ac7c05b6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19834443"
---
# <a name="meetingmessage"></a><span data-ttu-id="3f437-103">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="3f437-103">MeetingMessage</span></span>

<span data-ttu-id="3f437-104">Элемент **MeetingMessage** представляет собрания в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="3f437-104">The **MeetingMessage** element represents a meeting in the Exchange store.</span></span> 
  
```xml
<MeetingMessage>
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
   <AssociatedCalendarItemId/>
   <IsDelegated/>
   <IsOutOfDate/>
   <HasBeenProcessed/>
   <ResponseType/>
   <EffectiveRights/>
   <LastModifiedName/>
   <LastModifiedTime/>
   <IsAssociated/>
   <WebClientReadFormQueryString/>
   <WebClientEditFormQueryString/>
   <ConversationId/>
   <UniqueBody/>
</MeetingMessage>
```

 <span data-ttu-id="3f437-105">**MeetingMessageType**</span><span class="sxs-lookup"><span data-stu-id="3f437-105">**MeetingMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3f437-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="3f437-106">Attributes and elements</span></span>

<span data-ttu-id="3f437-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="3f437-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3f437-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="3f437-108">Attributes</span></span>

<span data-ttu-id="3f437-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="3f437-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3f437-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="3f437-110">Child elements</span></span>

|<span data-ttu-id="3f437-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="3f437-111">**Element**</span></span>|<span data-ttu-id="3f437-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="3f437-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3f437-113">MimeContent</span><span class="sxs-lookup"><span data-stu-id="3f437-113">MimeContent</span></span>](mimecontent.md) <br/> |<span data-ttu-id="3f437-114">Содержит собственный поток MIME, представленного в формате base64Binary объекта.</span><span class="sxs-lookup"><span data-stu-id="3f437-114">Contains the native MIME stream of an object that is represented in base64Binary format.</span></span>  <br/> |
|[<span data-ttu-id="3f437-115">Идентификатор элемента</span><span class="sxs-lookup"><span data-stu-id="3f437-115">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="3f437-116">Содержит уникальный идентификатор и меняет ключ элемента в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="3f437-116">Contains the unique identifier and change key of an item in the Exchange store.</span></span> <span data-ttu-id="3f437-117">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3f437-117">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="3f437-118">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="3f437-118">ParentFolderId</span></span>](parentfolderid.md) <br/> |<span data-ttu-id="3f437-119">Представляет идентификатор родительской папки, содержащей элемент или папку.</span><span class="sxs-lookup"><span data-stu-id="3f437-119">Represents the identifier of the parent folder that contains the item or folder.</span></span> <span data-ttu-id="3f437-120">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3f437-120">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="3f437-121">ItemClass</span><span class="sxs-lookup"><span data-stu-id="3f437-121">ItemClass</span></span>](itemclass.md) <br/> |<span data-ttu-id="3f437-122">Представляет класс сообщения элемента.</span><span class="sxs-lookup"><span data-stu-id="3f437-122">Represents the message class of an item.</span></span>  <br/> |
|[<span data-ttu-id="3f437-123">Subject</span><span class="sxs-lookup"><span data-stu-id="3f437-123">Subject</span></span>](subject.md) <br/> |<span data-ttu-id="3f437-124">Представляет тему для элементов хранилища Exchange и объекты ответа.</span><span class="sxs-lookup"><span data-stu-id="3f437-124">Represents the subject for Exchange store items and response objects.</span></span> <span data-ttu-id="3f437-125">Тема ограничена 255 символов.</span><span class="sxs-lookup"><span data-stu-id="3f437-125">The subject is limited to 255 characters.</span></span>  <br/> |
|[<span data-ttu-id="3f437-126">Уровень конфиденциальности сообщения</span><span class="sxs-lookup"><span data-stu-id="3f437-126">Sensitivity</span></span>](sensitivity.md) <br/> |<span data-ttu-id="3f437-127">Содержит сведения о состоянии уровень конфиденциальности сообщения элемента.</span><span class="sxs-lookup"><span data-stu-id="3f437-127">Contains the status for an item's sensitivity.</span></span>  <br/> |
|[<span data-ttu-id="3f437-128">Body</span><span class="sxs-lookup"><span data-stu-id="3f437-128">Body</span></span>](body.md) <br/> |<span data-ttu-id="3f437-129">Представляет фактическое содержимое основного текста сообщения.</span><span class="sxs-lookup"><span data-stu-id="3f437-129">Represents the actual body content of a message.</span></span>  <br/> |
|[<span data-ttu-id="3f437-130">Вложения</span><span class="sxs-lookup"><span data-stu-id="3f437-130">Attachments</span></span>](attachments-ex15websvcsotherref.md) <br/> |<span data-ttu-id="3f437-131">Содержит элементы или файлы, подключенные к элементу в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="3f437-131">Contains the items or files that are attached to an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="3f437-132">DateTimeReceived</span><span class="sxs-lookup"><span data-stu-id="3f437-132">DateTimeReceived</span></span>](datetimereceived.md) <br/> |<span data-ttu-id="3f437-133">Представляет дату и время получения элемента в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="3f437-133">Represents the date and time that an item in a mailbox was received.</span></span>  <br/> |
|[<span data-ttu-id="3f437-134">Размер</span><span class="sxs-lookup"><span data-stu-id="3f437-134">Size</span></span>](size.md) <br/> |<span data-ttu-id="3f437-135">Представляет размер в байтах элемента.</span><span class="sxs-lookup"><span data-stu-id="3f437-135">Represents the size in bytes of an item.</span></span> <span data-ttu-id="3f437-136">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3f437-136">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="3f437-137">Категории</span><span class="sxs-lookup"><span data-stu-id="3f437-137">Categories</span></span>](categories-ex15websvcsotherref.md) <br/> |<span data-ttu-id="3f437-138">Представляет набор строк, чтобы указать, к какой категории относится элемент в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="3f437-138">Represents a collection of strings that identify to which categories an item in the mailbox belongs.</span></span>  <br/> |
|[<span data-ttu-id="3f437-139">Важность</span><span class="sxs-lookup"><span data-stu-id="3f437-139">Importance</span></span>](importance.md) <br/> |<span data-ttu-id="3f437-140">Описывает важность элемента.</span><span class="sxs-lookup"><span data-stu-id="3f437-140">Describes the importance of an item.</span></span>  <br/> |
|[<span data-ttu-id="3f437-141">InReplyTo</span><span class="sxs-lookup"><span data-stu-id="3f437-141">InReplyTo</span></span>](inreplyto.md) <br/> |<span data-ttu-id="3f437-142">Представляет идентификатор элемента, к которому этот элемент является ее в ответ.</span><span class="sxs-lookup"><span data-stu-id="3f437-142">Represents the identifier of the item to which this item is a reply.</span></span>  <br/> |
|[<span data-ttu-id="3f437-143">IsSubmitted</span><span class="sxs-lookup"><span data-stu-id="3f437-143">IsSubmitted</span></span>](issubmitted.md) <br/> |<span data-ttu-id="3f437-144">Указывает, является ли элемент был отправлен исходящие папке по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="3f437-144">Indicates whether an item has been submitted to the Outbox default folder.</span></span>  <br/> |
|[<span data-ttu-id="3f437-145">IsDraft</span><span class="sxs-lookup"><span data-stu-id="3f437-145">IsDraft</span></span>](isdraft.md) <br/> |<span data-ttu-id="3f437-146">Представляет ли элемент еще не были отправлены.</span><span class="sxs-lookup"><span data-stu-id="3f437-146">Represents whether an item has not yet been sent.</span></span>  <br/> |
|[<span data-ttu-id="3f437-147">IsFromMe</span><span class="sxs-lookup"><span data-stu-id="3f437-147">IsFromMe</span></span>](isfromme.md) <br/> |<span data-ttu-id="3f437-148">Указывает, отправил ли пользователь элемента для его сами себя.</span><span class="sxs-lookup"><span data-stu-id="3f437-148">Indicates whether a user sent an item to him or herself.</span></span>  <br/> |
|[<span data-ttu-id="3f437-149">IsResend</span><span class="sxs-lookup"><span data-stu-id="3f437-149">IsResend</span></span>](isresend.md) <br/> |<span data-ttu-id="3f437-150">Указывает, является ли элемент ранее еще был отправлен.</span><span class="sxs-lookup"><span data-stu-id="3f437-150">Indicates whether the item had previously been sent.</span></span>  <br/> |
|[<span data-ttu-id="3f437-151">IsUnmodified</span><span class="sxs-lookup"><span data-stu-id="3f437-151">IsUnmodified</span></span>](isunmodified.md) <br/> |<span data-ttu-id="3f437-152">Указывает, были ли изменены элемента.</span><span class="sxs-lookup"><span data-stu-id="3f437-152">Indicates whether the item has been modified.</span></span>  <br/> |
|[<span data-ttu-id="3f437-153">InternetMessageHeaders</span><span class="sxs-lookup"><span data-stu-id="3f437-153">InternetMessageHeaders</span></span>](internetmessageheaders.md) <br/> |<span data-ttu-id="3f437-154">Представляет коллекцию всех заголовков сообщений Интернета, находящихся внутри элемента в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="3f437-154">Represents the collection of all Internet message headers that are contained within an item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="3f437-155">DateTimeSent</span><span class="sxs-lookup"><span data-stu-id="3f437-155">DateTimeSent</span></span>](datetimesent.md) <br/> |<span data-ttu-id="3f437-156">Представляет дату и время отправки элемента в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="3f437-156">Represents the date and time that an item in a mailbox was sent.</span></span>  <br/> |
|[<span data-ttu-id="3f437-157">DateTimeCreated</span><span class="sxs-lookup"><span data-stu-id="3f437-157">DateTimeCreated</span></span>](datetimecreated.md) <br/> |<span data-ttu-id="3f437-158">Представляет дату и время создания данного элемента в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="3f437-158">Represents the date and time that a given item in the mailbox was created.</span></span>  <br/> |
|[<span data-ttu-id="3f437-159">ResponseObjects</span><span class="sxs-lookup"><span data-stu-id="3f437-159">ResponseObjects</span></span>](responseobjects.md) <br/> |<span data-ttu-id="3f437-160">Содержит коллекцию всех объектов ответа, которые связаны с элемента в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="3f437-160">Contains a collection of all the response objects that are associated with an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="3f437-161">ReminderDueBy</span><span class="sxs-lookup"><span data-stu-id="3f437-161">ReminderDueBy</span></span>](reminderdueby.md) <br/> |<span data-ttu-id="3f437-162">Представляет дату и время, когда происходит событие.</span><span class="sxs-lookup"><span data-stu-id="3f437-162">Represents the date and time when the event occurs.</span></span> <span data-ttu-id="3f437-163">Используется в элементе [ReminderMinutesBeforeStart](reminderminutesbeforestart.md) определить, когда отображается оповещение.</span><span class="sxs-lookup"><span data-stu-id="3f437-163">This is used by the [ReminderMinutesBeforeStart](reminderminutesbeforestart.md) element to determine when the reminder is displayed.</span></span>  <br/> |
|[<span data-ttu-id="3f437-164">ReminderIsSet</span><span class="sxs-lookup"><span data-stu-id="3f437-164">ReminderIsSet</span></span>](reminderisset.md) <br/> |<span data-ttu-id="3f437-165">Указывает, установлен ли напоминания для элемента в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="3f437-165">Indicates whether a reminder has been set for an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="3f437-166">ReminderMinutesBeforeStart</span><span class="sxs-lookup"><span data-stu-id="3f437-166">ReminderMinutesBeforeStart</span></span>](reminderminutesbeforestart.md) <br/> |<span data-ttu-id="3f437-167">Представляет число минут и только потом событие, когда отображается напоминание.</span><span class="sxs-lookup"><span data-stu-id="3f437-167">Represents the number of minutes before an event when a reminder is displayed.</span></span>  <br/> |
|[<span data-ttu-id="3f437-168">DisplayCc</span><span class="sxs-lookup"><span data-stu-id="3f437-168">DisplayCc</span></span>](displaycc.md) <br/> |<span data-ttu-id="3f437-169">Строка отображения, который используется для содержимого в поле "Копия".</span><span class="sxs-lookup"><span data-stu-id="3f437-169">Represents the display string that is used for the contents of the Cc box.</span></span> <span data-ttu-id="3f437-170">Это составное строка всех получателей отображаемые имена «копия».</span><span class="sxs-lookup"><span data-stu-id="3f437-170">This is the concatenated string of all Cc recipient display names.</span></span>  <br/> |
|[<span data-ttu-id="3f437-171">DisplayTo</span><span class="sxs-lookup"><span data-stu-id="3f437-171">DisplayTo</span></span>](displayto.md) <br/> |<span data-ttu-id="3f437-172">Строка отображения, который используется для содержимого в поле «Кому».</span><span class="sxs-lookup"><span data-stu-id="3f437-172">Represents the display string that is used for the contents of the To box.</span></span> <span data-ttu-id="3f437-173">Это составное строка всех для получателей отображаемые имена.</span><span class="sxs-lookup"><span data-stu-id="3f437-173">This is the concatenated string of all To recipient display names.</span></span>  <br/> |
|[<span data-ttu-id="3f437-174">HasAttachments</span><span class="sxs-lookup"><span data-stu-id="3f437-174">HasAttachments</span></span>](hasattachments.md) <br/> |<span data-ttu-id="3f437-175">Представляет свойство, которое задано значение **true,** Если у элемента есть по крайней мере один видимым вложения.</span><span class="sxs-lookup"><span data-stu-id="3f437-175">Represents a property that is set to **true** if an item has at least one visible attachment.</span></span> <span data-ttu-id="3f437-176">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3f437-176">This property is read only.</span></span>  <br/> |
|[<span data-ttu-id="3f437-177">ExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="3f437-177">ExtendedProperty</span></span>](extendedproperty.md) <br/> |<span data-ttu-id="3f437-178">Определяет расширенные свойства для папок и элементов.</span><span class="sxs-lookup"><span data-stu-id="3f437-178">Identifies extended properties on folders and items.</span></span>  <br/> |
|[<span data-ttu-id="3f437-179">Язык и региональные параметры</span><span class="sxs-lookup"><span data-stu-id="3f437-179">Culture</span></span>](culture.md) <br/> |<span data-ttu-id="3f437-180">Представляет язык и региональные параметры для заданного элемента в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="3f437-180">Represents the culture for a given item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="3f437-181">Отправитель</span><span class="sxs-lookup"><span data-stu-id="3f437-181">Sender</span></span>](sender.md) <br/> |<span data-ttu-id="3f437-182">Идентифицирует отправителя элемента.</span><span class="sxs-lookup"><span data-stu-id="3f437-182">Identifies the sender of an item.</span></span>  <br/> |
|[<span data-ttu-id="3f437-183">ToRecipients</span><span class="sxs-lookup"><span data-stu-id="3f437-183">ToRecipients</span></span>](torecipients.md) <br/> |<span data-ttu-id="3f437-184">Содержит список получателей сообщения.</span><span class="sxs-lookup"><span data-stu-id="3f437-184">Contains a set of recipients of a message.</span></span>  <br/> |
|[<span data-ttu-id="3f437-185">CcRecipients</span><span class="sxs-lookup"><span data-stu-id="3f437-185">CcRecipients</span></span>](ccrecipients.md) <br/> |<span data-ttu-id="3f437-186">Представляет коллекцию получателей, которые будут получать копии сообщения.</span><span class="sxs-lookup"><span data-stu-id="3f437-186">Represents a collection of recipients that will receive a copy of the message.</span></span>  <br/> |
|[<span data-ttu-id="3f437-187">BccRecipients</span><span class="sxs-lookup"><span data-stu-id="3f437-187">BccRecipients</span></span>](bccrecipients.md) <br/> |<span data-ttu-id="3f437-188">Представляет коллекцию получателей скрытой копии (СК) сообщения электронной почты.</span><span class="sxs-lookup"><span data-stu-id="3f437-188">Represents a collection of recipients to receive a blind carbon copy (Bcc) of an e-mail.</span></span>  <br/> |
|[<span data-ttu-id="3f437-189">IsReadReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="3f437-189">IsReadReceiptRequested</span></span>](isreadreceiptrequested.md) <br/> |<span data-ttu-id="3f437-190">Указывает, будет ли отправителя элемента о прочтении.</span><span class="sxs-lookup"><span data-stu-id="3f437-190">Indicates whether the sender of an item requests a read receipt.</span></span>  <br/> |
|[<span data-ttu-id="3f437-191">IsDeliveryReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="3f437-191">IsDeliveryReceiptRequested</span></span>](isdeliveryreceiptrequested.md) <br/> |<span data-ttu-id="3f437-192">Указывает, требует ли отправитель элемента уведомление о доставке.</span><span class="sxs-lookup"><span data-stu-id="3f437-192">Indicates whether the sender of an item requests a delivery receipt.</span></span>  <br/> |
|[<span data-ttu-id="3f437-193">ConversationIndex</span><span class="sxs-lookup"><span data-stu-id="3f437-193">ConversationIndex</span></span>](conversationindex.md) <br/> |<span data-ttu-id="3f437-194">Содержит двоичные идентификатор, представляющий поток, к которой принадлежит это сообщение.</span><span class="sxs-lookup"><span data-stu-id="3f437-194">Contains a binary ID that represents the thread to which this message belongs.</span></span>  <br/> |
|[<span data-ttu-id="3f437-195">ConversationTopic</span><span class="sxs-lookup"><span data-stu-id="3f437-195">ConversationTopic</span></span>](conversationtopic.md) <br/> |<span data-ttu-id="3f437-196">Представляет идентификатор беседы.</span><span class="sxs-lookup"><span data-stu-id="3f437-196">Represents the conversation identifier.</span></span>  <br/> |
|[<span data-ttu-id="3f437-197">From</span><span class="sxs-lookup"><span data-stu-id="3f437-197">From</span></span>](from.md) <br/> |<span data-ttu-id="3f437-198">Представляет получателя, у которого было отправлено сообщение.</span><span class="sxs-lookup"><span data-stu-id="3f437-198">Represents the addressee from whom the message was sent.</span></span>  <br/> |
|[<span data-ttu-id="3f437-199">InternetMessageId</span><span class="sxs-lookup"><span data-stu-id="3f437-199">InternetMessageId</span></span>](internetmessageid.md) <br/> |<span data-ttu-id="3f437-200">Представляет идентификатор сообщения Интернета элемента.</span><span class="sxs-lookup"><span data-stu-id="3f437-200">Represents the Internet message identifier of an item.</span></span>  <br/> |
|[<span data-ttu-id="3f437-201">IsRead</span><span class="sxs-lookup"><span data-stu-id="3f437-201">IsRead</span></span>](isread.md) <br/> |<span data-ttu-id="3f437-202">Указывает, имеет ли чтение сообщения.</span><span class="sxs-lookup"><span data-stu-id="3f437-202">Indicates whether a message has been read.</span></span>  <br/> |
|[<span data-ttu-id="3f437-203">IsResponseRequested</span><span class="sxs-lookup"><span data-stu-id="3f437-203">IsResponseRequested</span></span>](isresponserequested.md) <br/> |<span data-ttu-id="3f437-204">Указывает, запрашивается ли ответ на сообщение электронной почты.</span><span class="sxs-lookup"><span data-stu-id="3f437-204">Indicates whether a response to an e-mail message is requested.</span></span>  <br/> |
|[<span data-ttu-id="3f437-205">Справочные материалы</span><span class="sxs-lookup"><span data-stu-id="3f437-205">References</span></span>](references.md) <br/> |<span data-ttu-id="3f437-206">Представляет заголовок групп, используемый для сопоставления ответов с исходными сообщениями.</span><span class="sxs-lookup"><span data-stu-id="3f437-206">Represents the Usenet header that is used to correlate replies with their original messages.</span></span>  <br/> |
|[<span data-ttu-id="3f437-207">ReplyTo</span><span class="sxs-lookup"><span data-stu-id="3f437-207">ReplyTo</span></span>](replyto.md) <br/> |<span data-ttu-id="3f437-208">Определяет набор адресов, к которым будут отправляться ответы.</span><span class="sxs-lookup"><span data-stu-id="3f437-208">Identifies a set of addresses to which replies should be sent.</span></span>  <br/> |
|[<span data-ttu-id="3f437-209">AssociatedCalendarItemId</span><span class="sxs-lookup"><span data-stu-id="3f437-209">AssociatedCalendarItemId</span></span>](associatedcalendaritemid.md) <br/> |<span data-ttu-id="3f437-210">Представляет элемент календаря, связанного с [MeetingMessage](meetingmessage.md).</span><span class="sxs-lookup"><span data-stu-id="3f437-210">Represents the calendar item that is associated with a [MeetingMessage](meetingmessage.md).</span></span>  <br/> |
|[<span data-ttu-id="3f437-211">IsDelegated</span><span class="sxs-lookup"><span data-stu-id="3f437-211">IsDelegated</span></span>](isdelegated.md) <br/> |<span data-ttu-id="3f437-212">Указывает, обработано ли собрания с помощью учетной записи с доступом к делегата.</span><span class="sxs-lookup"><span data-stu-id="3f437-212">Indicates whether a meeting was handled by an account with delegate access.</span></span>  <br/> |
|[<span data-ttu-id="3f437-213">IsOutOfDate</span><span class="sxs-lookup"><span data-stu-id="3f437-213">IsOutOfDate</span></span>](isoutofdate.md) <br/> |<span data-ttu-id="3f437-214">Указывает, является ли устаревших сообщений собрания.</span><span class="sxs-lookup"><span data-stu-id="3f437-214">Indicates whether a meeting message is out-of-date.</span></span>  <br/> |
|[<span data-ttu-id="3f437-215">HasBeenProcessed</span><span class="sxs-lookup"><span data-stu-id="3f437-215">HasBeenProcessed</span></span>](hasbeenprocessed.md) <br/> |<span data-ttu-id="3f437-216">Указывает ли сообщение собрания элемент обработки.</span><span class="sxs-lookup"><span data-stu-id="3f437-216">Indicates whether a meeting message item has been processed.</span></span>  <br/> |
|[<span data-ttu-id="3f437-217">ResponseType</span><span class="sxs-lookup"><span data-stu-id="3f437-217">ResponseType</span></span>](responsetype.md) <br/> |<span data-ttu-id="3f437-218">Представляет тип получателя ответа, полученные при проведении собраний.</span><span class="sxs-lookup"><span data-stu-id="3f437-218">Represents the type of recipient response received for a meeting.</span></span>  <br/> |
|[<span data-ttu-id="3f437-219">EffectiveRights</span><span class="sxs-lookup"><span data-stu-id="3f437-219">EffectiveRights</span></span>](effectiverights.md) <br/> |<span data-ttu-id="3f437-220">Содержит права клиента на основании параметров разрешений для элемента или папки.</span><span class="sxs-lookup"><span data-stu-id="3f437-220">Contains the client's rights based on the permission settings for the item or folder.</span></span> <span data-ttu-id="3f437-221">Этот элемент доступен только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3f437-221">This element is read-only.</span></span> <span data-ttu-id="3f437-222">Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="3f437-222">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span>  <br/> |
|[<span data-ttu-id="3f437-223">LastModifiedName</span><span class="sxs-lookup"><span data-stu-id="3f437-223">LastModifiedName</span></span>](lastmodifiedname.md) <br/> |<span data-ttu-id="3f437-224">Содержит отображаемое имя последнего пользователя, чтобы изменить элемент.</span><span class="sxs-lookup"><span data-stu-id="3f437-224">Contains the display name of the last user to modify an item.</span></span>  <br/> |
|[<span data-ttu-id="3f437-225">LastModifiedTime</span><span class="sxs-lookup"><span data-stu-id="3f437-225">LastModifiedTime</span></span>](lastmodifiedtime.md) <br/> |<span data-ttu-id="3f437-226">Указывает время последнего изменения элемента.</span><span class="sxs-lookup"><span data-stu-id="3f437-226">Indicates when an item was last modified.</span></span>  <br/> |
|[<span data-ttu-id="3f437-227">IsAssociated</span><span class="sxs-lookup"><span data-stu-id="3f437-227">IsAssociated</span></span>](isassociated.md) <br/> |<span data-ttu-id="3f437-228">Указывает, является ли элемент связан с папкой.</span><span class="sxs-lookup"><span data-stu-id="3f437-228">Indicates whether the item is associated with a folder.</span></span>  <br/> |
|[<span data-ttu-id="3f437-229">WebClientReadFormQueryString</span><span class="sxs-lookup"><span data-stu-id="3f437-229">WebClientReadFormQueryString</span></span>](webclientreadformquerystring.md) <br/> |<span data-ttu-id="3f437-230">Представляет URL-адрес для присоединения к конечной точке Microsoft Office Outlook Web App для чтения элемента в Outlook Web App.</span><span class="sxs-lookup"><span data-stu-id="3f437-230">Represents a URL to concatenate to the Microsoft Office Outlook Web App endpoint to read an item in Outlook Web App.</span></span>  <br/> |
|[<span data-ttu-id="3f437-231">WebClientEditFormQueryString</span><span class="sxs-lookup"><span data-stu-id="3f437-231">WebClientEditFormQueryString</span></span>](webclienteditformquerystring.md) <br/> |<span data-ttu-id="3f437-232">Представляет URL-адрес для объединения в конечную точку Outlook Web App для редактирования элемента в Outlook Web App.</span><span class="sxs-lookup"><span data-stu-id="3f437-232">Represents a URL to concatenate to the Outlook Web App endpoint to edit an item in Outlook Web App.</span></span>  <br/> |
|[<span data-ttu-id="3f437-233">ConversationId</span><span class="sxs-lookup"><span data-stu-id="3f437-233">ConversationId</span></span>](conversationid.md) <br/> |<span data-ttu-id="3f437-234">Содержит идентификатор элемента или беседы.</span><span class="sxs-lookup"><span data-stu-id="3f437-234">Contains the identifier of an item or conversation.</span></span>  <br/> |
|[<span data-ttu-id="3f437-235">UniqueBody</span><span class="sxs-lookup"><span data-stu-id="3f437-235">UniqueBody</span></span>](uniquebody.md) <br/> |<span data-ttu-id="3f437-236">Представляет фрагмент HTML или обычный текст, который представляет уникальное body эту беседу.</span><span class="sxs-lookup"><span data-stu-id="3f437-236">Represents an HTML fragment or plain text which represents the unique body of this conversation.</span></span>  <br/> |
|[<span data-ttu-id="3f437-237">ИД ПОЛЬЗОВАТЕЛЯ</span><span class="sxs-lookup"><span data-stu-id="3f437-237">UID</span></span>](uid.md) <br/> |<span data-ttu-id="3f437-238">Идентифицирует элемент календаря.</span><span class="sxs-lookup"><span data-stu-id="3f437-238">Identifies a calendar item.</span></span>  <br/> |
|[<span data-ttu-id="3f437-239">RecurrenceId</span><span class="sxs-lookup"><span data-stu-id="3f437-239">RecurrenceId</span></span>](recurrenceid.md) <br/> |<span data-ttu-id="3f437-240">Используется для идентификации определенный экземпляр повторяющегося элемента календаря.</span><span class="sxs-lookup"><span data-stu-id="3f437-240">Used to identify a specific instance of a recurring calendar item.</span></span>  <br/> |
|[<span data-ttu-id="3f437-241">DateTimeStamp</span><span class="sxs-lookup"><span data-stu-id="3f437-241">DateTimeStamp</span></span>](datetimestamp.md) <br/> |<span data-ttu-id="3f437-242">Указывает дату и время создания экземпляра объекта iCalendar.</span><span class="sxs-lookup"><span data-stu-id="3f437-242">Indicates the date and time that an instance of an iCalendar object was created.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="3f437-243">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="3f437-243">Parent elements</span></span>

|<span data-ttu-id="3f437-244">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="3f437-244">**Element**</span></span>|<span data-ttu-id="3f437-245">**Описание**</span><span class="sxs-lookup"><span data-stu-id="3f437-245">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3f437-246">AdjacentMeetings</span><span class="sxs-lookup"><span data-stu-id="3f437-246">AdjacentMeetings</span></span>](adjacentmeetings.md) <br/> |<span data-ttu-id="3f437-247">Описание всех элементов календаря, расположенных на время собрания.</span><span class="sxs-lookup"><span data-stu-id="3f437-247">Describes all calendar items that are adjacent to a meeting time.</span></span>  <br/> |
|[<span data-ttu-id="3f437-248">AppendToItemField</span><span class="sxs-lookup"><span data-stu-id="3f437-248">AppendToItemField</span></span>](appendtoitemfield.md) <br/> |<span data-ttu-id="3f437-249">Указывает данные для добавления к отдельное свойство элемента во время [операции UpdateItem](updateitem-operation.md).</span><span class="sxs-lookup"><span data-stu-id="3f437-249">Identifies data to append to a single property of an item during an [UpdateItem operation](updateitem-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="3f437-250">ConflictingMeetings</span><span class="sxs-lookup"><span data-stu-id="3f437-250">ConflictingMeetings</span></span>](conflictingmeetings.md) <br/> |<span data-ttu-id="3f437-251">Определяет все элементы, конфликтующие с время собрания.</span><span class="sxs-lookup"><span data-stu-id="3f437-251">Identifies all items that conflict with a meeting time.</span></span>  <br/> |
|[<span data-ttu-id="3f437-252">Создание (ItemSync)</span><span class="sxs-lookup"><span data-stu-id="3f437-252">Create (ItemSync)</span></span>](create-itemsync.md) <br/> |<span data-ttu-id="3f437-253">Определяет один элемент для создания в локальном хранилище клиента.</span><span class="sxs-lookup"><span data-stu-id="3f437-253">Identifies a single item to create in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="3f437-254">Обновление (ItemSync)</span><span class="sxs-lookup"><span data-stu-id="3f437-254">Update (ItemSync)</span></span>](update-itemsync.md) <br/> |<span data-ttu-id="3f437-255">Определяет один элемент для обновления в локальном хранилище клиента.</span><span class="sxs-lookup"><span data-stu-id="3f437-255">Identifies a single item to update in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="3f437-256">Элементы</span><span class="sxs-lookup"><span data-stu-id="3f437-256">Items</span></span>](items.md) <br/> |<span data-ttu-id="3f437-257">Содержит массив элементов.</span><span class="sxs-lookup"><span data-stu-id="3f437-257">Contains an array of items.</span></span>  <br/> |
|[<span data-ttu-id="3f437-258">Элементы (NonEmptyArrayOfAllItemsType)</span><span class="sxs-lookup"><span data-stu-id="3f437-258">Items (NonEmptyArrayOfAllItemsType)</span></span>](items-nonemptyarrayofallitemstype.md) <br/> |<span data-ttu-id="3f437-259">Содержит массив элементов для создания в папку, указанную в элементе [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) .</span><span class="sxs-lookup"><span data-stu-id="3f437-259">Contains an array of items to create in the folder identified by the [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) element.</span></span>  <br/> |
|[<span data-ttu-id="3f437-260">SetItemField</span><span class="sxs-lookup"><span data-stu-id="3f437-260">SetItemField</span></span>](setitemfield.md) <br/> |<span data-ttu-id="3f437-261">Представляет отдельное свойство элемента в [UpdateItem операции](updateitem-operation.md)обновления.</span><span class="sxs-lookup"><span data-stu-id="3f437-261">Represents an update to a single property of an item in an [UpdateItem operation](updateitem-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="3f437-262">ItemAttachment</span><span class="sxs-lookup"><span data-stu-id="3f437-262">ItemAttachment</span></span>](itemattachment.md) <br/> |<span data-ttu-id="3f437-263">Представляет собой элемент Exchange, подключенный к другой элемент Exchange.</span><span class="sxs-lookup"><span data-stu-id="3f437-263">Represents an Exchange item that is attached to another Exchange item.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="3f437-264">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="3f437-264">Text value</span></span>

<span data-ttu-id="3f437-265">Нет.</span><span class="sxs-lookup"><span data-stu-id="3f437-265">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="3f437-266">Замечания</span><span class="sxs-lookup"><span data-stu-id="3f437-266">Remarks</span></span>

<span data-ttu-id="3f437-267">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="3f437-267">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3f437-268">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="3f437-268">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3f437-269">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="3f437-269">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="3f437-270">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="3f437-270">Schema Name</span></span>  <br/> |<span data-ttu-id="3f437-271">Схема Types</span><span class="sxs-lookup"><span data-stu-id="3f437-271">Types schema</span></span>  <br/> |
|<span data-ttu-id="3f437-272">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="3f437-272">Validation File</span></span>  <br/> |<span data-ttu-id="3f437-273">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="3f437-273">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="3f437-274">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="3f437-274">Can be Empty</span></span>  <br/> |<span data-ttu-id="3f437-275">False</span><span class="sxs-lookup"><span data-stu-id="3f437-275">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3f437-276">См. также</span><span class="sxs-lookup"><span data-stu-id="3f437-276">See also</span></span>



- [<span data-ttu-id="3f437-277">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="3f437-277">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

