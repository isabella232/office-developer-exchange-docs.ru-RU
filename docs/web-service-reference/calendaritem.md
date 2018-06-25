---
title: Элемента календаря, имеющего
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CalendarItem
api_type:
- schema
ms.assetid: b0c1fd27-b6da-46e5-88b8-88f00c71ba80
description: Элемент элемента календаря, имеющего представляет собой элемент календаря Exchange.
ms.openlocfilehash: c7b6d4930bc42fbe26d35264e2eae0c986cc8db7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761648"
---
# <a name="calendaritem"></a><span data-ttu-id="513a2-103">Элемента календаря, имеющего</span><span class="sxs-lookup"><span data-stu-id="513a2-103">CalendarItem</span></span>

<span data-ttu-id="513a2-104">Элемент **элемента календаря, имеющего** представляет собой элемент календаря Exchange.</span><span class="sxs-lookup"><span data-stu-id="513a2-104">The **CalendarItem** element represents an Exchange calendar item.</span></span> 
  
```XML
<CalendarItem>
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
   <Start/>
   <End/>
   <OriginalStart/>
   <IsAllDayEvent/>
   <LegacyFreeBusyStatus/>
   <Location/>
   <When/>
   <IsMeeting/>
   <IsCancelled/>
   <IsRecurring/>
   <MeetingRequestWasSent/>
   <IsResponseRequested/>
   <CalendarItemType/>
   <MyResponseType/>
   <Organizer/>
   <RequiredAttendees/>
   <OptionalAttendees/>
   <Resources/>
   <ConflictingMeetingCount/>
   <AdjacentMeetingCount/>
   <ConflictingMeetings/>
   <AdjacentMeetings/>
   <Duration/>
   <TimeZone/>
   <AppointmentReplyTime/>
   <AppointmentSequenceNumber/>
   <AppointmentState/>
   <Recurrence/>
   <FirstOccurrence/>
   <LastOccurrence/>
   <ModifiedOccurrences/>
   <DeletedOccurrences/>
   <MeetingTimeZone/>
   <StartTimeZone/>
   <EndTimeZone/>
   <ConferenceType/>
   <AllowNewTimeProposal/>
   <IsOnlineMeeting/>
   <MeetingWorkspaceUrl/>
   <NetShowUrl/>
   <EffectiveRights/>
   <LastModifiedName/>
   <LastModifiedTime/>
   <IsAssociated/>
   <WebClientReadFormQueryString/>
   <WebClientEditFormQueryString/>
   <ConversationId/>
   <UniqueBody/>
</CalendarItem>
```

 <span data-ttu-id="513a2-105">**CalendarItemType**</span><span class="sxs-lookup"><span data-stu-id="513a2-105">**CalendarItemType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="513a2-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="513a2-106">Attributes and elements</span></span>

<span data-ttu-id="513a2-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="513a2-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="513a2-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="513a2-108">Attributes</span></span>

<span data-ttu-id="513a2-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="513a2-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="513a2-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="513a2-110">Child elements</span></span>

