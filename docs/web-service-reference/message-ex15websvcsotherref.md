---
title: Сообщение
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
description: Элемент Message представляет сообщение электронной почты Microsoft Exchange.
ms.openlocfilehash: 510e97572e54f0ea0cb65fc7c75910e69cc0651f
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44467783"
---
# <a name="message"></a><span data-ttu-id="d23e0-103">Сообщение</span><span class="sxs-lookup"><span data-stu-id="d23e0-103">Message</span></span>

<span data-ttu-id="d23e0-104">Элемент **Message** представляет сообщение электронной почты Microsoft Exchange.</span><span class="sxs-lookup"><span data-stu-id="d23e0-104">The **Message** element represents a Microsoft Exchange e-mail message.</span></span> 
  
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

 <span data-ttu-id="d23e0-105">**MessageType**</span><span class="sxs-lookup"><span data-stu-id="d23e0-105">**MessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d23e0-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="d23e0-106">Attributes and elements</span></span>

<span data-ttu-id="d23e0-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="d23e0-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d23e0-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="d23e0-108">Attributes</span></span>

<span data-ttu-id="d23e0-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="d23e0-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d23e0-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="d23e0-110">Child elements</span></span>

|<span data-ttu-id="d23e0-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="d23e0-111">**Element**</span></span>|<span data-ttu-id="d23e0-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d23e0-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d23e0-113">Сохранитьmimecontent</span><span class="sxs-lookup"><span data-stu-id="d23e0-113">MimeContent</span></span>](mimecontent.md) <br/> |<span data-ttu-id="d23e0-114">Содержит собственный многоцелевой поток расширений почты в Интернете (MIME) объекта, представленного в формате base64Binary.</span><span class="sxs-lookup"><span data-stu-id="d23e0-114">Contains the native Multipurpose Internet Mail Extensions (MIME) stream of an object that is represented in base64Binary format.</span></span>  <br/> |
|[<span data-ttu-id="d23e0-115">Идентификатор</span><span class="sxs-lookup"><span data-stu-id="d23e0-115">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="d23e0-116">Содержит уникальный идентификатор и ключ изменения элемента в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="d23e0-116">Contains the unique identifier and change key of an item in the Exchange store.</span></span> <span data-ttu-id="d23e0-117">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d23e0-117">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="d23e0-118">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="d23e0-118">ParentFolderId</span></span>](parentfolderid.md) <br/> |<span data-ttu-id="d23e0-119">Представляет идентификатор родительской папки, содержащей элемент или папку.</span><span class="sxs-lookup"><span data-stu-id="d23e0-119">Represents the identifier of the parent folder that contains the item or folder.</span></span> <span data-ttu-id="d23e0-120">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d23e0-120">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="d23e0-121">ItemClass</span><span class="sxs-lookup"><span data-stu-id="d23e0-121">ItemClass</span></span>](itemclass.md) <br/> |<span data-ttu-id="d23e0-122">Представляет класс сообщения для элемента.</span><span class="sxs-lookup"><span data-stu-id="d23e0-122">Represents the message class of an item.</span></span>  <br/> |
|[<span data-ttu-id="d23e0-123">Тема</span><span class="sxs-lookup"><span data-stu-id="d23e0-123">Subject</span></span>](subject.md) <br/> |<span data-ttu-id="d23e0-124">Представляет тему для элементов хранилища Exchange и объектов ответа.</span><span class="sxs-lookup"><span data-stu-id="d23e0-124">Represents the subject for Exchange store items and response objects.</span></span> <span data-ttu-id="d23e0-125">Тема может иметь не более 255 символов.</span><span class="sxs-lookup"><span data-stu-id="d23e0-125">The subject is limited to 255 characters.</span></span>  <br/> |
|[<span data-ttu-id="d23e0-126">Sensitivity</span><span class="sxs-lookup"><span data-stu-id="d23e0-126">Sensitivity</span></span>](sensitivity.md) <br/> |<span data-ttu-id="d23e0-127">Указывает уровень конфиденциальности элемента.</span><span class="sxs-lookup"><span data-stu-id="d23e0-127">Indicates the sensitivity level of an item.</span></span>  <br/> |
|[<span data-ttu-id="d23e0-128">Body</span><span class="sxs-lookup"><span data-stu-id="d23e0-128">Body</span></span>](body.md) <br/> |<span data-ttu-id="d23e0-129">Представляет реальное содержимое основного текста сообщения.</span><span class="sxs-lookup"><span data-stu-id="d23e0-129">Represents the actual body content of a message.</span></span>  <br/> |
|[<span data-ttu-id="d23e0-130">Вложения</span><span class="sxs-lookup"><span data-stu-id="d23e0-130">Attachments</span></span>](attachments-ex15websvcsotherref.md) <br/> |<span data-ttu-id="d23e0-131">Содержит элементы или файлы, вложенные в элемент в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="d23e0-131">Contains the items or files that are attached to an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="d23e0-132">DateTimeReceived</span><span class="sxs-lookup"><span data-stu-id="d23e0-132">DateTimeReceived</span></span>](datetimereceived.md) <br/> |<span data-ttu-id="d23e0-133">Представляет дату и время получения элемента в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="d23e0-133">Represents the date and time that an item in a mailbox was received.</span></span>  <br/> |
|[<span data-ttu-id="d23e0-134">Размер</span><span class="sxs-lookup"><span data-stu-id="d23e0-134">Size</span></span>](size.md) <br/> |<span data-ttu-id="d23e0-135">Представляет размер элемента в байтах.</span><span class="sxs-lookup"><span data-stu-id="d23e0-135">Represents the size in bytes of an item.</span></span> <span data-ttu-id="d23e0-136">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d23e0-136">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="d23e0-137">Категории</span><span class="sxs-lookup"><span data-stu-id="d23e0-137">Categories</span></span>](categories-ex15websvcsotherref.md) <br/> |<span data-ttu-id="d23e0-138">Представляет коллекцию строк, определяющих, к каким категориям принадлежит элемент в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="d23e0-138">Represents a collection of strings that identify to which categories an item in the mailbox belongs.</span></span>  <br/> |
|[<span data-ttu-id="d23e0-139">Importance</span><span class="sxs-lookup"><span data-stu-id="d23e0-139">Importance</span></span>](importance.md) <br/> |<span data-ttu-id="d23e0-140">Описывает важность элемента.</span><span class="sxs-lookup"><span data-stu-id="d23e0-140">Describes the importance of an item.</span></span>  <br/> |
|[<span data-ttu-id="d23e0-141">инреплито</span><span class="sxs-lookup"><span data-stu-id="d23e0-141">InReplyTo</span></span>](inreplyto.md) <br/> |<span data-ttu-id="d23e0-142">Представляет идентификатор элемента, который является ответом на этот элемент.</span><span class="sxs-lookup"><span data-stu-id="d23e0-142">Represents the identifier of the item to which this item is a reply.</span></span>  <br/> |
|[<span data-ttu-id="d23e0-143">Отправлено</span><span class="sxs-lookup"><span data-stu-id="d23e0-143">IsSubmitted</span></span>](issubmitted.md) <br/> |<span data-ttu-id="d23e0-144">Указывает, был ли элемент отправлен в папку "Исходящие" по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="d23e0-144">Indicates whether an item has been submitted to the Outbox default folder.</span></span>  <br/> |
|[<span data-ttu-id="d23e0-145">Черновик</span><span class="sxs-lookup"><span data-stu-id="d23e0-145">IsDraft</span></span>](isdraft.md) <br/> |<span data-ttu-id="d23e0-146">Указывает, был ли элемент еще не отправлен.</span><span class="sxs-lookup"><span data-stu-id="d23e0-146">Represents whether an item has not yet been sent.</span></span>  <br/> |
|[<span data-ttu-id="d23e0-147">исфромме</span><span class="sxs-lookup"><span data-stu-id="d23e0-147">IsFromMe</span></span>](isfromme.md) <br/> |<span data-ttu-id="d23e0-148">Указывает, отправляет ли пользователь элемент.</span><span class="sxs-lookup"><span data-stu-id="d23e0-148">Indicates whether a user sent an item to him or herself.</span></span>  <br/> |
|[<span data-ttu-id="d23e0-149">исресенд</span><span class="sxs-lookup"><span data-stu-id="d23e0-149">IsResend</span></span>](isresend.md) <br/> |<span data-ttu-id="d23e0-150">Указывает, был ли ранее отправлен элемент.</span><span class="sxs-lookup"><span data-stu-id="d23e0-150">Indicates whether the item had previously been sent.</span></span>  <br/> |
|[<span data-ttu-id="d23e0-151">исунмодифиед</span><span class="sxs-lookup"><span data-stu-id="d23e0-151">IsUnmodified</span></span>](isunmodified.md) <br/> |<span data-ttu-id="d23e0-152">Указывает, был ли изменен элемент.</span><span class="sxs-lookup"><span data-stu-id="d23e0-152">Indicates whether the item has been modified.</span></span>  <br/> |
|[<span data-ttu-id="d23e0-153">InternetMessageHeaders</span><span class="sxs-lookup"><span data-stu-id="d23e0-153">InternetMessageHeaders</span></span>](internetmessageheaders.md) <br/> |<span data-ttu-id="d23e0-154">Представляет коллекцию всех заголовков сообщений Интернета, содержащихся в элементе почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="d23e0-154">Represents the collection of all Internet message headers that are contained within an item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="d23e0-155">датетимесент</span><span class="sxs-lookup"><span data-stu-id="d23e0-155">DateTimeSent</span></span>](datetimesent.md) <br/> |<span data-ttu-id="d23e0-156">Представляет дату и время отправки элемента в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="d23e0-156">Represents the date and time that an item in a mailbox was sent.</span></span>  <br/> |
|[<span data-ttu-id="d23e0-157">DateTimeCreated</span><span class="sxs-lookup"><span data-stu-id="d23e0-157">DateTimeCreated</span></span>](datetimecreated.md) <br/> |<span data-ttu-id="d23e0-158">Представляет дату и время создания определенного элемента в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="d23e0-158">Represents the date and time that a given item in the mailbox was created.</span></span>  <br/> |
|[<span data-ttu-id="d23e0-159">респонсеобжектс</span><span class="sxs-lookup"><span data-stu-id="d23e0-159">ResponseObjects</span></span>](responseobjects.md) <br/> |<span data-ttu-id="d23e0-160">Содержит коллекцию всех объектов ответа, связанных с элементом в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="d23e0-160">Contains a collection of all the response objects that are associated with an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="d23e0-161">реминдердуеби</span><span class="sxs-lookup"><span data-stu-id="d23e0-161">ReminderDueBy</span></span>](reminderdueby.md) <br/> |<span data-ttu-id="d23e0-162">Представляет дату и время возникновения события.</span><span class="sxs-lookup"><span data-stu-id="d23e0-162">Represents the date and time when the event occurs.</span></span> <span data-ttu-id="d23e0-163">Он используется элементом [реминдерминутесбефорестарт](reminderminutesbeforestart.md) для определения времени отображения напоминания.</span><span class="sxs-lookup"><span data-stu-id="d23e0-163">This is used by the [ReminderMinutesBeforeStart](reminderminutesbeforestart.md) element to determine when the reminder is displayed.</span></span>  <br/> |
|[<span data-ttu-id="d23e0-164">реминдериссет</span><span class="sxs-lookup"><span data-stu-id="d23e0-164">ReminderIsSet</span></span>](reminderisset.md) <br/> |<span data-ttu-id="d23e0-165">Указывает, задано ли напоминание для элемента в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="d23e0-165">Indicates whether a reminder has been set for an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="d23e0-166">ReminderMinutesBeforeStart</span><span class="sxs-lookup"><span data-stu-id="d23e0-166">ReminderMinutesBeforeStart</span></span>](reminderminutesbeforestart.md) <br/> |<span data-ttu-id="d23e0-167">Представляет количество минут до события при отображении напоминания.</span><span class="sxs-lookup"><span data-stu-id="d23e0-167">Represents the number of minutes before an event when a reminder is displayed.</span></span>  <br/> |
|[<span data-ttu-id="d23e0-168">дисплайкк</span><span class="sxs-lookup"><span data-stu-id="d23e0-168">DisplayCc</span></span>](displaycc.md) <br/> |<span data-ttu-id="d23e0-169">Представляет отображаемую строку, используемую для содержимого строки "копия".</span><span class="sxs-lookup"><span data-stu-id="d23e0-169">Represents the display string that is used for the contents of the CC line.</span></span> <span data-ttu-id="d23e0-170">Это объединенная строка всех отображаемых имен получателей копии.</span><span class="sxs-lookup"><span data-stu-id="d23e0-170">This is the concatenated string of all CC recipient display names.</span></span>  <br/> |
|[<span data-ttu-id="d23e0-171">дисплайто</span><span class="sxs-lookup"><span data-stu-id="d23e0-171">DisplayTo</span></span>](displayto.md) <br/> |<span data-ttu-id="d23e0-172">Представляет отображаемую строку, используемую для содержимого поля "Кому".</span><span class="sxs-lookup"><span data-stu-id="d23e0-172">Represents the display string that is used for the contents of the To box.</span></span> <span data-ttu-id="d23e0-173">Это объединенная строка для отображаемых имен получателей.</span><span class="sxs-lookup"><span data-stu-id="d23e0-173">This is the concatenated string of all To recipient display names.</span></span>  <br/> |
|[<span data-ttu-id="d23e0-174">HasAttachments</span><span class="sxs-lookup"><span data-stu-id="d23e0-174">HasAttachments</span></span>](hasattachments.md) <br/> |<span data-ttu-id="d23e0-175">Представляет свойство, для которого задано значение **true** , если элемент имеет по крайней мере одно видимое вложение.</span><span class="sxs-lookup"><span data-stu-id="d23e0-175">Represents a property that is set to **true** if an item has at least one visible attachment.</span></span> <span data-ttu-id="d23e0-176">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d23e0-176">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="d23e0-177">ExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="d23e0-177">ExtendedProperty</span></span>](extendedproperty.md) <br/> |<span data-ttu-id="d23e0-178">Определяет расширенные свойства для папок и элементов.</span><span class="sxs-lookup"><span data-stu-id="d23e0-178">Identifies extended properties on folders and items.</span></span>  <br/> |
|[<span data-ttu-id="d23e0-179">Culture</span><span class="sxs-lookup"><span data-stu-id="d23e0-179">Culture</span></span>](culture.md) <br/> |<span data-ttu-id="d23e0-180">Представляет язык и региональные параметры для определенного элемента в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="d23e0-180">Represents the culture for a given item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="d23e0-181">Sender</span><span class="sxs-lookup"><span data-stu-id="d23e0-181">Sender</span></span>](sender.md) <br/> |<span data-ttu-id="d23e0-182">Определяет отправителя элемента.</span><span class="sxs-lookup"><span data-stu-id="d23e0-182">Identifies the sender of an item.</span></span>  <br/> |
|[<span data-ttu-id="d23e0-183">ToRecipients</span><span class="sxs-lookup"><span data-stu-id="d23e0-183">ToRecipients</span></span>](torecipients.md) <br/> |<span data-ttu-id="d23e0-184">Содержит набор получателей сообщения.</span><span class="sxs-lookup"><span data-stu-id="d23e0-184">Contains a set of recipients of a message.</span></span>  <br/> |
|[<span data-ttu-id="d23e0-185">CcRecipients</span><span class="sxs-lookup"><span data-stu-id="d23e0-185">CcRecipients</span></span>](ccrecipients.md) <br/> |<span data-ttu-id="d23e0-186">Представляет коллекцию получателей, которые будут получать копию сообщения.</span><span class="sxs-lookup"><span data-stu-id="d23e0-186">Represents a collection of recipients that will receive a copy of the message.</span></span>  <br/> |
|[<span data-ttu-id="d23e0-187">BccRecipients</span><span class="sxs-lookup"><span data-stu-id="d23e0-187">BccRecipients</span></span>](bccrecipients.md) <br/> |<span data-ttu-id="d23e0-188">Представляет коллекцию получателей для получения скрытой копии (BCC) сообщения электронной почты.</span><span class="sxs-lookup"><span data-stu-id="d23e0-188">Represents a collection of recipients to receive a blind carbon copy (Bcc) of an e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="d23e0-189">исреадрецеиптрекуестед</span><span class="sxs-lookup"><span data-stu-id="d23e0-189">IsReadReceiptRequested</span></span>](isreadreceiptrequested.md) <br/> |<span data-ttu-id="d23e0-190">Указывает, запрашивает ли отправитель элемента уведомление о прочтении.</span><span class="sxs-lookup"><span data-stu-id="d23e0-190">Indicates whether the sender of an item requests a read receipt.</span></span>  <br/> |
|[<span data-ttu-id="d23e0-191">исделиверирецеиптрекуестед</span><span class="sxs-lookup"><span data-stu-id="d23e0-191">IsDeliveryReceiptRequested</span></span>](isdeliveryreceiptrequested.md) <br/> |<span data-ttu-id="d23e0-192">Указывает, запрашивает ли отправитель элемента уведомление о доставке.</span><span class="sxs-lookup"><span data-stu-id="d23e0-192">Indicates whether the sender of an item requests a delivery receipt.</span></span>  <br/> |
|[<span data-ttu-id="d23e0-193">ConversationIndex</span><span class="sxs-lookup"><span data-stu-id="d23e0-193">ConversationIndex</span></span>](conversationindex.md) <br/> |<span data-ttu-id="d23e0-194">Содержит двоичный код, представляющий поток, к которому относится сообщение.</span><span class="sxs-lookup"><span data-stu-id="d23e0-194">Contains a binary ID that represents the thread to which this message belongs.</span></span>  <br/> |
|[<span data-ttu-id="d23e0-195">ConversationTopic</span><span class="sxs-lookup"><span data-stu-id="d23e0-195">ConversationTopic</span></span>](conversationtopic.md) <br/> |<span data-ttu-id="d23e0-196">Представляет идентификатор беседы.</span><span class="sxs-lookup"><span data-stu-id="d23e0-196">Represents the conversation identifier.</span></span>  <br/> |
|[<span data-ttu-id="d23e0-197">From</span><span class="sxs-lookup"><span data-stu-id="d23e0-197">From</span></span>](from.md) <br/> |<span data-ttu-id="d23e0-198">Представляет адрес получателя, от которого было отправлено сообщение.</span><span class="sxs-lookup"><span data-stu-id="d23e0-198">Represents the addressee from whom the message was sent.</span></span>  <br/> |
|[<span data-ttu-id="d23e0-199">InternetMessageId</span><span class="sxs-lookup"><span data-stu-id="d23e0-199">InternetMessageId</span></span>](internetmessageid.md) <br/> |<span data-ttu-id="d23e0-200">Представляет идентификатор сообщения Интернета для элемента.</span><span class="sxs-lookup"><span data-stu-id="d23e0-200">Represents the Internet message identifier of an item.</span></span>  <br/> |
|[<span data-ttu-id="d23e0-201">IsRead</span><span class="sxs-lookup"><span data-stu-id="d23e0-201">IsRead</span></span>](isread.md) <br/> |<span data-ttu-id="d23e0-202">Указывает, было ли Прочитано сообщение.</span><span class="sxs-lookup"><span data-stu-id="d23e0-202">Indicates whether a message has been read.</span></span>  <br/> |
|[<span data-ttu-id="d23e0-203">исреспонсерекуестед</span><span class="sxs-lookup"><span data-stu-id="d23e0-203">IsResponseRequested</span></span>](isresponserequested.md) <br/> |<span data-ttu-id="d23e0-204">Указывает, запрашивается ли ответ на сообщение электронной почты.</span><span class="sxs-lookup"><span data-stu-id="d23e0-204">Indicates whether a response to an e-mail message is requested.</span></span>  <br/> |
|[<span data-ttu-id="d23e0-205">References</span><span class="sxs-lookup"><span data-stu-id="d23e0-205">References</span></span>](references.md) <br/> |<span data-ttu-id="d23e0-206">Представляет заголовок Usenet, используемый для сопоставления ответов с их исходными сообщениями.</span><span class="sxs-lookup"><span data-stu-id="d23e0-206">Represents the Usenet header that is used to correlate replies with their original messages.</span></span>  <br/> |
|[<span data-ttu-id="d23e0-207">ReplyTo</span><span class="sxs-lookup"><span data-stu-id="d23e0-207">ReplyTo</span></span>](replyto.md) <br/> |<span data-ttu-id="d23e0-208">Определяет набор адресов, в который отправляются ответы.</span><span class="sxs-lookup"><span data-stu-id="d23e0-208">Identifies a set of addresses to which replies should be sent.</span></span>  <br/> |
|[<span data-ttu-id="d23e0-209">еффективеригхтс</span><span class="sxs-lookup"><span data-stu-id="d23e0-209">EffectiveRights</span></span>](effectiverights.md) <br/> |<span data-ttu-id="d23e0-210">Содержит права клиента на основе параметров разрешений для элемента или папки.</span><span class="sxs-lookup"><span data-stu-id="d23e0-210">Contains the client's rights based on the permission settings for the item or folder.</span></span> <span data-ttu-id="d23e0-211">Этот элемент доступен только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d23e0-211">This element is read-only.</span></span>  <br/> |
|[<span data-ttu-id="d23e0-212">рецеиведби</span><span class="sxs-lookup"><span data-stu-id="d23e0-212">ReceivedBy</span></span>](receivedby.md) <br/> |<span data-ttu-id="d23e0-213">Определяет делегат в сценарии доступа делегата.</span><span class="sxs-lookup"><span data-stu-id="d23e0-213">Identifies the delegate in a delegate access scenario.</span></span>  <br/> |
|[<span data-ttu-id="d23e0-214">рецеиведрепресентинг</span><span class="sxs-lookup"><span data-stu-id="d23e0-214">ReceivedRepresenting</span></span>](receivedrepresenting.md) <br/> |<span data-ttu-id="d23e0-215">Определяет участника в сценарии доступа делегата.</span><span class="sxs-lookup"><span data-stu-id="d23e0-215">Identifies the principal in a delegate access scenario.</span></span>  <br/> |
|[<span data-ttu-id="d23e0-216">ластмодифиеднаме</span><span class="sxs-lookup"><span data-stu-id="d23e0-216">LastModifiedName</span></span>](lastmodifiedname.md) <br/> |<span data-ttu-id="d23e0-217">Содержит отображаемое имя последнего пользователя для изменения элемента.</span><span class="sxs-lookup"><span data-stu-id="d23e0-217">Contains the display name of the last user to modify an item.</span></span>  <br/> |
|[<span data-ttu-id="d23e0-218">LastModifiedTime</span><span class="sxs-lookup"><span data-stu-id="d23e0-218">LastModifiedTime</span></span>](lastmodifiedtime.md) <br/> |<span data-ttu-id="d23e0-219">Указывает время последнего изменения элемента.</span><span class="sxs-lookup"><span data-stu-id="d23e0-219">Indicates when an item was last modified.</span></span>  <br/> |
|[<span data-ttu-id="d23e0-220">Связанный</span><span class="sxs-lookup"><span data-stu-id="d23e0-220">IsAssociated</span></span>](isassociated.md) <br/> |<span data-ttu-id="d23e0-221">Указывает, связан ли элемент с папкой.</span><span class="sxs-lookup"><span data-stu-id="d23e0-221">Indicates whether the item is associated with a folder.</span></span>  <br/> |
|[<span data-ttu-id="d23e0-222">вебклиентреадформкуеристринг</span><span class="sxs-lookup"><span data-stu-id="d23e0-222">WebClientReadFormQueryString</span></span>](webclientreadformquerystring.md) <br/> |<span data-ttu-id="d23e0-223">Представляет URL-адрес для сцепления с конечной точкой Microsoft Office Outlook Web App для чтения элемента в Outlook Web App.</span><span class="sxs-lookup"><span data-stu-id="d23e0-223">Represents a URL to concatenate to the Microsoft Office Outlook Web App endpoint to read an item in Outlook Web App.</span></span>  <br/> |
|[<span data-ttu-id="d23e0-224">вебклиентедитформкуеристринг</span><span class="sxs-lookup"><span data-stu-id="d23e0-224">WebClientEditFormQueryString</span></span>](webclienteditformquerystring.md) <br/> |<span data-ttu-id="d23e0-225">Представляет URL-адрес для сцепления с конечной точкой Outlook Web App для изменения элемента в Outlook Web App.</span><span class="sxs-lookup"><span data-stu-id="d23e0-225">Represents a URL to concatenate to the Outlook Web App endpoint to edit an item in Outlook Web App.</span></span>  <br/> |
|[<span data-ttu-id="d23e0-226">ConversationId</span><span class="sxs-lookup"><span data-stu-id="d23e0-226">ConversationId</span></span>](conversationid.md) <br/> |<span data-ttu-id="d23e0-227">Содержит идентификатор элемента или беседы.</span><span class="sxs-lookup"><span data-stu-id="d23e0-227">Contains the identifier of an item or conversation.</span></span>  <br/> |
|[<span data-ttu-id="d23e0-228">UniqueBody</span><span class="sxs-lookup"><span data-stu-id="d23e0-228">UniqueBody</span></span>](uniquebody.md) <br/> |<span data-ttu-id="d23e0-229">Представляет фрагмент HTML или обычный текст, представляющий уникальный основной текст этой беседы.</span><span class="sxs-lookup"><span data-stu-id="d23e0-229">Represents an HTML fragment or plain text which represents the unique body of this conversation.</span></span>  <br/> |
|[<span data-ttu-id="d23e0-230">реминдермессажедата</span><span class="sxs-lookup"><span data-stu-id="d23e0-230">ReminderMessageData</span></span>](remindermessagedata.md) <br/> |<span data-ttu-id="d23e0-231">Содержит данные для сообщения напоминания.</span><span class="sxs-lookup"><span data-stu-id="d23e0-231">Contains the data for a reminder message.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d23e0-232">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="d23e0-232">Parent elements</span></span>

