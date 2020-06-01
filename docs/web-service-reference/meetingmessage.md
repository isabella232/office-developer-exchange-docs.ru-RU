---
title: митингмессаже
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
description: Элемент Митингмессаже представляет собрание в хранилище Exchange.
ms.openlocfilehash: fee615a1da117e5df03cd5ce8576bd66d7e89a4e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/01/2020
ms.locfileid: "44468385"
---
# <a name="meetingmessage"></a><span data-ttu-id="6b41b-103">митингмессаже</span><span class="sxs-lookup"><span data-stu-id="6b41b-103">MeetingMessage</span></span>

<span data-ttu-id="6b41b-104">Элемент **митингмессаже** представляет собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="6b41b-104">The **MeetingMessage** element represents a meeting in the Exchange store.</span></span> 
  
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

 <span data-ttu-id="6b41b-105">**митингмессажетипе**</span><span class="sxs-lookup"><span data-stu-id="6b41b-105">**MeetingMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6b41b-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="6b41b-106">Attributes and elements</span></span>

<span data-ttu-id="6b41b-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="6b41b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6b41b-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="6b41b-108">Attributes</span></span>

<span data-ttu-id="6b41b-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="6b41b-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6b41b-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="6b41b-110">Child elements</span></span>

|<span data-ttu-id="6b41b-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="6b41b-111">**Element**</span></span>|<span data-ttu-id="6b41b-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="6b41b-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6b41b-113">Сохранитьmimecontent</span><span class="sxs-lookup"><span data-stu-id="6b41b-113">MimeContent</span></span>](mimecontent.md) <br/> |<span data-ttu-id="6b41b-114">Содержит собственный поток MIME объекта, представленный в формате base64Binary.</span><span class="sxs-lookup"><span data-stu-id="6b41b-114">Contains the native MIME stream of an object that is represented in base64Binary format.</span></span>  <br/> |
|[<span data-ttu-id="6b41b-115">Идентификатор</span><span class="sxs-lookup"><span data-stu-id="6b41b-115">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="6b41b-116">Содержит уникальный идентификатор и ключ изменения элемента в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="6b41b-116">Contains the unique identifier and change key of an item in the Exchange store.</span></span> <span data-ttu-id="6b41b-117">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6b41b-117">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="6b41b-118">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="6b41b-118">ParentFolderId</span></span>](parentfolderid.md) <br/> |<span data-ttu-id="6b41b-119">Представляет идентификатор родительской папки, содержащей элемент или папку.</span><span class="sxs-lookup"><span data-stu-id="6b41b-119">Represents the identifier of the parent folder that contains the item or folder.</span></span> <span data-ttu-id="6b41b-120">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6b41b-120">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="6b41b-121">ItemClass</span><span class="sxs-lookup"><span data-stu-id="6b41b-121">ItemClass</span></span>](itemclass.md) <br/> |<span data-ttu-id="6b41b-122">Представляет класс сообщения для элемента.</span><span class="sxs-lookup"><span data-stu-id="6b41b-122">Represents the message class of an item.</span></span>  <br/> |
|[<span data-ttu-id="6b41b-123">Тема</span><span class="sxs-lookup"><span data-stu-id="6b41b-123">Subject</span></span>](subject.md) <br/> |<span data-ttu-id="6b41b-124">Представляет тему для элементов хранилища Exchange и объектов ответа.</span><span class="sxs-lookup"><span data-stu-id="6b41b-124">Represents the subject for Exchange store items and response objects.</span></span> <span data-ttu-id="6b41b-125">Тема может иметь не более 255 символов.</span><span class="sxs-lookup"><span data-stu-id="6b41b-125">The subject is limited to 255 characters.</span></span>  <br/> |
|[<span data-ttu-id="6b41b-126">Sensitivity</span><span class="sxs-lookup"><span data-stu-id="6b41b-126">Sensitivity</span></span>](sensitivity.md) <br/> |<span data-ttu-id="6b41b-127">Содержит статус чувствительности элемента.</span><span class="sxs-lookup"><span data-stu-id="6b41b-127">Contains the status for an item's sensitivity.</span></span>  <br/> |
|[<span data-ttu-id="6b41b-128">Body</span><span class="sxs-lookup"><span data-stu-id="6b41b-128">Body</span></span>](body.md) <br/> |<span data-ttu-id="6b41b-129">Представляет реальное содержимое основного текста сообщения.</span><span class="sxs-lookup"><span data-stu-id="6b41b-129">Represents the actual body content of a message.</span></span>  <br/> |
|[<span data-ttu-id="6b41b-130">Вложения</span><span class="sxs-lookup"><span data-stu-id="6b41b-130">Attachments</span></span>](attachments-ex15websvcsotherref.md) <br/> |<span data-ttu-id="6b41b-131">Содержит элементы или файлы, вложенные в элемент в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="6b41b-131">Contains the items or files that are attached to an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="6b41b-132">DateTimeReceived</span><span class="sxs-lookup"><span data-stu-id="6b41b-132">DateTimeReceived</span></span>](datetimereceived.md) <br/> |<span data-ttu-id="6b41b-133">Представляет дату и время получения элемента в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="6b41b-133">Represents the date and time that an item in a mailbox was received.</span></span>  <br/> |
|[<span data-ttu-id="6b41b-134">Размер</span><span class="sxs-lookup"><span data-stu-id="6b41b-134">Size</span></span>](size.md) <br/> |<span data-ttu-id="6b41b-135">Представляет размер элемента в байтах.</span><span class="sxs-lookup"><span data-stu-id="6b41b-135">Represents the size in bytes of an item.</span></span> <span data-ttu-id="6b41b-136">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6b41b-136">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="6b41b-137">Категории</span><span class="sxs-lookup"><span data-stu-id="6b41b-137">Categories</span></span>](categories-ex15websvcsotherref.md) <br/> |<span data-ttu-id="6b41b-138">Представляет коллекцию строк, определяющих, к каким категориям принадлежит элемент в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="6b41b-138">Represents a collection of strings that identify to which categories an item in the mailbox belongs.</span></span>  <br/> |
|[<span data-ttu-id="6b41b-139">Importance</span><span class="sxs-lookup"><span data-stu-id="6b41b-139">Importance</span></span>](importance.md) <br/> |<span data-ttu-id="6b41b-140">Описывает важность элемента.</span><span class="sxs-lookup"><span data-stu-id="6b41b-140">Describes the importance of an item.</span></span>  <br/> |
|[<span data-ttu-id="6b41b-141">инреплито</span><span class="sxs-lookup"><span data-stu-id="6b41b-141">InReplyTo</span></span>](inreplyto.md) <br/> |<span data-ttu-id="6b41b-142">Представляет идентификатор элемента, который является ответом на этот элемент.</span><span class="sxs-lookup"><span data-stu-id="6b41b-142">Represents the identifier of the item to which this item is a reply.</span></span>  <br/> |
|[<span data-ttu-id="6b41b-143">Отправлено</span><span class="sxs-lookup"><span data-stu-id="6b41b-143">IsSubmitted</span></span>](issubmitted.md) <br/> |<span data-ttu-id="6b41b-144">Указывает, был ли элемент отправлен в папку "Исходящие" по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="6b41b-144">Indicates whether an item has been submitted to the Outbox default folder.</span></span>  <br/> |
|[<span data-ttu-id="6b41b-145">Черновик</span><span class="sxs-lookup"><span data-stu-id="6b41b-145">IsDraft</span></span>](isdraft.md) <br/> |<span data-ttu-id="6b41b-146">Указывает, был ли элемент еще не отправлен.</span><span class="sxs-lookup"><span data-stu-id="6b41b-146">Represents whether an item has not yet been sent.</span></span>  <br/> |
|[<span data-ttu-id="6b41b-147">исфромме</span><span class="sxs-lookup"><span data-stu-id="6b41b-147">IsFromMe</span></span>](isfromme.md) <br/> |<span data-ttu-id="6b41b-148">Указывает, отправляет ли пользователь элемент.</span><span class="sxs-lookup"><span data-stu-id="6b41b-148">Indicates whether a user sent an item to him or herself.</span></span>  <br/> |
|[<span data-ttu-id="6b41b-149">исресенд</span><span class="sxs-lookup"><span data-stu-id="6b41b-149">IsResend</span></span>](isresend.md) <br/> |<span data-ttu-id="6b41b-150">Указывает, был ли ранее отправлен элемент.</span><span class="sxs-lookup"><span data-stu-id="6b41b-150">Indicates whether the item had previously been sent.</span></span>  <br/> |
|[<span data-ttu-id="6b41b-151">исунмодифиед</span><span class="sxs-lookup"><span data-stu-id="6b41b-151">IsUnmodified</span></span>](isunmodified.md) <br/> |<span data-ttu-id="6b41b-152">Указывает, был ли изменен элемент.</span><span class="sxs-lookup"><span data-stu-id="6b41b-152">Indicates whether the item has been modified.</span></span>  <br/> |
|[<span data-ttu-id="6b41b-153">InternetMessageHeaders</span><span class="sxs-lookup"><span data-stu-id="6b41b-153">InternetMessageHeaders</span></span>](internetmessageheaders.md) <br/> |<span data-ttu-id="6b41b-154">Представляет коллекцию всех заголовков сообщений Интернета, содержащихся в элементе почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="6b41b-154">Represents the collection of all Internet message headers that are contained within an item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="6b41b-155">датетимесент</span><span class="sxs-lookup"><span data-stu-id="6b41b-155">DateTimeSent</span></span>](datetimesent.md) <br/> |<span data-ttu-id="6b41b-156">Представляет дату и время отправки элемента в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="6b41b-156">Represents the date and time that an item in a mailbox was sent.</span></span>  <br/> |
|[<span data-ttu-id="6b41b-157">DateTimeCreated</span><span class="sxs-lookup"><span data-stu-id="6b41b-157">DateTimeCreated</span></span>](datetimecreated.md) <br/> |<span data-ttu-id="6b41b-158">Представляет дату и время создания определенного элемента в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="6b41b-158">Represents the date and time that a given item in the mailbox was created.</span></span>  <br/> |
|[<span data-ttu-id="6b41b-159">респонсеобжектс</span><span class="sxs-lookup"><span data-stu-id="6b41b-159">ResponseObjects</span></span>](responseobjects.md) <br/> |<span data-ttu-id="6b41b-160">Содержит коллекцию всех объектов ответа, связанных с элементом в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="6b41b-160">Contains a collection of all the response objects that are associated with an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="6b41b-161">реминдердуеби</span><span class="sxs-lookup"><span data-stu-id="6b41b-161">ReminderDueBy</span></span>](reminderdueby.md) <br/> |<span data-ttu-id="6b41b-162">Представляет дату и время возникновения события.</span><span class="sxs-lookup"><span data-stu-id="6b41b-162">Represents the date and time when the event occurs.</span></span> <span data-ttu-id="6b41b-163">Он используется элементом [реминдерминутесбефорестарт](reminderminutesbeforestart.md) для определения времени отображения напоминания.</span><span class="sxs-lookup"><span data-stu-id="6b41b-163">This is used by the [ReminderMinutesBeforeStart](reminderminutesbeforestart.md) element to determine when the reminder is displayed.</span></span>  <br/> |
|[<span data-ttu-id="6b41b-164">реминдериссет</span><span class="sxs-lookup"><span data-stu-id="6b41b-164">ReminderIsSet</span></span>](reminderisset.md) <br/> |<span data-ttu-id="6b41b-165">Указывает, задано ли напоминание для элемента в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="6b41b-165">Indicates whether a reminder has been set for an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="6b41b-166">ReminderMinutesBeforeStart</span><span class="sxs-lookup"><span data-stu-id="6b41b-166">ReminderMinutesBeforeStart</span></span>](reminderminutesbeforestart.md) <br/> |<span data-ttu-id="6b41b-167">Представляет количество минут до события при отображении напоминания.</span><span class="sxs-lookup"><span data-stu-id="6b41b-167">Represents the number of minutes before an event when a reminder is displayed.</span></span>  <br/> |
|[<span data-ttu-id="6b41b-168">дисплайкк</span><span class="sxs-lookup"><span data-stu-id="6b41b-168">DisplayCc</span></span>](displaycc.md) <br/> |<span data-ttu-id="6b41b-169">Представляет отображаемую строку, используемую для содержимого поля "копия".</span><span class="sxs-lookup"><span data-stu-id="6b41b-169">Represents the display string that is used for the contents of the Cc box.</span></span> <span data-ttu-id="6b41b-170">Это объединенная строка всех отображаемых имен получателей копии.</span><span class="sxs-lookup"><span data-stu-id="6b41b-170">This is the concatenated string of all Cc recipient display names.</span></span>  <br/> |
|[<span data-ttu-id="6b41b-171">дисплайто</span><span class="sxs-lookup"><span data-stu-id="6b41b-171">DisplayTo</span></span>](displayto.md) <br/> |<span data-ttu-id="6b41b-172">Представляет отображаемую строку, используемую для содержимого поля "Кому".</span><span class="sxs-lookup"><span data-stu-id="6b41b-172">Represents the display string that is used for the contents of the To box.</span></span> <span data-ttu-id="6b41b-173">Это объединенная строка для отображаемых имен получателей.</span><span class="sxs-lookup"><span data-stu-id="6b41b-173">This is the concatenated string of all To recipient display names.</span></span>  <br/> |
|[<span data-ttu-id="6b41b-174">HasAttachments</span><span class="sxs-lookup"><span data-stu-id="6b41b-174">HasAttachments</span></span>](hasattachments.md) <br/> |<span data-ttu-id="6b41b-175">Представляет свойство, для которого задано значение **true** , если элемент имеет по крайней мере одно видимое вложение.</span><span class="sxs-lookup"><span data-stu-id="6b41b-175">Represents a property that is set to **true** if an item has at least one visible attachment.</span></span> <span data-ttu-id="6b41b-176">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6b41b-176">This property is read only.</span></span>  <br/> |
|[<span data-ttu-id="6b41b-177">ExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="6b41b-177">ExtendedProperty</span></span>](extendedproperty.md) <br/> |<span data-ttu-id="6b41b-178">Определяет расширенные свойства для папок и элементов.</span><span class="sxs-lookup"><span data-stu-id="6b41b-178">Identifies extended properties on folders and items.</span></span>  <br/> |
|[<span data-ttu-id="6b41b-179">Culture</span><span class="sxs-lookup"><span data-stu-id="6b41b-179">Culture</span></span>](culture.md) <br/> |<span data-ttu-id="6b41b-180">Представляет язык и региональные параметры для определенного элемента в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="6b41b-180">Represents the culture for a given item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="6b41b-181">Sender</span><span class="sxs-lookup"><span data-stu-id="6b41b-181">Sender</span></span>](sender.md) <br/> |<span data-ttu-id="6b41b-182">Определяет отправителя элемента.</span><span class="sxs-lookup"><span data-stu-id="6b41b-182">Identifies the sender of an item.</span></span>  <br/> |
|[<span data-ttu-id="6b41b-183">ToRecipients</span><span class="sxs-lookup"><span data-stu-id="6b41b-183">ToRecipients</span></span>](torecipients.md) <br/> |<span data-ttu-id="6b41b-184">Содержит набор получателей сообщения.</span><span class="sxs-lookup"><span data-stu-id="6b41b-184">Contains a set of recipients of a message.</span></span>  <br/> |
|[<span data-ttu-id="6b41b-185">CcRecipients</span><span class="sxs-lookup"><span data-stu-id="6b41b-185">CcRecipients</span></span>](ccrecipients.md) <br/> |<span data-ttu-id="6b41b-186">Представляет коллекцию получателей, которые будут получать копию сообщения.</span><span class="sxs-lookup"><span data-stu-id="6b41b-186">Represents a collection of recipients that will receive a copy of the message.</span></span>  <br/> |
|[<span data-ttu-id="6b41b-187">BccRecipients</span><span class="sxs-lookup"><span data-stu-id="6b41b-187">BccRecipients</span></span>](bccrecipients.md) <br/> |<span data-ttu-id="6b41b-188">Представляет коллекцию получателей для получения скрытой копии сообщения электронной почты.</span><span class="sxs-lookup"><span data-stu-id="6b41b-188">Represents a collection of recipients to receive a blind carbon copy (Bcc) of an e-mail.</span></span>  <br/> |
|[<span data-ttu-id="6b41b-189">исреадрецеиптрекуестед</span><span class="sxs-lookup"><span data-stu-id="6b41b-189">IsReadReceiptRequested</span></span>](isreadreceiptrequested.md) <br/> |<span data-ttu-id="6b41b-190">Указывает, запрашивает ли отправитель элемента уведомление о прочтении.</span><span class="sxs-lookup"><span data-stu-id="6b41b-190">Indicates whether the sender of an item requests a read receipt.</span></span>  <br/> |
|[<span data-ttu-id="6b41b-191">исделиверирецеиптрекуестед</span><span class="sxs-lookup"><span data-stu-id="6b41b-191">IsDeliveryReceiptRequested</span></span>](isdeliveryreceiptrequested.md) <br/> |<span data-ttu-id="6b41b-192">Указывает, запрашивает ли отправитель элемента уведомление о доставке.</span><span class="sxs-lookup"><span data-stu-id="6b41b-192">Indicates whether the sender of an item requests a delivery receipt.</span></span>  <br/> |
|[<span data-ttu-id="6b41b-193">ConversationIndex</span><span class="sxs-lookup"><span data-stu-id="6b41b-193">ConversationIndex</span></span>](conversationindex.md) <br/> |<span data-ttu-id="6b41b-194">Содержит двоичный код, представляющий поток, к которому относится сообщение.</span><span class="sxs-lookup"><span data-stu-id="6b41b-194">Contains a binary ID that represents the thread to which this message belongs.</span></span>  <br/> |
|[<span data-ttu-id="6b41b-195">ConversationTopic</span><span class="sxs-lookup"><span data-stu-id="6b41b-195">ConversationTopic</span></span>](conversationtopic.md) <br/> |<span data-ttu-id="6b41b-196">Представляет идентификатор беседы.</span><span class="sxs-lookup"><span data-stu-id="6b41b-196">Represents the conversation identifier.</span></span>  <br/> |
|[<span data-ttu-id="6b41b-197">From</span><span class="sxs-lookup"><span data-stu-id="6b41b-197">From</span></span>](from.md) <br/> |<span data-ttu-id="6b41b-198">Представляет адрес получателя, от которого было отправлено сообщение.</span><span class="sxs-lookup"><span data-stu-id="6b41b-198">Represents the addressee from whom the message was sent.</span></span>  <br/> |
|[<span data-ttu-id="6b41b-199">InternetMessageId</span><span class="sxs-lookup"><span data-stu-id="6b41b-199">InternetMessageId</span></span>](internetmessageid.md) <br/> |<span data-ttu-id="6b41b-200">Представляет идентификатор сообщения Интернета для элемента.</span><span class="sxs-lookup"><span data-stu-id="6b41b-200">Represents the Internet message identifier of an item.</span></span>  <br/> |
|[<span data-ttu-id="6b41b-201">IsRead</span><span class="sxs-lookup"><span data-stu-id="6b41b-201">IsRead</span></span>](isread.md) <br/> |<span data-ttu-id="6b41b-202">Указывает, было ли Прочитано сообщение.</span><span class="sxs-lookup"><span data-stu-id="6b41b-202">Indicates whether a message has been read.</span></span>  <br/> |
|[<span data-ttu-id="6b41b-203">исреспонсерекуестед</span><span class="sxs-lookup"><span data-stu-id="6b41b-203">IsResponseRequested</span></span>](isresponserequested.md) <br/> |<span data-ttu-id="6b41b-204">Указывает, запрашивается ли ответ на сообщение электронной почты.</span><span class="sxs-lookup"><span data-stu-id="6b41b-204">Indicates whether a response to an e-mail message is requested.</span></span>  <br/> |
|[<span data-ttu-id="6b41b-205">References</span><span class="sxs-lookup"><span data-stu-id="6b41b-205">References</span></span>](references.md) <br/> |<span data-ttu-id="6b41b-206">Представляет заголовок Usenet, используемый для сопоставления ответов с их исходными сообщениями.</span><span class="sxs-lookup"><span data-stu-id="6b41b-206">Represents the Usenet header that is used to correlate replies with their original messages.</span></span>  <br/> |
|[<span data-ttu-id="6b41b-207">ReplyTo</span><span class="sxs-lookup"><span data-stu-id="6b41b-207">ReplyTo</span></span>](replyto.md) <br/> |<span data-ttu-id="6b41b-208">Определяет набор адресов, в который отправляются ответы.</span><span class="sxs-lookup"><span data-stu-id="6b41b-208">Identifies a set of addresses to which replies should be sent.</span></span>  <br/> |
|[<span data-ttu-id="6b41b-209">ассоЦиатедкалендаритемид</span><span class="sxs-lookup"><span data-stu-id="6b41b-209">AssociatedCalendarItemId</span></span>](associatedcalendaritemid.md) <br/> |<span data-ttu-id="6b41b-210">Представляет элемент календаря, связанный с объектом [митингмессаже](meetingmessage.md).</span><span class="sxs-lookup"><span data-stu-id="6b41b-210">Represents the calendar item that is associated with a [MeetingMessage](meetingmessage.md).</span></span>  <br/> |
|[<span data-ttu-id="6b41b-211">Isdelegated для</span><span class="sxs-lookup"><span data-stu-id="6b41b-211">IsDelegated</span></span>](isdelegated.md) <br/> |<span data-ttu-id="6b41b-212">Указывает, было ли собрание обработано с помощью учетной записи с делегированным доступом.</span><span class="sxs-lookup"><span data-stu-id="6b41b-212">Indicates whether a meeting was handled by an account with delegate access.</span></span>  <br/> |
|[<span data-ttu-id="6b41b-213">IsOutOfDate</span><span class="sxs-lookup"><span data-stu-id="6b41b-213">IsOutOfDate</span></span>](isoutofdate.md) <br/> |<span data-ttu-id="6b41b-214">Указывает, является ли сообщение о собрании устаревшим.</span><span class="sxs-lookup"><span data-stu-id="6b41b-214">Indicates whether a meeting message is out-of-date.</span></span>  <br/> |
|[<span data-ttu-id="6b41b-215">хасбинпроцессед</span><span class="sxs-lookup"><span data-stu-id="6b41b-215">HasBeenProcessed</span></span>](hasbeenprocessed.md) <br/> |<span data-ttu-id="6b41b-216">Указывает, был ли обработан элемент сообщения о собрании.</span><span class="sxs-lookup"><span data-stu-id="6b41b-216">Indicates whether a meeting message item has been processed.</span></span>  <br/> |
|[<span data-ttu-id="6b41b-217">ResponseType</span><span class="sxs-lookup"><span data-stu-id="6b41b-217">ResponseType</span></span>](responsetype.md) <br/> |<span data-ttu-id="6b41b-218">Представляет тип ответа получателя, полученный для собрания.</span><span class="sxs-lookup"><span data-stu-id="6b41b-218">Represents the type of recipient response received for a meeting.</span></span>  <br/> |
|[<span data-ttu-id="6b41b-219">еффективеригхтс</span><span class="sxs-lookup"><span data-stu-id="6b41b-219">EffectiveRights</span></span>](effectiverights.md) <br/> |<span data-ttu-id="6b41b-220">Содержит права клиента на основе параметров разрешений для элемента или папки.</span><span class="sxs-lookup"><span data-stu-id="6b41b-220">Contains the client's rights based on the permission settings for the item or folder.</span></span> <span data-ttu-id="6b41b-221">Этот элемент доступен только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6b41b-221">This element is read-only.</span></span> <span data-ttu-id="6b41b-222">Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="6b41b-222">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span>  <br/> |
|[<span data-ttu-id="6b41b-223">ластмодифиеднаме</span><span class="sxs-lookup"><span data-stu-id="6b41b-223">LastModifiedName</span></span>](lastmodifiedname.md) <br/> |<span data-ttu-id="6b41b-224">Содержит отображаемое имя последнего пользователя для изменения элемента.</span><span class="sxs-lookup"><span data-stu-id="6b41b-224">Contains the display name of the last user to modify an item.</span></span>  <br/> |
|[<span data-ttu-id="6b41b-225">LastModifiedTime</span><span class="sxs-lookup"><span data-stu-id="6b41b-225">LastModifiedTime</span></span>](lastmodifiedtime.md) <br/> |<span data-ttu-id="6b41b-226">Указывает время последнего изменения элемента.</span><span class="sxs-lookup"><span data-stu-id="6b41b-226">Indicates when an item was last modified.</span></span>  <br/> |
|[<span data-ttu-id="6b41b-227">Связанный</span><span class="sxs-lookup"><span data-stu-id="6b41b-227">IsAssociated</span></span>](isassociated.md) <br/> |<span data-ttu-id="6b41b-228">Указывает, связан ли элемент с папкой.</span><span class="sxs-lookup"><span data-stu-id="6b41b-228">Indicates whether the item is associated with a folder.</span></span>  <br/> |
|[<span data-ttu-id="6b41b-229">вебклиентреадформкуеристринг</span><span class="sxs-lookup"><span data-stu-id="6b41b-229">WebClientReadFormQueryString</span></span>](webclientreadformquerystring.md) <br/> |<span data-ttu-id="6b41b-230">Представляет URL-адрес для сцепления с конечной точкой Microsoft Office Outlook Web App для чтения элемента в Outlook Web App.</span><span class="sxs-lookup"><span data-stu-id="6b41b-230">Represents a URL to concatenate to the Microsoft Office Outlook Web App endpoint to read an item in Outlook Web App.</span></span>  <br/> |
|[<span data-ttu-id="6b41b-231">вебклиентедитформкуеристринг</span><span class="sxs-lookup"><span data-stu-id="6b41b-231">WebClientEditFormQueryString</span></span>](webclienteditformquerystring.md) <br/> |<span data-ttu-id="6b41b-232">Представляет URL-адрес для сцепления с конечной точкой Outlook Web App для изменения элемента в Outlook Web App.</span><span class="sxs-lookup"><span data-stu-id="6b41b-232">Represents a URL to concatenate to the Outlook Web App endpoint to edit an item in Outlook Web App.</span></span>  <br/> |
|[<span data-ttu-id="6b41b-233">ConversationId</span><span class="sxs-lookup"><span data-stu-id="6b41b-233">ConversationId</span></span>](conversationid.md) <br/> |<span data-ttu-id="6b41b-234">Содержит идентификатор элемента или беседы.</span><span class="sxs-lookup"><span data-stu-id="6b41b-234">Contains the identifier of an item or conversation.</span></span>  <br/> |
|[<span data-ttu-id="6b41b-235">UniqueBody</span><span class="sxs-lookup"><span data-stu-id="6b41b-235">UniqueBody</span></span>](uniquebody.md) <br/> |<span data-ttu-id="6b41b-236">Представляет фрагмент HTML или обычный текст, представляющий уникальный основной текст этой беседы.</span><span class="sxs-lookup"><span data-stu-id="6b41b-236">Represents an HTML fragment or plain text which represents the unique body of this conversation.</span></span>  <br/> |
|[<span data-ttu-id="6b41b-237">UID</span><span class="sxs-lookup"><span data-stu-id="6b41b-237">UID</span></span>](uid.md) <br/> |<span data-ttu-id="6b41b-238">Определяет элемент календаря.</span><span class="sxs-lookup"><span data-stu-id="6b41b-238">Identifies a calendar item.</span></span>  <br/> |
|[<span data-ttu-id="6b41b-239">рекурренцеид</span><span class="sxs-lookup"><span data-stu-id="6b41b-239">RecurrenceId</span></span>](recurrenceid.md) <br/> |<span data-ttu-id="6b41b-240">Используется для идентификации определенного экземпляра повторяющегося элемента календаря.</span><span class="sxs-lookup"><span data-stu-id="6b41b-240">Used to identify a specific instance of a recurring calendar item.</span></span>  <br/> |
|[<span data-ttu-id="6b41b-241">датетиместамп</span><span class="sxs-lookup"><span data-stu-id="6b41b-241">DateTimeStamp</span></span>](datetimestamp.md) <br/> |<span data-ttu-id="6b41b-242">Указывает дату и время создания экземпляра объекта iCalendar.</span><span class="sxs-lookup"><span data-stu-id="6b41b-242">Indicates the date and time that an instance of an iCalendar object was created.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="6b41b-243">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="6b41b-243">Parent elements</span></span>

