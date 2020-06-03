---
title: календаритем
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
description: Элемент Календаритем представляет элемент календаря Exchange.
ms.openlocfilehash: b29141470d157ef5bd67be06a1e1fa1c9536b042
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529485"
---
# <a name="calendaritem"></a><span data-ttu-id="6122c-103">календаритем</span><span class="sxs-lookup"><span data-stu-id="6122c-103">CalendarItem</span></span>

<span data-ttu-id="6122c-104">Элемент **календаритем** представляет элемент календаря Exchange.</span><span class="sxs-lookup"><span data-stu-id="6122c-104">The **CalendarItem** element represents an Exchange calendar item.</span></span> 
  
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

 <span data-ttu-id="6122c-105">**календаритемтипе**</span><span class="sxs-lookup"><span data-stu-id="6122c-105">**CalendarItemType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6122c-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="6122c-106">Attributes and elements</span></span>

<span data-ttu-id="6122c-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="6122c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6122c-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="6122c-108">Attributes</span></span>

<span data-ttu-id="6122c-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="6122c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6122c-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="6122c-110">Child elements</span></span>

|<span data-ttu-id="6122c-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="6122c-111">**Element**</span></span>|<span data-ttu-id="6122c-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="6122c-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6122c-113">Сохранитьmimecontent</span><span class="sxs-lookup"><span data-stu-id="6122c-113">MimeContent</span></span>](mimecontent.md) <br/> |<span data-ttu-id="6122c-114">Содержит собственный многоцелевой поток расширений почты в Интернете (MIME) объекта, представленного в формате base64Binary.</span><span class="sxs-lookup"><span data-stu-id="6122c-114">Contains the native Multipurpose Internet Mail Extensions (MIME) stream of an object that is represented in base64Binary format.</span></span>  <br/> |
|[<span data-ttu-id="6122c-115">Идентификатор</span><span class="sxs-lookup"><span data-stu-id="6122c-115">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="6122c-116">Содержит уникальный идентификатор и ключ изменения элемента в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="6122c-116">Contains the unique identifier and change key of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="6122c-117">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="6122c-117">ParentFolderId</span></span>](parentfolderid.md) <br/> |<span data-ttu-id="6122c-118">Представляет идентификатор родительской папки, содержащей элемент или папку.</span><span class="sxs-lookup"><span data-stu-id="6122c-118">Represents the identifier of the parent folder that contains the item or folder.</span></span>  <br/> |
|[<span data-ttu-id="6122c-119">ItemClass</span><span class="sxs-lookup"><span data-stu-id="6122c-119">ItemClass</span></span>](itemclass.md) <br/> |<span data-ttu-id="6122c-120">Представляет класс сообщения для элемента.</span><span class="sxs-lookup"><span data-stu-id="6122c-120">Represents the message class of an item.</span></span>  <br/> |
|[<span data-ttu-id="6122c-121">Тема</span><span class="sxs-lookup"><span data-stu-id="6122c-121">Subject</span></span>](subject.md) <br/> |<span data-ttu-id="6122c-122">Представляет тему для элементов хранилища Exchange и объектов ответа.</span><span class="sxs-lookup"><span data-stu-id="6122c-122">Represents the subject for Exchange store items and response objects.</span></span>  <br/> |
|[<span data-ttu-id="6122c-123">Sensitivity</span><span class="sxs-lookup"><span data-stu-id="6122c-123">Sensitivity</span></span>](sensitivity.md) <br/> |<span data-ttu-id="6122c-124">Указывает уровень конфиденциальности элемента.</span><span class="sxs-lookup"><span data-stu-id="6122c-124">Indicates the sensitivity level of an item.</span></span>  <br/> |
|[<span data-ttu-id="6122c-125">Body</span><span class="sxs-lookup"><span data-stu-id="6122c-125">Body</span></span>](body.md) <br/> |<span data-ttu-id="6122c-126">Представляет реальное содержимое основного текста сообщения.</span><span class="sxs-lookup"><span data-stu-id="6122c-126">Represents the actual body content of a message.</span></span>  <br/> |
|[<span data-ttu-id="6122c-127">Вложения</span><span class="sxs-lookup"><span data-stu-id="6122c-127">Attachments</span></span>](attachments-ex15websvcsotherref.md) <br/> |<span data-ttu-id="6122c-128">Содержит элементы или файлы, вложенные в элемент в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="6122c-128">Contains the items or files that are attached to an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="6122c-129">DateTimeReceived</span><span class="sxs-lookup"><span data-stu-id="6122c-129">DateTimeReceived</span></span>](datetimereceived.md) <br/> |<span data-ttu-id="6122c-130">Представляет дату и время получения элемента в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="6122c-130">Represents the date and time that an item in a mailbox was received.</span></span>  <br/> |
|[<span data-ttu-id="6122c-131">Размер</span><span class="sxs-lookup"><span data-stu-id="6122c-131">Size</span></span>](size.md) <br/> |<span data-ttu-id="6122c-132">Представляет размер элемента в байтах.</span><span class="sxs-lookup"><span data-stu-id="6122c-132">Represents the size in bytes of an item.</span></span> <span data-ttu-id="6122c-133">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6122c-133">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="6122c-134">Категории</span><span class="sxs-lookup"><span data-stu-id="6122c-134">Categories</span></span>](categories-ex15websvcsotherref.md) <br/> |<span data-ttu-id="6122c-135">Представляет коллекцию строк, определяющих категории, к которым относится элемент в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="6122c-135">Represents a collection of strings that identify the categories to which an item in the mailbox belongs.</span></span>  <br/> |
|[<span data-ttu-id="6122c-136">Importance</span><span class="sxs-lookup"><span data-stu-id="6122c-136">Importance</span></span>](importance.md) <br/> |<span data-ttu-id="6122c-137">Описывает важность элемента.</span><span class="sxs-lookup"><span data-stu-id="6122c-137">Describes the importance of an item.</span></span>  <br/> |
|[<span data-ttu-id="6122c-138">инреплито</span><span class="sxs-lookup"><span data-stu-id="6122c-138">InReplyTo</span></span>](inreplyto.md) <br/> |<span data-ttu-id="6122c-139">Представляет идентификатор элемента, который является ответом на этот элемент.</span><span class="sxs-lookup"><span data-stu-id="6122c-139">Represents the identifier of the item to which this item is a reply.</span></span>  <br/> |
|[<span data-ttu-id="6122c-140">Отправлено</span><span class="sxs-lookup"><span data-stu-id="6122c-140">IsSubmitted</span></span>](issubmitted.md) <br/> |<span data-ttu-id="6122c-141">Указывает, был ли элемент отправлен в папку "Исходящие" по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="6122c-141">Indicates whether an item has been submitted to the Outbox default folder.</span></span>  <br/> |
|[<span data-ttu-id="6122c-142">Черновик</span><span class="sxs-lookup"><span data-stu-id="6122c-142">IsDraft</span></span>](isdraft.md) <br/> |<span data-ttu-id="6122c-143">Указывает, был ли элемент еще не отправлен.</span><span class="sxs-lookup"><span data-stu-id="6122c-143">Indicates whether an item has not yet been sent.</span></span>  <br/> |
|[<span data-ttu-id="6122c-144">исфромме</span><span class="sxs-lookup"><span data-stu-id="6122c-144">IsFromMe</span></span>](isfromme.md) <br/> |<span data-ttu-id="6122c-145">Указывает, отправляет ли пользователь элемент.</span><span class="sxs-lookup"><span data-stu-id="6122c-145">Indicates whether a user sent an item to him or herself.</span></span>  <br/> |
|[<span data-ttu-id="6122c-146">исресенд</span><span class="sxs-lookup"><span data-stu-id="6122c-146">IsResend</span></span>](isresend.md) <br/> |<span data-ttu-id="6122c-147">Указывает, был ли ранее отправлен элемент.</span><span class="sxs-lookup"><span data-stu-id="6122c-147">Indicates whether the item had previously been sent.</span></span>  <br/> |
|[<span data-ttu-id="6122c-148">исунмодифиед</span><span class="sxs-lookup"><span data-stu-id="6122c-148">IsUnmodified</span></span>](isunmodified.md) <br/> |<span data-ttu-id="6122c-149">Указывает, был ли изменен элемент.</span><span class="sxs-lookup"><span data-stu-id="6122c-149">Indicates whether the item has been modified.</span></span>  <br/> |
|[<span data-ttu-id="6122c-150">InternetMessageHeaders</span><span class="sxs-lookup"><span data-stu-id="6122c-150">InternetMessageHeaders</span></span>](internetmessageheaders.md) <br/> |<span data-ttu-id="6122c-151">Представляет коллекцию всех заголовков сообщений Интернета, которые находятся в элементе почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="6122c-151">Represents the collection of all Internet message headers that are contained in an item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="6122c-152">датетимесент</span><span class="sxs-lookup"><span data-stu-id="6122c-152">DateTimeSent</span></span>](datetimesent.md) <br/> |<span data-ttu-id="6122c-153">Представляет дату и время отправки элемента в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="6122c-153">Represents the date and time that an item in a mailbox was sent.</span></span>  <br/> |
|[<span data-ttu-id="6122c-154">DateTimeCreated</span><span class="sxs-lookup"><span data-stu-id="6122c-154">DateTimeCreated</span></span>](datetimecreated.md) <br/> |<span data-ttu-id="6122c-155">Представляет дату и время создания определенного элемента в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="6122c-155">Represents the date and time that a given item in the mailbox was created.</span></span>  <br/> |
|[<span data-ttu-id="6122c-156">респонсеобжектс</span><span class="sxs-lookup"><span data-stu-id="6122c-156">ResponseObjects</span></span>](responseobjects.md) <br/> |<span data-ttu-id="6122c-157">Содержит коллекцию всех объектов ответа, связанных с элементом в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="6122c-157">Contains a collection of all the response objects that are associated with an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="6122c-158">реминдердуеби</span><span class="sxs-lookup"><span data-stu-id="6122c-158">ReminderDueBy</span></span>](reminderdueby.md) <br/> |<span data-ttu-id="6122c-159">Представляет дату и время возникновения события.</span><span class="sxs-lookup"><span data-stu-id="6122c-159">Represents the date and time when the event occurs.</span></span> <span data-ttu-id="6122c-160">Он используется элементом [реминдерминутесбефорестарт](reminderminutesbeforestart.md) для определения времени отображения напоминания.</span><span class="sxs-lookup"><span data-stu-id="6122c-160">This is used by the [ReminderMinutesBeforeStart](reminderminutesbeforestart.md) element to determine when the reminder is displayed.</span></span>  <br/> |
|[<span data-ttu-id="6122c-161">реминдериссет</span><span class="sxs-lookup"><span data-stu-id="6122c-161">ReminderIsSet</span></span>](reminderisset.md) <br/> |<span data-ttu-id="6122c-162">Указывает, задано ли напоминание для элемента в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="6122c-162">Indicates whether a reminder has been set for an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="6122c-163">ReminderMinutesBeforeStart</span><span class="sxs-lookup"><span data-stu-id="6122c-163">ReminderMinutesBeforeStart</span></span>](reminderminutesbeforestart.md) <br/> |<span data-ttu-id="6122c-164">Представляет количество минут до события при отображении напоминания.</span><span class="sxs-lookup"><span data-stu-id="6122c-164">Represents the number of minutes before an event when a reminder is displayed.</span></span>  <br/> |
|[<span data-ttu-id="6122c-165">дисплайкк</span><span class="sxs-lookup"><span data-stu-id="6122c-165">DisplayCc</span></span>](displaycc.md) <br/> |<span data-ttu-id="6122c-166">Представляет отображаемую строку, используемую для содержимого строки "копия".</span><span class="sxs-lookup"><span data-stu-id="6122c-166">Represents the display string that is used for the contents of the Cc line.</span></span> <span data-ttu-id="6122c-167">Это объединенная строка всех отображаемых имен получателей копии.</span><span class="sxs-lookup"><span data-stu-id="6122c-167">This is the concatenated string of all Cc recipient display names.</span></span>  <br/> |
|[<span data-ttu-id="6122c-168">дисплайто</span><span class="sxs-lookup"><span data-stu-id="6122c-168">DisplayTo</span></span>](displayto.md) <br/> |<span data-ttu-id="6122c-169">Представляет отображаемую строку, используемую для содержимого строки "Кому".</span><span class="sxs-lookup"><span data-stu-id="6122c-169">Represents the display string that is used for the contents of the To line.</span></span> <span data-ttu-id="6122c-170">Это объединенная строка для отображаемых имен получателей.</span><span class="sxs-lookup"><span data-stu-id="6122c-170">This is the concatenated string of all To recipient display names.</span></span>  <br/> |
|[<span data-ttu-id="6122c-171">HasAttachments</span><span class="sxs-lookup"><span data-stu-id="6122c-171">HasAttachments</span></span>](hasattachments.md) <br/> |<span data-ttu-id="6122c-172">Представляет свойство, для которого задано значение **true** , если элемент имеет по крайней мере одно видимое вложение.</span><span class="sxs-lookup"><span data-stu-id="6122c-172">Represents a property that is set to **true** if an item has at least one visible attachment.</span></span> <span data-ttu-id="6122c-173">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6122c-173">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="6122c-174">ExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="6122c-174">ExtendedProperty</span></span>](extendedproperty.md) <br/> |<span data-ttu-id="6122c-175">Определяет расширенные свойства для папок и элементов.</span><span class="sxs-lookup"><span data-stu-id="6122c-175">Identifies extended properties on folders and items.</span></span>  <br/> |
|[<span data-ttu-id="6122c-176">Culture</span><span class="sxs-lookup"><span data-stu-id="6122c-176">Culture</span></span>](culture.md) <br/> |<span data-ttu-id="6122c-177">Представляет язык и региональные параметры для определенного элемента в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="6122c-177">Represents the culture for a given item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="6122c-178">UID</span><span class="sxs-lookup"><span data-stu-id="6122c-178">UID</span></span>](uid.md) <br/> |<span data-ttu-id="6122c-179">Определяет элемент календаря.</span><span class="sxs-lookup"><span data-stu-id="6122c-179">Identifies a calendar item.</span></span>  <br/> |
|[<span data-ttu-id="6122c-180">рекурренцеид</span><span class="sxs-lookup"><span data-stu-id="6122c-180">RecurrenceId</span></span>](recurrenceid.md) <br/> |<span data-ttu-id="6122c-181">Используется для идентификации определенного экземпляра повторяющегося элемента календаря.</span><span class="sxs-lookup"><span data-stu-id="6122c-181">Used to identify a specific instance of a recurring calendar item.</span></span>  <br/> |
|[<span data-ttu-id="6122c-182">датетиместамп</span><span class="sxs-lookup"><span data-stu-id="6122c-182">DateTimeStamp</span></span>](datetimestamp.md) <br/> |<span data-ttu-id="6122c-183">Указывает дату и время создания экземпляра объекта iCalendar.</span><span class="sxs-lookup"><span data-stu-id="6122c-183">Indicates the date and time that an instance of a iCalendar object was created.</span></span>  <br/> |
|[<span data-ttu-id="6122c-184">Начало</span><span class="sxs-lookup"><span data-stu-id="6122c-184">Start</span></span>](start.md) <br/> |<span data-ttu-id="6122c-185">Представляет начало элемента календаря.</span><span class="sxs-lookup"><span data-stu-id="6122c-185">Represents the start of a calendar item.</span></span> <span data-ttu-id="6122c-186">Этот элемент применяется только к одному экземпляру элемента календаря.</span><span class="sxs-lookup"><span data-stu-id="6122c-186">This element only applies to a single occurrence of a calendar item.</span></span>  <br/> |
|[<span data-ttu-id="6122c-187">Оканчиваться</span><span class="sxs-lookup"><span data-stu-id="6122c-187">End </span></span>](end-ex15websvcsotherref.md) <br/> |<span data-ttu-id="6122c-188">Представляет конец длительности.</span><span class="sxs-lookup"><span data-stu-id="6122c-188">Represents the end of a duration.</span></span> <span data-ttu-id="6122c-189">Этот элемент применяется только к одному экземпляру элемента календаря.</span><span class="sxs-lookup"><span data-stu-id="6122c-189">This element only applies to a single occurrence of a calendar item.</span></span>  <br/> |
|[<span data-ttu-id="6122c-190">оригиналстарт</span><span class="sxs-lookup"><span data-stu-id="6122c-190">OriginalStart</span></span>](originalstart.md) <br/> |<span data-ttu-id="6122c-191">Представляет исходное время начала элемента календаря.</span><span class="sxs-lookup"><span data-stu-id="6122c-191">Represents the original start time of a calendar item.</span></span>  <br/> |
|[<span data-ttu-id="6122c-192">исаллдайевент</span><span class="sxs-lookup"><span data-stu-id="6122c-192">IsAllDayEvent</span></span>](isalldayevent.md) <br/> |<span data-ttu-id="6122c-193">Указывает, представляет ли элемент календаря или приглашение на собрание событие на целый день.</span><span class="sxs-lookup"><span data-stu-id="6122c-193">Indicates whether a calendar item or meeting request represents an all-day event.</span></span>  <br/> |
|[<span data-ttu-id="6122c-194">легацифрибусистатус</span><span class="sxs-lookup"><span data-stu-id="6122c-194">LegacyFreeBusyStatus</span></span>](legacyfreebusystatus.md) <br/> |<span data-ttu-id="6122c-195">Представляет состояние занятости элемента календаря.</span><span class="sxs-lookup"><span data-stu-id="6122c-195">Represents the free/busy status of the calendar item.</span></span>  <br/> |
|[<span data-ttu-id="6122c-196">Location</span><span class="sxs-lookup"><span data-stu-id="6122c-196">Location</span></span>](location.md) <br/> |<span data-ttu-id="6122c-197">Представляет место собрания или встречи.</span><span class="sxs-lookup"><span data-stu-id="6122c-197">Represents the location of a meeting or appointment.</span></span>  <br/> |
|[<span data-ttu-id="6122c-198">Когда</span><span class="sxs-lookup"><span data-stu-id="6122c-198">When</span></span>](when.md) <br/> |<span data-ttu-id="6122c-199">Предоставляет сведения о том, когда встречается элемент календаря.</span><span class="sxs-lookup"><span data-stu-id="6122c-199">Provides information about when a calendar item occurs.</span></span>  <br/> |
|[<span data-ttu-id="6122c-200">"Собрание"</span><span class="sxs-lookup"><span data-stu-id="6122c-200">IsMeeting</span></span>](ismeeting.md) <br/> |<span data-ttu-id="6122c-201">Указывает, является ли элемент календаря собранием или встречей.</span><span class="sxs-lookup"><span data-stu-id="6122c-201">Indicates whether the calendar item is a meeting or appointment.</span></span>  <br/> |
|[<span data-ttu-id="6122c-202">С отменой</span><span class="sxs-lookup"><span data-stu-id="6122c-202">IsCancelled</span></span>](iscancelled.md) <br/> |<span data-ttu-id="6122c-203">Указывает, отменена ли встреча или собрание.</span><span class="sxs-lookup"><span data-stu-id="6122c-203">Indicates whether an appointment or meeting has been canceled.</span></span>  <br/> |
|[<span data-ttu-id="6122c-204">IsRecurring</span><span class="sxs-lookup"><span data-stu-id="6122c-204">IsRecurring</span></span>](isrecurring.md) <br/> |<span data-ttu-id="6122c-205">Указывает, является ли элемент календаря частью повторяющегося элемента.</span><span class="sxs-lookup"><span data-stu-id="6122c-205">Indicates whether a calendar item is part of a recurring item.</span></span> <span data-ttu-id="6122c-206">Этот элемент доступен только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6122c-206">This element is read-only.</span></span>  <br/> |
|[<span data-ttu-id="6122c-207">митингрекуествассент</span><span class="sxs-lookup"><span data-stu-id="6122c-207">MeetingRequestWasSent</span></span>](meetingrequestwassent.md) <br/> |<span data-ttu-id="6122c-208">Указывает, было ли приглашение на собрание отправлено запрошенным участникам.</span><span class="sxs-lookup"><span data-stu-id="6122c-208">Indicates whether a meeting request has been sent to requested attendees.</span></span>  <br/> |
|[<span data-ttu-id="6122c-209">исреспонсерекуестед</span><span class="sxs-lookup"><span data-stu-id="6122c-209">IsResponseRequested</span></span>](isresponserequested.md) <br/> |<span data-ttu-id="6122c-210">Указывает, требуется ли ответ на элемент.</span><span class="sxs-lookup"><span data-stu-id="6122c-210">Indicates whether a response to an item is required.</span></span>  <br/> |
|[<span data-ttu-id="6122c-211">календаритемтипе</span><span class="sxs-lookup"><span data-stu-id="6122c-211">CalendarItemType</span></span>](calendaritemtype.md) <br/> |<span data-ttu-id="6122c-212">Представляет тип вхождения элемента календаря.</span><span class="sxs-lookup"><span data-stu-id="6122c-212">Represents the occurrence type of a calendar item.</span></span>  <br/> |
|[<span data-ttu-id="6122c-213">миреспонсетипе</span><span class="sxs-lookup"><span data-stu-id="6122c-213">MyResponseType</span></span>](myresponsetype.md) <br/> |<span data-ttu-id="6122c-214">Содержит состояние или ответ на элемент календаря.</span><span class="sxs-lookup"><span data-stu-id="6122c-214">Contains the status of or response to a calendar item.</span></span>  <br/> |
|[<span data-ttu-id="6122c-215">Organizer</span><span class="sxs-lookup"><span data-stu-id="6122c-215">Organizer</span></span>](organizer.md) <br/> |<span data-ttu-id="6122c-216">Представляет организатор собрания.</span><span class="sxs-lookup"><span data-stu-id="6122c-216">Represents the organizer of a meeting.</span></span>  <br/> |
|[<span data-ttu-id="6122c-217">RequiredAttendees</span><span class="sxs-lookup"><span data-stu-id="6122c-217">RequiredAttendees</span></span>](requiredattendees.md) <br/> |<span data-ttu-id="6122c-218">Представляет участников, которые необходимы для участия в собрании.</span><span class="sxs-lookup"><span data-stu-id="6122c-218">Represents attendees that are required to attend a meeting.</span></span>  <br/> |
|[<span data-ttu-id="6122c-219">OptionalAttendees</span><span class="sxs-lookup"><span data-stu-id="6122c-219">OptionalAttendees</span></span>](optionalattendees.md) <br/> |<span data-ttu-id="6122c-220">Представляет участников, которые не являются обязательными для участия в собрании.</span><span class="sxs-lookup"><span data-stu-id="6122c-220">Represents attendees that are not required to attend a meeting.</span></span>  <br/> |
|[<span data-ttu-id="6122c-221">Ресурсы</span><span class="sxs-lookup"><span data-stu-id="6122c-221">Resources</span></span>](resources.md) <br/> |<span data-ttu-id="6122c-222">Представляет запланированный ресурс для собрания.</span><span class="sxs-lookup"><span data-stu-id="6122c-222">Represents a scheduled resource for a meeting.</span></span>  <br/> |
|[<span data-ttu-id="6122c-223">конфликтингмитингкаунт</span><span class="sxs-lookup"><span data-stu-id="6122c-223">ConflictingMeetingCount</span></span>](conflictingmeetingcount.md) <br/> |<span data-ttu-id="6122c-224">Представляет количество собраний, которые конфликтуют с элементом календаря.</span><span class="sxs-lookup"><span data-stu-id="6122c-224">Represents the number of meetings that conflict with the calendar item.</span></span>  <br/> |
|[<span data-ttu-id="6122c-225">аджацентмитингкаунт</span><span class="sxs-lookup"><span data-stu-id="6122c-225">AdjacentMeetingCount</span></span>](adjacentmeetingcount.md) <br/> |<span data-ttu-id="6122c-226">Представляет общее число элементов календаря, смежных с временем собрания.</span><span class="sxs-lookup"><span data-stu-id="6122c-226">Represents the total number of calendar items that are adjacent to a meeting time.</span></span>  <br/> |
|[<span data-ttu-id="6122c-227">конфликтингмитингс</span><span class="sxs-lookup"><span data-stu-id="6122c-227">ConflictingMeetings</span></span>](conflictingmeetings.md) <br/> |<span data-ttu-id="6122c-228">Определяет все элементы, которые конфликтуют с временем собрания.</span><span class="sxs-lookup"><span data-stu-id="6122c-228">Identifies all items that conflict with a meeting time.</span></span>  <br/> |
|[<span data-ttu-id="6122c-229">аджацентмитингс</span><span class="sxs-lookup"><span data-stu-id="6122c-229">AdjacentMeetings</span></span>](adjacentmeetings.md) <br/> |<span data-ttu-id="6122c-230">Описывает все элементы календаря, смежные с временем собрания.</span><span class="sxs-lookup"><span data-stu-id="6122c-230">Describes all calendar items that are adjacent to a meeting time.</span></span>  <br/> |
|[<span data-ttu-id="6122c-231">Длительность (элементы)</span><span class="sxs-lookup"><span data-stu-id="6122c-231">Duration (Items)</span></span>](duration-items.md) <br/> |<span data-ttu-id="6122c-232">Представляет продолжительность элемента календаря.</span><span class="sxs-lookup"><span data-stu-id="6122c-232">Represents the duration of a calendar item.</span></span>  <br/> |
|[<span data-ttu-id="6122c-233">Часовой пояс (элемент)</span><span class="sxs-lookup"><span data-stu-id="6122c-233">TimeZone (Item)</span></span>](timezone-item.md) <br/> |<span data-ttu-id="6122c-234">Содержит текст описания часового пояса.</span><span class="sxs-lookup"><span data-stu-id="6122c-234">Provides a text description of a time zone.</span></span>  <br/> |
|[<span data-ttu-id="6122c-235">аппоинтментреплитиме</span><span class="sxs-lookup"><span data-stu-id="6122c-235">AppointmentReplyTime</span></span>](appointmentreplytime.md) <br/> |<span data-ttu-id="6122c-236">Представляет дату и время, когда участник ответил на приглашение на собрание.</span><span class="sxs-lookup"><span data-stu-id="6122c-236">Represents the date and time when an attendee replied to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="6122c-237">аппоинтментсекуенценумбер</span><span class="sxs-lookup"><span data-stu-id="6122c-237">AppointmentSequenceNumber</span></span>](appointmentsequencenumber.md) <br/> |<span data-ttu-id="6122c-238">Задает порядковый номер версии встречи.</span><span class="sxs-lookup"><span data-stu-id="6122c-238">Specifies the sequence number of a version of an appointment.</span></span>  <br/> |
|[<span data-ttu-id="6122c-239">аппоинтментстате</span><span class="sxs-lookup"><span data-stu-id="6122c-239">AppointmentState</span></span>](appointmentstate.md) <br/> |<span data-ttu-id="6122c-240">Указывает состояние встречи.</span><span class="sxs-lookup"><span data-stu-id="6122c-240">Specifies the status of the appointment.</span></span>  <br/> |
|[<span data-ttu-id="6122c-241">Повторение (RecurrenceType)</span><span class="sxs-lookup"><span data-stu-id="6122c-241">Recurrence (RecurrenceType)</span></span>](recurrence-recurrencetype.md) <br/> |<span data-ttu-id="6122c-242">Содержит шаблон повторения для элементов календаря и приглашений на собрание.</span><span class="sxs-lookup"><span data-stu-id="6122c-242">Contains the recurrence pattern for calendar items and meeting requests.</span></span>  <br/> <span data-ttu-id="6122c-243">Этот элемент является допустимым, если [календаритемтипе](calendaritemtype.md) имеет значение рекуррингмастер.</span><span class="sxs-lookup"><span data-stu-id="6122c-243">This element is valid if [CalendarItemType](calendaritemtype.md) has the RecurringMaster value.</span></span>  <br/> |
|[<span data-ttu-id="6122c-244">фирстоккурренце</span><span class="sxs-lookup"><span data-stu-id="6122c-244">FirstOccurrence</span></span>](firstoccurrence.md) <br/> |<span data-ttu-id="6122c-245">Представляет первое вхождение повторяющегося элемента календаря.</span><span class="sxs-lookup"><span data-stu-id="6122c-245">Represents the first occurrence of a recurring calendar item.</span></span>  <br/> <span data-ttu-id="6122c-246">Этот элемент является допустимым, если [календаритемтипе](calendaritemtype.md) имеет значение рекуррингмастер.</span><span class="sxs-lookup"><span data-stu-id="6122c-246">This element is valid if [CalendarItemType](calendaritemtype.md) has the RecurringMaster value.</span></span>  <br/> |
|[<span data-ttu-id="6122c-247">ластоккурренце</span><span class="sxs-lookup"><span data-stu-id="6122c-247">LastOccurrence</span></span>](lastoccurrence.md) <br/> |<span data-ttu-id="6122c-248">Представляет последнее вхождение повторяющегося элемента календаря.</span><span class="sxs-lookup"><span data-stu-id="6122c-248">Represents the last occurrence of a recurring calendar item.</span></span>  <br/> <span data-ttu-id="6122c-249">Этот элемент является допустимым, если [календаритемтипе](calendaritemtype.md) имеет значение рекуррингмастер.</span><span class="sxs-lookup"><span data-stu-id="6122c-249">This element is valid if [CalendarItemType](calendaritemtype.md) has the RecurringMaster value.</span></span>  <br/> |
|[<span data-ttu-id="6122c-250">модифиедоккурренцес</span><span class="sxs-lookup"><span data-stu-id="6122c-250">ModifiedOccurrences</span></span>](modifiedoccurrences.md) <br/> |<span data-ttu-id="6122c-251">Содержит массив повторяющихся экземпляров повторяющихся элементов календаря, которые были изменены таким образом, что они отличаются от элемента шаблона повторения.</span><span class="sxs-lookup"><span data-stu-id="6122c-251">Contains an array of recurring calendar item occurrences that have been modified so that they differ from the recurrence master item.</span></span>  <br/> <span data-ttu-id="6122c-252">Этот элемент является допустимым, если [календаритемтипе](calendaritemtype.md) имеет значение рекуррингмастер.</span><span class="sxs-lookup"><span data-stu-id="6122c-252">This element is valid if [CalendarItemType](calendaritemtype.md) has the RecurringMaster value.</span></span>  <br/> |
|[<span data-ttu-id="6122c-253">делетедоккурренцес</span><span class="sxs-lookup"><span data-stu-id="6122c-253">DeletedOccurrences</span></span>](deletedoccurrences.md) <br/> |<span data-ttu-id="6122c-254">Содержит массив удаленных экземпляров повторяющегося элемента календаря.</span><span class="sxs-lookup"><span data-stu-id="6122c-254">Contains an array of deleted occurrences of a recurring calendar item.</span></span>  <br/> <span data-ttu-id="6122c-255">Этот элемент является допустимым, если [календаритемтипе](calendaritemtype.md) имеет значение рекуррингмастер.</span><span class="sxs-lookup"><span data-stu-id="6122c-255">This element is valid if [CalendarItemType](calendaritemtype.md) has the RecurringMaster value.</span></span>  <br/> |
|[<span data-ttu-id="6122c-256">митингтимезоне</span><span class="sxs-lookup"><span data-stu-id="6122c-256">MeetingTimeZone</span></span>](meetingtimezone.md) <br/> |<span data-ttu-id="6122c-257">Представляет часовой пояс для расположения, в котором размещается собрание.</span><span class="sxs-lookup"><span data-stu-id="6122c-257">Represents the time zone of the location where the meeting is hosted.</span></span>  <br/> |
|[<span data-ttu-id="6122c-258">StartTimeZone</span><span class="sxs-lookup"><span data-stu-id="6122c-258">StartTimeZone</span></span>](starttimezone.md) <br/> |<span data-ttu-id="6122c-259">Представляет часовой пояс элемента календаря.</span><span class="sxs-lookup"><span data-stu-id="6122c-259">Represents the start time zone of the calendar item.</span></span>  <br/> |
|[<span data-ttu-id="6122c-260">EndTimeZone</span><span class="sxs-lookup"><span data-stu-id="6122c-260">EndTimeZone</span></span>](endtimezone.md) <br/> |<span data-ttu-id="6122c-261">Представляет конечный часовой пояс элемента календаря.</span><span class="sxs-lookup"><span data-stu-id="6122c-261">Represents the end time zone of the calendar item.</span></span>  <br/> |
|[<span data-ttu-id="6122c-262">конференцетипе</span><span class="sxs-lookup"><span data-stu-id="6122c-262">ConferenceType</span></span>](conferencetype.md) <br/> |<span data-ttu-id="6122c-263">Описывает тип конференций, который выполняется с элементом календаря.</span><span class="sxs-lookup"><span data-stu-id="6122c-263">Describes the type of conferencing that is performed with a calendar item.</span></span>  <br/> |
|[<span data-ttu-id="6122c-264">алловневтимепропосал</span><span class="sxs-lookup"><span data-stu-id="6122c-264">AllowNewTimeProposal</span></span>](allownewtimeproposal.md) <br/> |<span data-ttu-id="6122c-265">Указывает, может ли новое время проведения собрания предлагаться участнику.</span><span class="sxs-lookup"><span data-stu-id="6122c-265">Indicates whether a new meeting time can be proposed for a meeting by an attendee.</span></span>  <br/> |
|[<span data-ttu-id="6122c-266">исонлинемитинг</span><span class="sxs-lookup"><span data-stu-id="6122c-266">IsOnlineMeeting</span></span>](isonlinemeeting.md) <br/> |<span data-ttu-id="6122c-267">Указывает, находится ли собрание в сети.</span><span class="sxs-lookup"><span data-stu-id="6122c-267">Indicates whether the meeting is online.</span></span>  <br/> |
|[<span data-ttu-id="6122c-268">митингворкспацеурл</span><span class="sxs-lookup"><span data-stu-id="6122c-268">MeetingWorkspaceUrl</span></span>](meetingworkspaceurl.md) <br/> |<span data-ttu-id="6122c-269">Содержит URL-адрес рабочей области для собраний, связанной с элементом календаря.</span><span class="sxs-lookup"><span data-stu-id="6122c-269">Contains the URL for the meeting workspace that is linked to by the calendar item.</span></span>  <br/> |
|[<span data-ttu-id="6122c-270">нетшовурл</span><span class="sxs-lookup"><span data-stu-id="6122c-270">NetShowUrl</span></span>](netshowurl.md) <br/> |<span data-ttu-id="6122c-271">Указывает URL-адрес собрания Microsoft NetShow.</span><span class="sxs-lookup"><span data-stu-id="6122c-271">Specifies the URL for a Microsoft NetShow online meeting.</span></span>  <br/> |
|[<span data-ttu-id="6122c-272">еффективеригхтс</span><span class="sxs-lookup"><span data-stu-id="6122c-272">EffectiveRights</span></span>](effectiverights.md) <br/> |<span data-ttu-id="6122c-273">Содержит права клиента на основе параметров разрешений для элемента или папки.</span><span class="sxs-lookup"><span data-stu-id="6122c-273">Contains the client's rights based on the permission settings for the item or folder.</span></span> <span data-ttu-id="6122c-274">Этот элемент доступен только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6122c-274">This element is read-only.</span></span>  <br/> |
|[<span data-ttu-id="6122c-275">ластмодифиеднаме</span><span class="sxs-lookup"><span data-stu-id="6122c-275">LastModifiedName</span></span>](lastmodifiedname.md) <br/> |<span data-ttu-id="6122c-276">Содержит отображаемое имя последнего пользователя для изменения элемента.</span><span class="sxs-lookup"><span data-stu-id="6122c-276">Contains the display name of the last user to modify an item.</span></span>  <br/> |
|[<span data-ttu-id="6122c-277">LastModifiedTime</span><span class="sxs-lookup"><span data-stu-id="6122c-277">LastModifiedTime</span></span>](lastmodifiedtime.md) <br/> |<span data-ttu-id="6122c-278">Указывает время последнего изменения элемента.</span><span class="sxs-lookup"><span data-stu-id="6122c-278">Indicates when an item was last modified.</span></span>  <br/> |
|[<span data-ttu-id="6122c-279">Связанный</span><span class="sxs-lookup"><span data-stu-id="6122c-279">IsAssociated</span></span>](isassociated.md) <br/> |<span data-ttu-id="6122c-280">Указывает, связан ли элемент с папкой.</span><span class="sxs-lookup"><span data-stu-id="6122c-280">Indicates whether the item is associated with a folder.</span></span>  <br/> |
|[<span data-ttu-id="6122c-281">вебклиентреадформкуеристринг</span><span class="sxs-lookup"><span data-stu-id="6122c-281">WebClientReadFormQueryString</span></span>](webclientreadformquerystring.md) <br/> |<span data-ttu-id="6122c-282">Представляет URL-адрес для сцепления с конечной точкой Microsoft Office Outlook Web App для чтения элемента в Outlook Web App.</span><span class="sxs-lookup"><span data-stu-id="6122c-282">Represents a URL to concatenate to the Microsoft Office Outlook Web App endpoint to read an item in Outlook Web App.</span></span>  <br/> |
|[<span data-ttu-id="6122c-283">вебклиентедитформкуеристринг</span><span class="sxs-lookup"><span data-stu-id="6122c-283">WebClientEditFormQueryString</span></span>](webclienteditformquerystring.md) <br/> |<span data-ttu-id="6122c-284">Представляет URL-адрес для сцепления с конечной точкой Microsoft Office Outlook Web App для изменения элемента в Outlook Web App.</span><span class="sxs-lookup"><span data-stu-id="6122c-284">Represents a URL to concatenate to the Microsoft Office Outlook Web App endpoint to edit an item in Outlook Web App.</span></span>  <br/> |
|[<span data-ttu-id="6122c-285">ConversationId</span><span class="sxs-lookup"><span data-stu-id="6122c-285">ConversationId</span></span>](conversationid.md) <br/> |<span data-ttu-id="6122c-286">Содержит идентификатор элемента или беседы.</span><span class="sxs-lookup"><span data-stu-id="6122c-286">Contains the identifier of an item or conversation.</span></span>  <br/> |
|[<span data-ttu-id="6122c-287">UniqueBody</span><span class="sxs-lookup"><span data-stu-id="6122c-287">UniqueBody</span></span>](uniquebody.md) <br/> |<span data-ttu-id="6122c-288">Представляет фрагмент HTML или обычный текст, представляющий уникальный основной текст этой беседы.</span><span class="sxs-lookup"><span data-stu-id="6122c-288">Represents an HTML fragment or plain text which represents the unique body of this conversation.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="6122c-289">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="6122c-289">Parent elements</span></span>

