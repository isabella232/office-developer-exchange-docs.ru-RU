---
title: постреплитем
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
description: Элемент Постреплитем содержит ответ на элемент POST. Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).
ms.openlocfilehash: 4104e79449acc6e358b729cf2de769d28dac52bd
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44461683"
---
# <a name="postreplyitem"></a><span data-ttu-id="9b8d1-104">постреплитем</span><span class="sxs-lookup"><span data-stu-id="9b8d1-104">PostReplyItem</span></span>

<span data-ttu-id="9b8d1-105">Элемент **постреплитем** содержит ответ на элемент POST.</span><span class="sxs-lookup"><span data-stu-id="9b8d1-105">The **PostReplyItem** element contains a reply to a post item.</span></span> <span data-ttu-id="9b8d1-106">Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="9b8d1-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
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

 <span data-ttu-id="9b8d1-107">**постреплитемтипе**</span><span class="sxs-lookup"><span data-stu-id="9b8d1-107">**PostReplyItemType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9b8d1-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="9b8d1-108">Attributes and elements</span></span>

<span data-ttu-id="9b8d1-109">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="9b8d1-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9b8d1-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="9b8d1-110">Attributes</span></span>

<span data-ttu-id="9b8d1-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="9b8d1-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9b8d1-112">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="9b8d1-112">Child elements</span></span>