|<span data-ttu-id="513a2-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="513a2-111">**Element**</span></span>|<span data-ttu-id="513a2-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="513a2-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="513a2-113">MimeContent</span><span class="sxs-lookup"><span data-stu-id="513a2-113">MimeContent</span></span>](mimecontent.md) <br/> |<span data-ttu-id="513a2-114">Содержит собственный поток Multipurpose Internet Mail Extensions (MIME), представленного в формате base64Binary объекта.</span><span class="sxs-lookup"><span data-stu-id="513a2-114">Contains the native Multipurpose Internet Mail Extensions (MIME) stream of an object that is represented in base64Binary format.</span></span>  <br/> |
|[<span data-ttu-id="513a2-115">Идентификатор элемента</span><span class="sxs-lookup"><span data-stu-id="513a2-115">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="513a2-116">Содержит уникальный идентификатор и меняет ключ элемента в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="513a2-116">Contains the unique identifier and change key of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="513a2-117">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="513a2-117">ParentFolderId</span></span>](parentfolderid.md) <br/> |<span data-ttu-id="513a2-118">Представляет идентификатор родительской папки, содержащей элемент или папку.</span><span class="sxs-lookup"><span data-stu-id="513a2-118">Represents the identifier of the parent folder that contains the item or folder.</span></span>  <br/> |
|[<span data-ttu-id="513a2-119">ItemClass</span><span class="sxs-lookup"><span data-stu-id="513a2-119">ItemClass</span></span>](itemclass.md) <br/> |<span data-ttu-id="513a2-120">Представляет класс сообщения элемента.</span><span class="sxs-lookup"><span data-stu-id="513a2-120">Represents the message class of an item.</span></span>  <br/> |
|[<span data-ttu-id="513a2-121">Subject</span><span class="sxs-lookup"><span data-stu-id="513a2-121">Subject</span></span>](subject.md) <br/> |<span data-ttu-id="513a2-122">Представляет тему для элементов хранилища Exchange и объекты ответа.</span><span class="sxs-lookup"><span data-stu-id="513a2-122">Represents the subject for Exchange store items and response objects.</span></span>  <br/> |
|[<span data-ttu-id="513a2-123">Уровень конфиденциальности сообщения</span><span class="sxs-lookup"><span data-stu-id="513a2-123">Sensitivity</span></span>](sensitivity.md) <br/> |<span data-ttu-id="513a2-124">Указывает уровень конфиденциальности для элемента.</span><span class="sxs-lookup"><span data-stu-id="513a2-124">Indicates the sensitivity level of an item.</span></span>  <br/> |
|[<span data-ttu-id="513a2-125">Body</span><span class="sxs-lookup"><span data-stu-id="513a2-125">Body</span></span>](body.md) <br/> |<span data-ttu-id="513a2-126">Представляет фактическое содержимое основного текста сообщения.</span><span class="sxs-lookup"><span data-stu-id="513a2-126">Represents the actual body content of a message.</span></span>  <br/> |
|[<span data-ttu-id="513a2-127">Вложения</span><span class="sxs-lookup"><span data-stu-id="513a2-127">Attachments</span></span>](attachments-ex15websvcsotherref.md) <br/> |<span data-ttu-id="513a2-128">Содержит элементы или файлы, подключенные к элементу в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="513a2-128">Contains the items or files that are attached to an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="513a2-129">DateTimeReceived</span><span class="sxs-lookup"><span data-stu-id="513a2-129">DateTimeReceived</span></span>](datetimereceived.md) <br/> |<span data-ttu-id="513a2-130">Представляет дату и время получения элемента в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="513a2-130">Represents the date and time that an item in a mailbox was received.</span></span>  <br/> |
|[<span data-ttu-id="513a2-131">Размер</span><span class="sxs-lookup"><span data-stu-id="513a2-131">Size</span></span>](size.md) <br/> |<span data-ttu-id="513a2-132">Представляет размер в байтах элемента.</span><span class="sxs-lookup"><span data-stu-id="513a2-132">Represents the size in bytes of an item.</span></span> <span data-ttu-id="513a2-133">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="513a2-133">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="513a2-134">Категории</span><span class="sxs-lookup"><span data-stu-id="513a2-134">Categories</span></span>](categories-ex15websvcsotherref.md) <br/> |<span data-ttu-id="513a2-135">Представляет набор строк, которые определяют категории, к которым принадлежит элемент в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="513a2-135">Represents a collection of strings that identify the categories to which an item in the mailbox belongs.</span></span>  <br/> |
|[<span data-ttu-id="513a2-136">Важность</span><span class="sxs-lookup"><span data-stu-id="513a2-136">Importance</span></span>](importance.md) <br/> |<span data-ttu-id="513a2-137">Описывает важность элемента.</span><span class="sxs-lookup"><span data-stu-id="513a2-137">Describes the importance of an item.</span></span>  <br/> |
|[<span data-ttu-id="513a2-138">InReplyTo</span><span class="sxs-lookup"><span data-stu-id="513a2-138">InReplyTo</span></span>](inreplyto.md) <br/> |<span data-ttu-id="513a2-139">Представляет идентификатор элемента, к которому этот элемент является ее в ответ.</span><span class="sxs-lookup"><span data-stu-id="513a2-139">Represents the identifier of the item to which this item is a reply.</span></span>  <br/> |
|[<span data-ttu-id="513a2-140">IsSubmitted</span><span class="sxs-lookup"><span data-stu-id="513a2-140">IsSubmitted</span></span>](issubmitted.md) <br/> |<span data-ttu-id="513a2-141">Указывает, является ли элемент был отправлен исходящие папке по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="513a2-141">Indicates whether an item has been submitted to the Outbox default folder.</span></span>  <br/> |
|[<span data-ttu-id="513a2-142">IsDraft</span><span class="sxs-lookup"><span data-stu-id="513a2-142">IsDraft</span></span>](isdraft.md) <br/> |<span data-ttu-id="513a2-143">Указывает, является ли элемент еще не были отправлены.</span><span class="sxs-lookup"><span data-stu-id="513a2-143">Indicates whether an item has not yet been sent.</span></span>  <br/> |
|[<span data-ttu-id="513a2-144">IsFromMe</span><span class="sxs-lookup"><span data-stu-id="513a2-144">IsFromMe</span></span>](isfromme.md) <br/> |<span data-ttu-id="513a2-145">Указывает, отправил ли пользователь элемента для его сами себя.</span><span class="sxs-lookup"><span data-stu-id="513a2-145">Indicates whether a user sent an item to him or herself.</span></span>  <br/> |
|[<span data-ttu-id="513a2-146">IsResend</span><span class="sxs-lookup"><span data-stu-id="513a2-146">IsResend</span></span>](isresend.md) <br/> |<span data-ttu-id="513a2-147">Указывает, является ли элемент ранее еще был отправлен.</span><span class="sxs-lookup"><span data-stu-id="513a2-147">Indicates whether the item had previously been sent.</span></span>  <br/> |
|[<span data-ttu-id="513a2-148">IsUnmodified</span><span class="sxs-lookup"><span data-stu-id="513a2-148">IsUnmodified</span></span>](isunmodified.md) <br/> |<span data-ttu-id="513a2-149">Указывает, были ли изменены элемента.</span><span class="sxs-lookup"><span data-stu-id="513a2-149">Indicates whether the item has been modified.</span></span>  <br/> |
|[<span data-ttu-id="513a2-150">InternetMessageHeaders</span><span class="sxs-lookup"><span data-stu-id="513a2-150">InternetMessageHeaders</span></span>](internetmessageheaders.md) <br/> |<span data-ttu-id="513a2-151">Представляет коллекцию всех заголовков сообщений Интернета, содержащихся в элемента в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="513a2-151">Represents the collection of all Internet message headers that are contained in an item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="513a2-152">DateTimeSent</span><span class="sxs-lookup"><span data-stu-id="513a2-152">DateTimeSent</span></span>](datetimesent.md) <br/> |<span data-ttu-id="513a2-153">Представляет дату и время отправки элемента в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="513a2-153">Represents the date and time that an item in a mailbox was sent.</span></span>  <br/> |
|[<span data-ttu-id="513a2-154">DateTimeCreated</span><span class="sxs-lookup"><span data-stu-id="513a2-154">DateTimeCreated</span></span>](datetimecreated.md) <br/> |<span data-ttu-id="513a2-155">Представляет дату и время создания данного элемента в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="513a2-155">Represents the date and time that a given item in the mailbox was created.</span></span>  <br/> |
|[<span data-ttu-id="513a2-156">ResponseObjects</span><span class="sxs-lookup"><span data-stu-id="513a2-156">ResponseObjects</span></span>](responseobjects.md) <br/> |<span data-ttu-id="513a2-157">Содержит коллекцию всех объектов ответа, которые связаны с элемента в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="513a2-157">Contains a collection of all the response objects that are associated with an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="513a2-158">ReminderDueBy</span><span class="sxs-lookup"><span data-stu-id="513a2-158">ReminderDueBy</span></span>](reminderdueby.md) <br/> |<span data-ttu-id="513a2-159">Представляет дату и время, когда происходит событие.</span><span class="sxs-lookup"><span data-stu-id="513a2-159">Represents the date and time when the event occurs.</span></span> <span data-ttu-id="513a2-160">Используется в элементе [ReminderMinutesBeforeStart](reminderminutesbeforestart.md) определить, когда отображается оповещение.</span><span class="sxs-lookup"><span data-stu-id="513a2-160">This is used by the [ReminderMinutesBeforeStart](reminderminutesbeforestart.md) element to determine when the reminder is displayed.</span></span>  <br/> |
|[<span data-ttu-id="513a2-161">ReminderIsSet</span><span class="sxs-lookup"><span data-stu-id="513a2-161">ReminderIsSet</span></span>](reminderisset.md) <br/> |<span data-ttu-id="513a2-162">Указывает, установлен ли напоминания для элемента в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="513a2-162">Indicates whether a reminder has been set for an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="513a2-163">ReminderMinutesBeforeStart</span><span class="sxs-lookup"><span data-stu-id="513a2-163">ReminderMinutesBeforeStart</span></span>](reminderminutesbeforestart.md) <br/> |<span data-ttu-id="513a2-164">Представляет число минут и только потом событие, когда отображается напоминание.</span><span class="sxs-lookup"><span data-stu-id="513a2-164">Represents the number of minutes before an event when a reminder is displayed.</span></span>  <br/> |
|[<span data-ttu-id="513a2-165">DisplayCc</span><span class="sxs-lookup"><span data-stu-id="513a2-165">DisplayCc</span></span>](displaycc.md) <br/> |<span data-ttu-id="513a2-166">Строка отображения, который используется для содержимого строку "Копия".</span><span class="sxs-lookup"><span data-stu-id="513a2-166">Represents the display string that is used for the contents of the Cc line.</span></span> <span data-ttu-id="513a2-167">Это составное строка всех получателей отображаемые имена «копия».</span><span class="sxs-lookup"><span data-stu-id="513a2-167">This is the concatenated string of all Cc recipient display names.</span></span>  <br/> |
|[<span data-ttu-id="513a2-168">DisplayTo</span><span class="sxs-lookup"><span data-stu-id="513a2-168">DisplayTo</span></span>](displayto.md) <br/> |<span data-ttu-id="513a2-169">Строка отображения, который используется для содержимого строке.</span><span class="sxs-lookup"><span data-stu-id="513a2-169">Represents the display string that is used for the contents of the To line.</span></span> <span data-ttu-id="513a2-170">Это составное строка всех для получателей отображаемые имена.</span><span class="sxs-lookup"><span data-stu-id="513a2-170">This is the concatenated string of all To recipient display names.</span></span>  <br/> |
|[<span data-ttu-id="513a2-171">HasAttachments</span><span class="sxs-lookup"><span data-stu-id="513a2-171">HasAttachments</span></span>](hasattachments.md) <br/> |<span data-ttu-id="513a2-172">Представляет свойство, которое задано значение **true,** Если у элемента есть по крайней мере один видимым вложения.</span><span class="sxs-lookup"><span data-stu-id="513a2-172">Represents a property that is set to **true** if an item has at least one visible attachment.</span></span> <span data-ttu-id="513a2-173">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="513a2-173">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="513a2-174">ExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="513a2-174">ExtendedProperty</span></span>](extendedproperty.md) <br/> |<span data-ttu-id="513a2-175">Определяет расширенные свойства для папок и элементов.</span><span class="sxs-lookup"><span data-stu-id="513a2-175">Identifies extended properties on folders and items.</span></span>  <br/> |
|[<span data-ttu-id="513a2-176">Язык и региональные параметры</span><span class="sxs-lookup"><span data-stu-id="513a2-176">Culture</span></span>](culture.md) <br/> |<span data-ttu-id="513a2-177">Представляет язык и региональные параметры для заданного элемента в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="513a2-177">Represents the culture for a given item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="513a2-178">ИД ПОЛЬЗОВАТЕЛЯ</span><span class="sxs-lookup"><span data-stu-id="513a2-178">UID</span></span>](uid.md) <br/> |<span data-ttu-id="513a2-179">Идентифицирует элемент календаря.</span><span class="sxs-lookup"><span data-stu-id="513a2-179">Identifies a calendar item.</span></span>  <br/> |
|[<span data-ttu-id="513a2-180">RecurrenceId</span><span class="sxs-lookup"><span data-stu-id="513a2-180">RecurrenceId</span></span>](recurrenceid.md) <br/> |<span data-ttu-id="513a2-181">Используется для идентификации определенный экземпляр повторяющегося элемента календаря.</span><span class="sxs-lookup"><span data-stu-id="513a2-181">Used to identify a specific instance of a recurring calendar item.</span></span>  <br/> |
|[<span data-ttu-id="513a2-182">DateTimeStamp</span><span class="sxs-lookup"><span data-stu-id="513a2-182">DateTimeStamp</span></span>](datetimestamp.md) <br/> |<span data-ttu-id="513a2-183">Указывает дату и время создания экземпляра объекта iCalendar.</span><span class="sxs-lookup"><span data-stu-id="513a2-183">Indicates the date and time that an instance of a iCalendar object was created.</span></span>  <br/> |
|[<span data-ttu-id="513a2-184">Start</span><span class="sxs-lookup"><span data-stu-id="513a2-184">Start</span></span>](start.md) <br/> |<span data-ttu-id="513a2-185">Представляет начало элемента календаря.</span><span class="sxs-lookup"><span data-stu-id="513a2-185">Represents the start of a calendar item.</span></span> <span data-ttu-id="513a2-186">Этот элемент применяется только для одного экземпляра элемента календаря.</span><span class="sxs-lookup"><span data-stu-id="513a2-186">This element only applies to a single occurrence of a calendar item.</span></span>  <br/> |
|[<span data-ttu-id="513a2-187">End</span><span class="sxs-lookup"><span data-stu-id="513a2-187">End </span></span>](end-ex15websvcsotherref.md) <br/> |<span data-ttu-id="513a2-188">Представляет конец длительность.</span><span class="sxs-lookup"><span data-stu-id="513a2-188">Represents the end of a duration.</span></span> <span data-ttu-id="513a2-189">Этот элемент применяется только для одного экземпляра элемента календаря.</span><span class="sxs-lookup"><span data-stu-id="513a2-189">This element only applies to a single occurrence of a calendar item.</span></span>  <br/> |
|[<span data-ttu-id="513a2-190">OriginalStart</span><span class="sxs-lookup"><span data-stu-id="513a2-190">OriginalStart</span></span>](originalstart.md) <br/> |<span data-ttu-id="513a2-191">Представляет исходное время начала элемента календаря.</span><span class="sxs-lookup"><span data-stu-id="513a2-191">Represents the original start time of a calendar item.</span></span>  <br/> |
|[<span data-ttu-id="513a2-192">IsAllDayEvent</span><span class="sxs-lookup"><span data-stu-id="513a2-192">IsAllDayEvent</span></span>](isalldayevent.md) <br/> |<span data-ttu-id="513a2-193">Указывает тип календаря элемента или приглашения на собрание событием на целый день.</span><span class="sxs-lookup"><span data-stu-id="513a2-193">Indicates whether a calendar item or meeting request represents an all-day event.</span></span>  <br/> |
|[<span data-ttu-id="513a2-194">LegacyFreeBusyStatus</span><span class="sxs-lookup"><span data-stu-id="513a2-194">LegacyFreeBusyStatus</span></span>](legacyfreebusystatus.md) <br/> |<span data-ttu-id="513a2-195">Представляет состояния занятости элемента календаря.</span><span class="sxs-lookup"><span data-stu-id="513a2-195">Represents the free/busy status of the calendar item.</span></span>  <br/> |
|[<span data-ttu-id="513a2-196">Location</span><span class="sxs-lookup"><span data-stu-id="513a2-196">Location</span></span>](location.md) <br/> |<span data-ttu-id="513a2-197">Представляет место собрания или встречи.</span><span class="sxs-lookup"><span data-stu-id="513a2-197">Represents the location of a meeting or appointment.</span></span>  <br/> |
|[<span data-ttu-id="513a2-198">Когда</span><span class="sxs-lookup"><span data-stu-id="513a2-198">When</span></span>](when.md) <br/> |<span data-ttu-id="513a2-199">Предоставляет сведения о при возникновении элемента календаря.</span><span class="sxs-lookup"><span data-stu-id="513a2-199">Provides information about when a calendar item occurs.</span></span>  <br/> |
|[<span data-ttu-id="513a2-200">IsMeeting</span><span class="sxs-lookup"><span data-stu-id="513a2-200">IsMeeting</span></span>](ismeeting.md) <br/> |<span data-ttu-id="513a2-201">Указывает, является ли элемент календаря собрания или встречи.</span><span class="sxs-lookup"><span data-stu-id="513a2-201">Indicates whether the calendar item is a meeting or appointment.</span></span>  <br/> |
|[<span data-ttu-id="513a2-202">IsCancelled</span><span class="sxs-lookup"><span data-stu-id="513a2-202">IsCancelled</span></span>](iscancelled.md) <br/> |<span data-ttu-id="513a2-203">Указывает, была ли отменена встречи или собрания.</span><span class="sxs-lookup"><span data-stu-id="513a2-203">Indicates whether an appointment or meeting has been canceled.</span></span>  <br/> |
|[<span data-ttu-id="513a2-204">IsRecurring</span><span class="sxs-lookup"><span data-stu-id="513a2-204">IsRecurring</span></span>](isrecurring.md) <br/> |<span data-ttu-id="513a2-205">Указывает, является ли элемент календаря часть повторяющегося элемента.</span><span class="sxs-lookup"><span data-stu-id="513a2-205">Indicates whether a calendar item is part of a recurring item.</span></span> <span data-ttu-id="513a2-206">Этот элемент доступен только для чтения.</span><span class="sxs-lookup"><span data-stu-id="513a2-206">This element is read-only.</span></span>  <br/> |
|[<span data-ttu-id="513a2-207">MeetingRequestWasSent</span><span class="sxs-lookup"><span data-stu-id="513a2-207">MeetingRequestWasSent</span></span>](meetingrequestwassent.md) <br/> |<span data-ttu-id="513a2-208">Указывает, был ли отправлен приглашения на собрание запрошенные участникам.</span><span class="sxs-lookup"><span data-stu-id="513a2-208">Indicates whether a meeting request has been sent to requested attendees.</span></span>  <br/> |
|[<span data-ttu-id="513a2-209">IsResponseRequested</span><span class="sxs-lookup"><span data-stu-id="513a2-209">IsResponseRequested</span></span>](isresponserequested.md) <br/> |<span data-ttu-id="513a2-210">Указывает, требуется ли ответа на элемент.</span><span class="sxs-lookup"><span data-stu-id="513a2-210">Indicates whether a response to an item is required.</span></span>  <br/> |
|[<span data-ttu-id="513a2-211">CalendarItemType</span><span class="sxs-lookup"><span data-stu-id="513a2-211">CalendarItemType</span></span>](calendaritemtype.md) <br/> |<span data-ttu-id="513a2-212">Представляет тип вхождение элемента календаря.</span><span class="sxs-lookup"><span data-stu-id="513a2-212">Represents the occurrence type of a calendar item.</span></span>  <br/> |
|[<span data-ttu-id="513a2-213">MyResponseType</span><span class="sxs-lookup"><span data-stu-id="513a2-213">MyResponseType</span></span>](myresponsetype.md) <br/> |<span data-ttu-id="513a2-214">Содержит состояние или ответа на элемент календаря.</span><span class="sxs-lookup"><span data-stu-id="513a2-214">Contains the status of or response to a calendar item.</span></span>  <br/> |
|[<span data-ttu-id="513a2-215">Организатор</span><span class="sxs-lookup"><span data-stu-id="513a2-215">Organizer</span></span>](organizer.md) <br/> |<span data-ttu-id="513a2-216">Представляет организатора собрания.</span><span class="sxs-lookup"><span data-stu-id="513a2-216">Represents the organizer of a meeting.</span></span>  <br/> |
|[<span data-ttu-id="513a2-217">RequiredAttendees</span><span class="sxs-lookup"><span data-stu-id="513a2-217">RequiredAttendees</span></span>](requiredattendees.md) <br/> |<span data-ttu-id="513a2-218">Представляет участников, которые необходимы на участие в собрании.</span><span class="sxs-lookup"><span data-stu-id="513a2-218">Represents attendees that are required to attend a meeting.</span></span>  <br/> |
|[<span data-ttu-id="513a2-219">OptionalAttendees</span><span class="sxs-lookup"><span data-stu-id="513a2-219">OptionalAttendees</span></span>](optionalattendees.md) <br/> |<span data-ttu-id="513a2-220">Представляет участников, которые не требуется на участие в собрании.</span><span class="sxs-lookup"><span data-stu-id="513a2-220">Represents attendees that are not required to attend a meeting.</span></span>  <br/> |
|[<span data-ttu-id="513a2-221">Ресурсы</span><span class="sxs-lookup"><span data-stu-id="513a2-221">Resources</span></span>](resources.md) <br/> |<span data-ttu-id="513a2-222">Ресурс запланированного собрания.</span><span class="sxs-lookup"><span data-stu-id="513a2-222">Represents a scheduled resource for a meeting.</span></span>  <br/> |
|[<span data-ttu-id="513a2-223">ConflictingMeetingCount</span><span class="sxs-lookup"><span data-stu-id="513a2-223">ConflictingMeetingCount</span></span>](conflictingmeetingcount.md) <br/> |<span data-ttu-id="513a2-224">Представляет число собраний, конфликтующие с элемента календаря.</span><span class="sxs-lookup"><span data-stu-id="513a2-224">Represents the number of meetings that conflict with the calendar item.</span></span>  <br/> |
|[<span data-ttu-id="513a2-225">AdjacentMeetingCount</span><span class="sxs-lookup"><span data-stu-id="513a2-225">AdjacentMeetingCount</span></span>](adjacentmeetingcount.md) <br/> |<span data-ttu-id="513a2-226">Представляет общее число элементов календаря, расположенных на время собрания.</span><span class="sxs-lookup"><span data-stu-id="513a2-226">Represents the total number of calendar items that are adjacent to a meeting time.</span></span>  <br/> |
|[<span data-ttu-id="513a2-227">ConflictingMeetings</span><span class="sxs-lookup"><span data-stu-id="513a2-227">ConflictingMeetings</span></span>](conflictingmeetings.md) <br/> |<span data-ttu-id="513a2-228">Определяет все элементы, конфликтующие с время собрания.</span><span class="sxs-lookup"><span data-stu-id="513a2-228">Identifies all items that conflict with a meeting time.</span></span>  <br/> |
|[<span data-ttu-id="513a2-229">AdjacentMeetings</span><span class="sxs-lookup"><span data-stu-id="513a2-229">AdjacentMeetings</span></span>](adjacentmeetings.md) <br/> |<span data-ttu-id="513a2-230">Описание всех элементов календаря, расположенных на время собрания.</span><span class="sxs-lookup"><span data-stu-id="513a2-230">Describes all calendar items that are adjacent to a meeting time.</span></span>  <br/> |
|[<span data-ttu-id="513a2-231">Продолжительность (элементы)</span><span class="sxs-lookup"><span data-stu-id="513a2-231">Duration (Items)</span></span>](duration-items.md) <br/> |<span data-ttu-id="513a2-232">Представляет длительность элемента календаря.</span><span class="sxs-lookup"><span data-stu-id="513a2-232">Represents the duration of a calendar item.</span></span>  <br/> |
|[<span data-ttu-id="513a2-233">Часовой пояс (элемент)</span><span class="sxs-lookup"><span data-stu-id="513a2-233">TimeZone (Item)</span></span>](timezone-item.md) <br/> |<span data-ttu-id="513a2-234">Предоставляет текстовое описание часового пояса.</span><span class="sxs-lookup"><span data-stu-id="513a2-234">Provides a text description of a time zone.</span></span>  <br/> |
|[<span data-ttu-id="513a2-235">AppointmentReplyTime</span><span class="sxs-lookup"><span data-stu-id="513a2-235">AppointmentReplyTime</span></span>](appointmentreplytime.md) <br/> |<span data-ttu-id="513a2-236">Представляет дату и время, когда участник дан ответ на приглашения на собрание.</span><span class="sxs-lookup"><span data-stu-id="513a2-236">Represents the date and time when an attendee replied to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="513a2-237">AppointmentSequenceNumber</span><span class="sxs-lookup"><span data-stu-id="513a2-237">AppointmentSequenceNumber</span></span>](appointmentsequencenumber.md) <br/> |<span data-ttu-id="513a2-238">Указывает порядковый номер версии встречи.</span><span class="sxs-lookup"><span data-stu-id="513a2-238">Specifies the sequence number of a version of an appointment.</span></span>  <br/> |
|[<span data-ttu-id="513a2-239">AppointmentState</span><span class="sxs-lookup"><span data-stu-id="513a2-239">AppointmentState</span></span>](appointmentstate.md) <br/> |<span data-ttu-id="513a2-240">Указывает состояние встречи.</span><span class="sxs-lookup"><span data-stu-id="513a2-240">Specifies the status of the appointment.</span></span>  <br/> |
|[<span data-ttu-id="513a2-241">Повторение (RecurrenceType)</span><span class="sxs-lookup"><span data-stu-id="513a2-241">Recurrence (RecurrenceType)</span></span>](recurrence-recurrencetype.md) <br/> |<span data-ttu-id="513a2-242">Содержит шаблон повторения для элементов календаря и приглашения на собрания.</span><span class="sxs-lookup"><span data-stu-id="513a2-242">Contains the recurrence pattern for calendar items and meeting requests.</span></span>  <br/> <span data-ttu-id="513a2-243">Этот элемент является допустимым, если [CalendarItemType](calendaritemtype.md) имеет значение RecurringMaster.</span><span class="sxs-lookup"><span data-stu-id="513a2-243">This element is valid if [CalendarItemType](calendaritemtype.md) has the RecurringMaster value.</span></span>  <br/> |
|[<span data-ttu-id="513a2-244">FirstOccurrence</span><span class="sxs-lookup"><span data-stu-id="513a2-244">FirstOccurrence</span></span>](firstoccurrence.md) <br/> |<span data-ttu-id="513a2-245">Представляет первого появления повторяющегося элемента календаря.</span><span class="sxs-lookup"><span data-stu-id="513a2-245">Represents the first occurrence of a recurring calendar item.</span></span>  <br/> <span data-ttu-id="513a2-246">Этот элемент является допустимым, если [CalendarItemType](calendaritemtype.md) имеет значение RecurringMaster.</span><span class="sxs-lookup"><span data-stu-id="513a2-246">This element is valid if [CalendarItemType](calendaritemtype.md) has the RecurringMaster value.</span></span>  <br/> |
|[<span data-ttu-id="513a2-247">LastOccurrence</span><span class="sxs-lookup"><span data-stu-id="513a2-247">LastOccurrence</span></span>](lastoccurrence.md) <br/> |<span data-ttu-id="513a2-248">Представляет последнего вхождения повторяющегося элемента календаря.</span><span class="sxs-lookup"><span data-stu-id="513a2-248">Represents the last occurrence of a recurring calendar item.</span></span>  <br/> <span data-ttu-id="513a2-249">Этот элемент является допустимым, если [CalendarItemType](calendaritemtype.md) имеет значение RecurringMaster.</span><span class="sxs-lookup"><span data-stu-id="513a2-249">This element is valid if [CalendarItemType](calendaritemtype.md) has the RecurringMaster value.</span></span>  <br/> |
|[<span data-ttu-id="513a2-250">ModifiedOccurrences</span><span class="sxs-lookup"><span data-stu-id="513a2-250">ModifiedOccurrences</span></span>](modifiedoccurrences.md) <br/> |<span data-ttu-id="513a2-251">Содержит массив повторяющихся вхождения элемента календаря, которые были изменены, чтобы они отличаются от элемента шаблона повторения.</span><span class="sxs-lookup"><span data-stu-id="513a2-251">Contains an array of recurring calendar item occurrences that have been modified so that they differ from the recurrence master item.</span></span>  <br/> <span data-ttu-id="513a2-252">Этот элемент является допустимым, если [CalendarItemType](calendaritemtype.md) имеет значение RecurringMaster.</span><span class="sxs-lookup"><span data-stu-id="513a2-252">This element is valid if [CalendarItemType](calendaritemtype.md) has the RecurringMaster value.</span></span>  <br/> |
|[<span data-ttu-id="513a2-253">DeletedOccurrences</span><span class="sxs-lookup"><span data-stu-id="513a2-253">DeletedOccurrences</span></span>](deletedoccurrences.md) <br/> |<span data-ttu-id="513a2-254">Содержит массив удаленных вхождения повторяющегося элемента календаря.</span><span class="sxs-lookup"><span data-stu-id="513a2-254">Contains an array of deleted occurrences of a recurring calendar item.</span></span>  <br/> <span data-ttu-id="513a2-255">Этот элемент является допустимым, если [CalendarItemType](calendaritemtype.md) имеет значение RecurringMaster.</span><span class="sxs-lookup"><span data-stu-id="513a2-255">This element is valid if [CalendarItemType](calendaritemtype.md) has the RecurringMaster value.</span></span>  <br/> |
|[<span data-ttu-id="513a2-256">MeetingTimeZone</span><span class="sxs-lookup"><span data-stu-id="513a2-256">MeetingTimeZone</span></span>](meetingtimezone.md) <br/> |<span data-ttu-id="513a2-257">Представляет часовой пояс расположение, где размещен собрания.</span><span class="sxs-lookup"><span data-stu-id="513a2-257">Represents the time zone of the location where the meeting is hosted.</span></span>  <br/> |
|[<span data-ttu-id="513a2-258">StartTimeZone</span><span class="sxs-lookup"><span data-stu-id="513a2-258">StartTimeZone</span></span>](starttimezone.md) <br/> |<span data-ttu-id="513a2-259">Представляет часовой пояс Пуск элемента календаря.</span><span class="sxs-lookup"><span data-stu-id="513a2-259">Represents the start time zone of the calendar item.</span></span>  <br/> |
|[<span data-ttu-id="513a2-260">EndTimeZone</span><span class="sxs-lookup"><span data-stu-id="513a2-260">EndTimeZone</span></span>](endtimezone.md) <br/> |<span data-ttu-id="513a2-261">Представляет часовой пояс конечных элемента календаря.</span><span class="sxs-lookup"><span data-stu-id="513a2-261">Represents the end time zone of the calendar item.</span></span>  <br/> |
|[<span data-ttu-id="513a2-262">ConferenceType</span><span class="sxs-lookup"><span data-stu-id="513a2-262">ConferenceType</span></span>](conferencetype.md) <br/> |<span data-ttu-id="513a2-263">Описывает тип конференц-связи, выполняемую с элементом календарь.</span><span class="sxs-lookup"><span data-stu-id="513a2-263">Describes the type of conferencing that is performed with a calendar item.</span></span>  <br/> |
|[<span data-ttu-id="513a2-264">AllowNewTimeProposal</span><span class="sxs-lookup"><span data-stu-id="513a2-264">AllowNewTimeProposal</span></span>](allownewtimeproposal.md) <br/> |<span data-ttu-id="513a2-265">Указывает, можно ли участником предлагаться собрание для собрания.</span><span class="sxs-lookup"><span data-stu-id="513a2-265">Indicates whether a new meeting time can be proposed for a meeting by an attendee.</span></span>  <br/> |
|[<span data-ttu-id="513a2-266">IsOnlineMeeting</span><span class="sxs-lookup"><span data-stu-id="513a2-266">IsOnlineMeeting</span></span>](isonlinemeeting.md) <br/> |<span data-ttu-id="513a2-267">Указывает, является ли online собрания.</span><span class="sxs-lookup"><span data-stu-id="513a2-267">Indicates whether the meeting is online.</span></span>  <br/> |
|[<span data-ttu-id="513a2-268">MeetingWorkspaceUrl</span><span class="sxs-lookup"><span data-stu-id="513a2-268">MeetingWorkspaceUrl</span></span>](meetingworkspaceurl.md) <br/> |<span data-ttu-id="513a2-269">Содержит URL-адрес для рабочей области для собраний, которая связана с элемента календаря.</span><span class="sxs-lookup"><span data-stu-id="513a2-269">Contains the URL for the meeting workspace that is linked to by the calendar item.</span></span>  <br/> |
|[<span data-ttu-id="513a2-270">NetShowUrl</span><span class="sxs-lookup"><span data-stu-id="513a2-270">NetShowUrl</span></span>](netshowurl.md) <br/> |<span data-ttu-id="513a2-271">Указывает URL-адрес для Microsoft NetShow собрание по сети.</span><span class="sxs-lookup"><span data-stu-id="513a2-271">Specifies the URL for a Microsoft NetShow online meeting.</span></span>  <br/> |
|[<span data-ttu-id="513a2-272">EffectiveRights</span><span class="sxs-lookup"><span data-stu-id="513a2-272">EffectiveRights</span></span>](effectiverights.md) <br/> |<span data-ttu-id="513a2-273">Содержит права клиента на основании параметров разрешений для элемента или папки.</span><span class="sxs-lookup"><span data-stu-id="513a2-273">Contains the client's rights based on the permission settings for the item or folder.</span></span> <span data-ttu-id="513a2-274">Этот элемент доступен только для чтения.</span><span class="sxs-lookup"><span data-stu-id="513a2-274">This element is read-only.</span></span>  <br/> |
|[<span data-ttu-id="513a2-275">LastModifiedName</span><span class="sxs-lookup"><span data-stu-id="513a2-275">LastModifiedName</span></span>](lastmodifiedname.md) <br/> |<span data-ttu-id="513a2-276">Содержит отображаемое имя последнего пользователя, чтобы изменить элемент.</span><span class="sxs-lookup"><span data-stu-id="513a2-276">Contains the display name of the last user to modify an item.</span></span>  <br/> |
|[<span data-ttu-id="513a2-277">LastModifiedTime</span><span class="sxs-lookup"><span data-stu-id="513a2-277">LastModifiedTime</span></span>](lastmodifiedtime.md) <br/> |<span data-ttu-id="513a2-278">Указывает время последнего изменения элемента.</span><span class="sxs-lookup"><span data-stu-id="513a2-278">Indicates when an item was last modified.</span></span>  <br/> |
|[<span data-ttu-id="513a2-279">IsAssociated</span><span class="sxs-lookup"><span data-stu-id="513a2-279">IsAssociated</span></span>](isassociated.md) <br/> |<span data-ttu-id="513a2-280">Указывает, является ли элемент связан с папкой.</span><span class="sxs-lookup"><span data-stu-id="513a2-280">Indicates whether the item is associated with a folder.</span></span>  <br/> |
|[<span data-ttu-id="513a2-281">WebClientReadFormQueryString</span><span class="sxs-lookup"><span data-stu-id="513a2-281">WebClientReadFormQueryString</span></span>](webclientreadformquerystring.md) <br/> |<span data-ttu-id="513a2-282">Представляет URL-адрес для присоединения к конечной точке Microsoft Office Outlook Web App для чтения элемента в Outlook Web App.</span><span class="sxs-lookup"><span data-stu-id="513a2-282">Represents a URL to concatenate to the Microsoft Office Outlook Web App endpoint to read an item in Outlook Web App.</span></span>  <br/> |
|[<span data-ttu-id="513a2-283">WebClientEditFormQueryString</span><span class="sxs-lookup"><span data-stu-id="513a2-283">WebClientEditFormQueryString</span></span>](webclienteditformquerystring.md) <br/> |<span data-ttu-id="513a2-284">Представляет URL-адрес для присоединения к конечной точке Microsoft Office Outlook Web App для редактирования элемента в Outlook Web App.</span><span class="sxs-lookup"><span data-stu-id="513a2-284">Represents a URL to concatenate to the Microsoft Office Outlook Web App endpoint to edit an item in Outlook Web App.</span></span>  <br/> |
|[<span data-ttu-id="513a2-285">ConversationId</span><span class="sxs-lookup"><span data-stu-id="513a2-285">ConversationId</span></span>](conversationid.md) <br/> |<span data-ttu-id="513a2-286">Содержит идентификатор элемента или беседы.</span><span class="sxs-lookup"><span data-stu-id="513a2-286">Contains the identifier of an item or conversation.</span></span>  <br/> |
|[<span data-ttu-id="513a2-287">UniqueBody</span><span class="sxs-lookup"><span data-stu-id="513a2-287">UniqueBody</span></span>](uniquebody.md) <br/> |<span data-ttu-id="513a2-288">Представляет фрагмент HTML или обычный текст, который представляет уникальное body эту беседу.</span><span class="sxs-lookup"><span data-stu-id="513a2-288">Represents an HTML fragment or plain text which represents the unique body of this conversation.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="513a2-289">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="513a2-289">Parent elements</span></span>

