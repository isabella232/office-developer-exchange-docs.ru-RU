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
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467783"
---
# <a name="message"></a><span data-ttu-id="5f7b7-103">Сообщение</span><span class="sxs-lookup"><span data-stu-id="5f7b7-103">Message</span></span>

<span data-ttu-id="5f7b7-104">Элемент **Message** представляет сообщение электронной почты Microsoft Exchange.</span><span class="sxs-lookup"><span data-stu-id="5f7b7-104">The **Message** element represents a Microsoft Exchange e-mail message.</span></span> 
  
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

 <span data-ttu-id="5f7b7-105">**MessageType**</span><span class="sxs-lookup"><span data-stu-id="5f7b7-105">**MessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5f7b7-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="5f7b7-106">Attributes and elements</span></span>

<span data-ttu-id="5f7b7-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="5f7b7-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5f7b7-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="5f7b7-108">Attributes</span></span>

<span data-ttu-id="5f7b7-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="5f7b7-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5f7b7-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="5f7b7-110">Child elements</span></span>

|<span data-ttu-id="5f7b7-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="5f7b7-111">**Element**</span></span>|<span data-ttu-id="5f7b7-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="5f7b7-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5f7b7-113">Сохранитьmimecontent</span><span class="sxs-lookup"><span data-stu-id="5f7b7-113">MimeContent</span></span>](mimecontent.md) <br/> |<span data-ttu-id="5f7b7-114">Содержит собственный многоцелевой поток расширений почты в Интернете (MIME) объекта, представленного в формате base64Binary.</span><span class="sxs-lookup"><span data-stu-id="5f7b7-114">Contains the native Multipurpose Internet Mail Extensions (MIME) stream of an object that is represented in base64Binary format.</span></span>  <br/> |
|[<span data-ttu-id="5f7b7-115">Идентификатор</span><span class="sxs-lookup"><span data-stu-id="5f7b7-115">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="5f7b7-116">Содержит уникальный идентификатор и ключ изменения элемента в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="5f7b7-116">Contains the unique identifier and change key of an item in the Exchange store.</span></span> <span data-ttu-id="5f7b7-117">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5f7b7-117">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="5f7b7-118">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="5f7b7-118">ParentFolderId</span></span>](parentfolderid.md) <br/> |<span data-ttu-id="5f7b7-119">Представляет идентификатор родительской папки, содержащей элемент или папку.</span><span class="sxs-lookup"><span data-stu-id="5f7b7-119">Represents the identifier of the parent folder that contains the item or folder.</span></span> <span data-ttu-id="5f7b7-120">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5f7b7-120">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="5f7b7-121">ItemClass</span><span class="sxs-lookup"><span data-stu-id="5f7b7-121">ItemClass</span></span>](itemclass.md) <br/> |<span data-ttu-id="5f7b7-122">Представляет класс сообщения для элемента.</span><span class="sxs-lookup"><span data-stu-id="5f7b7-122">Represents the message class of an item.</span></span>  <br/> |
|[<span data-ttu-id="5f7b7-123">Тема</span><span class="sxs-lookup"><span data-stu-id="5f7b7-123">Subject</span></span>](subject.md) <br/> |<span data-ttu-id="5f7b7-124">Представляет тему для элементов хранилища Exchange и объектов ответа.</span><span class="sxs-lookup"><span data-stu-id="5f7b7-124">Represents the subject for Exchange store items and response objects.</span></span> <span data-ttu-id="5f7b7-125">Тема может иметь не более 255 символов.</span><span class="sxs-lookup"><span data-stu-id="5f7b7-125">The subject is limited to 255 characters.</span></span>  <br/> |
|[<span data-ttu-id="5f7b7-126">Sensitivity</span><span class="sxs-lookup"><span data-stu-id="5f7b7-126">Sensitivity</span></span>](sensitivity.md) <br/> |<span data-ttu-id="5f7b7-127">Указывает уровень конфиденциальности элемента.</span><span class="sxs-lookup"><span data-stu-id="5f7b7-127">Indicates the sensitivity level of an item.</span></span>  <br/> |
|[<span data-ttu-id="5f7b7-128">Body</span><span class="sxs-lookup"><span data-stu-id="5f7b7-128">Body</span></span>](body.md) <br/> |<span data-ttu-id="5f7b7-129">Представляет реальное содержимое основного текста сообщения.</span><span class="sxs-lookup"><span data-stu-id="5f7b7-129">Represents the actual body content of a message.</span></span>  <br/> |
|[<span data-ttu-id="5f7b7-130">Вложения</span><span class="sxs-lookup"><span data-stu-id="5f7b7-130">Attachments</span></span>](attachments-ex15websvcsotherref.md) <br/> |<span data-ttu-id="5f7b7-131">Содержит элементы или файлы, вложенные в элемент в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="5f7b7-131">Contains the items or files that are attached to an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="5f7b7-132">DateTimeReceived</span><span class="sxs-lookup"><span data-stu-id="5f7b7-132">DateTimeReceived</span></span>](datetimereceived.md) <br/> |<span data-ttu-id="5f7b7-133">Представляет дату и время получения элемента в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="5f7b7-133">Represents the date and time that an item in a mailbox was received.</span></span>  <br/> |
|[<span data-ttu-id="5f7b7-134">Размер</span><span class="sxs-lookup"><span data-stu-id="5f7b7-134">Size</span></span>](size.md) <br/> |<span data-ttu-id="5f7b7-135">Представляет размер элемента в байтах.</span><span class="sxs-lookup"><span data-stu-id="5f7b7-135">Represents the size in bytes of an item.</span></span> <span data-ttu-id="5f7b7-136">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5f7b7-136">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="5f7b7-137">Категории</span><span class="sxs-lookup"><span data-stu-id="5f7b7-137">Categories</span></span>](categories-ex15websvcsotherref.md) <br/> |<span data-ttu-id="5f7b7-138">Представляет коллекцию строк, определяющих, к каким категориям принадлежит элемент в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="5f7b7-138">Represents a collection of strings that identify to which categories an item in the mailbox belongs.</span></span>  <br/> |
|[<span data-ttu-id="5f7b7-139">Importance</span><span class="sxs-lookup"><span data-stu-id="5f7b7-139">Importance</span></span>](importance.md) <br/> |<span data-ttu-id="5f7b7-140">Описывает важность элемента.</span><span class="sxs-lookup"><span data-stu-id="5f7b7-140">Describes the importance of an item.</span></span>  <br/> |
|[<span data-ttu-id="5f7b7-141">инреплито</span><span class="sxs-lookup"><span data-stu-id="5f7b7-141">InReplyTo</span></span>](inreplyto.md) <br/> |<span data-ttu-id="5f7b7-142">Представляет идентификатор элемента, который является ответом на этот элемент.</span><span class="sxs-lookup"><span data-stu-id="5f7b7-142">Represents the identifier of the item to which this item is a reply.</span></span>  <br/> |
|[<span data-ttu-id="5f7b7-143">Отправлено</span><span class="sxs-lookup"><span data-stu-id="5f7b7-143">IsSubmitted</span></span>](issubmitted.md) <br/> |<span data-ttu-id="5f7b7-144">Указывает, был ли элемент отправлен в папку "Исходящие" по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="5f7b7-144">Indicates whether an item has been submitted to the Outbox default folder.</span></span>  <br/> |
|[<span data-ttu-id="5f7b7-145">Черновик</span><span class="sxs-lookup"><span data-stu-id="5f7b7-145">IsDraft</span></span>](isdraft.md) <br/> |<span data-ttu-id="5f7b7-146">Указывает, был ли элемент еще не отправлен.</span><span class="sxs-lookup"><span data-stu-id="5f7b7-146">Represents whether an item has not yet been sent.</span></span>  <br/> |
|[<span data-ttu-id="5f7b7-147">исфромме</span><span class="sxs-lookup"><span data-stu-id="5f7b7-147">IsFromMe</span></span>](isfromme.md) <br/> |<span data-ttu-id="5f7b7-148">Указывает, отправляет ли пользователь элемент.</span><span class="sxs-lookup"><span data-stu-id="5f7b7-148">Indicates whether a user sent an item to him or herself.</span></span>  <br/> |
|[<span data-ttu-id="5f7b7-149">исресенд</span><span class="sxs-lookup"><span data-stu-id="5f7b7-149">IsResend</span></span>](isresend.md) <br/> |<span data-ttu-id="5f7b7-150">Указывает, был ли ранее отправлен элемент.</span><span class="sxs-lookup"><span data-stu-id="5f7b7-150">Indicates whether the item had previously been sent.</span></span>  <br/> |
|[<span data-ttu-id="5f7b7-151">исунмодифиед</span><span class="sxs-lookup"><span data-stu-id="5f7b7-151">IsUnmodified</span></span>](isunmodified.md) <br/> |<span data-ttu-id="5f7b7-152">Указывает, был ли изменен элемент.</span><span class="sxs-lookup"><span data-stu-id="5f7b7-152">Indicates whether the item has been modified.</span></span>  <br/> |
|[<span data-ttu-id="5f7b7-153">InternetMessageHeaders</span><span class="sxs-lookup"><span data-stu-id="5f7b7-153">InternetMessageHeaders</span></span>](internetmessageheaders.md) <br/> |<span data-ttu-id="5f7b7-154">Представляет коллекцию всех заголовков сообщений Интернета, содержащихся в элементе почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="5f7b7-154">Represents the collection of all Internet message headers that are contained within an item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="5f7b7-155">датетимесент</span><span class="sxs-lookup"><span data-stu-id="5f7b7-155">DateTimeSent</span></span>](datetimesent.md) <br/> |<span data-ttu-id="5f7b7-156">Представляет дату и время отправки элемента в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="5f7b7-156">Represents the date and time that an item in a mailbox was sent.</span></span>  <br/> |
|[<span data-ttu-id="5f7b7-157">DateTimeCreated</span><span class="sxs-lookup"><span data-stu-id="5f7b7-157">DateTimeCreated</span></span>](datetimecreated.md) <br/> |<span data-ttu-id="5f7b7-158">Представляет дату и время создания определенного элемента в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="5f7b7-158">Represents the date and time that a given item in the mailbox was created.</span></span>  <br/> |
|[<span data-ttu-id="5f7b7-159">респонсеобжектс</span><span class="sxs-lookup"><span data-stu-id="5f7b7-159">ResponseObjects</span></span>](responseobjects.md) <br/> |<span data-ttu-id="5f7b7-160">Содержит коллекцию всех объектов ответа, связанных с элементом в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="5f7b7-160">Contains a collection of all the response objects that are associated with an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="5f7b7-161">реминдердуеби</span><span class="sxs-lookup"><span data-stu-id="5f7b7-161">ReminderDueBy</span></span>](reminderdueby.md) <br/> |<span data-ttu-id="5f7b7-162">Представляет дату и время возникновения события.</span><span class="sxs-lookup"><span data-stu-id="5f7b7-162">Represents the date and time when the event occurs.</span></span> <span data-ttu-id="5f7b7-163">Он используется элементом [реминдерминутесбефорестарт](reminderminutesbeforestart.md) для определения времени отображения напоминания.</span><span class="sxs-lookup"><span data-stu-id="5f7b7-163">This is used by the [ReminderMinutesBeforeStart](reminderminutesbeforestart.md) element to determine when the reminder is displayed.</span></span>  <br/> |
|[<span data-ttu-id="5f7b7-164">реминдериссет</span><span class="sxs-lookup"><span data-stu-id="5f7b7-164">ReminderIsSet</span></span>](reminderisset.md) <br/> |<span data-ttu-id="5f7b7-165">Указывает, задано ли напоминание для элемента в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="5f7b7-165">Indicates whether a reminder has been set for an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="5f7b7-166">ReminderMinutesBeforeStart</span><span class="sxs-lookup"><span data-stu-id="5f7b7-166">ReminderMinutesBeforeStart</span></span>](reminderminutesbeforestart.md) <br/> |<span data-ttu-id="5f7b7-167">Представляет количество минут до события при отображении напоминания.</span><span class="sxs-lookup"><span data-stu-id="5f7b7-167">Represents the number of minutes before an event when a reminder is displayed.</span></span>  <br/> |
|[<span data-ttu-id="5f7b7-168">дисплайкк</span><span class="sxs-lookup"><span data-stu-id="5f7b7-168">DisplayCc</span></span>](displaycc.md) <br/> |<span data-ttu-id="5f7b7-169">Представляет отображаемую строку, используемую для содержимого строки "копия".</span><span class="sxs-lookup"><span data-stu-id="5f7b7-169">Represents the display string that is used for the contents of the CC line.</span></span> <span data-ttu-id="5f7b7-170">Это объединенная строка всех отображаемых имен получателей копии.</span><span class="sxs-lookup"><span data-stu-id="5f7b7-170">This is the concatenated string of all CC recipient display names.</span></span>  <br/> |
|[<span data-ttu-id="5f7b7-171">дисплайто</span><span class="sxs-lookup"><span data-stu-id="5f7b7-171">DisplayTo</span></span>](displayto.md) <br/> |<span data-ttu-id="5f7b7-172">Представляет отображаемую строку, используемую для содержимого поля "Кому".</span><span class="sxs-lookup"><span data-stu-id="5f7b7-172">Represents the display string that is used for the contents of the To box.</span></span> <span data-ttu-id="5f7b7-173">Это объединенная строка для отображаемых имен получателей.</span><span class="sxs-lookup"><span data-stu-id="5f7b7-173">This is the concatenated string of all To recipient display names.</span></span>  <br/> |
|[<span data-ttu-id="5f7b7-174">HasAttachments</span><span class="sxs-lookup"><span data-stu-id="5f7b7-174">HasAttachments</span></span>](hasattachments.md) <br/> |<span data-ttu-id="5f7b7-175">Представляет свойство, для которого задано значение **true** , если элемент имеет по крайней мере одно видимое вложение.</span><span class="sxs-lookup"><span data-stu-id="5f7b7-175">Represents a property that is set to **true** if an item has at least one visible attachment.</span></span> <span data-ttu-id="5f7b7-176">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5f7b7-176">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="5f7b7-177">ExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="5f7b7-177">ExtendedProperty</span></span>](extendedproperty.md) <br/> |<span data-ttu-id="5f7b7-178">Определяет расширенные свойства для папок и элементов.</span><span class="sxs-lookup"><span data-stu-id="5f7b7-178">Identifies extended properties on folders and items.</span></span>  <br/> |
|[<span data-ttu-id="5f7b7-179">Culture</span><span class="sxs-lookup"><span data-stu-id="5f7b7-179">Culture</span></span>](culture.md) <br/> |<span data-ttu-id="5f7b7-180">Представляет язык и региональные параметры для определенного элемента в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="5f7b7-180">Represents the culture for a given item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="5f7b7-181">Sender</span><span class="sxs-lookup"><span data-stu-id="5f7b7-181">Sender</span></span>](sender.md) <br/> |<span data-ttu-id="5f7b7-182">Определяет отправителя элемента.</span><span class="sxs-lookup"><span data-stu-id="5f7b7-182">Identifies the sender of an item.</span></span>  <br/> |
|[<span data-ttu-id="5f7b7-183">ToRecipients</span><span class="sxs-lookup"><span data-stu-id="5f7b7-183">ToRecipients</span></span>](torecipients.md) <br/> |<span data-ttu-id="5f7b7-184">Содержит набор получателей сообщения.</span><span class="sxs-lookup"><span data-stu-id="5f7b7-184">Contains a set of recipients of a message.</span></span>  <br/> |
|[<span data-ttu-id="5f7b7-185">CcRecipients</span><span class="sxs-lookup"><span data-stu-id="5f7b7-185">CcRecipients</span></span>](ccrecipients.md) <br/> |<span data-ttu-id="5f7b7-186">Представляет коллекцию получателей, которые будут получать копию сообщения.</span><span class="sxs-lookup"><span data-stu-id="5f7b7-186">Represents a collection of recipients that will receive a copy of the message.</span></span>  <br/> |
|[<span data-ttu-id="5f7b7-187">BccRecipients</span><span class="sxs-lookup"><span data-stu-id="5f7b7-187">BccRecipients</span></span>](bccrecipients.md) <br/> |<span data-ttu-id="5f7b7-188">Представляет коллекцию получателей для получения скрытой копии (BCC) сообщения электронной почты.</span><span class="sxs-lookup"><span data-stu-id="5f7b7-188">Represents a collection of recipients to receive a blind carbon copy (Bcc) of an e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="5f7b7-189">исреадрецеиптрекуестед</span><span class="sxs-lookup"><span data-stu-id="5f7b7-189">IsReadReceiptRequested</span></span>](isreadreceiptrequested.md) <br/> |<span data-ttu-id="5f7b7-190">Указывает, запрашивает ли отправитель элемента уведомление о прочтении.</span><span class="sxs-lookup"><span data-stu-id="5f7b7-190">Indicates whether the sender of an item requests a read receipt.</span></span>  <br/> |
|[<span data-ttu-id="5f7b7-191">исделиверирецеиптрекуестед</span><span class="sxs-lookup"><span data-stu-id="5f7b7-191">IsDeliveryReceiptRequested</span></span>](isdeliveryreceiptrequested.md) <br/> |<span data-ttu-id="5f7b7-192">Указывает, запрашивает ли отправитель элемента уведомление о доставке.</span><span class="sxs-lookup"><span data-stu-id="5f7b7-192">Indicates whether the sender of an item requests a delivery receipt.</span></span>  <br/> |
|[<span data-ttu-id="5f7b7-193">ConversationIndex</span><span class="sxs-lookup"><span data-stu-id="5f7b7-193">ConversationIndex</span></span>](conversationindex.md) <br/> |<span data-ttu-id="5f7b7-194">Содержит двоичный код, представляющий поток, к которому относится сообщение.</span><span class="sxs-lookup"><span data-stu-id="5f7b7-194">Contains a binary ID that represents the thread to which this message belongs.</span></span>  <br/> |
|[<span data-ttu-id="5f7b7-195">ConversationTopic</span><span class="sxs-lookup"><span data-stu-id="5f7b7-195">ConversationTopic</span></span>](conversationtopic.md) <br/> |<span data-ttu-id="5f7b7-196">Представляет идентификатор беседы.</span><span class="sxs-lookup"><span data-stu-id="5f7b7-196">Represents the conversation identifier.</span></span>  <br/> |
|[<span data-ttu-id="5f7b7-197">From</span><span class="sxs-lookup"><span data-stu-id="5f7b7-197">From</span></span>](from.md) <br/> |<span data-ttu-id="5f7b7-198">Представляет адрес получателя, от которого было отправлено сообщение.</span><span class="sxs-lookup"><span data-stu-id="5f7b7-198">Represents the addressee from whom the message was sent.</span></span>  <br/> |
|[<span data-ttu-id="5f7b7-199">InternetMessageId</span><span class="sxs-lookup"><span data-stu-id="5f7b7-199">InternetMessageId</span></span>](internetmessageid.md) <br/> |<span data-ttu-id="5f7b7-200">Представляет идентификатор сообщения Интернета для элемента.</span><span class="sxs-lookup"><span data-stu-id="5f7b7-200">Represents the Internet message identifier of an item.</span></span>  <br/> |
|[<span data-ttu-id="5f7b7-201">IsRead</span><span class="sxs-lookup"><span data-stu-id="5f7b7-201">IsRead</span></span>](isread.md) <br/> |<span data-ttu-id="5f7b7-202">Указывает, было ли Прочитано сообщение.</span><span class="sxs-lookup"><span data-stu-id="5f7b7-202">Indicates whether a message has been read.</span></span>  <br/> |
|[<span data-ttu-id="5f7b7-203">исреспонсерекуестед</span><span class="sxs-lookup"><span data-stu-id="5f7b7-203">IsResponseRequested</span></span>](isresponserequested.md) <br/> |<span data-ttu-id="5f7b7-204">Указывает, запрашивается ли ответ на сообщение электронной почты.</span><span class="sxs-lookup"><span data-stu-id="5f7b7-204">Indicates whether a response to an e-mail message is requested.</span></span>  <br/> |
|[<span data-ttu-id="5f7b7-205">References</span><span class="sxs-lookup"><span data-stu-id="5f7b7-205">References</span></span>](references.md) <br/> |<span data-ttu-id="5f7b7-206">Представляет заголовок Usenet, используемый для сопоставления ответов с их исходными сообщениями.</span><span class="sxs-lookup"><span data-stu-id="5f7b7-206">Represents the Usenet header that is used to correlate replies with their original messages.</span></span>  <br/> |
|[<span data-ttu-id="5f7b7-207">ReplyTo</span><span class="sxs-lookup"><span data-stu-id="5f7b7-207">ReplyTo</span></span>](replyto.md) <br/> |<span data-ttu-id="5f7b7-208">Определяет набор адресов, в который отправляются ответы.</span><span class="sxs-lookup"><span data-stu-id="5f7b7-208">Identifies a set of addresses to which replies should be sent.</span></span>  <br/> |
|[<span data-ttu-id="5f7b7-209">еффективеригхтс</span><span class="sxs-lookup"><span data-stu-id="5f7b7-209">EffectiveRights</span></span>](effectiverights.md) <br/> |<span data-ttu-id="5f7b7-210">Содержит права клиента на основе параметров разрешений для элемента или папки.</span><span class="sxs-lookup"><span data-stu-id="5f7b7-210">Contains the client's rights based on the permission settings for the item or folder.</span></span> <span data-ttu-id="5f7b7-211">Этот элемент доступен только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5f7b7-211">This element is read-only.</span></span>  <br/> |
|[<span data-ttu-id="5f7b7-212">рецеиведби</span><span class="sxs-lookup"><span data-stu-id="5f7b7-212">ReceivedBy</span></span>](receivedby.md) <br/> |<span data-ttu-id="5f7b7-213">Определяет делегат в сценарии доступа делегата.</span><span class="sxs-lookup"><span data-stu-id="5f7b7-213">Identifies the delegate in a delegate access scenario.</span></span>  <br/> |
|[<span data-ttu-id="5f7b7-214">рецеиведрепресентинг</span><span class="sxs-lookup"><span data-stu-id="5f7b7-214">ReceivedRepresenting</span></span>](receivedrepresenting.md) <br/> |<span data-ttu-id="5f7b7-215">Определяет участника в сценарии доступа делегата.</span><span class="sxs-lookup"><span data-stu-id="5f7b7-215">Identifies the principal in a delegate access scenario.</span></span>  <br/> |
|[<span data-ttu-id="5f7b7-216">ластмодифиеднаме</span><span class="sxs-lookup"><span data-stu-id="5f7b7-216">LastModifiedName</span></span>](lastmodifiedname.md) <br/> |<span data-ttu-id="5f7b7-217">Содержит отображаемое имя последнего пользователя для изменения элемента.</span><span class="sxs-lookup"><span data-stu-id="5f7b7-217">Contains the display name of the last user to modify an item.</span></span>  <br/> |
|[<span data-ttu-id="5f7b7-218">LastModifiedTime</span><span class="sxs-lookup"><span data-stu-id="5f7b7-218">LastModifiedTime</span></span>](lastmodifiedtime.md) <br/> |<span data-ttu-id="5f7b7-219">Указывает время последнего изменения элемента.</span><span class="sxs-lookup"><span data-stu-id="5f7b7-219">Indicates when an item was last modified.</span></span>  <br/> |
|[<span data-ttu-id="5f7b7-220">Связанный</span><span class="sxs-lookup"><span data-stu-id="5f7b7-220">IsAssociated</span></span>](isassociated.md) <br/> |<span data-ttu-id="5f7b7-221">Указывает, связан ли элемент с папкой.</span><span class="sxs-lookup"><span data-stu-id="5f7b7-221">Indicates whether the item is associated with a folder.</span></span>  <br/> |
|[<span data-ttu-id="5f7b7-222">вебклиентреадформкуеристринг</span><span class="sxs-lookup"><span data-stu-id="5f7b7-222">WebClientReadFormQueryString</span></span>](webclientreadformquerystring.md) <br/> |<span data-ttu-id="5f7b7-223">Представляет URL-адрес для сцепления с конечной точкой Microsoft Office Outlook Web App для чтения элемента в Outlook Web App.</span><span class="sxs-lookup"><span data-stu-id="5f7b7-223">Represents a URL to concatenate to the Microsoft Office Outlook Web App endpoint to read an item in Outlook Web App.</span></span>  <br/> |
|[<span data-ttu-id="5f7b7-224">вебклиентедитформкуеристринг</span><span class="sxs-lookup"><span data-stu-id="5f7b7-224">WebClientEditFormQueryString</span></span>](webclienteditformquerystring.md) <br/> |<span data-ttu-id="5f7b7-225">Представляет URL-адрес для сцепления с конечной точкой Outlook Web App для изменения элемента в Outlook Web App.</span><span class="sxs-lookup"><span data-stu-id="5f7b7-225">Represents a URL to concatenate to the Outlook Web App endpoint to edit an item in Outlook Web App.</span></span>  <br/> |
|[<span data-ttu-id="5f7b7-226">ConversationId</span><span class="sxs-lookup"><span data-stu-id="5f7b7-226">ConversationId</span></span>](conversationid.md) <br/> |<span data-ttu-id="5f7b7-227">Содержит идентификатор элемента или беседы.</span><span class="sxs-lookup"><span data-stu-id="5f7b7-227">Contains the identifier of an item or conversation.</span></span>  <br/> |
|[<span data-ttu-id="5f7b7-228">UniqueBody</span><span class="sxs-lookup"><span data-stu-id="5f7b7-228">UniqueBody</span></span>](uniquebody.md) <br/> |<span data-ttu-id="5f7b7-229">Представляет фрагмент HTML или обычный текст, представляющий уникальный основной текст этой беседы.</span><span class="sxs-lookup"><span data-stu-id="5f7b7-229">Represents an HTML fragment or plain text which represents the unique body of this conversation.</span></span>  <br/> |
|[<span data-ttu-id="5f7b7-230">реминдермессажедата</span><span class="sxs-lookup"><span data-stu-id="5f7b7-230">ReminderMessageData</span></span>](remindermessagedata.md) <br/> |<span data-ttu-id="5f7b7-231">Содержит данные для сообщения напоминания.</span><span class="sxs-lookup"><span data-stu-id="5f7b7-231">Contains the data for a reminder message.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="5f7b7-232">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="5f7b7-232">Parent elements</span></span>

