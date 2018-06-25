---
title: MeetingResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MeetingResponse
api_type:
- schema
ms.assetid: 9f798e79-dafd-4d4d-9967-95fd8e5c0502
description: Элемент MeetingResponse представляет ответ на приглашение в хранилище Exchange.
ms.openlocfilehash: c5f9f3ac2fcd12e9c95f663311c33cdd36783251
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834446"
---
# <a name="meetingresponse"></a><span data-ttu-id="127fa-103">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="127fa-103">MeetingResponse</span></span>

<span data-ttu-id="127fa-104">Элемент **MeetingResponse** представляет ответ на приглашение в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="127fa-104">The **MeetingResponse** element represents a meeting response in the Exchange store.</span></span> 
  
```xml
<MeetingResponse>
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
   <ReceivedBy/>
   <ReceivedRepresenting/>
</MeetingResponse>
```

 <span data-ttu-id="127fa-105">**MeetingResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="127fa-105">**MeetingResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="127fa-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="127fa-106">Attributes and elements</span></span>

<span data-ttu-id="127fa-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="127fa-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="127fa-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="127fa-108">Attributes</span></span>

<span data-ttu-id="127fa-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="127fa-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="127fa-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="127fa-110">Child elements</span></span>

|<span data-ttu-id="127fa-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="127fa-111">**Element**</span></span>|<span data-ttu-id="127fa-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="127fa-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="127fa-113">MimeContent</span><span class="sxs-lookup"><span data-stu-id="127fa-113">MimeContent</span></span>](mimecontent.md) <br/> |<span data-ttu-id="127fa-114">Содержит собственный поток MIME, представленного в формате base64Binary объекта.</span><span class="sxs-lookup"><span data-stu-id="127fa-114">Contains the native MIME stream of an object that is represented in base64Binary format.</span></span>  <br/> |
|[<span data-ttu-id="127fa-115">Идентификатор элемента</span><span class="sxs-lookup"><span data-stu-id="127fa-115">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="127fa-116">Содержит уникальный идентификатор и меняет ключ элемента в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="127fa-116">Contains the unique identifier and change key of an item in the Exchange store.</span></span> <span data-ttu-id="127fa-117">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="127fa-117">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="127fa-118">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="127fa-118">ParentFolderId</span></span>](parentfolderid.md) <br/> |<span data-ttu-id="127fa-119">Представляет идентификатор родительской папки, содержащей элемент или папку.</span><span class="sxs-lookup"><span data-stu-id="127fa-119">Represents the identifier of the parent folder that contains the item or folder.</span></span> <span data-ttu-id="127fa-120">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="127fa-120">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="127fa-121">ItemClass</span><span class="sxs-lookup"><span data-stu-id="127fa-121">ItemClass</span></span>](itemclass.md) <br/> |<span data-ttu-id="127fa-122">Представляет класс сообщения элемента.</span><span class="sxs-lookup"><span data-stu-id="127fa-122">Represents the message class of an item.</span></span>  <br/> |
|[<span data-ttu-id="127fa-123">Subject</span><span class="sxs-lookup"><span data-stu-id="127fa-123">Subject</span></span>](subject.md) <br/> |<span data-ttu-id="127fa-124">Представляет тему для элементов хранилища Exchange и объекты ответа.</span><span class="sxs-lookup"><span data-stu-id="127fa-124">Represents the subject for Exchange store items and response objects.</span></span> <span data-ttu-id="127fa-125">Тема ограничена 255 символов.</span><span class="sxs-lookup"><span data-stu-id="127fa-125">The subject is limited to 255 characters.</span></span>  <br/> |
|[<span data-ttu-id="127fa-126">Уровень конфиденциальности сообщения</span><span class="sxs-lookup"><span data-stu-id="127fa-126">Sensitivity</span></span>](sensitivity.md) <br/> |<span data-ttu-id="127fa-127">Указывает уровень конфиденциальности для элемента.</span><span class="sxs-lookup"><span data-stu-id="127fa-127">Indicates the sensitivity level of an item.</span></span>  <br/> |
|[<span data-ttu-id="127fa-128">Body</span><span class="sxs-lookup"><span data-stu-id="127fa-128">Body</span></span>](body.md) <br/> |<span data-ttu-id="127fa-129">Представляет фактическое содержимое основного текста сообщения.</span><span class="sxs-lookup"><span data-stu-id="127fa-129">Represents the actual body content of a message.</span></span>  <br/> |
|[<span data-ttu-id="127fa-130">Вложения</span><span class="sxs-lookup"><span data-stu-id="127fa-130">Attachments</span></span>](attachments-ex15websvcsotherref.md) <br/> |<span data-ttu-id="127fa-131">Содержит элементы или файлы, подключенные к элементу в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="127fa-131">Contains the items or files that are attached to an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="127fa-132">DateTimeReceived</span><span class="sxs-lookup"><span data-stu-id="127fa-132">DateTimeReceived</span></span>](datetimereceived.md) <br/> |<span data-ttu-id="127fa-133">Представляет дату и время получения элемента в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="127fa-133">Represents the data and time that an item in a mailbox was received.</span></span>  <br/> |
|[<span data-ttu-id="127fa-134">Размер</span><span class="sxs-lookup"><span data-stu-id="127fa-134">Size</span></span>](size.md) <br/> |<span data-ttu-id="127fa-135">Представляет размер в байтах элемента.</span><span class="sxs-lookup"><span data-stu-id="127fa-135">Represents the size in bytes of an item.</span></span> <span data-ttu-id="127fa-136">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="127fa-136">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="127fa-137">Категории</span><span class="sxs-lookup"><span data-stu-id="127fa-137">Categories</span></span>](categories-ex15websvcsotherref.md) <br/> |<span data-ttu-id="127fa-138">Представляет набор строк, чтобы указать, к какой категории относится элемент в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="127fa-138">Represents a collection of strings that identify to which categories an item in the mailbox belongs.</span></span>  <br/> |
|[<span data-ttu-id="127fa-139">Важность</span><span class="sxs-lookup"><span data-stu-id="127fa-139">Importance</span></span>](importance.md) <br/> |<span data-ttu-id="127fa-140">Описывает важность элемента.</span><span class="sxs-lookup"><span data-stu-id="127fa-140">Describes the importance of an item.</span></span>  <br/> |
|[<span data-ttu-id="127fa-141">InReplyTo</span><span class="sxs-lookup"><span data-stu-id="127fa-141">InReplyTo</span></span>](inreplyto.md) <br/> |<span data-ttu-id="127fa-142">Представляет идентификатор элемента, к которому этот элемент является ее в ответ.</span><span class="sxs-lookup"><span data-stu-id="127fa-142">Represents the identifier of the item to which this item is a reply.</span></span>  <br/> |
|[<span data-ttu-id="127fa-143">IsSubmitted</span><span class="sxs-lookup"><span data-stu-id="127fa-143">IsSubmitted</span></span>](issubmitted.md) <br/> |<span data-ttu-id="127fa-144">Указывает, является ли элемент был отправлен исходящие папке по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="127fa-144">Indicates whether an item has been submitted to the Outbox default folder.</span></span>  <br/> |
|[<span data-ttu-id="127fa-145">IsDraft</span><span class="sxs-lookup"><span data-stu-id="127fa-145">IsDraft</span></span>](isdraft.md) <br/> |<span data-ttu-id="127fa-146">Представляет ли элемент еще не были отправлены.</span><span class="sxs-lookup"><span data-stu-id="127fa-146">Represents whether an item has not yet been sent.</span></span>  <br/> |
|[<span data-ttu-id="127fa-147">IsFromMe</span><span class="sxs-lookup"><span data-stu-id="127fa-147">IsFromMe</span></span>](isfromme.md) <br/> |<span data-ttu-id="127fa-148">Указывает, отправил ли пользователь элемента для его сами себя.</span><span class="sxs-lookup"><span data-stu-id="127fa-148">Indicates whether a user sent an item to him or herself.</span></span>  <br/> |
|[<span data-ttu-id="127fa-149">IsResend</span><span class="sxs-lookup"><span data-stu-id="127fa-149">IsResend</span></span>](isresend.md) <br/> |<span data-ttu-id="127fa-150">Указывает, является ли элемент ранее еще был отправлен.</span><span class="sxs-lookup"><span data-stu-id="127fa-150">Indicates whether the item had previously been sent.</span></span>  <br/> |
|[<span data-ttu-id="127fa-151">IsUnmodified</span><span class="sxs-lookup"><span data-stu-id="127fa-151">IsUnmodified</span></span>](isunmodified.md) <br/> |<span data-ttu-id="127fa-152">Указывает, были ли изменены элемента.</span><span class="sxs-lookup"><span data-stu-id="127fa-152">Indicates whether the item has been modified.</span></span>  <br/> |
|[<span data-ttu-id="127fa-153">InternetMessageHeaders</span><span class="sxs-lookup"><span data-stu-id="127fa-153">InternetMessageHeaders</span></span>](internetmessageheaders.md) <br/> |<span data-ttu-id="127fa-154">Представляет коллекцию всех заголовков сообщений Интернета, находящихся внутри элемента в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="127fa-154">Represents the collection of all Internet message headers that are contained within an item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="127fa-155">DateTimeSent</span><span class="sxs-lookup"><span data-stu-id="127fa-155">DateTimeSent</span></span>](datetimesent.md) <br/> |<span data-ttu-id="127fa-156">Представляет дату и время отправки элемента в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="127fa-156">Represents the date and time that an item in a mailbox was sent.</span></span>  <br/> |
|[<span data-ttu-id="127fa-157">DateTimeCreated</span><span class="sxs-lookup"><span data-stu-id="127fa-157">DateTimeCreated</span></span>](datetimecreated.md) <br/> |<span data-ttu-id="127fa-158">Представляет дату и время создания данного элемента в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="127fa-158">Represents the date and time that a given item in the mailbox was created.</span></span>  <br/> |
|[<span data-ttu-id="127fa-159">ResponseObjects</span><span class="sxs-lookup"><span data-stu-id="127fa-159">ResponseObjects</span></span>](responseobjects.md) <br/> |<span data-ttu-id="127fa-160">Содержит коллекцию всех объектов ответа, которые связаны с элемента в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="127fa-160">Contains a collection of all the response objects that are associated with an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="127fa-161">ReminderDueBy</span><span class="sxs-lookup"><span data-stu-id="127fa-161">ReminderDueBy</span></span>](reminderdueby.md) <br/> |<span data-ttu-id="127fa-162">Представляет дату и время, когда происходит событие.</span><span class="sxs-lookup"><span data-stu-id="127fa-162">Represents the date and time when the event occurs.</span></span> <span data-ttu-id="127fa-163">Используется в элементе [ReminderMinutesBeforeStart](reminderminutesbeforestart.md) определить, когда отображается оповещение.</span><span class="sxs-lookup"><span data-stu-id="127fa-163">This is used by the [ReminderMinutesBeforeStart](reminderminutesbeforestart.md) element to determine when the reminder is displayed.</span></span>  <br/> |
|[<span data-ttu-id="127fa-164">ReminderIsSet</span><span class="sxs-lookup"><span data-stu-id="127fa-164">ReminderIsSet</span></span>](reminderisset.md) <br/> |<span data-ttu-id="127fa-165">Указывает, установлен ли напоминания для элемента в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="127fa-165">Indicates whether a reminder has been set for an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="127fa-166">ReminderMinutesBeforeStart</span><span class="sxs-lookup"><span data-stu-id="127fa-166">ReminderMinutesBeforeStart</span></span>](reminderminutesbeforestart.md) <br/> |<span data-ttu-id="127fa-167">Представляет число минут и только потом событие, когда отображается напоминание.</span><span class="sxs-lookup"><span data-stu-id="127fa-167">Represents the number of minutes before an event when a reminder is displayed.</span></span>  <br/> |
|[<span data-ttu-id="127fa-168">DisplayCc</span><span class="sxs-lookup"><span data-stu-id="127fa-168">DisplayCc</span></span>](displaycc.md) <br/> |<span data-ttu-id="127fa-169">Строка отображения, который используется для содержимого в поле "Копия".</span><span class="sxs-lookup"><span data-stu-id="127fa-169">Represents the display string that is used for the contents of the Cc box.</span></span> <span data-ttu-id="127fa-170">Это составное строка всех получателей отображаемые имена «копия».</span><span class="sxs-lookup"><span data-stu-id="127fa-170">This is the concatenated string of all Cc recipient display names.</span></span>  <br/> |
|[<span data-ttu-id="127fa-171">DisplayTo</span><span class="sxs-lookup"><span data-stu-id="127fa-171">DisplayTo</span></span>](displayto.md) <br/> |<span data-ttu-id="127fa-172">Строка отображения, который используется для содержимого в поле «Кому».</span><span class="sxs-lookup"><span data-stu-id="127fa-172">Represents the display string that is used for the contents of the To box.</span></span> <span data-ttu-id="127fa-173">Это составное строка всех для получателей отображаемые имена.</span><span class="sxs-lookup"><span data-stu-id="127fa-173">This is the concatenated string of all To recipient display names.</span></span>  <br/> |
|[<span data-ttu-id="127fa-174">HasAttachments</span><span class="sxs-lookup"><span data-stu-id="127fa-174">HasAttachments</span></span>](hasattachments.md) <br/> |<span data-ttu-id="127fa-175">Представляет свойство, которое задано значение **true,** Если у элемента есть по крайней мере один видимым вложения.</span><span class="sxs-lookup"><span data-stu-id="127fa-175">Represents a property that is set to **true** if an item has at least one visible attachment.</span></span> <span data-ttu-id="127fa-176">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="127fa-176">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="127fa-177">ExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="127fa-177">ExtendedProperty</span></span>](extendedproperty.md) <br/> |<span data-ttu-id="127fa-178">Определяет расширенные свойства для папок и элементов.</span><span class="sxs-lookup"><span data-stu-id="127fa-178">Identifies extended properties on folders and items.</span></span>  <br/> |
|[<span data-ttu-id="127fa-179">Язык и региональные параметры</span><span class="sxs-lookup"><span data-stu-id="127fa-179">Culture</span></span>](culture.md) <br/> |<span data-ttu-id="127fa-180">Представляет язык и региональные параметры для заданного элемента в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="127fa-180">Represents the culture for a given item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="127fa-181">Отправитель</span><span class="sxs-lookup"><span data-stu-id="127fa-181">Sender</span></span>](sender.md) <br/> |<span data-ttu-id="127fa-182">Идентифицирует отправителя элемента.</span><span class="sxs-lookup"><span data-stu-id="127fa-182">Identifies the sender of an item.</span></span>  <br/> |
|[<span data-ttu-id="127fa-183">ToRecipients</span><span class="sxs-lookup"><span data-stu-id="127fa-183">ToRecipients</span></span>](torecipients.md) <br/> |<span data-ttu-id="127fa-184">Содержит список получателей сообщения.</span><span class="sxs-lookup"><span data-stu-id="127fa-184">Contains a set of recipients of a message.</span></span>  <br/> |
|[<span data-ttu-id="127fa-185">CcRecipients</span><span class="sxs-lookup"><span data-stu-id="127fa-185">CcRecipients</span></span>](ccrecipients.md) <br/> |<span data-ttu-id="127fa-186">Представляет коллекцию получателей, которые будут получать копии сообщения.</span><span class="sxs-lookup"><span data-stu-id="127fa-186">Represents a collection of recipients that will receive a copy of the message.</span></span>  <br/> |
|[<span data-ttu-id="127fa-187">BccRecipients</span><span class="sxs-lookup"><span data-stu-id="127fa-187">BccRecipients</span></span>](bccrecipients.md) <br/> |<span data-ttu-id="127fa-188">Представляет коллекцию получателей скрытой копии (СК) сообщения электронной почты.</span><span class="sxs-lookup"><span data-stu-id="127fa-188">Represents a collection of recipients to receive a blind carbon copy (Bcc) of an e-mail.</span></span>  <br/> |
|[<span data-ttu-id="127fa-189">IsReadReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="127fa-189">IsReadReceiptRequested</span></span>](isreadreceiptrequested.md) <br/> |<span data-ttu-id="127fa-190">Указывает, будет ли отправителя элемента о прочтении.</span><span class="sxs-lookup"><span data-stu-id="127fa-190">Indicates whether the sender of an item requests a read receipt.</span></span>  <br/> |
|[<span data-ttu-id="127fa-191">IsDeliveryReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="127fa-191">IsDeliveryReceiptRequested</span></span>](isdeliveryreceiptrequested.md) <br/> |<span data-ttu-id="127fa-192">Указывает, требует ли отправитель элемента уведомление о доставке.</span><span class="sxs-lookup"><span data-stu-id="127fa-192">Indicates whether the sender of an item requests a delivery receipt.</span></span>  <br/> |
|[<span data-ttu-id="127fa-193">ConversationIndex</span><span class="sxs-lookup"><span data-stu-id="127fa-193">ConversationIndex</span></span>](conversationindex.md) <br/> |<span data-ttu-id="127fa-194">Содержит двоичные идентификатор, представляющий поток, к которой принадлежит это сообщение.</span><span class="sxs-lookup"><span data-stu-id="127fa-194">Contains a binary ID that represents the thread to which this message belongs.</span></span>  <br/> |
|[<span data-ttu-id="127fa-195">ConversationTopic</span><span class="sxs-lookup"><span data-stu-id="127fa-195">ConversationTopic</span></span>](conversationtopic.md) <br/> |<span data-ttu-id="127fa-196">Представляет идентификатор беседы.</span><span class="sxs-lookup"><span data-stu-id="127fa-196">Represents the conversation identifier.</span></span>  <br/> |
|[<span data-ttu-id="127fa-197">From</span><span class="sxs-lookup"><span data-stu-id="127fa-197">From</span></span>](from.md) <br/> |<span data-ttu-id="127fa-198">Представляет получателя, у которого было отправлено сообщение.</span><span class="sxs-lookup"><span data-stu-id="127fa-198">Represents the addressee from whom the message was sent.</span></span>  <br/> |
|[<span data-ttu-id="127fa-199">InternetMessageId</span><span class="sxs-lookup"><span data-stu-id="127fa-199">InternetMessageId</span></span>](internetmessageid.md) <br/> |<span data-ttu-id="127fa-200">Представляет идентификатор сообщения Интернета элемента.</span><span class="sxs-lookup"><span data-stu-id="127fa-200">Represents the Internet message identifier of an item.</span></span>  <br/> |
|[<span data-ttu-id="127fa-201">IsRead</span><span class="sxs-lookup"><span data-stu-id="127fa-201">IsRead</span></span>](isread.md) <br/> |<span data-ttu-id="127fa-202">Указывает, имеет ли чтение сообщения.</span><span class="sxs-lookup"><span data-stu-id="127fa-202">Indicates whether a message has been read.</span></span>  <br/> |
|[<span data-ttu-id="127fa-203">IsResponseRequested</span><span class="sxs-lookup"><span data-stu-id="127fa-203">IsResponseRequested</span></span>](isresponserequested.md) <br/> |<span data-ttu-id="127fa-204">Указывает, запрашивается ли ответ на сообщение электронной почты.</span><span class="sxs-lookup"><span data-stu-id="127fa-204">Indicates whether a response to an e-mail message is requested.</span></span>  <br/> |
|[<span data-ttu-id="127fa-205">Справочные материалы</span><span class="sxs-lookup"><span data-stu-id="127fa-205">References</span></span>](references.md) <br/> |<span data-ttu-id="127fa-206">Представляет заголовок групп, используемый для сопоставления ответов с исходными сообщениями.</span><span class="sxs-lookup"><span data-stu-id="127fa-206">Represents the Usenet header that is used to correlate replies with their original messages.</span></span>  <br/> |
|[<span data-ttu-id="127fa-207">ReplyTo</span><span class="sxs-lookup"><span data-stu-id="127fa-207">ReplyTo</span></span>](replyto.md) <br/> |<span data-ttu-id="127fa-208">Определяет набор адресов, к которым будут отправляться ответы.</span><span class="sxs-lookup"><span data-stu-id="127fa-208">Identifies a set of addresses to which replies should be sent.</span></span>  <br/> |
|[<span data-ttu-id="127fa-209">AssociatedCalendarItemId</span><span class="sxs-lookup"><span data-stu-id="127fa-209">AssociatedCalendarItemId</span></span>](associatedcalendaritemid.md) <br/> |<span data-ttu-id="127fa-210">Представляет элемент календаря, связанного с [MeetingMessage](meetingmessage.md).</span><span class="sxs-lookup"><span data-stu-id="127fa-210">Represents the calendar item that is associated with a [MeetingMessage](meetingmessage.md).</span></span>  <br/> |
|[<span data-ttu-id="127fa-211">IsDelegated</span><span class="sxs-lookup"><span data-stu-id="127fa-211">IsDelegated</span></span>](isdelegated.md) <br/> |<span data-ttu-id="127fa-212">Указывает, обработано ли собрания с помощью учетной записи с доступом к делегата.</span><span class="sxs-lookup"><span data-stu-id="127fa-212">Indicates whether a meeting was handled by an account with delegate access.</span></span>  <br/> |
|[<span data-ttu-id="127fa-213">IsOutOfDate</span><span class="sxs-lookup"><span data-stu-id="127fa-213">IsOutOfDate</span></span>](isoutofdate.md) <br/> |<span data-ttu-id="127fa-214">Указывает, является ли устаревших сообщений собрания.</span><span class="sxs-lookup"><span data-stu-id="127fa-214">Indicates whether a meeting message is out-of-date.</span></span>  <br/> |
|[<span data-ttu-id="127fa-215">HasBeenProcessed</span><span class="sxs-lookup"><span data-stu-id="127fa-215">HasBeenProcessed</span></span>](hasbeenprocessed.md) <br/> |<span data-ttu-id="127fa-216">Указывает ли сообщение собрания элемент обработки.</span><span class="sxs-lookup"><span data-stu-id="127fa-216">Indicates whether a meeting message item has been processed.</span></span>  <br/> |
|[<span data-ttu-id="127fa-217">ResponseType</span><span class="sxs-lookup"><span data-stu-id="127fa-217">ResponseType</span></span>](responsetype.md) <br/> |<span data-ttu-id="127fa-218">Представляет тип получателя ответа, полученные на собрание.</span><span class="sxs-lookup"><span data-stu-id="127fa-218">Represents the type of recipient response that is received for a meeting.</span></span>  <br/> |
|[<span data-ttu-id="127fa-219">EffectiveRights</span><span class="sxs-lookup"><span data-stu-id="127fa-219">EffectiveRights</span></span>](effectiverights.md) <br/> |<span data-ttu-id="127fa-220">Содержит права клиента на основании параметров разрешений для элемента или папки.</span><span class="sxs-lookup"><span data-stu-id="127fa-220">Contains the client's rights based on the permission settings for the item or folder.</span></span> <span data-ttu-id="127fa-221">Этот элемент доступен только для чтения.</span><span class="sxs-lookup"><span data-stu-id="127fa-221">This element is read-only.</span></span> <span data-ttu-id="127fa-222">Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="127fa-222">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span>  <br/> |
|[<span data-ttu-id="127fa-223">Получил</span><span class="sxs-lookup"><span data-stu-id="127fa-223">ReceivedBy</span></span>](receivedby.md) <br/> |<span data-ttu-id="127fa-224">Определяет делегат в сценарии доступа делегата.</span><span class="sxs-lookup"><span data-stu-id="127fa-224">Identifies the delegate in a delegate access scenario.</span></span> <span data-ttu-id="127fa-225">Этот элемент появился в Exchange 2007 с пакетом обновления 1.</span><span class="sxs-lookup"><span data-stu-id="127fa-225">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="127fa-226">ReceivedRepresenting</span><span class="sxs-lookup"><span data-stu-id="127fa-226">ReceivedRepresenting</span></span>](receivedrepresenting.md) <br/> |<span data-ttu-id="127fa-227">Идентифицирует участника в сценарии доступа делегата.</span><span class="sxs-lookup"><span data-stu-id="127fa-227">Identifies the principal in a delegate access scenario.</span></span> <span data-ttu-id="127fa-228">Этот элемент появился в Exchange 2007 с пакетом обновления 1.</span><span class="sxs-lookup"><span data-stu-id="127fa-228">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="127fa-229">ИД ПОЛЬЗОВАТЕЛЯ</span><span class="sxs-lookup"><span data-stu-id="127fa-229">UID</span></span>](uid.md) <br/> |<span data-ttu-id="127fa-230">Идентифицирует элемент календаря.</span><span class="sxs-lookup"><span data-stu-id="127fa-230">Identifies a calendar item.</span></span>  <br/> |
|[<span data-ttu-id="127fa-231">RecurrenceId</span><span class="sxs-lookup"><span data-stu-id="127fa-231">RecurrenceId</span></span>](recurrenceid.md) <br/> |<span data-ttu-id="127fa-232">Используется для идентификации определенный экземпляр повторяющегося элемента календаря.</span><span class="sxs-lookup"><span data-stu-id="127fa-232">Used to identify a specific instance of a recurring calendar item.</span></span>  <br/> |
|[<span data-ttu-id="127fa-233">DateTimeStamp</span><span class="sxs-lookup"><span data-stu-id="127fa-233">DateTimeStamp</span></span>](datetimestamp.md) <br/> |<span data-ttu-id="127fa-234">Указывает дату и время создания экземпляра объекта iCalendar.</span><span class="sxs-lookup"><span data-stu-id="127fa-234">Indicates the date and time that an instance of an iCalendar object was created.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="127fa-235">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="127fa-235">Parent elements</span></span>