|<span data-ttu-id="d23e0-233">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="d23e0-233">**Element**</span></span>|<span data-ttu-id="d23e0-234">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d23e0-234">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d23e0-235">аджацентмитингс</span><span class="sxs-lookup"><span data-stu-id="d23e0-235">AdjacentMeetings</span></span>](adjacentmeetings.md) <br/> |<span data-ttu-id="d23e0-236">Описывает все элементы календаря, смежные с временем собрания.</span><span class="sxs-lookup"><span data-stu-id="d23e0-236">Describes all calendar items that are adjacent to a meeting time.</span></span>  <br/> |
|[<span data-ttu-id="d23e0-237">аппендтоитемфиелд</span><span class="sxs-lookup"><span data-stu-id="d23e0-237">AppendToItemField</span></span>](appendtoitemfield.md) <br/> |<span data-ttu-id="d23e0-238">Определяет данные, добавляемые к одному свойству элемента во время [операции UpdateItem](updateitem-operation.md).</span><span class="sxs-lookup"><span data-stu-id="d23e0-238">Identifies data to append to a single property of an item during an [UpdateItem operation](updateitem-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="d23e0-239">конфликтингмитингс</span><span class="sxs-lookup"><span data-stu-id="d23e0-239">ConflictingMeetings</span></span>](conflictingmeetings.md) <br/> |<span data-ttu-id="d23e0-240">Определяет все элементы, которые конфликтуют с временем собрания.</span><span class="sxs-lookup"><span data-stu-id="d23e0-240">Identifies all items that conflict with a meeting time.</span></span>  <br/> |
|[<span data-ttu-id="d23e0-241">Create (Итемсинк)</span><span class="sxs-lookup"><span data-stu-id="d23e0-241">Create (ItemSync)</span></span>](create-itemsync.md) <br/> |<span data-ttu-id="d23e0-242">Определяет один элемент, который необходимо создать в локальном хранилище клиента.</span><span class="sxs-lookup"><span data-stu-id="d23e0-242">Identifies a single item to create in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="d23e0-243">ItemAttachment</span><span class="sxs-lookup"><span data-stu-id="d23e0-243">ItemAttachment</span></span>](itemattachment.md) <br/> |<span data-ttu-id="d23e0-244">Представляет элемент Exchange, присоединенный к другому элементу Exchange.</span><span class="sxs-lookup"><span data-stu-id="d23e0-244">Represents an Exchange item that is attached to another Exchange item.</span></span>  <br/> |
|[<span data-ttu-id="d23e0-245">Items</span><span class="sxs-lookup"><span data-stu-id="d23e0-245">Items</span></span>](items.md) <br/> |<span data-ttu-id="d23e0-246">Содержит массив элементов.</span><span class="sxs-lookup"><span data-stu-id="d23e0-246">Contains an array of items.</span></span>  <br/> |
|[<span data-ttu-id="d23e0-247">Элементы (Нонемптяррайофаллитемстипе)</span><span class="sxs-lookup"><span data-stu-id="d23e0-247">Items (NonEmptyArrayOfAllItemsType)</span></span>](items-nonemptyarrayofallitemstype.md) <br/> |<span data-ttu-id="d23e0-248">Содержит массив элементов для создания в папке, определяемой элементом [ParentFolderId (таржетфолдеридтипе)](parentfolderid-targetfolderidtype.md) .</span><span class="sxs-lookup"><span data-stu-id="d23e0-248">Contains an array of items to create in the folder that is identified by the [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) element.</span></span>  <br/> |
|[<span data-ttu-id="d23e0-249">сетитемфиелд</span><span class="sxs-lookup"><span data-stu-id="d23e0-249">SetItemField</span></span>](setitemfield.md) <br/> |<span data-ttu-id="d23e0-250">Представляет обновление одного свойства элемента в [операции UpdateItem](updateitem-operation.md).</span><span class="sxs-lookup"><span data-stu-id="d23e0-250">Represents an update to a single property of an item in an [UpdateItem operation](updateitem-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="d23e0-251">Обновление (Итемсинк)</span><span class="sxs-lookup"><span data-stu-id="d23e0-251">Update (ItemSync)</span></span>](update-itemsync.md) <br/> |<span data-ttu-id="d23e0-252">Определяет один элемент для обновления в локальном хранилище клиента.</span><span class="sxs-lookup"><span data-stu-id="d23e0-252">Identifies a single item to update in the local client store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="d23e0-253">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="d23e0-253">Text value</span></span>