|<span data-ttu-id="5f7b7-233">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="5f7b7-233">**Element**</span></span>|<span data-ttu-id="5f7b7-234">**Описание**</span><span class="sxs-lookup"><span data-stu-id="5f7b7-234">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5f7b7-235">аджацентмитингс</span><span class="sxs-lookup"><span data-stu-id="5f7b7-235">AdjacentMeetings</span></span>](adjacentmeetings.md) <br/> |<span data-ttu-id="5f7b7-236">Описывает все элементы календаря, смежные с временем собрания.</span><span class="sxs-lookup"><span data-stu-id="5f7b7-236">Describes all calendar items that are adjacent to a meeting time.</span></span>  <br/> |
|[<span data-ttu-id="5f7b7-237">аппендтоитемфиелд</span><span class="sxs-lookup"><span data-stu-id="5f7b7-237">AppendToItemField</span></span>](appendtoitemfield.md) <br/> |<span data-ttu-id="5f7b7-238">Определяет данные, добавляемые к одному свойству элемента во время [операции UpdateItem](updateitem-operation.md).</span><span class="sxs-lookup"><span data-stu-id="5f7b7-238">Identifies data to append to a single property of an item during an [UpdateItem operation](updateitem-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="5f7b7-239">конфликтингмитингс</span><span class="sxs-lookup"><span data-stu-id="5f7b7-239">ConflictingMeetings</span></span>](conflictingmeetings.md) <br/> |<span data-ttu-id="5f7b7-240">Определяет все элементы, которые конфликтуют с временем собрания.</span><span class="sxs-lookup"><span data-stu-id="5f7b7-240">Identifies all items that conflict with a meeting time.</span></span>  <br/> |
|[<span data-ttu-id="5f7b7-241">Create (Итемсинк)</span><span class="sxs-lookup"><span data-stu-id="5f7b7-241">Create (ItemSync)</span></span>](create-itemsync.md) <br/> |<span data-ttu-id="5f7b7-242">Определяет один элемент, который необходимо создать в локальном хранилище клиента.</span><span class="sxs-lookup"><span data-stu-id="5f7b7-242">Identifies a single item to create in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="5f7b7-243">ItemAttachment</span><span class="sxs-lookup"><span data-stu-id="5f7b7-243">ItemAttachment</span></span>](itemattachment.md) <br/> |<span data-ttu-id="5f7b7-244">Представляет элемент Exchange, присоединенный к другому элементу Exchange.</span><span class="sxs-lookup"><span data-stu-id="5f7b7-244">Represents an Exchange item that is attached to another Exchange item.</span></span>  <br/> |
|[<span data-ttu-id="5f7b7-245">Items</span><span class="sxs-lookup"><span data-stu-id="5f7b7-245">Items</span></span>](items.md) <br/> |<span data-ttu-id="5f7b7-246">Содержит массив элементов.</span><span class="sxs-lookup"><span data-stu-id="5f7b7-246">Contains an array of items.</span></span>  <br/> |
|[<span data-ttu-id="5f7b7-247">Элементы (Нонемптяррайофаллитемстипе)</span><span class="sxs-lookup"><span data-stu-id="5f7b7-247">Items (NonEmptyArrayOfAllItemsType)</span></span>](items-nonemptyarrayofallitemstype.md) <br/> |<span data-ttu-id="5f7b7-248">Содержит массив элементов для создания в папке, определяемой элементом [ParentFolderId (таржетфолдеридтипе)](parentfolderid-targetfolderidtype.md) .</span><span class="sxs-lookup"><span data-stu-id="5f7b7-248">Contains an array of items to create in the folder that is identified by the [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) element.</span></span>  <br/> |
|[<span data-ttu-id="5f7b7-249">сетитемфиелд</span><span class="sxs-lookup"><span data-stu-id="5f7b7-249">SetItemField</span></span>](setitemfield.md) <br/> |<span data-ttu-id="5f7b7-250">Представляет обновление одного свойства элемента в [операции UpdateItem](updateitem-operation.md).</span><span class="sxs-lookup"><span data-stu-id="5f7b7-250">Represents an update to a single property of an item in an [UpdateItem operation](updateitem-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="5f7b7-251">Обновление (Итемсинк)</span><span class="sxs-lookup"><span data-stu-id="5f7b7-251">Update (ItemSync)</span></span>](update-itemsync.md) <br/> |<span data-ttu-id="5f7b7-252">Определяет один элемент для обновления в локальном хранилище клиента.</span><span class="sxs-lookup"><span data-stu-id="5f7b7-252">Identifies a single item to update in the local client store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="5f7b7-253">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="5f7b7-253">Text value</span></span>

