---
title: митингреспонсе
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
description: Элемент Митингреспонсе представляет ответ на приглашение на собрание в хранилище Exchange.
ms.openlocfilehash: c5f9f3ac2fcd12e9c95f663311c33cdd36783251
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834446"
---
# <a name="meetingresponse"></a><span data-ttu-id="290b8-103">митингреспонсе</span><span class="sxs-lookup"><span data-stu-id="290b8-103">MeetingResponse</span></span>

<span data-ttu-id="290b8-104">Элемент **митингреспонсе** представляет ответ на приглашение на собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="290b8-104">The **MeetingResponse** element represents a meeting response in the Exchange store.</span></span> 
  
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

 <span data-ttu-id="290b8-105">**митингреспонсемессажетипе**</span><span class="sxs-lookup"><span data-stu-id="290b8-105">**MeetingResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="290b8-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="290b8-106">Attributes and elements</span></span>

<span data-ttu-id="290b8-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="290b8-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="290b8-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="290b8-108">Attributes</span></span>

<span data-ttu-id="290b8-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="290b8-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="290b8-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="290b8-110">Child elements</span></span>

|<span data-ttu-id="290b8-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="290b8-111">**Element**</span></span>|<span data-ttu-id="290b8-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="290b8-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="290b8-113">Сохранитьmimecontent</span><span class="sxs-lookup"><span data-stu-id="290b8-113">MimeContent</span></span>](mimecontent.md) <br/> |<span data-ttu-id="290b8-114">Содержит собственный поток MIME объекта, представленный в формате base64Binary.</span><span class="sxs-lookup"><span data-stu-id="290b8-114">Contains the native MIME stream of an object that is represented in base64Binary format.</span></span>  <br/> |
|[<span data-ttu-id="290b8-115">Идентификатор</span><span class="sxs-lookup"><span data-stu-id="290b8-115">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="290b8-116">Содержит уникальный идентификатор и ключ изменения элемента в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="290b8-116">Contains the unique identifier and change key of an item in the Exchange store.</span></span> <span data-ttu-id="290b8-117">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="290b8-117">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="290b8-118">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="290b8-118">ParentFolderId</span></span>](parentfolderid.md) <br/> |<span data-ttu-id="290b8-119">Представляет идентификатор родительской папки, содержащей элемент или папку.</span><span class="sxs-lookup"><span data-stu-id="290b8-119">Represents the identifier of the parent folder that contains the item or folder.</span></span> <span data-ttu-id="290b8-120">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="290b8-120">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="290b8-121">ItemClass</span><span class="sxs-lookup"><span data-stu-id="290b8-121">ItemClass</span></span>](itemclass.md) <br/> |<span data-ttu-id="290b8-122">Представляет класс сообщения для элемента.</span><span class="sxs-lookup"><span data-stu-id="290b8-122">Represents the message class of an item.</span></span>  <br/> |
|[<span data-ttu-id="290b8-123">Тема</span><span class="sxs-lookup"><span data-stu-id="290b8-123">Subject</span></span>](subject.md) <br/> |<span data-ttu-id="290b8-124">Представляет тему для элементов хранилища Exchange и объектов ответа.</span><span class="sxs-lookup"><span data-stu-id="290b8-124">Represents the subject for Exchange store items and response objects.</span></span> <span data-ttu-id="290b8-125">Тема может иметь не более 255 символов.</span><span class="sxs-lookup"><span data-stu-id="290b8-125">The subject is limited to 255 characters.</span></span>  <br/> |
|[<span data-ttu-id="290b8-126">Sensitivity</span><span class="sxs-lookup"><span data-stu-id="290b8-126">Sensitivity</span></span>](sensitivity.md) <br/> |<span data-ttu-id="290b8-127">Указывает уровень конфиденциальности элемента.</span><span class="sxs-lookup"><span data-stu-id="290b8-127">Indicates the sensitivity level of an item.</span></span>  <br/> |
|[<span data-ttu-id="290b8-128">Основной текст</span><span class="sxs-lookup"><span data-stu-id="290b8-128">Body</span></span>](body.md) <br/> |<span data-ttu-id="290b8-129">Представляет реальное содержимое основного текста сообщения.</span><span class="sxs-lookup"><span data-stu-id="290b8-129">Represents the actual body content of a message.</span></span>  <br/> |
|[<span data-ttu-id="290b8-130">Вложения</span><span class="sxs-lookup"><span data-stu-id="290b8-130">Attachments</span></span>](attachments-ex15websvcsotherref.md) <br/> |<span data-ttu-id="290b8-131">Содержит элементы или файлы, вложенные в элемент в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="290b8-131">Contains the items or files that are attached to an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="290b8-132">DateTimeReceived</span><span class="sxs-lookup"><span data-stu-id="290b8-132">DateTimeReceived</span></span>](datetimereceived.md) <br/> |<span data-ttu-id="290b8-133">Представляет данные и время получения элемента в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="290b8-133">Represents the data and time that an item in a mailbox was received.</span></span>  <br/> |
|[<span data-ttu-id="290b8-134">Размер</span><span class="sxs-lookup"><span data-stu-id="290b8-134">Size</span></span>](size.md) <br/> |<span data-ttu-id="290b8-135">Представляет размер элемента в байтах.</span><span class="sxs-lookup"><span data-stu-id="290b8-135">Represents the size in bytes of an item.</span></span> <span data-ttu-id="290b8-136">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="290b8-136">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="290b8-137">Категории</span><span class="sxs-lookup"><span data-stu-id="290b8-137">Categories</span></span>](categories-ex15websvcsotherref.md) <br/> |<span data-ttu-id="290b8-138">Представляет коллекцию строк, определяющих, к каким категориям принадлежит элемент в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="290b8-138">Represents a collection of strings that identify to which categories an item in the mailbox belongs.</span></span>  <br/> |
|[<span data-ttu-id="290b8-139">Importance</span><span class="sxs-lookup"><span data-stu-id="290b8-139">Importance</span></span>](importance.md) <br/> |<span data-ttu-id="290b8-140">Описывает важность элемента.</span><span class="sxs-lookup"><span data-stu-id="290b8-140">Describes the importance of an item.</span></span>  <br/> |
|[<span data-ttu-id="290b8-141">инреплито</span><span class="sxs-lookup"><span data-stu-id="290b8-141">InReplyTo</span></span>](inreplyto.md) <br/> |<span data-ttu-id="290b8-142">Представляет идентификатор элемента, который является ответом на этот элемент.</span><span class="sxs-lookup"><span data-stu-id="290b8-142">Represents the identifier of the item to which this item is a reply.</span></span>  <br/> |
|[<span data-ttu-id="290b8-143">Отправлено</span><span class="sxs-lookup"><span data-stu-id="290b8-143">IsSubmitted</span></span>](issubmitted.md) <br/> |<span data-ttu-id="290b8-144">Указывает, был ли элемент отправлен в папку "Исходящие" по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="290b8-144">Indicates whether an item has been submitted to the Outbox default folder.</span></span>  <br/> |
|[<span data-ttu-id="290b8-145">Черновик</span><span class="sxs-lookup"><span data-stu-id="290b8-145">IsDraft</span></span>](isdraft.md) <br/> |<span data-ttu-id="290b8-146">Указывает, был ли элемент еще не отправлен.</span><span class="sxs-lookup"><span data-stu-id="290b8-146">Represents whether an item has not yet been sent.</span></span>  <br/> |
|[<span data-ttu-id="290b8-147">исфромме</span><span class="sxs-lookup"><span data-stu-id="290b8-147">IsFromMe</span></span>](isfromme.md) <br/> |<span data-ttu-id="290b8-148">Указывает, отправляет ли пользователь элемент.</span><span class="sxs-lookup"><span data-stu-id="290b8-148">Indicates whether a user sent an item to him or herself.</span></span>  <br/> |
|[<span data-ttu-id="290b8-149">исресенд</span><span class="sxs-lookup"><span data-stu-id="290b8-149">IsResend</span></span>](isresend.md) <br/> |<span data-ttu-id="290b8-150">Указывает, был ли ранее отправлен элемент.</span><span class="sxs-lookup"><span data-stu-id="290b8-150">Indicates whether the item had previously been sent.</span></span>  <br/> |
|[<span data-ttu-id="290b8-151">исунмодифиед</span><span class="sxs-lookup"><span data-stu-id="290b8-151">IsUnmodified</span></span>](isunmodified.md) <br/> |<span data-ttu-id="290b8-152">Указывает, был ли изменен элемент.</span><span class="sxs-lookup"><span data-stu-id="290b8-152">Indicates whether the item has been modified.</span></span>  <br/> |
|[<span data-ttu-id="290b8-153">InternetMessageHeaders</span><span class="sxs-lookup"><span data-stu-id="290b8-153">InternetMessageHeaders</span></span>](internetmessageheaders.md) <br/> |<span data-ttu-id="290b8-154">Представляет коллекцию всех заголовков сообщений Интернета, содержащихся в элементе почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="290b8-154">Represents the collection of all Internet message headers that are contained within an item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="290b8-155">датетимесент</span><span class="sxs-lookup"><span data-stu-id="290b8-155">DateTimeSent</span></span>](datetimesent.md) <br/> |<span data-ttu-id="290b8-156">Представляет дату и время отправки элемента в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="290b8-156">Represents the date and time that an item in a mailbox was sent.</span></span>  <br/> |
|[<span data-ttu-id="290b8-157">DateTimeCreated</span><span class="sxs-lookup"><span data-stu-id="290b8-157">DateTimeCreated</span></span>](datetimecreated.md) <br/> |<span data-ttu-id="290b8-158">Представляет дату и время создания определенного элемента в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="290b8-158">Represents the date and time that a given item in the mailbox was created.</span></span>  <br/> |
|[<span data-ttu-id="290b8-159">респонсеобжектс</span><span class="sxs-lookup"><span data-stu-id="290b8-159">ResponseObjects</span></span>](responseobjects.md) <br/> |<span data-ttu-id="290b8-160">Содержит коллекцию всех объектов ответа, связанных с элементом в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="290b8-160">Contains a collection of all the response objects that are associated with an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="290b8-161">реминдердуеби</span><span class="sxs-lookup"><span data-stu-id="290b8-161">ReminderDueBy</span></span>](reminderdueby.md) <br/> |<span data-ttu-id="290b8-162">Представляет дату и время возникновения события.</span><span class="sxs-lookup"><span data-stu-id="290b8-162">Represents the date and time when the event occurs.</span></span> <span data-ttu-id="290b8-163">Он используется элементом [реминдерминутесбефорестарт](reminderminutesbeforestart.md) для определения времени отображения напоминания.</span><span class="sxs-lookup"><span data-stu-id="290b8-163">This is used by the [ReminderMinutesBeforeStart](reminderminutesbeforestart.md) element to determine when the reminder is displayed.</span></span>  <br/> |
|[<span data-ttu-id="290b8-164">реминдериссет</span><span class="sxs-lookup"><span data-stu-id="290b8-164">ReminderIsSet</span></span>](reminderisset.md) <br/> |<span data-ttu-id="290b8-165">Указывает, задано ли напоминание для элемента в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="290b8-165">Indicates whether a reminder has been set for an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="290b8-166">ReminderMinutesBeforeStart</span><span class="sxs-lookup"><span data-stu-id="290b8-166">ReminderMinutesBeforeStart</span></span>](reminderminutesbeforestart.md) <br/> |<span data-ttu-id="290b8-167">Представляет количество минут до события при отображении напоминания.</span><span class="sxs-lookup"><span data-stu-id="290b8-167">Represents the number of minutes before an event when a reminder is displayed.</span></span>  <br/> |
|[<span data-ttu-id="290b8-168">дисплайкк</span><span class="sxs-lookup"><span data-stu-id="290b8-168">DisplayCc</span></span>](displaycc.md) <br/> |<span data-ttu-id="290b8-169">Представляет отображаемую строку, используемую для содержимого поля "копия".</span><span class="sxs-lookup"><span data-stu-id="290b8-169">Represents the display string that is used for the contents of the Cc box.</span></span> <span data-ttu-id="290b8-170">Это объединенная строка всех отображаемых имен получателей копии.</span><span class="sxs-lookup"><span data-stu-id="290b8-170">This is the concatenated string of all Cc recipient display names.</span></span>  <br/> |
|[<span data-ttu-id="290b8-171">дисплайто</span><span class="sxs-lookup"><span data-stu-id="290b8-171">DisplayTo</span></span>](displayto.md) <br/> |<span data-ttu-id="290b8-172">Представляет отображаемую строку, используемую для содержимого поля "Кому".</span><span class="sxs-lookup"><span data-stu-id="290b8-172">Represents the display string that is used for the contents of the To box.</span></span> <span data-ttu-id="290b8-173">Это объединенная строка для отображаемых имен получателей.</span><span class="sxs-lookup"><span data-stu-id="290b8-173">This is the concatenated string of all To recipient display names.</span></span>  <br/> |
|[<span data-ttu-id="290b8-174">HasAttachments</span><span class="sxs-lookup"><span data-stu-id="290b8-174">HasAttachments</span></span>](hasattachments.md) <br/> |<span data-ttu-id="290b8-175">Представляет свойство, для которого задано значение **true** , если элемент имеет по крайней мере одно видимое вложение.</span><span class="sxs-lookup"><span data-stu-id="290b8-175">Represents a property that is set to **true** if an item has at least one visible attachment.</span></span> <span data-ttu-id="290b8-176">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="290b8-176">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="290b8-177">ExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="290b8-177">ExtendedProperty</span></span>](extendedproperty.md) <br/> |<span data-ttu-id="290b8-178">Определяет расширенные свойства для папок и элементов.</span><span class="sxs-lookup"><span data-stu-id="290b8-178">Identifies extended properties on folders and items.</span></span>  <br/> |
|[<span data-ttu-id="290b8-179">Culture</span><span class="sxs-lookup"><span data-stu-id="290b8-179">Culture</span></span>](culture.md) <br/> |<span data-ttu-id="290b8-180">Представляет язык и региональные параметры для определенного элемента в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="290b8-180">Represents the culture for a given item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="290b8-181">Sender</span><span class="sxs-lookup"><span data-stu-id="290b8-181">Sender</span></span>](sender.md) <br/> |<span data-ttu-id="290b8-182">Определяет отправителя элемента.</span><span class="sxs-lookup"><span data-stu-id="290b8-182">Identifies the sender of an item.</span></span>  <br/> |
|[<span data-ttu-id="290b8-183">ToRecipients</span><span class="sxs-lookup"><span data-stu-id="290b8-183">ToRecipients</span></span>](torecipients.md) <br/> |<span data-ttu-id="290b8-184">Содержит набор получателей сообщения.</span><span class="sxs-lookup"><span data-stu-id="290b8-184">Contains a set of recipients of a message.</span></span>  <br/> |
|[<span data-ttu-id="290b8-185">CcRecipients</span><span class="sxs-lookup"><span data-stu-id="290b8-185">CcRecipients</span></span>](ccrecipients.md) <br/> |<span data-ttu-id="290b8-186">Представляет коллекцию получателей, которые будут получать копию сообщения.</span><span class="sxs-lookup"><span data-stu-id="290b8-186">Represents a collection of recipients that will receive a copy of the message.</span></span>  <br/> |
|[<span data-ttu-id="290b8-187">BccRecipients</span><span class="sxs-lookup"><span data-stu-id="290b8-187">BccRecipients</span></span>](bccrecipients.md) <br/> |<span data-ttu-id="290b8-188">Представляет коллекцию получателей для получения скрытой копии сообщения электронной почты.</span><span class="sxs-lookup"><span data-stu-id="290b8-188">Represents a collection of recipients to receive a blind carbon copy (Bcc) of an e-mail.</span></span>  <br/> |
|[<span data-ttu-id="290b8-189">исреадрецеиптрекуестед</span><span class="sxs-lookup"><span data-stu-id="290b8-189">IsReadReceiptRequested</span></span>](isreadreceiptrequested.md) <br/> |<span data-ttu-id="290b8-190">Указывает, запрашивает ли отправитель элемента уведомление о прочтении.</span><span class="sxs-lookup"><span data-stu-id="290b8-190">Indicates whether the sender of an item requests a read receipt.</span></span>  <br/> |
|[<span data-ttu-id="290b8-191">исделиверирецеиптрекуестед</span><span class="sxs-lookup"><span data-stu-id="290b8-191">IsDeliveryReceiptRequested</span></span>](isdeliveryreceiptrequested.md) <br/> |<span data-ttu-id="290b8-192">Указывает, запрашивает ли отправитель элемента уведомление о доставке.</span><span class="sxs-lookup"><span data-stu-id="290b8-192">Indicates whether the sender of an item requests a delivery receipt.</span></span>  <br/> |
|[<span data-ttu-id="290b8-193">ConversationIndex</span><span class="sxs-lookup"><span data-stu-id="290b8-193">ConversationIndex</span></span>](conversationindex.md) <br/> |<span data-ttu-id="290b8-194">Содержит двоичный код, представляющий поток, к которому относится сообщение.</span><span class="sxs-lookup"><span data-stu-id="290b8-194">Contains a binary ID that represents the thread to which this message belongs.</span></span>  <br/> |
|[<span data-ttu-id="290b8-195">ConversationTopic</span><span class="sxs-lookup"><span data-stu-id="290b8-195">ConversationTopic</span></span>](conversationtopic.md) <br/> |<span data-ttu-id="290b8-196">Представляет идентификатор беседы.</span><span class="sxs-lookup"><span data-stu-id="290b8-196">Represents the conversation identifier.</span></span>  <br/> |
|[<span data-ttu-id="290b8-197">From</span><span class="sxs-lookup"><span data-stu-id="290b8-197">From</span></span>](from.md) <br/> |<span data-ttu-id="290b8-198">Представляет адрес получателя, от которого было отправлено сообщение.</span><span class="sxs-lookup"><span data-stu-id="290b8-198">Represents the addressee from whom the message was sent.</span></span>  <br/> |
|[<span data-ttu-id="290b8-199">InternetMessageId</span><span class="sxs-lookup"><span data-stu-id="290b8-199">InternetMessageId</span></span>](internetmessageid.md) <br/> |<span data-ttu-id="290b8-200">Представляет идентификатор сообщения Интернета для элемента.</span><span class="sxs-lookup"><span data-stu-id="290b8-200">Represents the Internet message identifier of an item.</span></span>  <br/> |
|[<span data-ttu-id="290b8-201">IsRead</span><span class="sxs-lookup"><span data-stu-id="290b8-201">IsRead</span></span>](isread.md) <br/> |<span data-ttu-id="290b8-202">Указывает, было ли Прочитано сообщение.</span><span class="sxs-lookup"><span data-stu-id="290b8-202">Indicates whether a message has been read.</span></span>  <br/> |
|[<span data-ttu-id="290b8-203">исреспонсерекуестед</span><span class="sxs-lookup"><span data-stu-id="290b8-203">IsResponseRequested</span></span>](isresponserequested.md) <br/> |<span data-ttu-id="290b8-204">Указывает, запрашивается ли ответ на сообщение электронной почты.</span><span class="sxs-lookup"><span data-stu-id="290b8-204">Indicates whether a response to an e-mail message is requested.</span></span>  <br/> |
|[<span data-ttu-id="290b8-205">References</span><span class="sxs-lookup"><span data-stu-id="290b8-205">References</span></span>](references.md) <br/> |<span data-ttu-id="290b8-206">Представляет заголовок Usenet, используемый для сопоставления ответов с их исходными сообщениями.</span><span class="sxs-lookup"><span data-stu-id="290b8-206">Represents the Usenet header that is used to correlate replies with their original messages.</span></span>  <br/> |
|[<span data-ttu-id="290b8-207">ReplyTo</span><span class="sxs-lookup"><span data-stu-id="290b8-207">ReplyTo</span></span>](replyto.md) <br/> |<span data-ttu-id="290b8-208">Определяет набор адресов, в который отправляются ответы.</span><span class="sxs-lookup"><span data-stu-id="290b8-208">Identifies a set of addresses to which replies should be sent.</span></span>  <br/> |
|[<span data-ttu-id="290b8-209">ассоЦиатедкалендаритемид</span><span class="sxs-lookup"><span data-stu-id="290b8-209">AssociatedCalendarItemId</span></span>](associatedcalendaritemid.md) <br/> |<span data-ttu-id="290b8-210">Представляет элемент календаря, связанный с объектом [митингмессаже](meetingmessage.md).</span><span class="sxs-lookup"><span data-stu-id="290b8-210">Represents the calendar item that is associated with a [MeetingMessage](meetingmessage.md).</span></span>  <br/> |
|[<span data-ttu-id="290b8-211">Isdelegated для</span><span class="sxs-lookup"><span data-stu-id="290b8-211">IsDelegated</span></span>](isdelegated.md) <br/> |<span data-ttu-id="290b8-212">Указывает, было ли собрание обработано с помощью учетной записи с делегированным доступом.</span><span class="sxs-lookup"><span data-stu-id="290b8-212">Indicates whether a meeting was handled by an account with delegate access.</span></span>  <br/> |
|[<span data-ttu-id="290b8-213">IsOutOfDate</span><span class="sxs-lookup"><span data-stu-id="290b8-213">IsOutOfDate</span></span>](isoutofdate.md) <br/> |<span data-ttu-id="290b8-214">Указывает, является ли сообщение о собрании устаревшим.</span><span class="sxs-lookup"><span data-stu-id="290b8-214">Indicates whether a meeting message is out-of-date.</span></span>  <br/> |
|[<span data-ttu-id="290b8-215">хасбинпроцессед</span><span class="sxs-lookup"><span data-stu-id="290b8-215">HasBeenProcessed</span></span>](hasbeenprocessed.md) <br/> |<span data-ttu-id="290b8-216">Указывает, был ли обработан элемент сообщения о собрании.</span><span class="sxs-lookup"><span data-stu-id="290b8-216">Indicates whether a meeting message item has been processed.</span></span>  <br/> |
|[<span data-ttu-id="290b8-217">ResponseType</span><span class="sxs-lookup"><span data-stu-id="290b8-217">ResponseType</span></span>](responsetype.md) <br/> |<span data-ttu-id="290b8-218">Представляет тип ответа получателя, полученный для собрания.</span><span class="sxs-lookup"><span data-stu-id="290b8-218">Represents the type of recipient response that is received for a meeting.</span></span>  <br/> |
|[<span data-ttu-id="290b8-219">еффективеригхтс</span><span class="sxs-lookup"><span data-stu-id="290b8-219">EffectiveRights</span></span>](effectiverights.md) <br/> |<span data-ttu-id="290b8-220">Содержит права клиента на основе параметров разрешений для элемента или папки.</span><span class="sxs-lookup"><span data-stu-id="290b8-220">Contains the client's rights based on the permission settings for the item or folder.</span></span> <span data-ttu-id="290b8-221">Этот элемент доступен только для чтения.</span><span class="sxs-lookup"><span data-stu-id="290b8-221">This element is read-only.</span></span> <span data-ttu-id="290b8-222">Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="290b8-222">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span>  <br/> |
|[<span data-ttu-id="290b8-223">рецеиведби</span><span class="sxs-lookup"><span data-stu-id="290b8-223">ReceivedBy</span></span>](receivedby.md) <br/> |<span data-ttu-id="290b8-224">Определяет делегат в сценарии доступа делегата.</span><span class="sxs-lookup"><span data-stu-id="290b8-224">Identifies the delegate in a delegate access scenario.</span></span> <span data-ttu-id="290b8-225">Этот элемент появился в Exchange 2007 с пакетом обновления 1.</span><span class="sxs-lookup"><span data-stu-id="290b8-225">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="290b8-226">рецеиведрепресентинг</span><span class="sxs-lookup"><span data-stu-id="290b8-226">ReceivedRepresenting</span></span>](receivedrepresenting.md) <br/> |<span data-ttu-id="290b8-227">Определяет участника в сценарии доступа делегата.</span><span class="sxs-lookup"><span data-stu-id="290b8-227">Identifies the principal in a delegate access scenario.</span></span> <span data-ttu-id="290b8-228">Этот элемент появился в Exchange 2007 с пакетом обновления 1.</span><span class="sxs-lookup"><span data-stu-id="290b8-228">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="290b8-229">UID</span><span class="sxs-lookup"><span data-stu-id="290b8-229">UID</span></span>](uid.md) <br/> |<span data-ttu-id="290b8-230">Определяет элемент календаря.</span><span class="sxs-lookup"><span data-stu-id="290b8-230">Identifies a calendar item.</span></span>  <br/> |
|[<span data-ttu-id="290b8-231">рекурренцеид</span><span class="sxs-lookup"><span data-stu-id="290b8-231">RecurrenceId</span></span>](recurrenceid.md) <br/> |<span data-ttu-id="290b8-232">Используется для идентификации определенного экземпляра повторяющегося элемента календаря.</span><span class="sxs-lookup"><span data-stu-id="290b8-232">Used to identify a specific instance of a recurring calendar item.</span></span>  <br/> |
|[<span data-ttu-id="290b8-233">датетиместамп</span><span class="sxs-lookup"><span data-stu-id="290b8-233">DateTimeStamp</span></span>](datetimestamp.md) <br/> |<span data-ttu-id="290b8-234">Указывает дату и время создания экземпляра объекта iCalendar.</span><span class="sxs-lookup"><span data-stu-id="290b8-234">Indicates the date and time that an instance of an iCalendar object was created.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="290b8-235">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="290b8-235">Parent elements</span></span>