<span data-ttu-id="d23e0-254">Нет.</span><span class="sxs-lookup"><span data-stu-id="d23e0-254">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="d23e0-255">Примечания</span><span class="sxs-lookup"><span data-stu-id="d23e0-255">Remarks</span></span>

<span data-ttu-id="d23e0-256">Другой элемент **Message** , [Message (Availability)](message-availability.md) используется операциями доступности для возврата сообщений об отсутствии на работе.</span><span class="sxs-lookup"><span data-stu-id="d23e0-256">Another **Message** element, [Message (Availability)](message-availability.md) is used by the Availability operations to return OOF messages.</span></span> 
  
<span data-ttu-id="d23e0-257">Элементы [Message](message-ex15websvcsotherref.md) представляют сообщения электронной почты и все другие элементы, которые не являются строго типизированными схемой веб-служб Exchange (EWS).</span><span class="sxs-lookup"><span data-stu-id="d23e0-257">[Message](message-ex15websvcsotherref.md) elements represent e-mail messages and all other items that are not strongly typed by the Exchange Web Services (EWS) schema.</span></span> <span data-ttu-id="d23e0-258">Элементы, такие как IPM. Общий доступ и IPM. InfoPath возвращаются в виде элементов **Message** .</span><span class="sxs-lookup"><span data-stu-id="d23e0-258">Items such as IPM.Sharing and IPM.InfoPath are returned as **Message** elements.</span></span> <span data-ttu-id="d23e0-259">Exchange 2010 не возвращает элемент базового **элемента** в ответах.</span><span class="sxs-lookup"><span data-stu-id="d23e0-259">Exchange 2010 does not return the base **Item** element in responses.</span></span> 
  
<span data-ttu-id="d23e0-260">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="d23e0-260">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d23e0-261">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="d23e0-261">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d23e0-262">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="d23e0-262">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d23e0-263">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="d23e0-263">Schema Name</span></span>  <br/> |<span data-ttu-id="d23e0-264">Схема Types</span><span class="sxs-lookup"><span data-stu-id="d23e0-264">Types schema</span></span>  <br/> |
|<span data-ttu-id="d23e0-265">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="d23e0-265">Validation File</span></span>  <br/> |<span data-ttu-id="d23e0-266">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="d23e0-266">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d23e0-267">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="d23e0-267">Can be Empty</span></span>  <br/> |<span data-ttu-id="d23e0-268">False</span><span class="sxs-lookup"><span data-stu-id="d23e0-268">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d23e0-269">См. также</span><span class="sxs-lookup"><span data-stu-id="d23e0-269">See also</span></span>



- [<span data-ttu-id="d23e0-270">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="d23e0-270">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

