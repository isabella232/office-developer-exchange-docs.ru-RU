---
title: митингканцеллатион
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MeetingCancellation
api_type:
- schema
ms.assetid: a9c61f7f-2ecd-4b21-9dce-24d9f61aeeea
description: Элемент Митингканцеллатион представляет отмену собрания в хранилище Exchange.
ms.openlocfilehash: b0fca0a2dcbdf8685f7b9fb2197db1c3123d54b1
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/01/2020
ms.locfileid: "44467531"
---
# <a name="meetingcancellation"></a><span data-ttu-id="0161f-103">митингканцеллатион</span><span class="sxs-lookup"><span data-stu-id="0161f-103">MeetingCancellation</span></span>

<span data-ttu-id="0161f-104">Элемент **митингканцеллатион** представляет отмену собрания в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="0161f-104">The **MeetingCancellation** element represents a meeting cancellation in the Exchange store.</span></span> 
  
```xml
<MeetingCancellation>
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
   <EffectiveRights/>
   <LastModifiedName/>
   <LastModifiedTime/>
   <IsAssociated/>
   <WebClientReadFormQueryString/>
   <WebClientEditFormQueryString/>
   <ConversationId/>
   <UniqueBody/>
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
</MeetingCancellation>
```

 <span data-ttu-id="0161f-105">**митингканцеллатионмессажетипе**</span><span class="sxs-lookup"><span data-stu-id="0161f-105">**MeetingCancellationMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0161f-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="0161f-106">Attributes and elements</span></span>

<span data-ttu-id="0161f-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="0161f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0161f-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="0161f-108">Attributes</span></span>

<span data-ttu-id="0161f-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="0161f-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0161f-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="0161f-110">Child elements</span></span>