<span data-ttu-id="5f7b7-254">Нет.</span><span class="sxs-lookup"><span data-stu-id="5f7b7-254">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="5f7b7-255">Примечания</span><span class="sxs-lookup"><span data-stu-id="5f7b7-255">Remarks</span></span>

<span data-ttu-id="5f7b7-256">Другой элемент **Message** , [Message (Availability)](message-availability.md) используется операциями доступности для возврата сообщений об отсутствии на работе.</span><span class="sxs-lookup"><span data-stu-id="5f7b7-256">Another **Message** element, [Message (Availability)](message-availability.md) is used by the Availability operations to return OOF messages.</span></span> 
  
<span data-ttu-id="5f7b7-257">Элементы [Message](message-ex15websvcsotherref.md) представляют сообщения электронной почты и все другие элементы, которые не являются строго типизированными схемой веб-служб Exchange (EWS).</span><span class="sxs-lookup"><span data-stu-id="5f7b7-257">[Message](message-ex15websvcsotherref.md) elements represent e-mail messages and all other items that are not strongly typed by the Exchange Web Services (EWS) schema.</span></span> <span data-ttu-id="5f7b7-258">Элементы, такие как IPM. Общий доступ и IPM. InfoPath возвращаются в виде элементов **Message** .</span><span class="sxs-lookup"><span data-stu-id="5f7b7-258">Items such as IPM.Sharing and IPM.InfoPath are returned as **Message** elements.</span></span> <span data-ttu-id="5f7b7-259">Exchange 2010 не возвращает элемент базового **элемента** в ответах.</span><span class="sxs-lookup"><span data-stu-id="5f7b7-259">Exchange 2010 does not return the base **Item** element in responses.</span></span> 
  
<span data-ttu-id="5f7b7-260">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="5f7b7-260">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5f7b7-261">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="5f7b7-261">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5f7b7-262">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="5f7b7-262">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="5f7b7-263">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="5f7b7-263">Schema Name</span></span>  <br/> |<span data-ttu-id="5f7b7-264">Схема Types</span><span class="sxs-lookup"><span data-stu-id="5f7b7-264">Types schema</span></span>  <br/> |
|<span data-ttu-id="5f7b7-265">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="5f7b7-265">Validation File</span></span>  <br/> |<span data-ttu-id="5f7b7-266">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="5f7b7-266">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="5f7b7-267">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="5f7b7-267">Can be Empty</span></span>  <br/> |<span data-ttu-id="5f7b7-268">False</span><span class="sxs-lookup"><span data-stu-id="5f7b7-268">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="5f7b7-269">См. также</span><span class="sxs-lookup"><span data-stu-id="5f7b7-269">See also</span></span>



- [<span data-ttu-id="5f7b7-270">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="5f7b7-270">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