|<span data-ttu-id="6122c-290">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="6122c-290">**Element**</span></span>|<span data-ttu-id="6122c-291">**Описание**</span><span class="sxs-lookup"><span data-stu-id="6122c-291">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6122c-292">аджацентмитингс</span><span class="sxs-lookup"><span data-stu-id="6122c-292">AdjacentMeetings</span></span>](adjacentmeetings.md) <br/> |<span data-ttu-id="6122c-293">Описывает все элементы календаря, смежные с временем собрания.</span><span class="sxs-lookup"><span data-stu-id="6122c-293">Describes all calendar items that are adjacent to a meeting time.</span></span>  <br/> |
|[<span data-ttu-id="6122c-294">аппендтоитемфиелд</span><span class="sxs-lookup"><span data-stu-id="6122c-294">AppendToItemField</span></span>](appendtoitemfield.md) <br/> |<span data-ttu-id="6122c-295">Определяет данные, добавляемые к одному свойству элемента или папки во время [операции UpdateItem](updateitem-operation.md).</span><span class="sxs-lookup"><span data-stu-id="6122c-295">Identifies data to append to a single property of an item or folder during an [UpdateItem operation](updateitem-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="6122c-296">конфликтингмитингс</span><span class="sxs-lookup"><span data-stu-id="6122c-296">ConflictingMeetings</span></span>](conflictingmeetings.md) <br/> |<span data-ttu-id="6122c-297">Определяет все элементы, которые конфликтуют с временем собрания.</span><span class="sxs-lookup"><span data-stu-id="6122c-297">Identifies all items that conflict with a meeting time.</span></span>  <br/> |
|[<span data-ttu-id="6122c-298">Create (Итемсинк)</span><span class="sxs-lookup"><span data-stu-id="6122c-298">Create (ItemSync)</span></span>](create-itemsync.md) <br/> |<span data-ttu-id="6122c-299">Определяет одну папку для создания в локальном хранилище клиента.</span><span class="sxs-lookup"><span data-stu-id="6122c-299">Identifies a single folder to create in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="6122c-300">ItemAttachment</span><span class="sxs-lookup"><span data-stu-id="6122c-300">ItemAttachment</span></span>](itemattachment.md) <br/> |<span data-ttu-id="6122c-301">Представляет элемент Exchange, присоединенный к другому элементу Exchange.</span><span class="sxs-lookup"><span data-stu-id="6122c-301">Represents an Exchange item that is attached to another Exchange item.</span></span>  <br/> |
|[<span data-ttu-id="6122c-302">Items</span><span class="sxs-lookup"><span data-stu-id="6122c-302">Items</span></span>](items.md) <br/> |<span data-ttu-id="6122c-303">Содержит массив элементов.</span><span class="sxs-lookup"><span data-stu-id="6122c-303">Contains an array of items.</span></span>  <br/> |
|[<span data-ttu-id="6122c-304">Элементы (Нонемптяррайофаллитемстипе)</span><span class="sxs-lookup"><span data-stu-id="6122c-304">Items (NonEmptyArrayOfAllItemsType)</span></span>](items-nonemptyarrayofallitemstype.md) <br/> |<span data-ttu-id="6122c-305">Содержит массив элементов для создания в папке, определяемой элементом [ParentFolderId (таржетфолдеридтипе)](parentfolderid-targetfolderidtype.md) .</span><span class="sxs-lookup"><span data-stu-id="6122c-305">Contains an array of items to create in the folder that is identified by the [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) element.</span></span>  <br/> |
|[<span data-ttu-id="6122c-306">сетитемфиелд</span><span class="sxs-lookup"><span data-stu-id="6122c-306">SetItemField</span></span>](setitemfield.md) <br/> |<span data-ttu-id="6122c-307">Представляет обновление одного свойства элемента в [операции UpdateItem](updateitem-operation.md).</span><span class="sxs-lookup"><span data-stu-id="6122c-307">Represents an update to a single property of an item in an [UpdateItem operation](updateitem-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="6122c-308">Обновление (Итемсинк)</span><span class="sxs-lookup"><span data-stu-id="6122c-308">Update (ItemSync)</span></span>](update-itemsync.md) <br/> |<span data-ttu-id="6122c-309">Определяет один элемент для обновления в локальном хранилище клиента.</span><span class="sxs-lookup"><span data-stu-id="6122c-309">Identifies a single item to update in the local client store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="6122c-310">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="6122c-310">Text value</span></span>