|<span data-ttu-id="0161f-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="0161f-111">**Element**</span></span>|<span data-ttu-id="0161f-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="0161f-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0161f-113">Сохранитьmimecontent</span><span class="sxs-lookup"><span data-stu-id="0161f-113">MimeContent</span></span>](mimecontent.md) <br/> |<span data-ttu-id="0161f-114">Содержит собственный поток MIME объекта, представленный в формате base64Binary.</span><span class="sxs-lookup"><span data-stu-id="0161f-114">Contains the native MIME stream of an object that is represented in base64Binary format.</span></span>  <br/> |
|[<span data-ttu-id="0161f-115">Идентификатор</span><span class="sxs-lookup"><span data-stu-id="0161f-115">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="0161f-116">Содержит уникальный идентификатор и ключ изменения элемента в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="0161f-116">Contains the unique identifier and change key of an item in the Exchange store.</span></span> <span data-ttu-id="0161f-117">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0161f-117">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="0161f-118">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="0161f-118">ParentFolderId</span></span>](parentfolderid.md) <br/> |<span data-ttu-id="0161f-119">Представляет идентификатор родительской папки, содержащей элемент или папку.</span><span class="sxs-lookup"><span data-stu-id="0161f-119">Represents the identifier of the parent folder that contains the item or folder.</span></span> <span data-ttu-id="0161f-120">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0161f-120">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="0161f-121">ItemClass</span><span class="sxs-lookup"><span data-stu-id="0161f-121">ItemClass</span></span>](itemclass.md) <br/> |<span data-ttu-id="0161f-122">Представляет класс сообщения для элемента.</span><span class="sxs-lookup"><span data-stu-id="0161f-122">Represents the message class of an item.</span></span>  <br/> |
|[<span data-ttu-id="0161f-123">Тема</span><span class="sxs-lookup"><span data-stu-id="0161f-123">Subject</span></span>](subject.md) <br/> |<span data-ttu-id="0161f-124">Представляет тему для элементов хранилища Exchange и объектов ответа.</span><span class="sxs-lookup"><span data-stu-id="0161f-124">Represents the subject for Exchange store items and response objects.</span></span> <span data-ttu-id="0161f-125">Тема может иметь не более 255 символов.</span><span class="sxs-lookup"><span data-stu-id="0161f-125">The subject is limited to 255 characters.</span></span>  <br/> |
|[<span data-ttu-id="0161f-126">Sensitivity</span><span class="sxs-lookup"><span data-stu-id="0161f-126">Sensitivity</span></span>](sensitivity.md) <br/> |<span data-ttu-id="0161f-127">Указывает уровень конфиденциальности элемента.</span><span class="sxs-lookup"><span data-stu-id="0161f-127">Indicates the sensitivity level of an item.</span></span>  <br/> |
|[<span data-ttu-id="0161f-128">Body</span><span class="sxs-lookup"><span data-stu-id="0161f-128">Body</span></span>](body.md) <br/> |<span data-ttu-id="0161f-129">Представляет реальное содержимое основного текста сообщения.</span><span class="sxs-lookup"><span data-stu-id="0161f-129">Represents the actual body content of a message.</span></span>  <br/> |
|[<span data-ttu-id="0161f-130">Вложения</span><span class="sxs-lookup"><span data-stu-id="0161f-130">Attachments</span></span>](attachments-ex15websvcsotherref.md) <br/> |<span data-ttu-id="0161f-131">Содержит элементы или файлы, вложенные в элемент в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="0161f-131">Contains the items or files that are attached to an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="0161f-132">DateTimeReceived</span><span class="sxs-lookup"><span data-stu-id="0161f-132">DateTimeReceived</span></span>](datetimereceived.md) <br/> |<span data-ttu-id="0161f-133">Представляет дату и время получения элемента в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="0161f-133">Represents the date and time that an item in a mailbox was received.</span></span>  <br/> |
|[<span data-ttu-id="0161f-134">Размер</span><span class="sxs-lookup"><span data-stu-id="0161f-134">Size</span></span>](size.md) <br/> |<span data-ttu-id="0161f-135">Представляет размер элемента в байтах.</span><span class="sxs-lookup"><span data-stu-id="0161f-135">Represents the size in bytes of an item.</span></span> <span data-ttu-id="0161f-136">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0161f-136">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="0161f-137">Категории</span><span class="sxs-lookup"><span data-stu-id="0161f-137">Categories</span></span>](categories-ex15websvcsotherref.md) <br/> |<span data-ttu-id="0161f-138">Представляет коллекцию строк, определяющих, к каким категориям принадлежит элемент в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="0161f-138">Represents a collection of strings that identify to which categories an item in the mailbox belongs.</span></span>  <br/> |
|[<span data-ttu-id="0161f-139">Importance</span><span class="sxs-lookup"><span data-stu-id="0161f-139">Importance</span></span>](importance.md) <br/> |<span data-ttu-id="0161f-140">Описывает важность элемента.</span><span class="sxs-lookup"><span data-stu-id="0161f-140">Describes the importance of an item.</span></span>  <br/> |
|[<span data-ttu-id="0161f-141">инреплито</span><span class="sxs-lookup"><span data-stu-id="0161f-141">InReplyTo</span></span>](inreplyto.md) <br/> |<span data-ttu-id="0161f-142">Представляет идентификатор элемента, который является ответом на этот элемент.</span><span class="sxs-lookup"><span data-stu-id="0161f-142">Represents the identifier of the item to which this item is a reply.</span></span>  <br/> |
|[<span data-ttu-id="0161f-143">Отправлено</span><span class="sxs-lookup"><span data-stu-id="0161f-143">IsSubmitted</span></span>](issubmitted.md) <br/> |<span data-ttu-id="0161f-144">Указывает, был ли элемент отправлен в папку "Исходящие" по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="0161f-144">Indicates whether an item has been submitted to the Outbox default folder.</span></span>  <br/> |
|[<span data-ttu-id="0161f-145">Черновик</span><span class="sxs-lookup"><span data-stu-id="0161f-145">IsDraft</span></span>](isdraft.md) <br/> |<span data-ttu-id="0161f-146">Указывает, был ли элемент еще не отправлен.</span><span class="sxs-lookup"><span data-stu-id="0161f-146">Represents whether an item has not yet been sent.</span></span>  <br/> |
|[<span data-ttu-id="0161f-147">исфромме</span><span class="sxs-lookup"><span data-stu-id="0161f-147">IsFromMe</span></span>](isfromme.md) <br/> |<span data-ttu-id="0161f-148">Указывает, отправляет ли пользователь элемент.</span><span class="sxs-lookup"><span data-stu-id="0161f-148">Indicates whether a user sent an item to him or herself.</span></span>  <br/> |
|[<span data-ttu-id="0161f-149">исресенд</span><span class="sxs-lookup"><span data-stu-id="0161f-149">IsResend</span></span>](isresend.md) <br/> |<span data-ttu-id="0161f-150">Указывает, был ли ранее отправлен элемент.</span><span class="sxs-lookup"><span data-stu-id="0161f-150">Indicates whether the item had previously been sent.</span></span>  <br/> |
|[<span data-ttu-id="0161f-151">исунмодифиед</span><span class="sxs-lookup"><span data-stu-id="0161f-151">IsUnmodified</span></span>](isunmodified.md) <br/> |<span data-ttu-id="0161f-152">Указывает, был ли изменен элемент.</span><span class="sxs-lookup"><span data-stu-id="0161f-152">Indicates whether the item has been modified.</span></span>  <br/> |
|[<span data-ttu-id="0161f-153">InternetMessageHeaders</span><span class="sxs-lookup"><span data-stu-id="0161f-153">InternetMessageHeaders</span></span>](internetmessageheaders.md) <br/> |<span data-ttu-id="0161f-154">Представляет коллекцию всех заголовков сообщений Интернета, содержащихся в элементе почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="0161f-154">Represents the collection of all Internet message headers that are contained within an item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="0161f-155">датетимесент</span><span class="sxs-lookup"><span data-stu-id="0161f-155">DateTimeSent</span></span>](datetimesent.md) <br/> |<span data-ttu-id="0161f-156">Представляет дату и время отправки элемента в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="0161f-156">Represents the date and time that an item in a mailbox was sent.</span></span>  <br/> |
|[<span data-ttu-id="0161f-157">DateTimeCreated</span><span class="sxs-lookup"><span data-stu-id="0161f-157">DateTimeCreated</span></span>](datetimecreated.md) <br/> |<span data-ttu-id="0161f-158">Представляет дату и время создания определенного элемента в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="0161f-158">Represents the date and time that a given item in the mailbox was created.</span></span>  <br/> |
|[<span data-ttu-id="0161f-159">респонсеобжектс</span><span class="sxs-lookup"><span data-stu-id="0161f-159">ResponseObjects</span></span>](responseobjects.md) <br/> |<span data-ttu-id="0161f-160">Содержит коллекцию всех объектов ответа, связанных с элементом в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="0161f-160">Contains a collection of all the response objects that are associated with an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="0161f-161">реминдердуеби</span><span class="sxs-lookup"><span data-stu-id="0161f-161">ReminderDueBy</span></span>](reminderdueby.md) <br/> |<span data-ttu-id="0161f-162">Представляет дату и время возникновения события.</span><span class="sxs-lookup"><span data-stu-id="0161f-162">Represents the date and time when the event occurs.</span></span> <span data-ttu-id="0161f-163">Он используется элементом [реминдерминутесбефорестарт](reminderminutesbeforestart.md) для определения времени отображения напоминания.</span><span class="sxs-lookup"><span data-stu-id="0161f-163">This is used by the [ReminderMinutesBeforeStart](reminderminutesbeforestart.md) element to determine when the reminder is displayed.</span></span>  <br/> |
|[<span data-ttu-id="0161f-164">реминдериссет</span><span class="sxs-lookup"><span data-stu-id="0161f-164">ReminderIsSet</span></span>](reminderisset.md) <br/> |<span data-ttu-id="0161f-165">Указывает, задано ли напоминание для элемента в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="0161f-165">Indicates whether a reminder has been set for an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="0161f-166">ReminderMinutesBeforeStart</span><span class="sxs-lookup"><span data-stu-id="0161f-166">ReminderMinutesBeforeStart</span></span>](reminderminutesbeforestart.md) <br/> |<span data-ttu-id="0161f-167">Представляет количество минут до события, в течение которого отображается напоминание.</span><span class="sxs-lookup"><span data-stu-id="0161f-167">Represents the number of minutes before an event that a reminder is displayed.</span></span>  <br/> |
|[<span data-ttu-id="0161f-168">дисплайкк</span><span class="sxs-lookup"><span data-stu-id="0161f-168">DisplayCc</span></span>](displaycc.md) <br/> |<span data-ttu-id="0161f-169">Представляет отображаемую строку, используемую для содержимого поля "копия".</span><span class="sxs-lookup"><span data-stu-id="0161f-169">Represents the display string that is used for the contents of the Cc box.</span></span> <span data-ttu-id="0161f-170">Это объединенная строка всех отображаемых имен получателей копии.</span><span class="sxs-lookup"><span data-stu-id="0161f-170">This is the concatenated string of all Cc recipient display names.</span></span>  <br/> |
|[<span data-ttu-id="0161f-171">дисплайто</span><span class="sxs-lookup"><span data-stu-id="0161f-171">DisplayTo</span></span>](displayto.md) <br/> |<span data-ttu-id="0161f-172">Представляет отображаемую строку, используемую для содержимого поля "Кому".</span><span class="sxs-lookup"><span data-stu-id="0161f-172">Represents the display string that is used for the contents of the To box.</span></span> <span data-ttu-id="0161f-173">Это объединенная строка для отображаемых имен получателей.</span><span class="sxs-lookup"><span data-stu-id="0161f-173">This is the concatenated string of all To recipient display names.</span></span>  <br/> |
|[<span data-ttu-id="0161f-174">HasAttachments</span><span class="sxs-lookup"><span data-stu-id="0161f-174">HasAttachments</span></span>](hasattachments.md) <br/> |<span data-ttu-id="0161f-175">Представляет свойство, для которого задано значение **true** , если элемент имеет по крайней мере одно видимое вложение.</span><span class="sxs-lookup"><span data-stu-id="0161f-175">Represents a property that is set to **true** if an item has at least one visible attachment.</span></span> <span data-ttu-id="0161f-176">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0161f-176">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="0161f-177">ExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="0161f-177">ExtendedProperty</span></span>](extendedproperty.md) <br/> |<span data-ttu-id="0161f-178">Определяет расширенные свойства для папок и элементов.</span><span class="sxs-lookup"><span data-stu-id="0161f-178">Identifies extended properties on folders and items.</span></span>  <br/> |
|[<span data-ttu-id="0161f-179">Culture</span><span class="sxs-lookup"><span data-stu-id="0161f-179">Culture</span></span>](culture.md) <br/> |<span data-ttu-id="0161f-180">Представляет язык и региональные параметры для определенного элемента в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="0161f-180">Represents the culture for a given item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="0161f-181">еффективеригхтс</span><span class="sxs-lookup"><span data-stu-id="0161f-181">EffectiveRights</span></span>](effectiverights.md) <br/> |<span data-ttu-id="0161f-182">Содержит права клиента на основе параметров разрешений для элемента или папки.</span><span class="sxs-lookup"><span data-stu-id="0161f-182">Contains the client's rights based on the permission settings for the item or folder.</span></span> <span data-ttu-id="0161f-183">Этот элемент доступен только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0161f-183">This element is read-only.</span></span>  <br/> |
|[<span data-ttu-id="0161f-184">ластмодифиеднаме</span><span class="sxs-lookup"><span data-stu-id="0161f-184">LastModifiedName</span></span>](lastmodifiedname.md) <br/> |<span data-ttu-id="0161f-185">Содержит отображаемое имя последнего пользователя для изменения элемента.</span><span class="sxs-lookup"><span data-stu-id="0161f-185">Contains the display name of the last user to modify an item.</span></span>  <br/> |
|[<span data-ttu-id="0161f-186">LastModifiedTime</span><span class="sxs-lookup"><span data-stu-id="0161f-186">LastModifiedTime</span></span>](lastmodifiedtime.md) <br/> |<span data-ttu-id="0161f-187">Указывает время последнего изменения элемента.</span><span class="sxs-lookup"><span data-stu-id="0161f-187">Indicates when an item was last modified.</span></span>  <br/> |
|[<span data-ttu-id="0161f-188">Связанный</span><span class="sxs-lookup"><span data-stu-id="0161f-188">IsAssociated</span></span>](isassociated.md) <br/> |<span data-ttu-id="0161f-189">Указывает, связан ли элемент с папкой.</span><span class="sxs-lookup"><span data-stu-id="0161f-189">Indicates whether the item is associated with a folder.</span></span>  <br/> |
|[<span data-ttu-id="0161f-190">вебклиентреадформкуеристринг</span><span class="sxs-lookup"><span data-stu-id="0161f-190">WebClientReadFormQueryString</span></span>](webclientreadformquerystring.md) <br/> |<span data-ttu-id="0161f-191">Представляет URL-адрес для сцепления с конечной точкой Microsoft Office Outlook Web App для чтения элемента в Outlook Web App.</span><span class="sxs-lookup"><span data-stu-id="0161f-191">Represents a URL to concatenate to the Microsoft Office Outlook Web App endpoint to read an item in Outlook Web App.</span></span>  <br/> |
|[<span data-ttu-id="0161f-192">вебклиентедитформкуеристринг</span><span class="sxs-lookup"><span data-stu-id="0161f-192">WebClientEditFormQueryString</span></span>](webclienteditformquerystring.md) <br/> |<span data-ttu-id="0161f-193">Представляет URL-адрес для сцепления с конечной точкой Outlook Web App для изменения элемента в Outlook Web App.</span><span class="sxs-lookup"><span data-stu-id="0161f-193">Represents a URL to concatenate to the Outlook Web App endpoint to edit an item in Outlook Web App.</span></span>  <br/> |
|[<span data-ttu-id="0161f-194">ConversationId</span><span class="sxs-lookup"><span data-stu-id="0161f-194">ConversationId</span></span>](conversationid.md) <br/> |<span data-ttu-id="0161f-195">Содержит идентификатор элемента или беседы.</span><span class="sxs-lookup"><span data-stu-id="0161f-195">Contains the identifier of an item or conversation.</span></span>  <br/> |
|[<span data-ttu-id="0161f-196">UniqueBody</span><span class="sxs-lookup"><span data-stu-id="0161f-196">UniqueBody</span></span>](uniquebody.md) <br/> |<span data-ttu-id="0161f-197">Представляет фрагмент HTML или обычный текст, представляющий уникальный основной текст этой беседы.</span><span class="sxs-lookup"><span data-stu-id="0161f-197">Represents an HTML fragment or plain text which represents the unique body of this conversation.</span></span>  <br/> |
|[<span data-ttu-id="0161f-198">Sender</span><span class="sxs-lookup"><span data-stu-id="0161f-198">Sender</span></span>](sender.md) <br/> |<span data-ttu-id="0161f-199">Определяет отправителя элемента.</span><span class="sxs-lookup"><span data-stu-id="0161f-199">Identifies the sender of an item.</span></span>  <br/> |
|[<span data-ttu-id="0161f-200">ToRecipients</span><span class="sxs-lookup"><span data-stu-id="0161f-200">ToRecipients</span></span>](torecipients.md) <br/> |<span data-ttu-id="0161f-201">Содержит набор получателей сообщения.</span><span class="sxs-lookup"><span data-stu-id="0161f-201">Contains a set of recipients of a message.</span></span>  <br/> |
|[<span data-ttu-id="0161f-202">CcRecipients</span><span class="sxs-lookup"><span data-stu-id="0161f-202">CcRecipients</span></span>](ccrecipients.md) <br/> |<span data-ttu-id="0161f-203">Представляет коллекцию получателей, которые будут получать копию сообщения.</span><span class="sxs-lookup"><span data-stu-id="0161f-203">Represents a collection of recipients that will receive a copy of the message.</span></span>  <br/> |
|[<span data-ttu-id="0161f-204">BccRecipients</span><span class="sxs-lookup"><span data-stu-id="0161f-204">BccRecipients</span></span>](bccrecipients.md) <br/> |<span data-ttu-id="0161f-205">Представляет коллекцию получателей для получения скрытой копии сообщения электронной почты.</span><span class="sxs-lookup"><span data-stu-id="0161f-205">Represents a collection of recipients to receive a blind carbon copy (Bcc) of an e-mail.</span></span>  <br/> |
|[<span data-ttu-id="0161f-206">исреадрецеиптрекуестед</span><span class="sxs-lookup"><span data-stu-id="0161f-206">IsReadReceiptRequested</span></span>](isreadreceiptrequested.md) <br/> |<span data-ttu-id="0161f-207">Указывает, запрашивает ли отправитель элемента уведомление о прочтении.</span><span class="sxs-lookup"><span data-stu-id="0161f-207">Indicates whether the sender of an item requests a read receipt.</span></span>  <br/> |
|[<span data-ttu-id="0161f-208">исделиверирецеиптрекуестед</span><span class="sxs-lookup"><span data-stu-id="0161f-208">IsDeliveryReceiptRequested</span></span>](isdeliveryreceiptrequested.md) <br/> |<span data-ttu-id="0161f-209">Указывает, запрашивает ли отправитель элемента уведомление о доставке.</span><span class="sxs-lookup"><span data-stu-id="0161f-209">Indicates whether the sender of an item requests a delivery receipt.</span></span>  <br/> |
|[<span data-ttu-id="0161f-210">ConversationIndex</span><span class="sxs-lookup"><span data-stu-id="0161f-210">ConversationIndex</span></span>](conversationindex.md) <br/> |<span data-ttu-id="0161f-211">Содержит двоичный код, представляющий поток, к которому относится сообщение.</span><span class="sxs-lookup"><span data-stu-id="0161f-211">Contains a binary ID that represents the thread to which this message belongs.</span></span>  <br/> |
|[<span data-ttu-id="0161f-212">ConversationTopic</span><span class="sxs-lookup"><span data-stu-id="0161f-212">ConversationTopic</span></span>](conversationtopic.md) <br/> |<span data-ttu-id="0161f-213">Представляет идентификатор беседы.</span><span class="sxs-lookup"><span data-stu-id="0161f-213">Represents the conversation identifier.</span></span>  <br/> |
|[<span data-ttu-id="0161f-214">From</span><span class="sxs-lookup"><span data-stu-id="0161f-214">From</span></span>](from.md) <br/> |<span data-ttu-id="0161f-215">Представляет адрес получателя, от которого было отправлено сообщение.</span><span class="sxs-lookup"><span data-stu-id="0161f-215">Represents the addressee from whom the message was sent.</span></span>  <br/> |
|[<span data-ttu-id="0161f-216">InternetMessageId</span><span class="sxs-lookup"><span data-stu-id="0161f-216">InternetMessageId</span></span>](internetmessageid.md) <br/> |<span data-ttu-id="0161f-217">Представляет идентификатор сообщения Интернета для элемента.</span><span class="sxs-lookup"><span data-stu-id="0161f-217">Represents the Internet message identifier of an item.</span></span>  <br/> |
|[<span data-ttu-id="0161f-218">IsRead</span><span class="sxs-lookup"><span data-stu-id="0161f-218">IsRead</span></span>](isread.md) <br/> |<span data-ttu-id="0161f-219">Указывает, было ли Прочитано сообщение.</span><span class="sxs-lookup"><span data-stu-id="0161f-219">Indicates whether a message has been read.</span></span>  <br/> |
|[<span data-ttu-id="0161f-220">исреспонсерекуестед</span><span class="sxs-lookup"><span data-stu-id="0161f-220">IsResponseRequested</span></span>](isresponserequested.md) <br/> |<span data-ttu-id="0161f-221">Указывает, запрашивается ли ответ на сообщение электронной почты.</span><span class="sxs-lookup"><span data-stu-id="0161f-221">Indicates whether a response to an e-mail message is requested.</span></span>  <br/> |
|[<span data-ttu-id="0161f-222">References</span><span class="sxs-lookup"><span data-stu-id="0161f-222">References</span></span>](references.md) <br/> |<span data-ttu-id="0161f-223">Представляет заголовок Usenet, используемый для сопоставления ответов с их исходными сообщениями.</span><span class="sxs-lookup"><span data-stu-id="0161f-223">Represents the Usenet header that is used to correlate replies with their original messages.</span></span>  <br/> |
|[<span data-ttu-id="0161f-224">ReplyTo</span><span class="sxs-lookup"><span data-stu-id="0161f-224">ReplyTo</span></span>](replyto.md) <br/> |<span data-ttu-id="0161f-225">Определяет набор адресов, в который отправляются ответы.</span><span class="sxs-lookup"><span data-stu-id="0161f-225">Identifies a set of addresses to which replies should be sent.</span></span>  <br/> |
|[<span data-ttu-id="0161f-226">ассоЦиатедкалендаритемид</span><span class="sxs-lookup"><span data-stu-id="0161f-226">AssociatedCalendarItemId</span></span>](associatedcalendaritemid.md) <br/> |<span data-ttu-id="0161f-227">Представляет элемент календаря, связанный с объектом [митингмессаже](meetingmessage.md).</span><span class="sxs-lookup"><span data-stu-id="0161f-227">Represents the calendar item that is associated with a [MeetingMessage](meetingmessage.md).</span></span>  <br/> |
|[<span data-ttu-id="0161f-228">Isdelegated для</span><span class="sxs-lookup"><span data-stu-id="0161f-228">IsDelegated</span></span>](isdelegated.md) <br/> |<span data-ttu-id="0161f-229">Указывает, было ли собрание обработано с помощью учетной записи с делегированным доступом.</span><span class="sxs-lookup"><span data-stu-id="0161f-229">Indicates whether a meeting was handled by an account with delegate access.</span></span>  <br/> |
|[<span data-ttu-id="0161f-230">IsOutOfDate</span><span class="sxs-lookup"><span data-stu-id="0161f-230">IsOutOfDate</span></span>](isoutofdate.md) <br/> |<span data-ttu-id="0161f-231">Указывает, является ли сообщение о собрании устаревшим.</span><span class="sxs-lookup"><span data-stu-id="0161f-231">Indicates whether a meeting message is out-of-date.</span></span>  <br/> |
|[<span data-ttu-id="0161f-232">хасбинпроцессед</span><span class="sxs-lookup"><span data-stu-id="0161f-232">HasBeenProcessed</span></span>](hasbeenprocessed.md) <br/> |<span data-ttu-id="0161f-233">Указывает, был ли обработан элемент сообщения о собрании.</span><span class="sxs-lookup"><span data-stu-id="0161f-233">Indicates whether a meeting message item has been processed.</span></span>  <br/> |
|[<span data-ttu-id="0161f-234">ResponseType</span><span class="sxs-lookup"><span data-stu-id="0161f-234">ResponseType</span></span>](responsetype.md) <br/> |<span data-ttu-id="0161f-235">Представляет тип ответа получателя, полученный для собрания.</span><span class="sxs-lookup"><span data-stu-id="0161f-235">Represents the type of recipient response received for a meeting.</span></span>  <br/> |
|[<span data-ttu-id="0161f-236">еффективеригхтс</span><span class="sxs-lookup"><span data-stu-id="0161f-236">EffectiveRights</span></span>](effectiverights.md) <br/> |<span data-ttu-id="0161f-237">Содержит права клиента на основе параметров разрешений для элемента или папки.</span><span class="sxs-lookup"><span data-stu-id="0161f-237">Contains the client's rights based on the permission settings for the item or folder.</span></span> <span data-ttu-id="0161f-238">Этот элемент доступен только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0161f-238">This element is read-only.</span></span> <span data-ttu-id="0161f-239">Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="0161f-239">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span>  <br/> |
|[<span data-ttu-id="0161f-240">рецеиведби</span><span class="sxs-lookup"><span data-stu-id="0161f-240">ReceivedBy</span></span>](receivedby.md) <br/> |<span data-ttu-id="0161f-241">Определяет делегат в сценарии доступа делегата.</span><span class="sxs-lookup"><span data-stu-id="0161f-241">Identifies the delegate in a delegate access scenario.</span></span> <span data-ttu-id="0161f-242">Этот элемент появился в Exchange 2007 с пакетом обновления 1.</span><span class="sxs-lookup"><span data-stu-id="0161f-242">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="0161f-243">рецеиведрепресентинг</span><span class="sxs-lookup"><span data-stu-id="0161f-243">ReceivedRepresenting</span></span>](receivedrepresenting.md) <br/> |<span data-ttu-id="0161f-244">Определяет участника в сценарии доступа делегата.</span><span class="sxs-lookup"><span data-stu-id="0161f-244">Identifies the principal in a delegate access scenario.</span></span> <span data-ttu-id="0161f-245">Этот элемент появился в Exchange 2007 с пакетом обновления 1.</span><span class="sxs-lookup"><span data-stu-id="0161f-245">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="0161f-246">UID</span><span class="sxs-lookup"><span data-stu-id="0161f-246">UID</span></span>](uid.md) <br/> |<span data-ttu-id="0161f-247">Определяет элемент календаря.</span><span class="sxs-lookup"><span data-stu-id="0161f-247">Identifies a calendar item.</span></span>  <br/> |
|[<span data-ttu-id="0161f-248">рекурренцеид</span><span class="sxs-lookup"><span data-stu-id="0161f-248">RecurrenceId</span></span>](recurrenceid.md) <br/> |<span data-ttu-id="0161f-249">Используется для идентификации определенного экземпляра повторяющегося элемента календаря.</span><span class="sxs-lookup"><span data-stu-id="0161f-249">Used to identify a specific instance of a recurring calendar item.</span></span>  <br/> |
|[<span data-ttu-id="0161f-250">датетиместамп</span><span class="sxs-lookup"><span data-stu-id="0161f-250">DateTimeStamp</span></span>](datetimestamp.md) <br/> |<span data-ttu-id="0161f-251">Указывает дату и время создания экземпляра объекта iCalendar.</span><span class="sxs-lookup"><span data-stu-id="0161f-251">Indicates the date and time that an instance of an iCalendar object was created.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="0161f-252">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="0161f-252">Parent elements</span></span>