|<span data-ttu-id="6b41b-244">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="6b41b-244">**Element**</span></span>|<span data-ttu-id="6b41b-245">**Описание**</span><span class="sxs-lookup"><span data-stu-id="6b41b-245">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6b41b-246">аджацентмитингс</span><span class="sxs-lookup"><span data-stu-id="6b41b-246">AdjacentMeetings</span></span>](adjacentmeetings.md) <br/> |<span data-ttu-id="6b41b-247">Описывает все элементы календаря, смежные с временем собрания.</span><span class="sxs-lookup"><span data-stu-id="6b41b-247">Describes all calendar items that are adjacent to a meeting time.</span></span>  <br/> |
|[<span data-ttu-id="6b41b-248">аппендтоитемфиелд</span><span class="sxs-lookup"><span data-stu-id="6b41b-248">AppendToItemField</span></span>](appendtoitemfield.md) <br/> |<span data-ttu-id="6b41b-249">Определяет данные, добавляемые к одному свойству элемента во время [операции UpdateItem](updateitem-operation.md).</span><span class="sxs-lookup"><span data-stu-id="6b41b-249">Identifies data to append to a single property of an item during an [UpdateItem operation](updateitem-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="6b41b-250">конфликтингмитингс</span><span class="sxs-lookup"><span data-stu-id="6b41b-250">ConflictingMeetings</span></span>](conflictingmeetings.md) <br/> |<span data-ttu-id="6b41b-251">Определяет все элементы, которые конфликтуют с временем собрания.</span><span class="sxs-lookup"><span data-stu-id="6b41b-251">Identifies all items that conflict with a meeting time.</span></span>  <br/> |
|[<span data-ttu-id="6b41b-252">Create (Итемсинк)</span><span class="sxs-lookup"><span data-stu-id="6b41b-252">Create (ItemSync)</span></span>](create-itemsync.md) <br/> |<span data-ttu-id="6b41b-253">Определяет один элемент, который необходимо создать в локальном хранилище клиента.</span><span class="sxs-lookup"><span data-stu-id="6b41b-253">Identifies a single item to create in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="6b41b-254">Обновление (Итемсинк)</span><span class="sxs-lookup"><span data-stu-id="6b41b-254">Update (ItemSync)</span></span>](update-itemsync.md) <br/> |<span data-ttu-id="6b41b-255">Определяет один элемент для обновления в локальном хранилище клиента.</span><span class="sxs-lookup"><span data-stu-id="6b41b-255">Identifies a single item to update in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="6b41b-256">Items</span><span class="sxs-lookup"><span data-stu-id="6b41b-256">Items</span></span>](items.md) <br/> |<span data-ttu-id="6b41b-257">Содержит массив элементов.</span><span class="sxs-lookup"><span data-stu-id="6b41b-257">Contains an array of items.</span></span>  <br/> |
|[<span data-ttu-id="6b41b-258">Элементы (Нонемптяррайофаллитемстипе)</span><span class="sxs-lookup"><span data-stu-id="6b41b-258">Items (NonEmptyArrayOfAllItemsType)</span></span>](items-nonemptyarrayofallitemstype.md) <br/> |<span data-ttu-id="6b41b-259">Содержит массив элементов для создания в папке, определенной элементом [ParentFolderId (таржетфолдеридтипе)](parentfolderid-targetfolderidtype.md) .</span><span class="sxs-lookup"><span data-stu-id="6b41b-259">Contains an array of items to create in the folder identified by the [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) element.</span></span>  <br/> |
|[<span data-ttu-id="6b41b-260">сетитемфиелд</span><span class="sxs-lookup"><span data-stu-id="6b41b-260">SetItemField</span></span>](setitemfield.md) <br/> |<span data-ttu-id="6b41b-261">Представляет обновление одного свойства элемента в [операции UpdateItem](updateitem-operation.md).</span><span class="sxs-lookup"><span data-stu-id="6b41b-261">Represents an update to a single property of an item in an [UpdateItem operation](updateitem-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="6b41b-262">ItemAttachment</span><span class="sxs-lookup"><span data-stu-id="6b41b-262">ItemAttachment</span></span>](itemattachment.md) <br/> |<span data-ttu-id="6b41b-263">Представляет элемент Exchange, присоединенный к другому элементу Exchange.</span><span class="sxs-lookup"><span data-stu-id="6b41b-263">Represents an Exchange item that is attached to another Exchange item.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="6b41b-264">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="6b41b-264">Text value</span></span>

<span data-ttu-id="6b41b-265">Нет.</span><span class="sxs-lookup"><span data-stu-id="6b41b-265">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="6b41b-266">Примечания</span><span class="sxs-lookup"><span data-stu-id="6b41b-266">Remarks</span></span>

<span data-ttu-id="6b41b-267">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="6b41b-267">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6b41b-268">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="6b41b-268">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6b41b-269">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="6b41b-269">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="6b41b-270">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="6b41b-270">Schema Name</span></span>  <br/> |<span data-ttu-id="6b41b-271">Схема Types</span><span class="sxs-lookup"><span data-stu-id="6b41b-271">Types schema</span></span>  <br/> |
|<span data-ttu-id="6b41b-272">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="6b41b-272">Validation File</span></span>  <br/> |<span data-ttu-id="6b41b-273">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="6b41b-273">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="6b41b-274">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="6b41b-274">Can be Empty</span></span>  <br/> |<span data-ttu-id="6b41b-275">False</span><span class="sxs-lookup"><span data-stu-id="6b41b-275">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6b41b-276">См. также</span><span class="sxs-lookup"><span data-stu-id="6b41b-276">See also</span></span>



- [<span data-ttu-id="6b41b-277">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="6b41b-277">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

