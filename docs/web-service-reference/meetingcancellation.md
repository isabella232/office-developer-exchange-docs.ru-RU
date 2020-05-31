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
ms.openlocfilehash: b68135e2743c675bed92c54172369c2ef21f1a6d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834447"
---
# <a name="meetingcancellation"></a><span data-ttu-id="95a08-103">митингканцеллатион</span><span class="sxs-lookup"><span data-stu-id="95a08-103">MeetingCancellation</span></span>

<span data-ttu-id="95a08-104">Элемент **митингканцеллатион** представляет отмену собрания в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="95a08-104">The **MeetingCancellation** element represents a meeting cancellation in the Exchange store.</span></span> 
  
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

 <span data-ttu-id="95a08-105">**митингканцеллатионмессажетипе**</span><span class="sxs-lookup"><span data-stu-id="95a08-105">**MeetingCancellationMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="95a08-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="95a08-106">Attributes and elements</span></span>

<span data-ttu-id="95a08-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="95a08-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="95a08-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="95a08-108">Attributes</span></span>

<span data-ttu-id="95a08-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="95a08-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="95a08-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="95a08-110">Child elements</span></span>

|<span data-ttu-id="95a08-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="95a08-111">**Element**</span></span>|<span data-ttu-id="95a08-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="95a08-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="95a08-113">Сохранитьmimecontent</span><span class="sxs-lookup"><span data-stu-id="95a08-113">MimeContent</span></span>](mimecontent.md) <br/> |<span data-ttu-id="95a08-114">Содержит собственный поток MIME объекта, представленный в формате base64Binary.</span><span class="sxs-lookup"><span data-stu-id="95a08-114">Contains the native MIME stream of an object that is represented in base64Binary format.</span></span>  <br/> |
|[<span data-ttu-id="95a08-115">Идентификатор</span><span class="sxs-lookup"><span data-stu-id="95a08-115">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="95a08-116">Содержит уникальный идентификатор и ключ изменения элемента в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="95a08-116">Contains the unique identifier and change key of an item in the Exchange store.</span></span> <span data-ttu-id="95a08-117">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="95a08-117">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="95a08-118">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="95a08-118">ParentFolderId</span></span>](parentfolderid.md) <br/> |<span data-ttu-id="95a08-119">Представляет идентификатор родительской папки, содержащей элемент или папку.</span><span class="sxs-lookup"><span data-stu-id="95a08-119">Represents the identifier of the parent folder that contains the item or folder.</span></span> <span data-ttu-id="95a08-120">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="95a08-120">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="95a08-121">ItemClass</span><span class="sxs-lookup"><span data-stu-id="95a08-121">ItemClass</span></span>](itemclass.md) <br/> |<span data-ttu-id="95a08-122">Представляет класс сообщения для элемента.</span><span class="sxs-lookup"><span data-stu-id="95a08-122">Represents the message class of an item.</span></span>  <br/> |
|[<span data-ttu-id="95a08-123">Тема</span><span class="sxs-lookup"><span data-stu-id="95a08-123">Subject</span></span>](subject.md) <br/> |<span data-ttu-id="95a08-124">Представляет тему для элементов хранилища Exchange и объектов ответа.</span><span class="sxs-lookup"><span data-stu-id="95a08-124">Represents the subject for Exchange store items and response objects.</span></span> <span data-ttu-id="95a08-125">Тема может иметь не более 255 символов.</span><span class="sxs-lookup"><span data-stu-id="95a08-125">The subject is limited to 255 characters.</span></span>  <br/> |
|[<span data-ttu-id="95a08-126">Sensitivity</span><span class="sxs-lookup"><span data-stu-id="95a08-126">Sensitivity</span></span>](sensitivity.md) <br/> |<span data-ttu-id="95a08-127">Указывает уровень конфиденциальности элемента.</span><span class="sxs-lookup"><span data-stu-id="95a08-127">Indicates the sensitivity level of an item.</span></span>  <br/> |
|[<span data-ttu-id="95a08-128">Основной текст</span><span class="sxs-lookup"><span data-stu-id="95a08-128">Body</span></span>](body.md) <br/> |<span data-ttu-id="95a08-129">Представляет реальное содержимое основного текста сообщения.</span><span class="sxs-lookup"><span data-stu-id="95a08-129">Represents the actual body content of a message.</span></span>  <br/> |
|[<span data-ttu-id="95a08-130">Вложения</span><span class="sxs-lookup"><span data-stu-id="95a08-130">Attachments</span></span>](attachments-ex15websvcsotherref.md) <br/> |<span data-ttu-id="95a08-131">Содержит элементы или файлы, вложенные в элемент в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="95a08-131">Contains the items or files that are attached to an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="95a08-132">DateTimeReceived</span><span class="sxs-lookup"><span data-stu-id="95a08-132">DateTimeReceived</span></span>](datetimereceived.md) <br/> |<span data-ttu-id="95a08-133">Представляет дату и время получения элемента в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="95a08-133">Represents the date and time that an item in a mailbox was received.</span></span>  <br/> |
|[<span data-ttu-id="95a08-134">Размер</span><span class="sxs-lookup"><span data-stu-id="95a08-134">Size</span></span>](size.md) <br/> |<span data-ttu-id="95a08-135">Представляет размер элемента в байтах.</span><span class="sxs-lookup"><span data-stu-id="95a08-135">Represents the size in bytes of an item.</span></span> <span data-ttu-id="95a08-136">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="95a08-136">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="95a08-137">Категории</span><span class="sxs-lookup"><span data-stu-id="95a08-137">Categories</span></span>](categories-ex15websvcsotherref.md) <br/> |<span data-ttu-id="95a08-138">Представляет коллекцию строк, определяющих, к каким категориям принадлежит элемент в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="95a08-138">Represents a collection of strings that identify to which categories an item in the mailbox belongs.</span></span>  <br/> |
|[<span data-ttu-id="95a08-139">Importance</span><span class="sxs-lookup"><span data-stu-id="95a08-139">Importance</span></span>](importance.md) <br/> |<span data-ttu-id="95a08-140">Описывает важность элемента.</span><span class="sxs-lookup"><span data-stu-id="95a08-140">Describes the importance of an item.</span></span>  <br/> |
|[<span data-ttu-id="95a08-141">инреплито</span><span class="sxs-lookup"><span data-stu-id="95a08-141">InReplyTo</span></span>](inreplyto.md) <br/> |<span data-ttu-id="95a08-142">Представляет идентификатор элемента, который является ответом на этот элемент.</span><span class="sxs-lookup"><span data-stu-id="95a08-142">Represents the identifier of the item to which this item is a reply.</span></span>  <br/> |
|[<span data-ttu-id="95a08-143">Отправлено</span><span class="sxs-lookup"><span data-stu-id="95a08-143">IsSubmitted</span></span>](issubmitted.md) <br/> |<span data-ttu-id="95a08-144">Указывает, был ли элемент отправлен в папку "Исходящие" по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="95a08-144">Indicates whether an item has been submitted to the Outbox default folder.</span></span>  <br/> |
|[<span data-ttu-id="95a08-145">Черновик</span><span class="sxs-lookup"><span data-stu-id="95a08-145">IsDraft</span></span>](isdraft.md) <br/> |<span data-ttu-id="95a08-146">Указывает, был ли элемент еще не отправлен.</span><span class="sxs-lookup"><span data-stu-id="95a08-146">Represents whether an item has not yet been sent.</span></span>  <br/> |
|[<span data-ttu-id="95a08-147">исфромме</span><span class="sxs-lookup"><span data-stu-id="95a08-147">IsFromMe</span></span>](isfromme.md) <br/> |<span data-ttu-id="95a08-148">Указывает, отправляет ли пользователь элемент.</span><span class="sxs-lookup"><span data-stu-id="95a08-148">Indicates whether a user sent an item to him or herself.</span></span>  <br/> |
|[<span data-ttu-id="95a08-149">исресенд</span><span class="sxs-lookup"><span data-stu-id="95a08-149">IsResend</span></span>](isresend.md) <br/> |<span data-ttu-id="95a08-150">Указывает, был ли ранее отправлен элемент.</span><span class="sxs-lookup"><span data-stu-id="95a08-150">Indicates whether the item had previously been sent.</span></span>  <br/> |
|[<span data-ttu-id="95a08-151">исунмодифиед</span><span class="sxs-lookup"><span data-stu-id="95a08-151">IsUnmodified</span></span>](isunmodified.md) <br/> |<span data-ttu-id="95a08-152">Указывает, был ли изменен элемент.</span><span class="sxs-lookup"><span data-stu-id="95a08-152">Indicates whether the item has been modified.</span></span>  <br/> |
|[<span data-ttu-id="95a08-153">InternetMessageHeaders</span><span class="sxs-lookup"><span data-stu-id="95a08-153">InternetMessageHeaders</span></span>](internetmessageheaders.md) <br/> |<span data-ttu-id="95a08-154">Представляет коллекцию всех заголовков сообщений Интернета, содержащихся в элементе почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="95a08-154">Represents the collection of all Internet message headers that are contained within an item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="95a08-155">датетимесент</span><span class="sxs-lookup"><span data-stu-id="95a08-155">DateTimeSent</span></span>](datetimesent.md) <br/> |<span data-ttu-id="95a08-156">Представляет дату и время отправки элемента в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="95a08-156">Represents the date and time that an item in a mailbox was sent.</span></span>  <br/> |
|[<span data-ttu-id="95a08-157">DateTimeCreated</span><span class="sxs-lookup"><span data-stu-id="95a08-157">DateTimeCreated</span></span>](datetimecreated.md) <br/> |<span data-ttu-id="95a08-158">Представляет дату и время создания определенного элемента в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="95a08-158">Represents the date and time that a given item in the mailbox was created.</span></span>  <br/> |
|[<span data-ttu-id="95a08-159">респонсеобжектс</span><span class="sxs-lookup"><span data-stu-id="95a08-159">ResponseObjects</span></span>](responseobjects.md) <br/> |<span data-ttu-id="95a08-160">Содержит коллекцию всех объектов ответа, связанных с элементом в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="95a08-160">Contains a collection of all the response objects that are associated with an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="95a08-161">реминдердуеби</span><span class="sxs-lookup"><span data-stu-id="95a08-161">ReminderDueBy</span></span>](reminderdueby.md) <br/> |<span data-ttu-id="95a08-162">Представляет дату и время возникновения события.</span><span class="sxs-lookup"><span data-stu-id="95a08-162">Represents the date and time when the event occurs.</span></span> <span data-ttu-id="95a08-163">Он используется элементом [реминдерминутесбефорестарт](reminderminutesbeforestart.md) для определения времени отображения напоминания.</span><span class="sxs-lookup"><span data-stu-id="95a08-163">This is used by the [ReminderMinutesBeforeStart](reminderminutesbeforestart.md) element to determine when the reminder is displayed.</span></span>  <br/> |
|[<span data-ttu-id="95a08-164">реминдериссет</span><span class="sxs-lookup"><span data-stu-id="95a08-164">ReminderIsSet</span></span>](reminderisset.md) <br/> |<span data-ttu-id="95a08-165">Указывает, задано ли напоминание для элемента в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="95a08-165">Indicates whether a reminder has been set for an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="95a08-166">ReminderMinutesBeforeStart</span><span class="sxs-lookup"><span data-stu-id="95a08-166">ReminderMinutesBeforeStart</span></span>](reminderminutesbeforestart.md) <br/> |<span data-ttu-id="95a08-167">Представляет количество минут до события, в течение которого отображается напоминание.</span><span class="sxs-lookup"><span data-stu-id="95a08-167">Represents the number of minutes before an event that a reminder is displayed.</span></span>  <br/> |
|[<span data-ttu-id="95a08-168">дисплайкк</span><span class="sxs-lookup"><span data-stu-id="95a08-168">DisplayCc</span></span>](displaycc.md) <br/> |<span data-ttu-id="95a08-169">Представляет отображаемую строку, используемую для содержимого поля "копия".</span><span class="sxs-lookup"><span data-stu-id="95a08-169">Represents the display string that is used for the contents of the Cc box.</span></span> <span data-ttu-id="95a08-170">Это объединенная строка всех отображаемых имен получателей копии.</span><span class="sxs-lookup"><span data-stu-id="95a08-170">This is the concatenated string of all Cc recipient display names.</span></span>  <br/> |
|[<span data-ttu-id="95a08-171">дисплайто</span><span class="sxs-lookup"><span data-stu-id="95a08-171">DisplayTo</span></span>](displayto.md) <br/> |<span data-ttu-id="95a08-172">Представляет отображаемую строку, используемую для содержимого поля "Кому".</span><span class="sxs-lookup"><span data-stu-id="95a08-172">Represents the display string that is used for the contents of the To box.</span></span> <span data-ttu-id="95a08-173">Это объединенная строка для отображаемых имен получателей.</span><span class="sxs-lookup"><span data-stu-id="95a08-173">This is the concatenated string of all To recipient display names.</span></span>  <br/> |
|[<span data-ttu-id="95a08-174">HasAttachments</span><span class="sxs-lookup"><span data-stu-id="95a08-174">HasAttachments</span></span>](hasattachments.md) <br/> |<span data-ttu-id="95a08-175">Представляет свойство, для которого задано значение **true** , если элемент имеет по крайней мере одно видимое вложение.</span><span class="sxs-lookup"><span data-stu-id="95a08-175">Represents a property that is set to **true** if an item has at least one visible attachment.</span></span> <span data-ttu-id="95a08-176">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="95a08-176">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="95a08-177">ExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="95a08-177">ExtendedProperty</span></span>](extendedproperty.md) <br/> |<span data-ttu-id="95a08-178">Определяет расширенные свойства для папок и элементов.</span><span class="sxs-lookup"><span data-stu-id="95a08-178">Identifies extended properties on folders and items.</span></span>  <br/> |
|[<span data-ttu-id="95a08-179">Culture</span><span class="sxs-lookup"><span data-stu-id="95a08-179">Culture</span></span>](culture.md) <br/> |<span data-ttu-id="95a08-180">Представляет язык и региональные параметры для определенного элемента в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="95a08-180">Represents the culture for a given item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="95a08-181">еффективеригхтс</span><span class="sxs-lookup"><span data-stu-id="95a08-181">EffectiveRights</span></span>](effectiverights.md) <br/> |<span data-ttu-id="95a08-182">Содержит права клиента на основе параметров разрешений для элемента или папки.</span><span class="sxs-lookup"><span data-stu-id="95a08-182">Contains the client's rights based on the permission settings for the item or folder.</span></span> <span data-ttu-id="95a08-183">Этот элемент доступен только для чтения.</span><span class="sxs-lookup"><span data-stu-id="95a08-183">This element is read-only.</span></span>  <br/> |
|[<span data-ttu-id="95a08-184">ластмодифиеднаме</span><span class="sxs-lookup"><span data-stu-id="95a08-184">LastModifiedName</span></span>](lastmodifiedname.md) <br/> |<span data-ttu-id="95a08-185">Содержит отображаемое имя последнего пользователя для изменения элемента.</span><span class="sxs-lookup"><span data-stu-id="95a08-185">Contains the display name of the last user to modify an item.</span></span>  <br/> |
|[<span data-ttu-id="95a08-186">LastModifiedTime</span><span class="sxs-lookup"><span data-stu-id="95a08-186">LastModifiedTime</span></span>](lastmodifiedtime.md) <br/> |<span data-ttu-id="95a08-187">Указывает время последнего изменения элемента.</span><span class="sxs-lookup"><span data-stu-id="95a08-187">Indicates when an item was last modified.</span></span>  <br/> |
|[<span data-ttu-id="95a08-188">Связанный</span><span class="sxs-lookup"><span data-stu-id="95a08-188">IsAssociated</span></span>](isassociated.md) <br/> |<span data-ttu-id="95a08-189">Указывает, связан ли элемент с папкой.</span><span class="sxs-lookup"><span data-stu-id="95a08-189">Indicates whether the item is associated with a folder.</span></span>  <br/> |
|[<span data-ttu-id="95a08-190">вебклиентреадформкуеристринг</span><span class="sxs-lookup"><span data-stu-id="95a08-190">WebClientReadFormQueryString</span></span>](webclientreadformquerystring.md) <br/> |<span data-ttu-id="95a08-191">Представляет URL-адрес для сцепления с конечной точкой Microsoft Office Outlook Web App для чтения элемента в Outlook Web App.</span><span class="sxs-lookup"><span data-stu-id="95a08-191">Represents a URL to concatenate to the Microsoft Office Outlook Web App endpoint to read an item in Outlook Web App.</span></span>  <br/> |
|[<span data-ttu-id="95a08-192">вебклиентедитформкуеристринг</span><span class="sxs-lookup"><span data-stu-id="95a08-192">WebClientEditFormQueryString</span></span>](webclienteditformquerystring.md) <br/> |<span data-ttu-id="95a08-193">Представляет URL-адрес для сцепления с конечной точкой Outlook Web App для изменения элемента в Outlook Web App.</span><span class="sxs-lookup"><span data-stu-id="95a08-193">Represents a URL to concatenate to the Outlook Web App endpoint to edit an item in Outlook Web App.</span></span>  <br/> |
|[<span data-ttu-id="95a08-194">ConversationId</span><span class="sxs-lookup"><span data-stu-id="95a08-194">ConversationId</span></span>](conversationid.md) <br/> |<span data-ttu-id="95a08-195">Содержит идентификатор элемента или беседы.</span><span class="sxs-lookup"><span data-stu-id="95a08-195">Contains the identifier of an item or conversation.</span></span>  <br/> |
|[<span data-ttu-id="95a08-196">UniqueBody</span><span class="sxs-lookup"><span data-stu-id="95a08-196">UniqueBody</span></span>](uniquebody.md) <br/> |<span data-ttu-id="95a08-197">Представляет фрагмент HTML или обычный текст, представляющий уникальный основной текст этой беседы.</span><span class="sxs-lookup"><span data-stu-id="95a08-197">Represents an HTML fragment or plain text which represents the unique body of this conversation.</span></span>  <br/> |
|[<span data-ttu-id="95a08-198">Sender</span><span class="sxs-lookup"><span data-stu-id="95a08-198">Sender</span></span>](sender.md) <br/> |<span data-ttu-id="95a08-199">Определяет отправителя элемента.</span><span class="sxs-lookup"><span data-stu-id="95a08-199">Identifies the sender of an item.</span></span>  <br/> |
|[<span data-ttu-id="95a08-200">ToRecipients</span><span class="sxs-lookup"><span data-stu-id="95a08-200">ToRecipients</span></span>](torecipients.md) <br/> |<span data-ttu-id="95a08-201">Содержит набор получателей сообщения.</span><span class="sxs-lookup"><span data-stu-id="95a08-201">Contains a set of recipients of a message.</span></span>  <br/> |
|[<span data-ttu-id="95a08-202">CcRecipients</span><span class="sxs-lookup"><span data-stu-id="95a08-202">CcRecipients</span></span>](ccrecipients.md) <br/> |<span data-ttu-id="95a08-203">Представляет коллекцию получателей, которые будут получать копию сообщения.</span><span class="sxs-lookup"><span data-stu-id="95a08-203">Represents a collection of recipients that will receive a copy of the message.</span></span>  <br/> |
|[<span data-ttu-id="95a08-204">BccRecipients</span><span class="sxs-lookup"><span data-stu-id="95a08-204">BccRecipients</span></span>](bccrecipients.md) <br/> |<span data-ttu-id="95a08-205">Представляет коллекцию получателей для получения скрытой копии сообщения электронной почты.</span><span class="sxs-lookup"><span data-stu-id="95a08-205">Represents a collection of recipients to receive a blind carbon copy (Bcc) of an e-mail.</span></span>  <br/> |
|[<span data-ttu-id="95a08-206">исреадрецеиптрекуестед</span><span class="sxs-lookup"><span data-stu-id="95a08-206">IsReadReceiptRequested</span></span>](isreadreceiptrequested.md) <br/> |<span data-ttu-id="95a08-207">Указывает, запрашивает ли отправитель элемента уведомление о прочтении.</span><span class="sxs-lookup"><span data-stu-id="95a08-207">Indicates whether the sender of an item requests a read receipt.</span></span>  <br/> |
|[<span data-ttu-id="95a08-208">исделиверирецеиптрекуестед</span><span class="sxs-lookup"><span data-stu-id="95a08-208">IsDeliveryReceiptRequested</span></span>](isdeliveryreceiptrequested.md) <br/> |<span data-ttu-id="95a08-209">Указывает, запрашивает ли отправитель элемента уведомление о доставке.</span><span class="sxs-lookup"><span data-stu-id="95a08-209">Indicates whether the sender of an item requests a delivery receipt.</span></span>  <br/> |
|[<span data-ttu-id="95a08-210">ConversationIndex</span><span class="sxs-lookup"><span data-stu-id="95a08-210">ConversationIndex</span></span>](conversationindex.md) <br/> |<span data-ttu-id="95a08-211">Содержит двоичный код, представляющий поток, к которому относится сообщение.</span><span class="sxs-lookup"><span data-stu-id="95a08-211">Contains a binary ID that represents the thread to which this message belongs.</span></span>  <br/> |
|[<span data-ttu-id="95a08-212">ConversationTopic</span><span class="sxs-lookup"><span data-stu-id="95a08-212">ConversationTopic</span></span>](conversationtopic.md) <br/> |<span data-ttu-id="95a08-213">Представляет идентификатор беседы.</span><span class="sxs-lookup"><span data-stu-id="95a08-213">Represents the conversation identifier.</span></span>  <br/> |
|[<span data-ttu-id="95a08-214">From</span><span class="sxs-lookup"><span data-stu-id="95a08-214">From</span></span>](from.md) <br/> |<span data-ttu-id="95a08-215">Представляет адрес получателя, от которого было отправлено сообщение.</span><span class="sxs-lookup"><span data-stu-id="95a08-215">Represents the addressee from whom the message was sent.</span></span>  <br/> |
|[<span data-ttu-id="95a08-216">InternetMessageId</span><span class="sxs-lookup"><span data-stu-id="95a08-216">InternetMessageId</span></span>](internetmessageid.md) <br/> |<span data-ttu-id="95a08-217">Представляет идентификатор сообщения Интернета для элемента.</span><span class="sxs-lookup"><span data-stu-id="95a08-217">Represents the Internet message identifier of an item.</span></span>  <br/> |
|[<span data-ttu-id="95a08-218">IsRead</span><span class="sxs-lookup"><span data-stu-id="95a08-218">IsRead</span></span>](isread.md) <br/> |<span data-ttu-id="95a08-219">Указывает, было ли Прочитано сообщение.</span><span class="sxs-lookup"><span data-stu-id="95a08-219">Indicates whether a message has been read.</span></span>  <br/> |
|[<span data-ttu-id="95a08-220">исреспонсерекуестед</span><span class="sxs-lookup"><span data-stu-id="95a08-220">IsResponseRequested</span></span>](isresponserequested.md) <br/> |<span data-ttu-id="95a08-221">Указывает, запрашивается ли ответ на сообщение электронной почты.</span><span class="sxs-lookup"><span data-stu-id="95a08-221">Indicates whether a response to an e-mail message is requested.</span></span>  <br/> |
|[<span data-ttu-id="95a08-222">References</span><span class="sxs-lookup"><span data-stu-id="95a08-222">References</span></span>](references.md) <br/> |<span data-ttu-id="95a08-223">Представляет заголовок Usenet, используемый для сопоставления ответов с их исходными сообщениями.</span><span class="sxs-lookup"><span data-stu-id="95a08-223">Represents the Usenet header that is used to correlate replies with their original messages.</span></span>  <br/> |
|[<span data-ttu-id="95a08-224">ReplyTo</span><span class="sxs-lookup"><span data-stu-id="95a08-224">ReplyTo</span></span>](replyto.md) <br/> |<span data-ttu-id="95a08-225">Определяет набор адресов, в который отправляются ответы.</span><span class="sxs-lookup"><span data-stu-id="95a08-225">Identifies a set of addresses to which replies should be sent.</span></span>  <br/> |
|[<span data-ttu-id="95a08-226">ассоЦиатедкалендаритемид</span><span class="sxs-lookup"><span data-stu-id="95a08-226">AssociatedCalendarItemId</span></span>](associatedcalendaritemid.md) <br/> |<span data-ttu-id="95a08-227">Представляет элемент календаря, связанный с объектом [митингмессаже](meetingmessage.md).</span><span class="sxs-lookup"><span data-stu-id="95a08-227">Represents the calendar item that is associated with a [MeetingMessage](meetingmessage.md).</span></span>  <br/> |
|[<span data-ttu-id="95a08-228">Isdelegated для</span><span class="sxs-lookup"><span data-stu-id="95a08-228">IsDelegated</span></span>](isdelegated.md) <br/> |<span data-ttu-id="95a08-229">Указывает, было ли собрание обработано с помощью учетной записи с делегированным доступом.</span><span class="sxs-lookup"><span data-stu-id="95a08-229">Indicates whether a meeting was handled by an account with delegate access.</span></span>  <br/> |
|[<span data-ttu-id="95a08-230">IsOutOfDate</span><span class="sxs-lookup"><span data-stu-id="95a08-230">IsOutOfDate</span></span>](isoutofdate.md) <br/> |<span data-ttu-id="95a08-231">Указывает, является ли сообщение о собрании устаревшим.</span><span class="sxs-lookup"><span data-stu-id="95a08-231">Indicates whether a meeting message is out-of-date.</span></span>  <br/> |
|[<span data-ttu-id="95a08-232">хасбинпроцессед</span><span class="sxs-lookup"><span data-stu-id="95a08-232">HasBeenProcessed</span></span>](hasbeenprocessed.md) <br/> |<span data-ttu-id="95a08-233">Указывает, был ли обработан элемент сообщения о собрании.</span><span class="sxs-lookup"><span data-stu-id="95a08-233">Indicates whether a meeting message item has been processed.</span></span>  <br/> |
|[<span data-ttu-id="95a08-234">ResponseType</span><span class="sxs-lookup"><span data-stu-id="95a08-234">ResponseType</span></span>](responsetype.md) <br/> |<span data-ttu-id="95a08-235">Представляет тип ответа получателя, полученный для собрания.</span><span class="sxs-lookup"><span data-stu-id="95a08-235">Represents the type of recipient response received for a meeting.</span></span>  <br/> |
|[<span data-ttu-id="95a08-236">еффективеригхтс</span><span class="sxs-lookup"><span data-stu-id="95a08-236">EffectiveRights</span></span>](effectiverights.md) <br/> |<span data-ttu-id="95a08-237">Содержит права клиента на основе параметров разрешений для элемента или папки.</span><span class="sxs-lookup"><span data-stu-id="95a08-237">Contains the client's rights based on the permission settings for the item or folder.</span></span> <span data-ttu-id="95a08-238">Этот элемент доступен только для чтения.</span><span class="sxs-lookup"><span data-stu-id="95a08-238">This element is read-only.</span></span> <span data-ttu-id="95a08-239">Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="95a08-239">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span>  <br/> |
|[<span data-ttu-id="95a08-240">рецеиведби</span><span class="sxs-lookup"><span data-stu-id="95a08-240">ReceivedBy</span></span>](receivedby.md) <br/> |<span data-ttu-id="95a08-241">Определяет делегат в сценарии доступа делегата.</span><span class="sxs-lookup"><span data-stu-id="95a08-241">Identifies the delegate in a delegate access scenario.</span></span> <span data-ttu-id="95a08-242">Этот элемент появился в Exchange 2007 с пакетом обновления 1.</span><span class="sxs-lookup"><span data-stu-id="95a08-242">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="95a08-243">рецеиведрепресентинг</span><span class="sxs-lookup"><span data-stu-id="95a08-243">ReceivedRepresenting</span></span>](receivedrepresenting.md) <br/> |<span data-ttu-id="95a08-244">Определяет участника в сценарии доступа делегата.</span><span class="sxs-lookup"><span data-stu-id="95a08-244">Identifies the principal in a delegate access scenario.</span></span> <span data-ttu-id="95a08-245">Этот элемент появился в Exchange 2007 с пакетом обновления 1.</span><span class="sxs-lookup"><span data-stu-id="95a08-245">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="95a08-246">UID</span><span class="sxs-lookup"><span data-stu-id="95a08-246">UID</span></span>](uid.md) <br/> |<span data-ttu-id="95a08-247">Определяет элемент календаря.</span><span class="sxs-lookup"><span data-stu-id="95a08-247">Identifies a calendar item.</span></span>  <br/> |
|[<span data-ttu-id="95a08-248">рекурренцеид</span><span class="sxs-lookup"><span data-stu-id="95a08-248">RecurrenceId</span></span>](recurrenceid.md) <br/> |<span data-ttu-id="95a08-249">Используется для идентификации определенного экземпляра повторяющегося элемента календаря.</span><span class="sxs-lookup"><span data-stu-id="95a08-249">Used to identify a specific instance of a recurring calendar item.</span></span>  <br/> |
|[<span data-ttu-id="95a08-250">датетиместамп</span><span class="sxs-lookup"><span data-stu-id="95a08-250">DateTimeStamp</span></span>](datetimestamp.md) <br/> |<span data-ttu-id="95a08-251">Указывает дату и время создания экземпляра объекта iCalendar.</span><span class="sxs-lookup"><span data-stu-id="95a08-251">Indicates the date and time that an instance of an iCalendar object was created.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="95a08-252">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="95a08-252">Parent elements</span></span>

