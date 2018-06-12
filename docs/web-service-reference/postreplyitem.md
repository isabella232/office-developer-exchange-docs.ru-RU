---
title: PostReplyItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- PostReplyItem
api_type:
- schema
ms.assetid: e5d93d63-0a3b-470f-9a94-2d57284c6745
description: Элемент PostReplyItem содержит ответ элемента записи. Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).
ms.openlocfilehash: 70a0d6a7c670d0f16a55e66e7ef329331a04a5f8
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19834868"
---
# <a name="postreplyitem"></a><span data-ttu-id="8e506-104">PostReplyItem</span><span class="sxs-lookup"><span data-stu-id="8e506-104">PostReplyItem</span></span>

<span data-ttu-id="8e506-105">Элемент **PostReplyItem** содержит ответ элемента записи.</span><span class="sxs-lookup"><span data-stu-id="8e506-105">The **PostReplyItem** element contains a reply to a post item.</span></span> <span data-ttu-id="8e506-106">Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="8e506-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<PostReplyItem>
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
      <NewBodyContent/>
</PostReplyItem>
```

 <span data-ttu-id="8e506-107">**PostReplyItemType**</span><span class="sxs-lookup"><span data-stu-id="8e506-107">**PostReplyItemType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="8e506-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="8e506-108">Attributes and elements</span></span>

<span data-ttu-id="8e506-109">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="8e506-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8e506-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="8e506-110">Attributes</span></span>

<span data-ttu-id="8e506-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="8e506-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8e506-112">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="8e506-112">Child elements</span></span>

|<span data-ttu-id="8e506-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="8e506-113">**Element**</span></span>|<span data-ttu-id="8e506-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="8e506-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8e506-115">MimeContent</span><span class="sxs-lookup"><span data-stu-id="8e506-115">MimeContent</span></span>](mimecontent.md) <br/> |<span data-ttu-id="8e506-116">Содержит собственный поток Multipurpose Internet Mail Extensions (MIME), представленного в формате base64Binary объекта.</span><span class="sxs-lookup"><span data-stu-id="8e506-116">Contains the native Multipurpose Internet Mail Extensions (MIME) stream of an object that is represented in base64Binary format.</span></span>  <br/> |
|[<span data-ttu-id="8e506-117">Идентификатор элемента</span><span class="sxs-lookup"><span data-stu-id="8e506-117">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="8e506-118">Содержит уникальный идентификатор и меняет ключ элемента в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="8e506-118">Contains the unique identifier and change key of an item in the Exchange store.</span></span> <span data-ttu-id="8e506-119">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8e506-119">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="8e506-120">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="8e506-120">ParentFolderId</span></span>](parentfolderid.md) <br/> |<span data-ttu-id="8e506-121">Представляет идентификатор родительской папки, содержащей элемент или папку.</span><span class="sxs-lookup"><span data-stu-id="8e506-121">Represents the identifier of the parent folder that contains the item or folder.</span></span> <span data-ttu-id="8e506-122">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8e506-122">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="8e506-123">ItemClass</span><span class="sxs-lookup"><span data-stu-id="8e506-123">ItemClass</span></span>](itemclass.md) <br/> |<span data-ttu-id="8e506-124">Представляет класс сообщения элемента.</span><span class="sxs-lookup"><span data-stu-id="8e506-124">Represents the message class of an item.</span></span>  <br/> |
|[<span data-ttu-id="8e506-125">Subject</span><span class="sxs-lookup"><span data-stu-id="8e506-125">Subject</span></span>](subject.md) <br/> |<span data-ttu-id="8e506-126">Представляет тему для элементов хранилища Exchange и объекты ответа.</span><span class="sxs-lookup"><span data-stu-id="8e506-126">Represents the subject for Exchange store items and response objects.</span></span> <span data-ttu-id="8e506-127">Тема ограничена 255 символов.</span><span class="sxs-lookup"><span data-stu-id="8e506-127">The subject is limited to 255 characters.</span></span>  <br/> |
|[<span data-ttu-id="8e506-128">Уровень конфиденциальности сообщения</span><span class="sxs-lookup"><span data-stu-id="8e506-128">Sensitivity</span></span>](sensitivity.md) <br/> |<span data-ttu-id="8e506-129">Указывает уровень конфиденциальности для элемента.</span><span class="sxs-lookup"><span data-stu-id="8e506-129">Indicates the sensitivity level of an item.</span></span>  <br/> |
|[<span data-ttu-id="8e506-130">Body</span><span class="sxs-lookup"><span data-stu-id="8e506-130">Body</span></span>](body.md) <br/> |<span data-ttu-id="8e506-131">Представляет фактическое содержимое основного текста сообщения.</span><span class="sxs-lookup"><span data-stu-id="8e506-131">Represents the actual body content of a message.</span></span>  <br/> |
|[<span data-ttu-id="8e506-132">Вложения</span><span class="sxs-lookup"><span data-stu-id="8e506-132">Attachments</span></span>](attachments-ex15websvcsotherref.md) <br/> |<span data-ttu-id="8e506-133">Содержит элементы или файлы, подключенные к элементу в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="8e506-133">Contains the items or files that are attached to an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="8e506-134">DateTimeReceived</span><span class="sxs-lookup"><span data-stu-id="8e506-134">DateTimeReceived</span></span>](datetimereceived.md) <br/> |<span data-ttu-id="8e506-135">Представляет дату и время получения элемента в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="8e506-135">Represents the date and time that an item in a mailbox was received.</span></span>  <br/> |
|[<span data-ttu-id="8e506-136">Размер</span><span class="sxs-lookup"><span data-stu-id="8e506-136">Size</span></span>](size.md) <br/> |<span data-ttu-id="8e506-137">Представляет размер в байтах элемента.</span><span class="sxs-lookup"><span data-stu-id="8e506-137">Represents the size in bytes of an item.</span></span> <span data-ttu-id="8e506-138">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8e506-138">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="8e506-139">Категории</span><span class="sxs-lookup"><span data-stu-id="8e506-139">Categories</span></span>](categories-ex15websvcsotherref.md) <br/> |<span data-ttu-id="8e506-140">Представляет набор строк, которые определяют категории, к которым принадлежит элемент в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="8e506-140">Represents a collection of strings that identify categories to which an item in the mailbox belongs.</span></span>  <br/> |
|[<span data-ttu-id="8e506-141">Важность</span><span class="sxs-lookup"><span data-stu-id="8e506-141">Importance</span></span>](importance.md) <br/> |<span data-ttu-id="8e506-142">Описывает важность элемента.</span><span class="sxs-lookup"><span data-stu-id="8e506-142">Describes the importance of an item.</span></span>  <br/> |
|[<span data-ttu-id="8e506-143">InReplyTo</span><span class="sxs-lookup"><span data-stu-id="8e506-143">InReplyTo</span></span>](inreplyto.md) <br/> |<span data-ttu-id="8e506-144">Представляет идентификатор элемента, к которому этот элемент является ее в ответ.</span><span class="sxs-lookup"><span data-stu-id="8e506-144">Represents the identifier of the item to which this item is a reply.</span></span>  <br/> |
|[<span data-ttu-id="8e506-145">IsSubmitted</span><span class="sxs-lookup"><span data-stu-id="8e506-145">IsSubmitted</span></span>](issubmitted.md) <br/> |<span data-ttu-id="8e506-146">Указывает, является ли элемент был отправлен исходящие папке по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="8e506-146">Indicates whether an item has been submitted to the Outbox default folder.</span></span>  <br/> |
|[<span data-ttu-id="8e506-147">IsDraft</span><span class="sxs-lookup"><span data-stu-id="8e506-147">IsDraft</span></span>](isdraft.md) <br/> |<span data-ttu-id="8e506-148">Представляет ли элемент еще не были отправлены.</span><span class="sxs-lookup"><span data-stu-id="8e506-148">Represents whether an item has not yet been sent.</span></span>  <br/> |
|[<span data-ttu-id="8e506-149">IsFromMe</span><span class="sxs-lookup"><span data-stu-id="8e506-149">IsFromMe</span></span>](isfromme.md) <br/> |<span data-ttu-id="8e506-150">Указывает, отправил ли пользователь элемента для его сами себя.</span><span class="sxs-lookup"><span data-stu-id="8e506-150">Indicates whether a user sent an item to him or herself.</span></span>  <br/> |
|[<span data-ttu-id="8e506-151">IsResend</span><span class="sxs-lookup"><span data-stu-id="8e506-151">IsResend</span></span>](isresend.md) <br/> |<span data-ttu-id="8e506-152">Указывает, является ли элемент ранее еще был отправлен.</span><span class="sxs-lookup"><span data-stu-id="8e506-152">Indicates whether the item had previously been sent.</span></span>  <br/> |
|[<span data-ttu-id="8e506-153">IsUnmodified</span><span class="sxs-lookup"><span data-stu-id="8e506-153">IsUnmodified</span></span>](isunmodified.md) <br/> |<span data-ttu-id="8e506-154">Указывает, были ли изменены элемента.</span><span class="sxs-lookup"><span data-stu-id="8e506-154">Indicates whether the item has been modified.</span></span>  <br/> |
|[<span data-ttu-id="8e506-155">InternetMessageHeaders</span><span class="sxs-lookup"><span data-stu-id="8e506-155">InternetMessageHeaders</span></span>](internetmessageheaders.md) <br/> |<span data-ttu-id="8e506-156">Представляет коллекцию всех заголовков сообщений Интернета, содержащихся в элемента в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="8e506-156">Represents the collection of all Internet message headers that are contained in an item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="8e506-157">DateTimeSent</span><span class="sxs-lookup"><span data-stu-id="8e506-157">DateTimeSent</span></span>](datetimesent.md) <br/> |<span data-ttu-id="8e506-158">Представляет дату и время отправки элемента в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="8e506-158">Represents the date and time that an item in a mailbox was sent.</span></span>  <br/> |
|[<span data-ttu-id="8e506-159">DateTimeCreated</span><span class="sxs-lookup"><span data-stu-id="8e506-159">DateTimeCreated</span></span>](datetimecreated.md) <br/> |<span data-ttu-id="8e506-160">Представляет дату и время создания данного элемента в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="8e506-160">Represents the date and time that a given item in the mailbox was created.</span></span>  <br/> |
|[<span data-ttu-id="8e506-161">ResponseObjects</span><span class="sxs-lookup"><span data-stu-id="8e506-161">ResponseObjects</span></span>](responseobjects.md) <br/> |<span data-ttu-id="8e506-162">Содержит коллекцию всех объектов ответа, которые связаны с элемента в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="8e506-162">Contains a collection of all the response objects that are associated with an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="8e506-163">ReminderDueBy</span><span class="sxs-lookup"><span data-stu-id="8e506-163">ReminderDueBy</span></span>](reminderdueby.md) <br/> |<span data-ttu-id="8e506-164">Представляет дату и время, когда происходит событие.</span><span class="sxs-lookup"><span data-stu-id="8e506-164">Represents the date and time when the event occurs.</span></span> <span data-ttu-id="8e506-165">Используется в элементе [ReminderMinutesBeforeStart](reminderminutesbeforestart.md) определить, когда отображается оповещение.</span><span class="sxs-lookup"><span data-stu-id="8e506-165">This is used by the [ReminderMinutesBeforeStart](reminderminutesbeforestart.md) element to determine when the reminder is displayed.</span></span>  <br/> |
|[<span data-ttu-id="8e506-166">ReminderIsSet</span><span class="sxs-lookup"><span data-stu-id="8e506-166">ReminderIsSet</span></span>](reminderisset.md) <br/> |<span data-ttu-id="8e506-167">Указывает, установлен ли напоминания для элемента в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="8e506-167">Indicates whether a reminder has been set for an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="8e506-168">ReminderMinutesBeforeStart</span><span class="sxs-lookup"><span data-stu-id="8e506-168">ReminderMinutesBeforeStart</span></span>](reminderminutesbeforestart.md) <br/> |<span data-ttu-id="8e506-169">Представляет число минут и только потом событие, когда отображается напоминание.</span><span class="sxs-lookup"><span data-stu-id="8e506-169">Represents the number of minutes before an event when a reminder is displayed.</span></span>  <br/> |
|[<span data-ttu-id="8e506-170">DisplayCc</span><span class="sxs-lookup"><span data-stu-id="8e506-170">DisplayCc</span></span>](displaycc.md) <br/> |<span data-ttu-id="8e506-171">Строка отображения, который используется для содержимого строку "Копия".</span><span class="sxs-lookup"><span data-stu-id="8e506-171">Represents the display string that is used for the contents of the Cc line.</span></span> <span data-ttu-id="8e506-172">Это составное строка всех получателей отображаемые имена «копия».</span><span class="sxs-lookup"><span data-stu-id="8e506-172">This is the concatenated string of all Cc recipient display names.</span></span>  <br/> |
|[<span data-ttu-id="8e506-173">DisplayTo</span><span class="sxs-lookup"><span data-stu-id="8e506-173">DisplayTo</span></span>](displayto.md) <br/> |<span data-ttu-id="8e506-174">Строка отображения, который используется для содержимого в поле «Кому».</span><span class="sxs-lookup"><span data-stu-id="8e506-174">Represents the display string that is used for the contents of the To box.</span></span> <span data-ttu-id="8e506-175">Это составное строка всех для получателей отображаемые имена.</span><span class="sxs-lookup"><span data-stu-id="8e506-175">This is the concatenated string of all To recipient display names.</span></span>  <br/> |
|[<span data-ttu-id="8e506-176">HasAttachments</span><span class="sxs-lookup"><span data-stu-id="8e506-176">HasAttachments</span></span>](hasattachments.md) <br/> |<span data-ttu-id="8e506-177">Представляет свойство, которое задано значение **true,** Если элемент содержит вложение.</span><span class="sxs-lookup"><span data-stu-id="8e506-177">Represents a property that is set to **true** if an item has an attachment.</span></span> <span data-ttu-id="8e506-178">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8e506-178">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="8e506-179">ExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="8e506-179">ExtendedProperty</span></span>](extendedproperty.md) <br/> |<span data-ttu-id="8e506-180">Определяет расширенные свойства для папок и элементов.</span><span class="sxs-lookup"><span data-stu-id="8e506-180">Identifies extended properties on folders and items.</span></span>  <br/> |
|[<span data-ttu-id="8e506-181">Язык и региональные параметры</span><span class="sxs-lookup"><span data-stu-id="8e506-181">Culture</span></span>](culture.md) <br/> |<span data-ttu-id="8e506-182">Представляет язык и региональные параметры для заданного элемента в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="8e506-182">Represents the culture for a given item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="8e506-183">Отправитель</span><span class="sxs-lookup"><span data-stu-id="8e506-183">Sender</span></span>](sender.md) <br/> |<span data-ttu-id="8e506-184">Идентифицирует отправителя элемента.</span><span class="sxs-lookup"><span data-stu-id="8e506-184">Identifies the sender of an item.</span></span>  <br/> |
|[<span data-ttu-id="8e506-185">ToRecipients</span><span class="sxs-lookup"><span data-stu-id="8e506-185">ToRecipients</span></span>](torecipients.md) <br/> |<span data-ttu-id="8e506-186">Содержит список получателей сообщения.</span><span class="sxs-lookup"><span data-stu-id="8e506-186">Contains a set of recipients of a message.</span></span>  <br/> |
|[<span data-ttu-id="8e506-187">CcRecipients</span><span class="sxs-lookup"><span data-stu-id="8e506-187">CcRecipients</span></span>](ccrecipients.md) <br/> |<span data-ttu-id="8e506-188">Представляет коллекцию получателей, которые будут получать копии сообщения.</span><span class="sxs-lookup"><span data-stu-id="8e506-188">Represents a collection of recipients that will receive a copy of the message.</span></span>  <br/> |
|[<span data-ttu-id="8e506-189">BccRecipients</span><span class="sxs-lookup"><span data-stu-id="8e506-189">BccRecipients</span></span>](bccrecipients.md) <br/> |<span data-ttu-id="8e506-190">Представляет коллекцию получателей скрытой копии (СК) сообщения электронной почты.</span><span class="sxs-lookup"><span data-stu-id="8e506-190">Represents a collection of recipients to receive a blind carbon copy (Bcc) of an e-mail.</span></span>  <br/> |
|[<span data-ttu-id="8e506-191">IsReadReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="8e506-191">IsReadReceiptRequested</span></span>](isreadreceiptrequested.md) <br/> |<span data-ttu-id="8e506-192">Указывает, будет ли отправителя элемента о прочтении.</span><span class="sxs-lookup"><span data-stu-id="8e506-192">Indicates whether the sender of an item requests a read receipt.</span></span>  <br/> |
|[<span data-ttu-id="8e506-193">IsDeliveryReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="8e506-193">IsDeliveryReceiptRequested</span></span>](isdeliveryreceiptrequested.md) <br/> |<span data-ttu-id="8e506-194">Указывает, требует ли отправитель элемента уведомление о доставке.</span><span class="sxs-lookup"><span data-stu-id="8e506-194">Indicates whether the sender of an item requests a delivery receipt.</span></span>  <br/> |
|[<span data-ttu-id="8e506-195">ConversationIndex</span><span class="sxs-lookup"><span data-stu-id="8e506-195">ConversationIndex</span></span>](conversationindex.md) <br/> |<span data-ttu-id="8e506-196">Содержит двоичные идентификатор, представляющий поток, к которой принадлежит это сообщение.</span><span class="sxs-lookup"><span data-stu-id="8e506-196">Contains a binary ID that represents the thread to which this message belongs.</span></span>  <br/> |
|[<span data-ttu-id="8e506-197">ConversationTopic</span><span class="sxs-lookup"><span data-stu-id="8e506-197">ConversationTopic</span></span>](conversationtopic.md) <br/> |<span data-ttu-id="8e506-198">Представляет идентификатор беседы.</span><span class="sxs-lookup"><span data-stu-id="8e506-198">Represents the conversation identifier.</span></span>  <br/> |
|[<span data-ttu-id="8e506-199">From</span><span class="sxs-lookup"><span data-stu-id="8e506-199">From</span></span>](from.md) <br/> |<span data-ttu-id="8e506-200">Представляет адрес, с которого было отправлено сообщение.</span><span class="sxs-lookup"><span data-stu-id="8e506-200">Represents the address from which the message was sent.</span></span>  <br/> |
|[<span data-ttu-id="8e506-201">InternetMessageId</span><span class="sxs-lookup"><span data-stu-id="8e506-201">InternetMessageId</span></span>](internetmessageid.md) <br/> |<span data-ttu-id="8e506-202">Представляет идентификатор сообщения Интернета элемента.</span><span class="sxs-lookup"><span data-stu-id="8e506-202">Represents the Internet message identifier of an item.</span></span>  <br/> |
|[<span data-ttu-id="8e506-203">IsRead</span><span class="sxs-lookup"><span data-stu-id="8e506-203">IsRead</span></span>](isread.md) <br/> |<span data-ttu-id="8e506-204">Указывает, имеет ли чтение сообщения.</span><span class="sxs-lookup"><span data-stu-id="8e506-204">Indicates whether a message has been read.</span></span>  <br/> |
|[<span data-ttu-id="8e506-205">IsResponseRequested</span><span class="sxs-lookup"><span data-stu-id="8e506-205">IsResponseRequested</span></span>](isresponserequested.md) <br/> |<span data-ttu-id="8e506-206">Указывает, запрашивается ли ответ на сообщение электронной почты.</span><span class="sxs-lookup"><span data-stu-id="8e506-206">Indicates whether a response to an e-mail message is requested.</span></span>  <br/> |
|[<span data-ttu-id="8e506-207">Справочные материалы</span><span class="sxs-lookup"><span data-stu-id="8e506-207">References</span></span>](references.md) <br/> |<span data-ttu-id="8e506-208">Представляет заголовок групп, используемый для связи с исходными сообщениями ответов.</span><span class="sxs-lookup"><span data-stu-id="8e506-208">Represents the Usenet header that is used to associate replies with their original messages.</span></span>  <br/> |
|[<span data-ttu-id="8e506-209">ReplyTo</span><span class="sxs-lookup"><span data-stu-id="8e506-209">ReplyTo</span></span>](replyto.md) <br/> |<span data-ttu-id="8e506-210">Определяет набор адресов, к которым будут отправляться ответы.</span><span class="sxs-lookup"><span data-stu-id="8e506-210">Identifies a set of addresses to which replies should be sent.</span></span>  <br/> |
|[<span data-ttu-id="8e506-211">EffectiveRights</span><span class="sxs-lookup"><span data-stu-id="8e506-211">EffectiveRights</span></span>](effectiverights.md) <br/> |<span data-ttu-id="8e506-212">Содержит права клиента на основании параметров разрешений для элемента или папки.</span><span class="sxs-lookup"><span data-stu-id="8e506-212">Contains the client's rights based on the permission settings for the item or folder.</span></span> <span data-ttu-id="8e506-213">Этот элемент доступен только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8e506-213">This element is read-only.</span></span> <span data-ttu-id="8e506-214">Этот элемент появился в Exchange 2007 с пакетом обновления 1.</span><span class="sxs-lookup"><span data-stu-id="8e506-214">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="8e506-215">Получил</span><span class="sxs-lookup"><span data-stu-id="8e506-215">ReceivedBy</span></span>](receivedby.md) <br/> |<span data-ttu-id="8e506-216">Определяет делегат в сценарии доступа делегата.</span><span class="sxs-lookup"><span data-stu-id="8e506-216">Identifies the delegate in a delegate access scenario.</span></span> <span data-ttu-id="8e506-217">Этот элемент появился в Exchange 2007 с пакетом обновления 1.</span><span class="sxs-lookup"><span data-stu-id="8e506-217">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="8e506-218">ReceivedRepresenting</span><span class="sxs-lookup"><span data-stu-id="8e506-218">ReceivedRepresenting</span></span>](receivedrepresenting.md) <br/> |<span data-ttu-id="8e506-219">Идентифицирует участника в сценарии доступа делегата.</span><span class="sxs-lookup"><span data-stu-id="8e506-219">Identifies the principal in a delegate access scenario.</span></span> <span data-ttu-id="8e506-220">Этот элемент появился в Exchange 2007 с пакетом обновления 1.</span><span class="sxs-lookup"><span data-stu-id="8e506-220">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="8e506-221">NewBodyContent</span><span class="sxs-lookup"><span data-stu-id="8e506-221">NewBodyContent</span></span>](newbodycontent.md) <br/> |<span data-ttu-id="8e506-222">Представляет новое содержимое текста элемента записи.</span><span class="sxs-lookup"><span data-stu-id="8e506-222">Represents the new body content of a post item.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="8e506-223">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="8e506-223">Parent elements</span></span>

|<span data-ttu-id="8e506-224">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="8e506-224">**Element**</span></span>|<span data-ttu-id="8e506-225">**Описание**</span><span class="sxs-lookup"><span data-stu-id="8e506-225">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8e506-226">AdjacentMeetings</span><span class="sxs-lookup"><span data-stu-id="8e506-226">AdjacentMeetings</span></span>](adjacentmeetings.md) <br/> |<span data-ttu-id="8e506-227">Описание всех элементов, расположенных во время собрания.</span><span class="sxs-lookup"><span data-stu-id="8e506-227">Describes all items that are adjacent to a meeting time.</span></span>  <br/> |
|[<span data-ttu-id="8e506-228">ConflictingMeetings</span><span class="sxs-lookup"><span data-stu-id="8e506-228">ConflictingMeetings</span></span>](conflictingmeetings.md) <br/> |<span data-ttu-id="8e506-229">Описание всех элементов, конфликтующие с время собрания.</span><span class="sxs-lookup"><span data-stu-id="8e506-229">Describes all items that conflict with a meeting time.</span></span>  <br/> |
|[<span data-ttu-id="8e506-230">ResponseObjects</span><span class="sxs-lookup"><span data-stu-id="8e506-230">ResponseObjects</span></span>](responseobjects.md) <br/> |<span data-ttu-id="8e506-231">Содержит коллекцию всех объектов ответа, которые связаны с элемента в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="8e506-231">Contains a collection of all the response objects that are associated with an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="8e506-232">Элементы (NonEmptyArrayOfAllItemsType)</span><span class="sxs-lookup"><span data-stu-id="8e506-232">Items (NonEmptyArrayOfAllItemsType)</span></span>](items-nonemptyarrayofallitemstype.md) <br/> |<span data-ttu-id="8e506-233">Содержит массив элементов для создания в папке, указанной с помощью элемента [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) .</span><span class="sxs-lookup"><span data-stu-id="8e506-233">Contains an array of items to create in the folder that is identified by the [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) element.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="8e506-234">Замечания</span><span class="sxs-lookup"><span data-stu-id="8e506-234">Remarks</span></span>

<span data-ttu-id="8e506-235">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="8e506-235">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="8e506-236">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="8e506-236">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8e506-237">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="8e506-237">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="8e506-238">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="8e506-238">Schema Name</span></span>  <br/> |<span data-ttu-id="8e506-239">Схема Types</span><span class="sxs-lookup"><span data-stu-id="8e506-239">Types schema</span></span>  <br/> |
|<span data-ttu-id="8e506-240">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="8e506-240">Validation File</span></span>  <br/> |<span data-ttu-id="8e506-241">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="8e506-241">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="8e506-242">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="8e506-242">Can be Empty</span></span>  <br/> |<span data-ttu-id="8e506-243">False</span><span class="sxs-lookup"><span data-stu-id="8e506-243">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="8e506-244">См. также</span><span class="sxs-lookup"><span data-stu-id="8e506-244">See also</span></span>



- [<span data-ttu-id="8e506-245">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="8e506-245">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