|<span data-ttu-id="127fa-236">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="127fa-236">**Element**</span></span>|<span data-ttu-id="127fa-237">**Описание**</span><span class="sxs-lookup"><span data-stu-id="127fa-237">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="127fa-238">AdjacentMeetings</span><span class="sxs-lookup"><span data-stu-id="127fa-238">AdjacentMeetings</span></span>](adjacentmeetings.md) <br/> |<span data-ttu-id="127fa-239">Определяет все элементы календаря, расположенных на время собрания.</span><span class="sxs-lookup"><span data-stu-id="127fa-239">Identifies all calendar items that are adjacent to a meeting time.</span></span>  <br/> |
|[<span data-ttu-id="127fa-240">AppendToItemField</span><span class="sxs-lookup"><span data-stu-id="127fa-240">AppendToItemField</span></span>](appendtoitemfield.md) <br/> |<span data-ttu-id="127fa-241">Указывает данные для добавления к отдельное свойство элемента во время [операции UpdateItem](updateitem-operation.md).</span><span class="sxs-lookup"><span data-stu-id="127fa-241">Identifies data to append to a single property of an item during an [UpdateItem operation](updateitem-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="127fa-242">ConflictingMeetings</span><span class="sxs-lookup"><span data-stu-id="127fa-242">ConflictingMeetings</span></span>](conflictingmeetings.md) <br/> |<span data-ttu-id="127fa-243">Определяет все элементы, конфликтующие с время собрания.</span><span class="sxs-lookup"><span data-stu-id="127fa-243">Identifies all items that conflict with a meeting time.</span></span>  <br/> |
|[<span data-ttu-id="127fa-244">Создание (ItemSync)</span><span class="sxs-lookup"><span data-stu-id="127fa-244">Create (ItemSync)</span></span>](create-itemsync.md) <br/> |<span data-ttu-id="127fa-245">Определяет один элемент для создания в локальном хранилище клиента.</span><span class="sxs-lookup"><span data-stu-id="127fa-245">Identifies a single item to create in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="127fa-246">Элементы</span><span class="sxs-lookup"><span data-stu-id="127fa-246">Items</span></span>](items.md) <br/> |<span data-ttu-id="127fa-247">Содержит массив элементов.</span><span class="sxs-lookup"><span data-stu-id="127fa-247">Contains an array of items.</span></span>  <br/> |
|[<span data-ttu-id="127fa-248">Элементы (NonEmptyArrayOfAllItemsType)</span><span class="sxs-lookup"><span data-stu-id="127fa-248">Items (NonEmptyArrayOfAllItemsType)</span></span>](items-nonemptyarrayofallitemstype.md) <br/> |<span data-ttu-id="127fa-249">Содержит массив элементов для создания.</span><span class="sxs-lookup"><span data-stu-id="127fa-249">Contains an array of items to create.</span></span>  <br/> |
|[<span data-ttu-id="127fa-250">ItemAttachment</span><span class="sxs-lookup"><span data-stu-id="127fa-250">ItemAttachment</span></span>](itemattachment.md) <br/> |<span data-ttu-id="127fa-251">Представляет собой элемент Exchange, подключенный к другой элемент Exchange.</span><span class="sxs-lookup"><span data-stu-id="127fa-251">Represents an Exchange item that is attached to another Exchange item.</span></span>  <br/> |
|[<span data-ttu-id="127fa-252">SetItemField</span><span class="sxs-lookup"><span data-stu-id="127fa-252">SetItemField</span></span>](setitemfield.md) <br/> |<span data-ttu-id="127fa-253">Представляет отдельное свойство элемента в [UpdateItem операции](updateitem-operation.md)обновления.</span><span class="sxs-lookup"><span data-stu-id="127fa-253">Represents an update to a single property of an item in an [UpdateItem operation](updateitem-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="127fa-254">Обновление (ItemSync)</span><span class="sxs-lookup"><span data-stu-id="127fa-254">Update (ItemSync)</span></span>](update-itemsync.md) <br/> |<span data-ttu-id="127fa-255">Определяет один элемент для обновления в локальном хранилище клиента.</span><span class="sxs-lookup"><span data-stu-id="127fa-255">Identifies a single item to update in the local client store.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="127fa-256">Замечания</span><span class="sxs-lookup"><span data-stu-id="127fa-256">Remarks</span></span>

<span data-ttu-id="127fa-257">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="127fa-257">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="127fa-258">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="127fa-258">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="127fa-259">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="127fa-259">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="127fa-260">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="127fa-260">Schema Name</span></span>  <br/> |<span data-ttu-id="127fa-261">Схема Types</span><span class="sxs-lookup"><span data-stu-id="127fa-261">Types schema</span></span>  <br/> |
|<span data-ttu-id="127fa-262">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="127fa-262">Validation File</span></span>  <br/> |<span data-ttu-id="127fa-263">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="127fa-263">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="127fa-264">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="127fa-264">Can be Empty</span></span>  <br/> |<span data-ttu-id="127fa-265">False</span><span class="sxs-lookup"><span data-stu-id="127fa-265">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="127fa-266">См. также</span><span class="sxs-lookup"><span data-stu-id="127fa-266">See also</span></span>



- [<span data-ttu-id="127fa-267">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="127fa-267">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