<span data-ttu-id="6122c-311">Нет.</span><span class="sxs-lookup"><span data-stu-id="6122c-311">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="6122c-312">Примечания</span><span class="sxs-lookup"><span data-stu-id="6122c-312">Remarks</span></span>

<span data-ttu-id="6122c-313">Когда один элемент календаря обновляется, чтобы стать повторяющимся элементом основного календаря, необходимо указать элемент [митингтимезоне](meetingtimezone.md) , чтобы сохранить исходный часовой пояс элемента календаря.</span><span class="sxs-lookup"><span data-stu-id="6122c-313">When a single calendar item is updated to become a recurring master calendar item, the [MeetingTimeZone](meetingtimezone.md) element must be specified in order to preserve the calendar item's original time zone.</span></span> 
  
<span data-ttu-id="6122c-314">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="6122c-314">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6122c-315">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="6122c-315">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6122c-316">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="6122c-316">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="6122c-317">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="6122c-317">Schema name</span></span>  <br/> |<span data-ttu-id="6122c-318">Схема Types</span><span class="sxs-lookup"><span data-stu-id="6122c-318">Types schema</span></span>  <br/> |
|<span data-ttu-id="6122c-319">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="6122c-319">Validation file</span></span>  <br/> |<span data-ttu-id="6122c-320">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="6122c-320">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="6122c-321">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="6122c-321">Can be empty</span></span>  <br/> |<span data-ttu-id="6122c-322">False</span><span class="sxs-lookup"><span data-stu-id="6122c-322">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6122c-323">См. также</span><span class="sxs-lookup"><span data-stu-id="6122c-323">See also</span></span>



- [<span data-ttu-id="6122c-324">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="6122c-324">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
  
[<span data-ttu-id="6122c-325">Справка по веб-служб Exchange для Exchange</span><span class="sxs-lookup"><span data-stu-id="6122c-325">EWS reference for Exchange</span></span>](ews-reference-for-exchange.md)