|<span data-ttu-id="95a08-253">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="95a08-253">**Element**</span></span>|<span data-ttu-id="95a08-254">**Описание**</span><span class="sxs-lookup"><span data-stu-id="95a08-254">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="95a08-255">аджацентмитингс</span><span class="sxs-lookup"><span data-stu-id="95a08-255">AdjacentMeetings</span></span>](adjacentmeetings.md) <br/> |<span data-ttu-id="95a08-256">Определяет все элементы календаря, смежные с временем собрания.</span><span class="sxs-lookup"><span data-stu-id="95a08-256">Identifies all calendar items that are adjacent to a meeting time.</span></span>  <br/> |
|[<span data-ttu-id="95a08-257">аппендтоитемфиелд</span><span class="sxs-lookup"><span data-stu-id="95a08-257">AppendToItemField</span></span>](appendtoitemfield.md) <br/> |<span data-ttu-id="95a08-258">Определяет данные, добавляемые к одному свойству элемента во время [операции UpdateItem](updateitem-operation.md).</span><span class="sxs-lookup"><span data-stu-id="95a08-258">Identifies data to append to a single property of an item during an [UpdateItem operation](updateitem-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="95a08-259">конфликтингмитингс</span><span class="sxs-lookup"><span data-stu-id="95a08-259">ConflictingMeetings</span></span>](conflictingmeetings.md) <br/> |<span data-ttu-id="95a08-260">Определяет все элементы, которые конфликтуют с временем собрания.</span><span class="sxs-lookup"><span data-stu-id="95a08-260">Identifies all items that conflict with a meeting time.</span></span>  <br/> |
|[<span data-ttu-id="95a08-261">Create (Итемсинк)</span><span class="sxs-lookup"><span data-stu-id="95a08-261">Create (ItemSync)</span></span>](create-itemsync.md) <br/> |<span data-ttu-id="95a08-262">Определяет один элемент, который необходимо создать в локальном хранилище клиента.</span><span class="sxs-lookup"><span data-stu-id="95a08-262">Identifies a single item to create in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="95a08-263">Items</span><span class="sxs-lookup"><span data-stu-id="95a08-263">Items</span></span>](items.md) <br/> |<span data-ttu-id="95a08-264">Содержит массив элементов.</span><span class="sxs-lookup"><span data-stu-id="95a08-264">Contains an array of items.</span></span>  <br/> |
|[<span data-ttu-id="95a08-265">Элементы (Нонемптяррайофаллитемстипе)</span><span class="sxs-lookup"><span data-stu-id="95a08-265">Items (NonEmptyArrayOfAllItemsType)</span></span>](items-nonemptyarrayofallitemstype.md) <br/> |<span data-ttu-id="95a08-266">Содержит массив создаваемых элементов.</span><span class="sxs-lookup"><span data-stu-id="95a08-266">Contains an array of items to create.</span></span>  <br/> |
|[<span data-ttu-id="95a08-267">ItemAttachment</span><span class="sxs-lookup"><span data-stu-id="95a08-267">ItemAttachment</span></span>](itemattachment.md) <br/> |<span data-ttu-id="95a08-268">Представляет элемент Exchange, присоединенный к другому элементу Exchange.</span><span class="sxs-lookup"><span data-stu-id="95a08-268">Represents an Exchange item that is attached to another Exchange item.</span></span>  <br/> |
|[<span data-ttu-id="95a08-269">сетитемфиелд</span><span class="sxs-lookup"><span data-stu-id="95a08-269">SetItemField</span></span>](setitemfield.md) <br/> |<span data-ttu-id="95a08-270">Представляет обновление одного свойства элемента в [операции UpdateItem](updateitem-operation.md).</span><span class="sxs-lookup"><span data-stu-id="95a08-270">Represents an update to a single property of an item in an [UpdateItem operation](updateitem-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="95a08-271">Обновление (Итемсинк)</span><span class="sxs-lookup"><span data-stu-id="95a08-271">Update (ItemSync)</span></span>](update-itemsync.md) <br/> |<span data-ttu-id="95a08-272">Определяет один элемент для обновления в локальном хранилище клиента.</span><span class="sxs-lookup"><span data-stu-id="95a08-272">Identifies a single item to update in the local client store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="95a08-273">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="95a08-273">Text value</span></span>

<span data-ttu-id="95a08-274">Нет.</span><span class="sxs-lookup"><span data-stu-id="95a08-274">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="95a08-275">Примечания</span><span class="sxs-lookup"><span data-stu-id="95a08-275">Remarks</span></span>

<span data-ttu-id="95a08-276">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="95a08-276">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="95a08-277">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="95a08-277">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="95a08-278">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="95a08-278">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="95a08-279">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="95a08-279">Schema Name</span></span>  <br/> |<span data-ttu-id="95a08-280">Схема Types</span><span class="sxs-lookup"><span data-stu-id="95a08-280">Types schema</span></span>  <br/> |
|<span data-ttu-id="95a08-281">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="95a08-281">Validation File</span></span>  <br/> |<span data-ttu-id="95a08-282">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="95a08-282">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="95a08-283">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="95a08-283">Can be Empty</span></span>  <br/> |<span data-ttu-id="95a08-284">False</span><span class="sxs-lookup"><span data-stu-id="95a08-284">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="95a08-285">См. также</span><span class="sxs-lookup"><span data-stu-id="95a08-285">See also</span></span>



- [<span data-ttu-id="95a08-286">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="95a08-286">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

