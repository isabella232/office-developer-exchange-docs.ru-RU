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
ms.openlocfilehash: 70a0d6a7c670d0f16a55e66e7ef329331a04a5f8
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834868"
---
# <a name="postreplyitem"></a><span data-ttu-id="07ced-104">постреплитем</span><span class="sxs-lookup"><span data-stu-id="07ced-104">PostReplyItem</span></span>

<span data-ttu-id="07ced-105">Элемент **постреплитем** содержит ответ на элемент POST.</span><span class="sxs-lookup"><span data-stu-id="07ced-105">The **PostReplyItem** element contains a reply to a post item.</span></span> <span data-ttu-id="07ced-106">Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="07ced-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
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

 <span data-ttu-id="07ced-107">**постреплитемтипе**</span><span class="sxs-lookup"><span data-stu-id="07ced-107">**PostReplyItemType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="07ced-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="07ced-108">Attributes and elements</span></span>

<span data-ttu-id="07ced-109">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="07ced-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="07ced-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="07ced-110">Attributes</span></span>

<span data-ttu-id="07ced-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="07ced-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="07ced-112">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="07ced-112">Child elements</span></span>

|<span data-ttu-id="07ced-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="07ced-113">**Element**</span></span>|<span data-ttu-id="07ced-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="07ced-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="07ced-115">Сохранитьmimecontent</span><span class="sxs-lookup"><span data-stu-id="07ced-115">MimeContent</span></span>](mimecontent.md) <br/> |<span data-ttu-id="07ced-116">Содержит собственный многоцелевой поток расширений почты в Интернете (MIME) объекта, представленного в формате base64Binary.</span><span class="sxs-lookup"><span data-stu-id="07ced-116">Contains the native Multipurpose Internet Mail Extensions (MIME) stream of an object that is represented in base64Binary format.</span></span>  <br/> |
|[<span data-ttu-id="07ced-117">Идентификатор</span><span class="sxs-lookup"><span data-stu-id="07ced-117">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="07ced-118">Содержит уникальный идентификатор и ключ изменения элемента в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="07ced-118">Contains the unique identifier and change key of an item in the Exchange store.</span></span> <span data-ttu-id="07ced-119">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="07ced-119">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="07ced-120">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="07ced-120">ParentFolderId</span></span>](parentfolderid.md) <br/> |<span data-ttu-id="07ced-121">Представляет идентификатор родительской папки, содержащей элемент или папку.</span><span class="sxs-lookup"><span data-stu-id="07ced-121">Represents the identifier of the parent folder that contains the item or folder.</span></span> <span data-ttu-id="07ced-122">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="07ced-122">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="07ced-123">ItemClass</span><span class="sxs-lookup"><span data-stu-id="07ced-123">ItemClass</span></span>](itemclass.md) <br/> |<span data-ttu-id="07ced-124">Представляет класс сообщения для элемента.</span><span class="sxs-lookup"><span data-stu-id="07ced-124">Represents the message class of an item.</span></span>  <br/> |
|[<span data-ttu-id="07ced-125">Тема</span><span class="sxs-lookup"><span data-stu-id="07ced-125">Subject</span></span>](subject.md) <br/> |<span data-ttu-id="07ced-126">Представляет тему для элементов хранилища Exchange и объектов ответа.</span><span class="sxs-lookup"><span data-stu-id="07ced-126">Represents the subject for Exchange store items and response objects.</span></span> <span data-ttu-id="07ced-127">Тема может иметь не более 255 символов.</span><span class="sxs-lookup"><span data-stu-id="07ced-127">The subject is limited to 255 characters.</span></span>  <br/> |
|[<span data-ttu-id="07ced-128">Sensitivity</span><span class="sxs-lookup"><span data-stu-id="07ced-128">Sensitivity</span></span>](sensitivity.md) <br/> |<span data-ttu-id="07ced-129">Указывает уровень конфиденциальности элемента.</span><span class="sxs-lookup"><span data-stu-id="07ced-129">Indicates the sensitivity level of an item.</span></span>  <br/> |
|[<span data-ttu-id="07ced-130">Основной текст</span><span class="sxs-lookup"><span data-stu-id="07ced-130">Body</span></span>](body.md) <br/> |<span data-ttu-id="07ced-131">Представляет реальное содержимое основного текста сообщения.</span><span class="sxs-lookup"><span data-stu-id="07ced-131">Represents the actual body content of a message.</span></span>  <br/> |
|[<span data-ttu-id="07ced-132">Вложения</span><span class="sxs-lookup"><span data-stu-id="07ced-132">Attachments</span></span>](attachments-ex15websvcsotherref.md) <br/> |<span data-ttu-id="07ced-133">Содержит элементы или файлы, вложенные в элемент в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="07ced-133">Contains the items or files that are attached to an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="07ced-134">DateTimeReceived</span><span class="sxs-lookup"><span data-stu-id="07ced-134">DateTimeReceived</span></span>](datetimereceived.md) <br/> |<span data-ttu-id="07ced-135">Представляет дату и время получения элемента в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="07ced-135">Represents the date and time that an item in a mailbox was received.</span></span>  <br/> |
|[<span data-ttu-id="07ced-136">Размер</span><span class="sxs-lookup"><span data-stu-id="07ced-136">Size</span></span>](size.md) <br/> |<span data-ttu-id="07ced-137">Представляет размер элемента в байтах.</span><span class="sxs-lookup"><span data-stu-id="07ced-137">Represents the size in bytes of an item.</span></span> <span data-ttu-id="07ced-138">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="07ced-138">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="07ced-139">Категории</span><span class="sxs-lookup"><span data-stu-id="07ced-139">Categories</span></span>](categories-ex15websvcsotherref.md) <br/> |<span data-ttu-id="07ced-140">Представляет коллекцию строк, определяющих категории, к которым относится элемент в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="07ced-140">Represents a collection of strings that identify categories to which an item in the mailbox belongs.</span></span>  <br/> |
|[<span data-ttu-id="07ced-141">Importance</span><span class="sxs-lookup"><span data-stu-id="07ced-141">Importance</span></span>](importance.md) <br/> |<span data-ttu-id="07ced-142">Описывает важность элемента.</span><span class="sxs-lookup"><span data-stu-id="07ced-142">Describes the importance of an item.</span></span>  <br/> |
|[<span data-ttu-id="07ced-143">инреплито</span><span class="sxs-lookup"><span data-stu-id="07ced-143">InReplyTo</span></span>](inreplyto.md) <br/> |<span data-ttu-id="07ced-144">Представляет идентификатор элемента, который является ответом на этот элемент.</span><span class="sxs-lookup"><span data-stu-id="07ced-144">Represents the identifier of the item to which this item is a reply.</span></span>  <br/> |
|[<span data-ttu-id="07ced-145">Отправлено</span><span class="sxs-lookup"><span data-stu-id="07ced-145">IsSubmitted</span></span>](issubmitted.md) <br/> |<span data-ttu-id="07ced-146">Указывает, был ли элемент отправлен в папку "Исходящие" по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="07ced-146">Indicates whether an item has been submitted to the Outbox default folder.</span></span>  <br/> |
|[<span data-ttu-id="07ced-147">Черновик</span><span class="sxs-lookup"><span data-stu-id="07ced-147">IsDraft</span></span>](isdraft.md) <br/> |<span data-ttu-id="07ced-148">Указывает, был ли элемент еще не отправлен.</span><span class="sxs-lookup"><span data-stu-id="07ced-148">Represents whether an item has not yet been sent.</span></span>  <br/> |
|[<span data-ttu-id="07ced-149">исфромме</span><span class="sxs-lookup"><span data-stu-id="07ced-149">IsFromMe</span></span>](isfromme.md) <br/> |<span data-ttu-id="07ced-150">Указывает, отправляет ли пользователь элемент.</span><span class="sxs-lookup"><span data-stu-id="07ced-150">Indicates whether a user sent an item to him or herself.</span></span>  <br/> |
|[<span data-ttu-id="07ced-151">исресенд</span><span class="sxs-lookup"><span data-stu-id="07ced-151">IsResend</span></span>](isresend.md) <br/> |<span data-ttu-id="07ced-152">Указывает, был ли ранее отправлен элемент.</span><span class="sxs-lookup"><span data-stu-id="07ced-152">Indicates whether the item had previously been sent.</span></span>  <br/> |
|[<span data-ttu-id="07ced-153">исунмодифиед</span><span class="sxs-lookup"><span data-stu-id="07ced-153">IsUnmodified</span></span>](isunmodified.md) <br/> |<span data-ttu-id="07ced-154">Указывает, был ли изменен элемент.</span><span class="sxs-lookup"><span data-stu-id="07ced-154">Indicates whether the item has been modified.</span></span>  <br/> |
|[<span data-ttu-id="07ced-155">InternetMessageHeaders</span><span class="sxs-lookup"><span data-stu-id="07ced-155">InternetMessageHeaders</span></span>](internetmessageheaders.md) <br/> |<span data-ttu-id="07ced-156">Представляет коллекцию всех заголовков сообщений Интернета, которые находятся в элементе почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="07ced-156">Represents the collection of all Internet message headers that are contained in an item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="07ced-157">датетимесент</span><span class="sxs-lookup"><span data-stu-id="07ced-157">DateTimeSent</span></span>](datetimesent.md) <br/> |<span data-ttu-id="07ced-158">Представляет дату и время отправки элемента в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="07ced-158">Represents the date and time that an item in a mailbox was sent.</span></span>  <br/> |
|[<span data-ttu-id="07ced-159">DateTimeCreated</span><span class="sxs-lookup"><span data-stu-id="07ced-159">DateTimeCreated</span></span>](datetimecreated.md) <br/> |<span data-ttu-id="07ced-160">Представляет дату и время создания определенного элемента в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="07ced-160">Represents the date and time that a given item in the mailbox was created.</span></span>  <br/> |
|[<span data-ttu-id="07ced-161">респонсеобжектс</span><span class="sxs-lookup"><span data-stu-id="07ced-161">ResponseObjects</span></span>](responseobjects.md) <br/> |<span data-ttu-id="07ced-162">Содержит коллекцию всех объектов ответа, связанных с элементом в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="07ced-162">Contains a collection of all the response objects that are associated with an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="07ced-163">реминдердуеби</span><span class="sxs-lookup"><span data-stu-id="07ced-163">ReminderDueBy</span></span>](reminderdueby.md) <br/> |<span data-ttu-id="07ced-164">Представляет дату и время возникновения события.</span><span class="sxs-lookup"><span data-stu-id="07ced-164">Represents the date and time when the event occurs.</span></span> <span data-ttu-id="07ced-165">Он используется элементом [реминдерминутесбефорестарт](reminderminutesbeforestart.md) для определения времени отображения напоминания.</span><span class="sxs-lookup"><span data-stu-id="07ced-165">This is used by the [ReminderMinutesBeforeStart](reminderminutesbeforestart.md) element to determine when the reminder is displayed.</span></span>  <br/> |
|[<span data-ttu-id="07ced-166">реминдериссет</span><span class="sxs-lookup"><span data-stu-id="07ced-166">ReminderIsSet</span></span>](reminderisset.md) <br/> |<span data-ttu-id="07ced-167">Указывает, задано ли напоминание для элемента в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="07ced-167">Indicates whether a reminder has been set for an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="07ced-168">ReminderMinutesBeforeStart</span><span class="sxs-lookup"><span data-stu-id="07ced-168">ReminderMinutesBeforeStart</span></span>](reminderminutesbeforestart.md) <br/> |<span data-ttu-id="07ced-169">Представляет количество минут до события при отображении напоминания.</span><span class="sxs-lookup"><span data-stu-id="07ced-169">Represents the number of minutes before an event when a reminder is displayed.</span></span>  <br/> |
|[<span data-ttu-id="07ced-170">дисплайкк</span><span class="sxs-lookup"><span data-stu-id="07ced-170">DisplayCc</span></span>](displaycc.md) <br/> |<span data-ttu-id="07ced-171">Представляет отображаемую строку, используемую для содержимого строки "копия".</span><span class="sxs-lookup"><span data-stu-id="07ced-171">Represents the display string that is used for the contents of the Cc line.</span></span> <span data-ttu-id="07ced-172">Это объединенная строка всех отображаемых имен получателей копии.</span><span class="sxs-lookup"><span data-stu-id="07ced-172">This is the concatenated string of all Cc recipient display names.</span></span>  <br/> |
|[<span data-ttu-id="07ced-173">дисплайто</span><span class="sxs-lookup"><span data-stu-id="07ced-173">DisplayTo</span></span>](displayto.md) <br/> |<span data-ttu-id="07ced-174">Представляет отображаемую строку, используемую для содержимого поля "Кому".</span><span class="sxs-lookup"><span data-stu-id="07ced-174">Represents the display string that is used for the contents of the To box.</span></span> <span data-ttu-id="07ced-175">Это объединенная строка для отображаемых имен получателей.</span><span class="sxs-lookup"><span data-stu-id="07ced-175">This is the concatenated string of all To recipient display names.</span></span>  <br/> |
|[<span data-ttu-id="07ced-176">HasAttachments</span><span class="sxs-lookup"><span data-stu-id="07ced-176">HasAttachments</span></span>](hasattachments.md) <br/> |<span data-ttu-id="07ced-177">Представляет свойство, для которого задано значение **true** , если элемент имеет вложение.</span><span class="sxs-lookup"><span data-stu-id="07ced-177">Represents a property that is set to **true** if an item has an attachment.</span></span> <span data-ttu-id="07ced-178">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="07ced-178">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="07ced-179">ExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="07ced-179">ExtendedProperty</span></span>](extendedproperty.md) <br/> |<span data-ttu-id="07ced-180">Определяет расширенные свойства для папок и элементов.</span><span class="sxs-lookup"><span data-stu-id="07ced-180">Identifies extended properties on folders and items.</span></span>  <br/> |
|[<span data-ttu-id="07ced-181">Culture</span><span class="sxs-lookup"><span data-stu-id="07ced-181">Culture</span></span>](culture.md) <br/> |<span data-ttu-id="07ced-182">Представляет язык и региональные параметры для определенного элемента в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="07ced-182">Represents the culture for a given item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="07ced-183">Sender</span><span class="sxs-lookup"><span data-stu-id="07ced-183">Sender</span></span>](sender.md) <br/> |<span data-ttu-id="07ced-184">Определяет отправителя элемента.</span><span class="sxs-lookup"><span data-stu-id="07ced-184">Identifies the sender of an item.</span></span>  <br/> |
|[<span data-ttu-id="07ced-185">ToRecipients</span><span class="sxs-lookup"><span data-stu-id="07ced-185">ToRecipients</span></span>](torecipients.md) <br/> |<span data-ttu-id="07ced-186">Содержит набор получателей сообщения.</span><span class="sxs-lookup"><span data-stu-id="07ced-186">Contains a set of recipients of a message.</span></span>  <br/> |
|[<span data-ttu-id="07ced-187">CcRecipients</span><span class="sxs-lookup"><span data-stu-id="07ced-187">CcRecipients</span></span>](ccrecipients.md) <br/> |<span data-ttu-id="07ced-188">Представляет коллекцию получателей, которые будут получать копию сообщения.</span><span class="sxs-lookup"><span data-stu-id="07ced-188">Represents a collection of recipients that will receive a copy of the message.</span></span>  <br/> |
|[<span data-ttu-id="07ced-189">BccRecipients</span><span class="sxs-lookup"><span data-stu-id="07ced-189">BccRecipients</span></span>](bccrecipients.md) <br/> |<span data-ttu-id="07ced-190">Представляет коллекцию получателей для получения скрытой копии сообщения электронной почты.</span><span class="sxs-lookup"><span data-stu-id="07ced-190">Represents a collection of recipients to receive a blind carbon copy (Bcc) of an e-mail.</span></span>  <br/> |
|[<span data-ttu-id="07ced-191">исреадрецеиптрекуестед</span><span class="sxs-lookup"><span data-stu-id="07ced-191">IsReadReceiptRequested</span></span>](isreadreceiptrequested.md) <br/> |<span data-ttu-id="07ced-192">Указывает, запрашивает ли отправитель элемента уведомление о прочтении.</span><span class="sxs-lookup"><span data-stu-id="07ced-192">Indicates whether the sender of an item requests a read receipt.</span></span>  <br/> |
|[<span data-ttu-id="07ced-193">исделиверирецеиптрекуестед</span><span class="sxs-lookup"><span data-stu-id="07ced-193">IsDeliveryReceiptRequested</span></span>](isdeliveryreceiptrequested.md) <br/> |<span data-ttu-id="07ced-194">Указывает, запрашивает ли отправитель элемента уведомление о доставке.</span><span class="sxs-lookup"><span data-stu-id="07ced-194">Indicates whether the sender of an item requests a delivery receipt.</span></span>  <br/> |
|[<span data-ttu-id="07ced-195">ConversationIndex</span><span class="sxs-lookup"><span data-stu-id="07ced-195">ConversationIndex</span></span>](conversationindex.md) <br/> |<span data-ttu-id="07ced-196">Содержит двоичный код, представляющий поток, к которому относится сообщение.</span><span class="sxs-lookup"><span data-stu-id="07ced-196">Contains a binary ID that represents the thread to which this message belongs.</span></span>  <br/> |
|[<span data-ttu-id="07ced-197">ConversationTopic</span><span class="sxs-lookup"><span data-stu-id="07ced-197">ConversationTopic</span></span>](conversationtopic.md) <br/> |<span data-ttu-id="07ced-198">Представляет идентификатор беседы.</span><span class="sxs-lookup"><span data-stu-id="07ced-198">Represents the conversation identifier.</span></span>  <br/> |
|[<span data-ttu-id="07ced-199">From</span><span class="sxs-lookup"><span data-stu-id="07ced-199">From</span></span>](from.md) <br/> |<span data-ttu-id="07ced-200">Представляет адрес, с которого было отправлено сообщение.</span><span class="sxs-lookup"><span data-stu-id="07ced-200">Represents the address from which the message was sent.</span></span>  <br/> |
|[<span data-ttu-id="07ced-201">InternetMessageId</span><span class="sxs-lookup"><span data-stu-id="07ced-201">InternetMessageId</span></span>](internetmessageid.md) <br/> |<span data-ttu-id="07ced-202">Представляет идентификатор сообщения Интернета для элемента.</span><span class="sxs-lookup"><span data-stu-id="07ced-202">Represents the Internet message identifier of an item.</span></span>  <br/> |
|[<span data-ttu-id="07ced-203">IsRead</span><span class="sxs-lookup"><span data-stu-id="07ced-203">IsRead</span></span>](isread.md) <br/> |<span data-ttu-id="07ced-204">Указывает, было ли Прочитано сообщение.</span><span class="sxs-lookup"><span data-stu-id="07ced-204">Indicates whether a message has been read.</span></span>  <br/> |
|[<span data-ttu-id="07ced-205">исреспонсерекуестед</span><span class="sxs-lookup"><span data-stu-id="07ced-205">IsResponseRequested</span></span>](isresponserequested.md) <br/> |<span data-ttu-id="07ced-206">Указывает, запрашивается ли ответ на сообщение электронной почты.</span><span class="sxs-lookup"><span data-stu-id="07ced-206">Indicates whether a response to an e-mail message is requested.</span></span>  <br/> |
|[<span data-ttu-id="07ced-207">References</span><span class="sxs-lookup"><span data-stu-id="07ced-207">References</span></span>](references.md) <br/> |<span data-ttu-id="07ced-208">Представляет заголовок Usenet, используемый для связывания ответов с их исходными сообщениями.</span><span class="sxs-lookup"><span data-stu-id="07ced-208">Represents the Usenet header that is used to associate replies with their original messages.</span></span>  <br/> |
|[<span data-ttu-id="07ced-209">ReplyTo</span><span class="sxs-lookup"><span data-stu-id="07ced-209">ReplyTo</span></span>](replyto.md) <br/> |<span data-ttu-id="07ced-210">Определяет набор адресов, в который отправляются ответы.</span><span class="sxs-lookup"><span data-stu-id="07ced-210">Identifies a set of addresses to which replies should be sent.</span></span>  <br/> |
|[<span data-ttu-id="07ced-211">еффективеригхтс</span><span class="sxs-lookup"><span data-stu-id="07ced-211">EffectiveRights</span></span>](effectiverights.md) <br/> |<span data-ttu-id="07ced-212">Содержит права клиента на основе параметров разрешений для элемента или папки.</span><span class="sxs-lookup"><span data-stu-id="07ced-212">Contains the client's rights based on the permission settings for the item or folder.</span></span> <span data-ttu-id="07ced-213">Этот элемент доступен только для чтения.</span><span class="sxs-lookup"><span data-stu-id="07ced-213">This element is read-only.</span></span> <span data-ttu-id="07ced-214">Этот элемент появился в Exchange 2007 с пакетом обновления 1.</span><span class="sxs-lookup"><span data-stu-id="07ced-214">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="07ced-215">рецеиведби</span><span class="sxs-lookup"><span data-stu-id="07ced-215">ReceivedBy</span></span>](receivedby.md) <br/> |<span data-ttu-id="07ced-216">Определяет делегат в сценарии доступа делегата.</span><span class="sxs-lookup"><span data-stu-id="07ced-216">Identifies the delegate in a delegate access scenario.</span></span> <span data-ttu-id="07ced-217">Этот элемент появился в Exchange 2007 с пакетом обновления 1.</span><span class="sxs-lookup"><span data-stu-id="07ced-217">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="07ced-218">рецеиведрепресентинг</span><span class="sxs-lookup"><span data-stu-id="07ced-218">ReceivedRepresenting</span></span>](receivedrepresenting.md) <br/> |<span data-ttu-id="07ced-219">Определяет участника в сценарии доступа делегата.</span><span class="sxs-lookup"><span data-stu-id="07ced-219">Identifies the principal in a delegate access scenario.</span></span> <span data-ttu-id="07ced-220">Этот элемент появился в Exchange 2007 с пакетом обновления 1.</span><span class="sxs-lookup"><span data-stu-id="07ced-220">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="07ced-221">невбодиконтент</span><span class="sxs-lookup"><span data-stu-id="07ced-221">NewBodyContent</span></span>](newbodycontent.md) <br/> |<span data-ttu-id="07ced-222">Представляет новое содержимое тела элемента POST.</span><span class="sxs-lookup"><span data-stu-id="07ced-222">Represents the new body content of a post item.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="07ced-223">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="07ced-223">Parent elements</span></span>