|<span data-ttu-id="9b8d1-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="9b8d1-113">**Element**</span></span>|<span data-ttu-id="9b8d1-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="9b8d1-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9b8d1-115">Сохранитьmimecontent</span><span class="sxs-lookup"><span data-stu-id="9b8d1-115">MimeContent</span></span>](mimecontent.md) <br/> |<span data-ttu-id="9b8d1-116">Содержит собственный многоцелевой поток расширений почты в Интернете (MIME) объекта, представленного в формате base64Binary.</span><span class="sxs-lookup"><span data-stu-id="9b8d1-116">Contains the native Multipurpose Internet Mail Extensions (MIME) stream of an object that is represented in base64Binary format.</span></span>  <br/> |
|[<span data-ttu-id="9b8d1-117">Идентификатор</span><span class="sxs-lookup"><span data-stu-id="9b8d1-117">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="9b8d1-118">Содержит уникальный идентификатор и ключ изменения элемента в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="9b8d1-118">Contains the unique identifier and change key of an item in the Exchange store.</span></span> <span data-ttu-id="9b8d1-119">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9b8d1-119">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="9b8d1-120">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="9b8d1-120">ParentFolderId</span></span>](parentfolderid.md) <br/> |<span data-ttu-id="9b8d1-121">Представляет идентификатор родительской папки, содержащей элемент или папку.</span><span class="sxs-lookup"><span data-stu-id="9b8d1-121">Represents the identifier of the parent folder that contains the item or folder.</span></span> <span data-ttu-id="9b8d1-122">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9b8d1-122">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="9b8d1-123">ItemClass</span><span class="sxs-lookup"><span data-stu-id="9b8d1-123">ItemClass</span></span>](itemclass.md) <br/> |<span data-ttu-id="9b8d1-124">Представляет класс сообщения для элемента.</span><span class="sxs-lookup"><span data-stu-id="9b8d1-124">Represents the message class of an item.</span></span>  <br/> |
|[<span data-ttu-id="9b8d1-125">Тема</span><span class="sxs-lookup"><span data-stu-id="9b8d1-125">Subject</span></span>](subject.md) <br/> |<span data-ttu-id="9b8d1-126">Представляет тему для элементов хранилища Exchange и объектов ответа.</span><span class="sxs-lookup"><span data-stu-id="9b8d1-126">Represents the subject for Exchange store items and response objects.</span></span> <span data-ttu-id="9b8d1-127">Тема может иметь не более 255 символов.</span><span class="sxs-lookup"><span data-stu-id="9b8d1-127">The subject is limited to 255 characters.</span></span>  <br/> |
|[<span data-ttu-id="9b8d1-128">Sensitivity</span><span class="sxs-lookup"><span data-stu-id="9b8d1-128">Sensitivity</span></span>](sensitivity.md) <br/> |<span data-ttu-id="9b8d1-129">Указывает уровень конфиденциальности элемента.</span><span class="sxs-lookup"><span data-stu-id="9b8d1-129">Indicates the sensitivity level of an item.</span></span>  <br/> |
|[<span data-ttu-id="9b8d1-130">Body</span><span class="sxs-lookup"><span data-stu-id="9b8d1-130">Body</span></span>](body.md) <br/> |<span data-ttu-id="9b8d1-131">Представляет реальное содержимое основного текста сообщения.</span><span class="sxs-lookup"><span data-stu-id="9b8d1-131">Represents the actual body content of a message.</span></span>  <br/> |
|[<span data-ttu-id="9b8d1-132">Вложения</span><span class="sxs-lookup"><span data-stu-id="9b8d1-132">Attachments</span></span>](attachments-ex15websvcsotherref.md) <br/> |<span data-ttu-id="9b8d1-133">Содержит элементы или файлы, вложенные в элемент в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="9b8d1-133">Contains the items or files that are attached to an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="9b8d1-134">DateTimeReceived</span><span class="sxs-lookup"><span data-stu-id="9b8d1-134">DateTimeReceived</span></span>](datetimereceived.md) <br/> |<span data-ttu-id="9b8d1-135">Представляет дату и время получения элемента в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="9b8d1-135">Represents the date and time that an item in a mailbox was received.</span></span>  <br/> |
|[<span data-ttu-id="9b8d1-136">Размер</span><span class="sxs-lookup"><span data-stu-id="9b8d1-136">Size</span></span>](size.md) <br/> |<span data-ttu-id="9b8d1-137">Представляет размер элемента в байтах.</span><span class="sxs-lookup"><span data-stu-id="9b8d1-137">Represents the size in bytes of an item.</span></span> <span data-ttu-id="9b8d1-138">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9b8d1-138">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="9b8d1-139">Категории</span><span class="sxs-lookup"><span data-stu-id="9b8d1-139">Categories</span></span>](categories-ex15websvcsotherref.md) <br/> |<span data-ttu-id="9b8d1-140">Представляет коллекцию строк, определяющих категории, к которым относится элемент в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="9b8d1-140">Represents a collection of strings that identify categories to which an item in the mailbox belongs.</span></span>  <br/> |
|[<span data-ttu-id="9b8d1-141">Importance</span><span class="sxs-lookup"><span data-stu-id="9b8d1-141">Importance</span></span>](importance.md) <br/> |<span data-ttu-id="9b8d1-142">Описывает важность элемента.</span><span class="sxs-lookup"><span data-stu-id="9b8d1-142">Describes the importance of an item.</span></span>  <br/> |
|[<span data-ttu-id="9b8d1-143">инреплито</span><span class="sxs-lookup"><span data-stu-id="9b8d1-143">InReplyTo</span></span>](inreplyto.md) <br/> |<span data-ttu-id="9b8d1-144">Представляет идентификатор элемента, который является ответом на этот элемент.</span><span class="sxs-lookup"><span data-stu-id="9b8d1-144">Represents the identifier of the item to which this item is a reply.</span></span>  <br/> |
|[<span data-ttu-id="9b8d1-145">Отправлено</span><span class="sxs-lookup"><span data-stu-id="9b8d1-145">IsSubmitted</span></span>](issubmitted.md) <br/> |<span data-ttu-id="9b8d1-146">Указывает, был ли элемент отправлен в папку "Исходящие" по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="9b8d1-146">Indicates whether an item has been submitted to the Outbox default folder.</span></span>  <br/> |
|[<span data-ttu-id="9b8d1-147">Черновик</span><span class="sxs-lookup"><span data-stu-id="9b8d1-147">IsDraft</span></span>](isdraft.md) <br/> |<span data-ttu-id="9b8d1-148">Указывает, был ли элемент еще не отправлен.</span><span class="sxs-lookup"><span data-stu-id="9b8d1-148">Represents whether an item has not yet been sent.</span></span>  <br/> |
|[<span data-ttu-id="9b8d1-149">исфромме</span><span class="sxs-lookup"><span data-stu-id="9b8d1-149">IsFromMe</span></span>](isfromme.md) <br/> |<span data-ttu-id="9b8d1-150">Указывает, отправляет ли пользователь элемент.</span><span class="sxs-lookup"><span data-stu-id="9b8d1-150">Indicates whether a user sent an item to him or herself.</span></span>  <br/> |
|[<span data-ttu-id="9b8d1-151">исресенд</span><span class="sxs-lookup"><span data-stu-id="9b8d1-151">IsResend</span></span>](isresend.md) <br/> |<span data-ttu-id="9b8d1-152">Указывает, был ли ранее отправлен элемент.</span><span class="sxs-lookup"><span data-stu-id="9b8d1-152">Indicates whether the item had previously been sent.</span></span>  <br/> |
|[<span data-ttu-id="9b8d1-153">исунмодифиед</span><span class="sxs-lookup"><span data-stu-id="9b8d1-153">IsUnmodified</span></span>](isunmodified.md) <br/> |<span data-ttu-id="9b8d1-154">Указывает, был ли изменен элемент.</span><span class="sxs-lookup"><span data-stu-id="9b8d1-154">Indicates whether the item has been modified.</span></span>  <br/> |
|[<span data-ttu-id="9b8d1-155">InternetMessageHeaders</span><span class="sxs-lookup"><span data-stu-id="9b8d1-155">InternetMessageHeaders</span></span>](internetmessageheaders.md) <br/> |<span data-ttu-id="9b8d1-156">Представляет коллекцию всех заголовков сообщений Интернета, которые находятся в элементе почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="9b8d1-156">Represents the collection of all Internet message headers that are contained in an item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="9b8d1-157">датетимесент</span><span class="sxs-lookup"><span data-stu-id="9b8d1-157">DateTimeSent</span></span>](datetimesent.md) <br/> |<span data-ttu-id="9b8d1-158">Представляет дату и время отправки элемента в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="9b8d1-158">Represents the date and time that an item in a mailbox was sent.</span></span>  <br/> |
|[<span data-ttu-id="9b8d1-159">DateTimeCreated</span><span class="sxs-lookup"><span data-stu-id="9b8d1-159">DateTimeCreated</span></span>](datetimecreated.md) <br/> |<span data-ttu-id="9b8d1-160">Представляет дату и время создания определенного элемента в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="9b8d1-160">Represents the date and time that a given item in the mailbox was created.</span></span>  <br/> |
|[<span data-ttu-id="9b8d1-161">респонсеобжектс</span><span class="sxs-lookup"><span data-stu-id="9b8d1-161">ResponseObjects</span></span>](responseobjects.md) <br/> |<span data-ttu-id="9b8d1-162">Содержит коллекцию всех объектов ответа, связанных с элементом в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="9b8d1-162">Contains a collection of all the response objects that are associated with an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="9b8d1-163">реминдердуеби</span><span class="sxs-lookup"><span data-stu-id="9b8d1-163">ReminderDueBy</span></span>](reminderdueby.md) <br/> |<span data-ttu-id="9b8d1-164">Представляет дату и время возникновения события.</span><span class="sxs-lookup"><span data-stu-id="9b8d1-164">Represents the date and time when the event occurs.</span></span> <span data-ttu-id="9b8d1-165">Он используется элементом [реминдерминутесбефорестарт](reminderminutesbeforestart.md) для определения времени отображения напоминания.</span><span class="sxs-lookup"><span data-stu-id="9b8d1-165">This is used by the [ReminderMinutesBeforeStart](reminderminutesbeforestart.md) element to determine when the reminder is displayed.</span></span>  <br/> |
|[<span data-ttu-id="9b8d1-166">реминдериссет</span><span class="sxs-lookup"><span data-stu-id="9b8d1-166">ReminderIsSet</span></span>](reminderisset.md) <br/> |<span data-ttu-id="9b8d1-167">Указывает, задано ли напоминание для элемента в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="9b8d1-167">Indicates whether a reminder has been set for an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="9b8d1-168">ReminderMinutesBeforeStart</span><span class="sxs-lookup"><span data-stu-id="9b8d1-168">ReminderMinutesBeforeStart</span></span>](reminderminutesbeforestart.md) <br/> |<span data-ttu-id="9b8d1-169">Представляет количество минут до события при отображении напоминания.</span><span class="sxs-lookup"><span data-stu-id="9b8d1-169">Represents the number of minutes before an event when a reminder is displayed.</span></span>  <br/> |
|[<span data-ttu-id="9b8d1-170">дисплайкк</span><span class="sxs-lookup"><span data-stu-id="9b8d1-170">DisplayCc</span></span>](displaycc.md) <br/> |<span data-ttu-id="9b8d1-171">Представляет отображаемую строку, используемую для содержимого строки "копия".</span><span class="sxs-lookup"><span data-stu-id="9b8d1-171">Represents the display string that is used for the contents of the Cc line.</span></span> <span data-ttu-id="9b8d1-172">Это объединенная строка всех отображаемых имен получателей копии.</span><span class="sxs-lookup"><span data-stu-id="9b8d1-172">This is the concatenated string of all Cc recipient display names.</span></span>  <br/> |
|[<span data-ttu-id="9b8d1-173">дисплайто</span><span class="sxs-lookup"><span data-stu-id="9b8d1-173">DisplayTo</span></span>](displayto.md) <br/> |<span data-ttu-id="9b8d1-174">Представляет отображаемую строку, используемую для содержимого поля "Кому".</span><span class="sxs-lookup"><span data-stu-id="9b8d1-174">Represents the display string that is used for the contents of the To box.</span></span> <span data-ttu-id="9b8d1-175">Это объединенная строка для отображаемых имен получателей.</span><span class="sxs-lookup"><span data-stu-id="9b8d1-175">This is the concatenated string of all To recipient display names.</span></span>  <br/> |
|[<span data-ttu-id="9b8d1-176">HasAttachments</span><span class="sxs-lookup"><span data-stu-id="9b8d1-176">HasAttachments</span></span>](hasattachments.md) <br/> |<span data-ttu-id="9b8d1-177">Представляет свойство, для которого задано значение **true** , если элемент имеет вложение.</span><span class="sxs-lookup"><span data-stu-id="9b8d1-177">Represents a property that is set to **true** if an item has an attachment.</span></span> <span data-ttu-id="9b8d1-178">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9b8d1-178">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="9b8d1-179">ExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="9b8d1-179">ExtendedProperty</span></span>](extendedproperty.md) <br/> |<span data-ttu-id="9b8d1-180">Определяет расширенные свойства для папок и элементов.</span><span class="sxs-lookup"><span data-stu-id="9b8d1-180">Identifies extended properties on folders and items.</span></span>  <br/> |
|[<span data-ttu-id="9b8d1-181">Culture</span><span class="sxs-lookup"><span data-stu-id="9b8d1-181">Culture</span></span>](culture.md) <br/> |<span data-ttu-id="9b8d1-182">Представляет язык и региональные параметры для определенного элемента в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="9b8d1-182">Represents the culture for a given item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="9b8d1-183">Sender</span><span class="sxs-lookup"><span data-stu-id="9b8d1-183">Sender</span></span>](sender.md) <br/> |<span data-ttu-id="9b8d1-184">Определяет отправителя элемента.</span><span class="sxs-lookup"><span data-stu-id="9b8d1-184">Identifies the sender of an item.</span></span>  <br/> |
|[<span data-ttu-id="9b8d1-185">ToRecipients</span><span class="sxs-lookup"><span data-stu-id="9b8d1-185">ToRecipients</span></span>](torecipients.md) <br/> |<span data-ttu-id="9b8d1-186">Содержит набор получателей сообщения.</span><span class="sxs-lookup"><span data-stu-id="9b8d1-186">Contains a set of recipients of a message.</span></span>  <br/> |
|[<span data-ttu-id="9b8d1-187">CcRecipients</span><span class="sxs-lookup"><span data-stu-id="9b8d1-187">CcRecipients</span></span>](ccrecipients.md) <br/> |<span data-ttu-id="9b8d1-188">Представляет коллекцию получателей, которые будут получать копию сообщения.</span><span class="sxs-lookup"><span data-stu-id="9b8d1-188">Represents a collection of recipients that will receive a copy of the message.</span></span>  <br/> |
|[<span data-ttu-id="9b8d1-189">BccRecipients</span><span class="sxs-lookup"><span data-stu-id="9b8d1-189">BccRecipients</span></span>](bccrecipients.md) <br/> |<span data-ttu-id="9b8d1-190">Представляет коллекцию получателей для получения скрытой копии сообщения электронной почты.</span><span class="sxs-lookup"><span data-stu-id="9b8d1-190">Represents a collection of recipients to receive a blind carbon copy (Bcc) of an e-mail.</span></span>  <br/> |
|[<span data-ttu-id="9b8d1-191">исреадрецеиптрекуестед</span><span class="sxs-lookup"><span data-stu-id="9b8d1-191">IsReadReceiptRequested</span></span>](isreadreceiptrequested.md) <br/> |<span data-ttu-id="9b8d1-192">Указывает, запрашивает ли отправитель элемента уведомление о прочтении.</span><span class="sxs-lookup"><span data-stu-id="9b8d1-192">Indicates whether the sender of an item requests a read receipt.</span></span>  <br/> |
|[<span data-ttu-id="9b8d1-193">исделиверирецеиптрекуестед</span><span class="sxs-lookup"><span data-stu-id="9b8d1-193">IsDeliveryReceiptRequested</span></span>](isdeliveryreceiptrequested.md) <br/> |<span data-ttu-id="9b8d1-194">Указывает, запрашивает ли отправитель элемента уведомление о доставке.</span><span class="sxs-lookup"><span data-stu-id="9b8d1-194">Indicates whether the sender of an item requests a delivery receipt.</span></span>  <br/> |
|[<span data-ttu-id="9b8d1-195">ConversationIndex</span><span class="sxs-lookup"><span data-stu-id="9b8d1-195">ConversationIndex</span></span>](conversationindex.md) <br/> |<span data-ttu-id="9b8d1-196">Содержит двоичный код, представляющий поток, к которому относится сообщение.</span><span class="sxs-lookup"><span data-stu-id="9b8d1-196">Contains a binary ID that represents the thread to which this message belongs.</span></span>  <br/> |
|[<span data-ttu-id="9b8d1-197">ConversationTopic</span><span class="sxs-lookup"><span data-stu-id="9b8d1-197">ConversationTopic</span></span>](conversationtopic.md) <br/> |<span data-ttu-id="9b8d1-198">Представляет идентификатор беседы.</span><span class="sxs-lookup"><span data-stu-id="9b8d1-198">Represents the conversation identifier.</span></span>  <br/> |
|[<span data-ttu-id="9b8d1-199">From</span><span class="sxs-lookup"><span data-stu-id="9b8d1-199">From</span></span>](from.md) <br/> |<span data-ttu-id="9b8d1-200">Представляет адрес, с которого было отправлено сообщение.</span><span class="sxs-lookup"><span data-stu-id="9b8d1-200">Represents the address from which the message was sent.</span></span>  <br/> |
|[<span data-ttu-id="9b8d1-201">InternetMessageId</span><span class="sxs-lookup"><span data-stu-id="9b8d1-201">InternetMessageId</span></span>](internetmessageid.md) <br/> |<span data-ttu-id="9b8d1-202">Представляет идентификатор сообщения Интернета для элемента.</span><span class="sxs-lookup"><span data-stu-id="9b8d1-202">Represents the Internet message identifier of an item.</span></span>  <br/> |
|[<span data-ttu-id="9b8d1-203">IsRead</span><span class="sxs-lookup"><span data-stu-id="9b8d1-203">IsRead</span></span>](isread.md) <br/> |<span data-ttu-id="9b8d1-204">Указывает, было ли Прочитано сообщение.</span><span class="sxs-lookup"><span data-stu-id="9b8d1-204">Indicates whether a message has been read.</span></span>  <br/> |
|[<span data-ttu-id="9b8d1-205">исреспонсерекуестед</span><span class="sxs-lookup"><span data-stu-id="9b8d1-205">IsResponseRequested</span></span>](isresponserequested.md) <br/> |<span data-ttu-id="9b8d1-206">Указывает, запрашивается ли ответ на сообщение электронной почты.</span><span class="sxs-lookup"><span data-stu-id="9b8d1-206">Indicates whether a response to an e-mail message is requested.</span></span>  <br/> |
|[<span data-ttu-id="9b8d1-207">References</span><span class="sxs-lookup"><span data-stu-id="9b8d1-207">References</span></span>](references.md) <br/> |<span data-ttu-id="9b8d1-208">Представляет заголовок Usenet, используемый для связывания ответов с их исходными сообщениями.</span><span class="sxs-lookup"><span data-stu-id="9b8d1-208">Represents the Usenet header that is used to associate replies with their original messages.</span></span>  <br/> |
|[<span data-ttu-id="9b8d1-209">ReplyTo</span><span class="sxs-lookup"><span data-stu-id="9b8d1-209">ReplyTo</span></span>](replyto.md) <br/> |<span data-ttu-id="9b8d1-210">Определяет набор адресов, в который отправляются ответы.</span><span class="sxs-lookup"><span data-stu-id="9b8d1-210">Identifies a set of addresses to which replies should be sent.</span></span>  <br/> |
|[<span data-ttu-id="9b8d1-211">еффективеригхтс</span><span class="sxs-lookup"><span data-stu-id="9b8d1-211">EffectiveRights</span></span>](effectiverights.md) <br/> |<span data-ttu-id="9b8d1-212">Содержит права клиента на основе параметров разрешений для элемента или папки.</span><span class="sxs-lookup"><span data-stu-id="9b8d1-212">Contains the client's rights based on the permission settings for the item or folder.</span></span> <span data-ttu-id="9b8d1-213">Этот элемент доступен только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9b8d1-213">This element is read-only.</span></span> <span data-ttu-id="9b8d1-214">Этот элемент появился в Exchange 2007 с пакетом обновления 1.</span><span class="sxs-lookup"><span data-stu-id="9b8d1-214">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="9b8d1-215">рецеиведби</span><span class="sxs-lookup"><span data-stu-id="9b8d1-215">ReceivedBy</span></span>](receivedby.md) <br/> |<span data-ttu-id="9b8d1-216">Определяет делегат в сценарии доступа делегата.</span><span class="sxs-lookup"><span data-stu-id="9b8d1-216">Identifies the delegate in a delegate access scenario.</span></span> <span data-ttu-id="9b8d1-217">Этот элемент появился в Exchange 2007 с пакетом обновления 1.</span><span class="sxs-lookup"><span data-stu-id="9b8d1-217">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="9b8d1-218">рецеиведрепресентинг</span><span class="sxs-lookup"><span data-stu-id="9b8d1-218">ReceivedRepresenting</span></span>](receivedrepresenting.md) <br/> |<span data-ttu-id="9b8d1-219">Определяет участника в сценарии доступа делегата.</span><span class="sxs-lookup"><span data-stu-id="9b8d1-219">Identifies the principal in a delegate access scenario.</span></span> <span data-ttu-id="9b8d1-220">Этот элемент появился в Exchange 2007 с пакетом обновления 1.</span><span class="sxs-lookup"><span data-stu-id="9b8d1-220">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="9b8d1-221">невбодиконтент</span><span class="sxs-lookup"><span data-stu-id="9b8d1-221">NewBodyContent</span></span>](newbodycontent.md) <br/> |<span data-ttu-id="9b8d1-222">Представляет новое содержимое тела элемента POST.</span><span class="sxs-lookup"><span data-stu-id="9b8d1-222">Represents the new body content of a post item.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="9b8d1-223">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="9b8d1-223">Parent elements</span></span>