|<span data-ttu-id="513a2-290">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="513a2-290">**Element**</span></span>|<span data-ttu-id="513a2-291">**Описание**</span><span class="sxs-lookup"><span data-stu-id="513a2-291">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="513a2-292">AdjacentMeetings</span><span class="sxs-lookup"><span data-stu-id="513a2-292">AdjacentMeetings</span></span>](adjacentmeetings.md) <br/> |<span data-ttu-id="513a2-293">Описание всех элементов календаря, расположенных на время собрания.</span><span class="sxs-lookup"><span data-stu-id="513a2-293">Describes all calendar items that are adjacent to a meeting time.</span></span>  <br/> |
|[<span data-ttu-id="513a2-294">AppendToItemField</span><span class="sxs-lookup"><span data-stu-id="513a2-294">AppendToItemField</span></span>](appendtoitemfield.md) <br/> |<span data-ttu-id="513a2-295">Указывает данные для добавления во время [операции UpdateItem](updateitem-operation.md)отдельное свойство элемента или папки.</span><span class="sxs-lookup"><span data-stu-id="513a2-295">Identifies data to append to a single property of an item or folder during an [UpdateItem operation](updateitem-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="513a2-296">ConflictingMeetings</span><span class="sxs-lookup"><span data-stu-id="513a2-296">ConflictingMeetings</span></span>](conflictingmeetings.md) <br/> |<span data-ttu-id="513a2-297">Определяет все элементы, конфликтующие с время собрания.</span><span class="sxs-lookup"><span data-stu-id="513a2-297">Identifies all items that conflict with a meeting time.</span></span>  <br/> |
|[<span data-ttu-id="513a2-298">Создание (ItemSync)</span><span class="sxs-lookup"><span data-stu-id="513a2-298">Create (ItemSync)</span></span>](create-itemsync.md) <br/> |<span data-ttu-id="513a2-299">Определяет одну папку для создания в локальном хранилище клиента.</span><span class="sxs-lookup"><span data-stu-id="513a2-299">Identifies a single folder to create in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="513a2-300">ItemAttachment</span><span class="sxs-lookup"><span data-stu-id="513a2-300">ItemAttachment</span></span>](itemattachment.md) <br/> |<span data-ttu-id="513a2-301">Представляет собой элемент Exchange, подключенный к другой элемент Exchange.</span><span class="sxs-lookup"><span data-stu-id="513a2-301">Represents an Exchange item that is attached to another Exchange item.</span></span>  <br/> |
|[<span data-ttu-id="513a2-302">Элементы</span><span class="sxs-lookup"><span data-stu-id="513a2-302">Items</span></span>](items.md) <br/> |<span data-ttu-id="513a2-303">Содержит массив элементов.</span><span class="sxs-lookup"><span data-stu-id="513a2-303">Contains an array of items.</span></span>  <br/> |
|[<span data-ttu-id="513a2-304">Элементы (NonEmptyArrayOfAllItemsType)</span><span class="sxs-lookup"><span data-stu-id="513a2-304">Items (NonEmptyArrayOfAllItemsType)</span></span>](items-nonemptyarrayofallitemstype.md) <br/> |<span data-ttu-id="513a2-305">Содержит массив элементов для создания в папке, указанной с помощью элемента [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) .</span><span class="sxs-lookup"><span data-stu-id="513a2-305">Contains an array of items to create in the folder that is identified by the [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) element.</span></span>  <br/> |
|[<span data-ttu-id="513a2-306">SetItemField</span><span class="sxs-lookup"><span data-stu-id="513a2-306">SetItemField</span></span>](setitemfield.md) <br/> |<span data-ttu-id="513a2-307">Представляет отдельное свойство элемента в [UpdateItem операции](updateitem-operation.md)обновления.</span><span class="sxs-lookup"><span data-stu-id="513a2-307">Represents an update to a single property of an item in an [UpdateItem operation](updateitem-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="513a2-308">Обновление (ItemSync)</span><span class="sxs-lookup"><span data-stu-id="513a2-308">Update (ItemSync)</span></span>](update-itemsync.md) <br/> |<span data-ttu-id="513a2-309">Определяет один элемент для обновления в локальном хранилище клиента.</span><span class="sxs-lookup"><span data-stu-id="513a2-309">Identifies a single item to update in the local client store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="513a2-310">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="513a2-310">Text value</span></span>