|<span data-ttu-id="290b8-236">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="290b8-236">**Element**</span></span>|<span data-ttu-id="290b8-237">**Описание**</span><span class="sxs-lookup"><span data-stu-id="290b8-237">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="290b8-238">аджацентмитингс</span><span class="sxs-lookup"><span data-stu-id="290b8-238">AdjacentMeetings</span></span>](adjacentmeetings.md) <br/> |<span data-ttu-id="290b8-239">Определяет все элементы календаря, смежные с временем собрания.</span><span class="sxs-lookup"><span data-stu-id="290b8-239">Identifies all calendar items that are adjacent to a meeting time.</span></span>  <br/> |
|[<span data-ttu-id="290b8-240">аппендтоитемфиелд</span><span class="sxs-lookup"><span data-stu-id="290b8-240">AppendToItemField</span></span>](appendtoitemfield.md) <br/> |<span data-ttu-id="290b8-241">Определяет данные, добавляемые к одному свойству элемента во время [операции UpdateItem](updateitem-operation.md).</span><span class="sxs-lookup"><span data-stu-id="290b8-241">Identifies data to append to a single property of an item during an [UpdateItem operation](updateitem-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="290b8-242">конфликтингмитингс</span><span class="sxs-lookup"><span data-stu-id="290b8-242">ConflictingMeetings</span></span>](conflictingmeetings.md) <br/> |<span data-ttu-id="290b8-243">Определяет все элементы, которые конфликтуют с временем собрания.</span><span class="sxs-lookup"><span data-stu-id="290b8-243">Identifies all items that conflict with a meeting time.</span></span>  <br/> |
|[<span data-ttu-id="290b8-244">Create (Итемсинк)</span><span class="sxs-lookup"><span data-stu-id="290b8-244">Create (ItemSync)</span></span>](create-itemsync.md) <br/> |<span data-ttu-id="290b8-245">Определяет один элемент, который необходимо создать в локальном хранилище клиента.</span><span class="sxs-lookup"><span data-stu-id="290b8-245">Identifies a single item to create in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="290b8-246">Items</span><span class="sxs-lookup"><span data-stu-id="290b8-246">Items</span></span>](items.md) <br/> |<span data-ttu-id="290b8-247">Содержит массив элементов.</span><span class="sxs-lookup"><span data-stu-id="290b8-247">Contains an array of items.</span></span>  <br/> |
|[<span data-ttu-id="290b8-248">Элементы (Нонемптяррайофаллитемстипе)</span><span class="sxs-lookup"><span data-stu-id="290b8-248">Items (NonEmptyArrayOfAllItemsType)</span></span>](items-nonemptyarrayofallitemstype.md) <br/> |<span data-ttu-id="290b8-249">Содержит массив создаваемых элементов.</span><span class="sxs-lookup"><span data-stu-id="290b8-249">Contains an array of items to create.</span></span>  <br/> |
|[<span data-ttu-id="290b8-250">ItemAttachment</span><span class="sxs-lookup"><span data-stu-id="290b8-250">ItemAttachment</span></span>](itemattachment.md) <br/> |<span data-ttu-id="290b8-251">Представляет элемент Exchange, присоединенный к другому элементу Exchange.</span><span class="sxs-lookup"><span data-stu-id="290b8-251">Represents an Exchange item that is attached to another Exchange item.</span></span>  <br/> |
|[<span data-ttu-id="290b8-252">сетитемфиелд</span><span class="sxs-lookup"><span data-stu-id="290b8-252">SetItemField</span></span>](setitemfield.md) <br/> |<span data-ttu-id="290b8-253">Представляет обновление одного свойства элемента в [операции UpdateItem](updateitem-operation.md).</span><span class="sxs-lookup"><span data-stu-id="290b8-253">Represents an update to a single property of an item in an [UpdateItem operation](updateitem-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="290b8-254">Обновление (Итемсинк)</span><span class="sxs-lookup"><span data-stu-id="290b8-254">Update (ItemSync)</span></span>](update-itemsync.md) <br/> |<span data-ttu-id="290b8-255">Определяет один элемент для обновления в локальном хранилище клиента.</span><span class="sxs-lookup"><span data-stu-id="290b8-255">Identifies a single item to update in the local client store.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="290b8-256">Примечания</span><span class="sxs-lookup"><span data-stu-id="290b8-256">Remarks</span></span>

<span data-ttu-id="290b8-257">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="290b8-257">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="290b8-258">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="290b8-258">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="290b8-259">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="290b8-259">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="290b8-260">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="290b8-260">Schema Name</span></span>  <br/> |<span data-ttu-id="290b8-261">Схема Types</span><span class="sxs-lookup"><span data-stu-id="290b8-261">Types schema</span></span>  <br/> |
|<span data-ttu-id="290b8-262">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="290b8-262">Validation File</span></span>  <br/> |<span data-ttu-id="290b8-263">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="290b8-263">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="290b8-264">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="290b8-264">Can be Empty</span></span>  <br/> |<span data-ttu-id="290b8-265">False</span><span class="sxs-lookup"><span data-stu-id="290b8-265">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="290b8-266">См. также</span><span class="sxs-lookup"><span data-stu-id="290b8-266">See also</span></span>



- [<span data-ttu-id="290b8-267">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="290b8-267">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