|<span data-ttu-id="9b8d1-224">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="9b8d1-224">**Element**</span></span>|<span data-ttu-id="9b8d1-225">**Описание**</span><span class="sxs-lookup"><span data-stu-id="9b8d1-225">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9b8d1-226">аджацентмитингс</span><span class="sxs-lookup"><span data-stu-id="9b8d1-226">AdjacentMeetings</span></span>](adjacentmeetings.md) <br/> |<span data-ttu-id="9b8d1-227">Описывает все элементы, смежные с временем собрания.</span><span class="sxs-lookup"><span data-stu-id="9b8d1-227">Describes all items that are adjacent to a meeting time.</span></span>  <br/> |
|[<span data-ttu-id="9b8d1-228">конфликтингмитингс</span><span class="sxs-lookup"><span data-stu-id="9b8d1-228">ConflictingMeetings</span></span>](conflictingmeetings.md) <br/> |<span data-ttu-id="9b8d1-229">Описывает все элементы, которые конфликтуют с временем собрания.</span><span class="sxs-lookup"><span data-stu-id="9b8d1-229">Describes all items that conflict with a meeting time.</span></span>  <br/> |
|[<span data-ttu-id="9b8d1-230">респонсеобжектс</span><span class="sxs-lookup"><span data-stu-id="9b8d1-230">ResponseObjects</span></span>](responseobjects.md) <br/> |<span data-ttu-id="9b8d1-231">Содержит коллекцию всех объектов ответа, связанных с элементом в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="9b8d1-231">Contains a collection of all the response objects that are associated with an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="9b8d1-232">Элементы (Нонемптяррайофаллитемстипе)</span><span class="sxs-lookup"><span data-stu-id="9b8d1-232">Items (NonEmptyArrayOfAllItemsType)</span></span>](items-nonemptyarrayofallitemstype.md) <br/> |<span data-ttu-id="9b8d1-233">Содержит массив элементов для создания в папке, определяемой элементом [ParentFolderId (таржетфолдеридтипе)](parentfolderid-targetfolderidtype.md) .</span><span class="sxs-lookup"><span data-stu-id="9b8d1-233">Contains an array of items to create in the folder that is identified by the [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) element.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="9b8d1-234">Примечания</span><span class="sxs-lookup"><span data-stu-id="9b8d1-234">Remarks</span></span>

<span data-ttu-id="9b8d1-235">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="9b8d1-235">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9b8d1-236">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="9b8d1-236">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9b8d1-237">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="9b8d1-237">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="9b8d1-238">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="9b8d1-238">Schema Name</span></span>  <br/> |<span data-ttu-id="9b8d1-239">Схема Types</span><span class="sxs-lookup"><span data-stu-id="9b8d1-239">Types schema</span></span>  <br/> |
|<span data-ttu-id="9b8d1-240">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="9b8d1-240">Validation File</span></span>  <br/> |<span data-ttu-id="9b8d1-241">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="9b8d1-241">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="9b8d1-242">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="9b8d1-242">Can be Empty</span></span>  <br/> |<span data-ttu-id="9b8d1-243">False</span><span class="sxs-lookup"><span data-stu-id="9b8d1-243">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9b8d1-244">См. также</span><span class="sxs-lookup"><span data-stu-id="9b8d1-244">See also</span></span>



- [<span data-ttu-id="9b8d1-245">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="9b8d1-245">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