<span data-ttu-id="513a2-311">Нет.</span><span class="sxs-lookup"><span data-stu-id="513a2-311">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="513a2-312">Замечания</span><span class="sxs-lookup"><span data-stu-id="513a2-312">Remarks</span></span>

<span data-ttu-id="513a2-313">При обновлении элемента одного календаря стать повторяющегося элемента календаря главной [MeetingTimeZone](meetingtimezone.md) элемент должен быть указан для сохранения часового пояса исходного элемента календаря.</span><span class="sxs-lookup"><span data-stu-id="513a2-313">When a single calendar item is updated to become a recurring master calendar item, the [MeetingTimeZone](meetingtimezone.md) element must be specified in order to preserve the calendar item's original time zone.</span></span> 
  
<span data-ttu-id="513a2-314">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="513a2-314">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="513a2-315">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="513a2-315">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="513a2-316">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="513a2-316">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="513a2-317">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="513a2-317">Schema name</span></span>  <br/> |<span data-ttu-id="513a2-318">Схема Types</span><span class="sxs-lookup"><span data-stu-id="513a2-318">Types schema</span></span>  <br/> |
|<span data-ttu-id="513a2-319">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="513a2-319">Validation file</span></span>  <br/> |<span data-ttu-id="513a2-320">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="513a2-320">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="513a2-321">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="513a2-321">Can be empty</span></span>  <br/> |<span data-ttu-id="513a2-322">False</span><span class="sxs-lookup"><span data-stu-id="513a2-322">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="513a2-323">См. также</span><span class="sxs-lookup"><span data-stu-id="513a2-323">See also</span></span>



- [<span data-ttu-id="513a2-324">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="513a2-324">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
  
[<span data-ttu-id="513a2-325">Справка по веб-служб Exchange для Exchange</span><span class="sxs-lookup"><span data-stu-id="513a2-325">EWS reference for Exchange</span></span>](ews-reference-for-exchange.md)