|<span data-ttu-id="0161f-253">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="0161f-253">**Element**</span></span>|<span data-ttu-id="0161f-254">**Описание**</span><span class="sxs-lookup"><span data-stu-id="0161f-254">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0161f-255">аджацентмитингс</span><span class="sxs-lookup"><span data-stu-id="0161f-255">AdjacentMeetings</span></span>](adjacentmeetings.md) <br/> |<span data-ttu-id="0161f-256">Определяет все элементы календаря, смежные с временем собрания.</span><span class="sxs-lookup"><span data-stu-id="0161f-256">Identifies all calendar items that are adjacent to a meeting time.</span></span>  <br/> |
|[<span data-ttu-id="0161f-257">аппендтоитемфиелд</span><span class="sxs-lookup"><span data-stu-id="0161f-257">AppendToItemField</span></span>](appendtoitemfield.md) <br/> |<span data-ttu-id="0161f-258">Определяет данные, добавляемые к одному свойству элемента во время [операции UpdateItem](updateitem-operation.md).</span><span class="sxs-lookup"><span data-stu-id="0161f-258">Identifies data to append to a single property of an item during an [UpdateItem operation](updateitem-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="0161f-259">конфликтингмитингс</span><span class="sxs-lookup"><span data-stu-id="0161f-259">ConflictingMeetings</span></span>](conflictingmeetings.md) <br/> |<span data-ttu-id="0161f-260">Определяет все элементы, которые конфликтуют с временем собрания.</span><span class="sxs-lookup"><span data-stu-id="0161f-260">Identifies all items that conflict with a meeting time.</span></span>  <br/> |
|[<span data-ttu-id="0161f-261">Create (Итемсинк)</span><span class="sxs-lookup"><span data-stu-id="0161f-261">Create (ItemSync)</span></span>](create-itemsync.md) <br/> |<span data-ttu-id="0161f-262">Определяет один элемент, который необходимо создать в локальном хранилище клиента.</span><span class="sxs-lookup"><span data-stu-id="0161f-262">Identifies a single item to create in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="0161f-263">Items</span><span class="sxs-lookup"><span data-stu-id="0161f-263">Items</span></span>](items.md) <br/> |<span data-ttu-id="0161f-264">Содержит массив элементов.</span><span class="sxs-lookup"><span data-stu-id="0161f-264">Contains an array of items.</span></span>  <br/> |
|[<span data-ttu-id="0161f-265">Элементы (Нонемптяррайофаллитемстипе)</span><span class="sxs-lookup"><span data-stu-id="0161f-265">Items (NonEmptyArrayOfAllItemsType)</span></span>](items-nonemptyarrayofallitemstype.md) <br/> |<span data-ttu-id="0161f-266">Содержит массив создаваемых элементов.</span><span class="sxs-lookup"><span data-stu-id="0161f-266">Contains an array of items to create.</span></span>  <br/> |
|[<span data-ttu-id="0161f-267">ItemAttachment</span><span class="sxs-lookup"><span data-stu-id="0161f-267">ItemAttachment</span></span>](itemattachment.md) <br/> |<span data-ttu-id="0161f-268">Представляет элемент Exchange, присоединенный к другому элементу Exchange.</span><span class="sxs-lookup"><span data-stu-id="0161f-268">Represents an Exchange item that is attached to another Exchange item.</span></span>  <br/> |
|[<span data-ttu-id="0161f-269">сетитемфиелд</span><span class="sxs-lookup"><span data-stu-id="0161f-269">SetItemField</span></span>](setitemfield.md) <br/> |<span data-ttu-id="0161f-270">Представляет обновление одного свойства элемента в [операции UpdateItem](updateitem-operation.md).</span><span class="sxs-lookup"><span data-stu-id="0161f-270">Represents an update to a single property of an item in an [UpdateItem operation](updateitem-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="0161f-271">Обновление (Итемсинк)</span><span class="sxs-lookup"><span data-stu-id="0161f-271">Update (ItemSync)</span></span>](update-itemsync.md) <br/> |<span data-ttu-id="0161f-272">Определяет один элемент для обновления в локальном хранилище клиента.</span><span class="sxs-lookup"><span data-stu-id="0161f-272">Identifies a single item to update in the local client store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="0161f-273">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="0161f-273">Text value</span></span>

<span data-ttu-id="0161f-274">Нет.</span><span class="sxs-lookup"><span data-stu-id="0161f-274">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="0161f-275">Примечания</span><span class="sxs-lookup"><span data-stu-id="0161f-275">Remarks</span></span>

<span data-ttu-id="0161f-276">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="0161f-276">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0161f-277">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="0161f-277">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0161f-278">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="0161f-278">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="0161f-279">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="0161f-279">Schema Name</span></span>  <br/> |<span data-ttu-id="0161f-280">Схема Types</span><span class="sxs-lookup"><span data-stu-id="0161f-280">Types schema</span></span>  <br/> |
|<span data-ttu-id="0161f-281">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="0161f-281">Validation File</span></span>  <br/> |<span data-ttu-id="0161f-282">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="0161f-282">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="0161f-283">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="0161f-283">Can be Empty</span></span>  <br/> |<span data-ttu-id="0161f-284">False</span><span class="sxs-lookup"><span data-stu-id="0161f-284">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0161f-285">См. также</span><span class="sxs-lookup"><span data-stu-id="0161f-285">See also</span></span>



- [<span data-ttu-id="0161f-286">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="0161f-286">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