|<span data-ttu-id="07ced-224">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="07ced-224">**Element**</span></span>|<span data-ttu-id="07ced-225">**Описание**</span><span class="sxs-lookup"><span data-stu-id="07ced-225">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="07ced-226">аджацентмитингс</span><span class="sxs-lookup"><span data-stu-id="07ced-226">AdjacentMeetings</span></span>](adjacentmeetings.md) <br/> |<span data-ttu-id="07ced-227">Описывает все элементы, смежные с временем собрания.</span><span class="sxs-lookup"><span data-stu-id="07ced-227">Describes all items that are adjacent to a meeting time.</span></span>  <br/> |
|[<span data-ttu-id="07ced-228">конфликтингмитингс</span><span class="sxs-lookup"><span data-stu-id="07ced-228">ConflictingMeetings</span></span>](conflictingmeetings.md) <br/> |<span data-ttu-id="07ced-229">Описывает все элементы, которые конфликтуют с временем собрания.</span><span class="sxs-lookup"><span data-stu-id="07ced-229">Describes all items that conflict with a meeting time.</span></span>  <br/> |
|[<span data-ttu-id="07ced-230">респонсеобжектс</span><span class="sxs-lookup"><span data-stu-id="07ced-230">ResponseObjects</span></span>](responseobjects.md) <br/> |<span data-ttu-id="07ced-231">Содержит коллекцию всех объектов ответа, связанных с элементом в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="07ced-231">Contains a collection of all the response objects that are associated with an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="07ced-232">Элементы (Нонемптяррайофаллитемстипе)</span><span class="sxs-lookup"><span data-stu-id="07ced-232">Items (NonEmptyArrayOfAllItemsType)</span></span>](items-nonemptyarrayofallitemstype.md) <br/> |<span data-ttu-id="07ced-233">Содержит массив элементов для создания в папке, определяемой элементом [ParentFolderId (таржетфолдеридтипе)](parentfolderid-targetfolderidtype.md) .</span><span class="sxs-lookup"><span data-stu-id="07ced-233">Contains an array of items to create in the folder that is identified by the [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) element.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="07ced-234">Примечания</span><span class="sxs-lookup"><span data-stu-id="07ced-234">Remarks</span></span>

<span data-ttu-id="07ced-235">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="07ced-235">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="07ced-236">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="07ced-236">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="07ced-237">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="07ced-237">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="07ced-238">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="07ced-238">Schema Name</span></span>  <br/> |<span data-ttu-id="07ced-239">Схема Types</span><span class="sxs-lookup"><span data-stu-id="07ced-239">Types schema</span></span>  <br/> |
|<span data-ttu-id="07ced-240">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="07ced-240">Validation File</span></span>  <br/> |<span data-ttu-id="07ced-241">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="07ced-241">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="07ced-242">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="07ced-242">Can be Empty</span></span>  <br/> |<span data-ttu-id="07ced-243">False</span><span class="sxs-lookup"><span data-stu-id="07ced-243">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="07ced-244">См. также</span><span class="sxs-lookup"><span data-stu-id="07ced-244">See also</span></span>



- [<span data-ttu-id="07ced-245">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="07ced-245">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

