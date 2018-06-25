---
title: Элемент
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Item
api_type:
- schema
ms.assetid: 4dfe8f48-e7b4-444d-bdf9-a34e180f598b
description: Элемент представляет универсальный элемент в хранилище Exchange.
ms.openlocfilehash: 7af8e063c3bfd77bd87b80463c11c58d996626b5
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834143"
---
# <a name="item"></a><span data-ttu-id="bd305-103">Элемент</span><span class="sxs-lookup"><span data-stu-id="bd305-103">Item</span></span>

<span data-ttu-id="bd305-104">**Элемент** представляет универсальный элемент в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="bd305-104">The **Item** element represents a generic item in the Exchange store.</span></span> 
  
```xml
<Item>
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
</Item>
```

 <span data-ttu-id="bd305-105">**ItemType**</span><span class="sxs-lookup"><span data-stu-id="bd305-105">**ItemType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="bd305-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="bd305-106">Attributes and elements</span></span>

<span data-ttu-id="bd305-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="bd305-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="bd305-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="bd305-108">Attributes</span></span>

<span data-ttu-id="bd305-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="bd305-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="bd305-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="bd305-110">Child elements</span></span>

|<span data-ttu-id="bd305-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="bd305-111">**Element**</span></span>|<span data-ttu-id="bd305-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="bd305-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bd305-113">MimeContent</span><span class="sxs-lookup"><span data-stu-id="bd305-113">MimeContent</span></span>](mimecontent.md) <br/> |<span data-ttu-id="bd305-114">Содержит собственный поток Multipurpose Internet Mail Extensions (MIME), представленного в формате base64Binary объекта.</span><span class="sxs-lookup"><span data-stu-id="bd305-114">Contains the native Multipurpose Internet Mail Extensions (MIME) stream of an object that is represented in base64Binary format.</span></span>  <br/> |
|[<span data-ttu-id="bd305-115">Идентификатор элемента</span><span class="sxs-lookup"><span data-stu-id="bd305-115">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="bd305-116">Содержит уникальный идентификатор и меняет ключ элемента в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="bd305-116">Contains the unique identifier and change key of an item in the Exchange store.</span></span> <span data-ttu-id="bd305-117">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="bd305-117">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="bd305-118">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="bd305-118">ParentFolderId</span></span>](parentfolderid.md) <br/> |<span data-ttu-id="bd305-119">Представляет идентификатор родительской папки, содержащей элемент или папку.</span><span class="sxs-lookup"><span data-stu-id="bd305-119">Represents the identifier of the parent folder that contains the item or folder.</span></span> <span data-ttu-id="bd305-120">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="bd305-120">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="bd305-121">ItemClass</span><span class="sxs-lookup"><span data-stu-id="bd305-121">ItemClass</span></span>](itemclass.md) <br/> |<span data-ttu-id="bd305-122">Представляет класс сообщения элемента.</span><span class="sxs-lookup"><span data-stu-id="bd305-122">Represents the message class of an item.</span></span>  <br/> |
|[<span data-ttu-id="bd305-123">Subject</span><span class="sxs-lookup"><span data-stu-id="bd305-123">Subject</span></span>](subject.md) <br/> |<span data-ttu-id="bd305-124">Представляет тему для элементов хранилища Exchange и объекты ответа.</span><span class="sxs-lookup"><span data-stu-id="bd305-124">Represents the subject for Exchange store items and response objects.</span></span> <span data-ttu-id="bd305-125">Тема ограничена 255 символов.</span><span class="sxs-lookup"><span data-stu-id="bd305-125">The subject is limited to 255 characters.</span></span>  <br/> |
|[<span data-ttu-id="bd305-126">Уровень конфиденциальности сообщения</span><span class="sxs-lookup"><span data-stu-id="bd305-126">Sensitivity</span></span>](sensitivity.md) <br/> |<span data-ttu-id="bd305-127">Указывает уровень конфиденциальности для элемента.</span><span class="sxs-lookup"><span data-stu-id="bd305-127">Indicates the sensitivity level of an item.</span></span>  <br/> |
|[<span data-ttu-id="bd305-128">Body</span><span class="sxs-lookup"><span data-stu-id="bd305-128">Body</span></span>](body.md) <br/> |<span data-ttu-id="bd305-129">Представляет фактическое содержимое основного текста сообщения.</span><span class="sxs-lookup"><span data-stu-id="bd305-129">Represents the actual body content of a message.</span></span>  <br/> |
|[<span data-ttu-id="bd305-130">Вложения</span><span class="sxs-lookup"><span data-stu-id="bd305-130">Attachments</span></span>](attachments-ex15websvcsotherref.md) <br/> |<span data-ttu-id="bd305-131">Содержит элементы или файлы, подключенные к элементу в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="bd305-131">Contains the items or files that are attached to an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="bd305-132">DateTimeReceived</span><span class="sxs-lookup"><span data-stu-id="bd305-132">DateTimeReceived</span></span>](datetimereceived.md) <br/> |<span data-ttu-id="bd305-133">Представляет дату и время получения элемента в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="bd305-133">Represents the date and time that an item in a mailbox was received.</span></span>  <br/> |
|[<span data-ttu-id="bd305-134">Размер</span><span class="sxs-lookup"><span data-stu-id="bd305-134">Size</span></span>](size.md) <br/> |<span data-ttu-id="bd305-135">Представляет размер в байтах элемента.</span><span class="sxs-lookup"><span data-stu-id="bd305-135">Represents the size in bytes of an item.</span></span> <span data-ttu-id="bd305-136">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="bd305-136">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="bd305-137">Категории</span><span class="sxs-lookup"><span data-stu-id="bd305-137">Categories</span></span>](categories-ex15websvcsotherref.md) <br/> |<span data-ttu-id="bd305-138">Представляет набор строк, чтобы указать, к какой категории относится элемент в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="bd305-138">Represents a collection of strings that identify to which categories an item in the mailbox belongs.</span></span>  <br/> |
|[<span data-ttu-id="bd305-139">Важность</span><span class="sxs-lookup"><span data-stu-id="bd305-139">Importance</span></span>](importance.md) <br/> |<span data-ttu-id="bd305-140">Описывает важность элемента.</span><span class="sxs-lookup"><span data-stu-id="bd305-140">Describes the importance of an item.</span></span>  <br/> |
|[<span data-ttu-id="bd305-141">InReplyTo</span><span class="sxs-lookup"><span data-stu-id="bd305-141">InReplyTo</span></span>](inreplyto.md) <br/> |<span data-ttu-id="bd305-142">Представляет идентификатор элемента, к которому этот элемент является ее в ответ.</span><span class="sxs-lookup"><span data-stu-id="bd305-142">Represents the identifier of the item to which this item is a reply.</span></span>  <br/> |
|[<span data-ttu-id="bd305-143">IsSubmitted</span><span class="sxs-lookup"><span data-stu-id="bd305-143">IsSubmitted</span></span>](issubmitted.md) <br/> |<span data-ttu-id="bd305-144">Указывает, является ли элемент был отправлен исходящие папке по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="bd305-144">Indicates whether an item has been submitted to the Outbox default folder.</span></span>  <br/> |
|[<span data-ttu-id="bd305-145">IsDraft</span><span class="sxs-lookup"><span data-stu-id="bd305-145">IsDraft</span></span>](isdraft.md) <br/> |<span data-ttu-id="bd305-146">Представляет ли элемент еще не были отправлены.</span><span class="sxs-lookup"><span data-stu-id="bd305-146">Represents whether an item has not yet been sent.</span></span>  <br/> |
|[<span data-ttu-id="bd305-147">IsFromMe</span><span class="sxs-lookup"><span data-stu-id="bd305-147">IsFromMe</span></span>](isfromme.md) <br/> |<span data-ttu-id="bd305-148">Показывает пользователя отправить элемент на себя.</span><span class="sxs-lookup"><span data-stu-id="bd305-148">Indicates whether a user sent an item to itself.</span></span>  <br/> |
|[<span data-ttu-id="bd305-149">IsResend</span><span class="sxs-lookup"><span data-stu-id="bd305-149">IsResend</span></span>](isresend.md) <br/> |<span data-ttu-id="bd305-150">Указывает, является ли элемент ранее еще был отправлен.</span><span class="sxs-lookup"><span data-stu-id="bd305-150">Indicates whether the item had previously been sent.</span></span>  <br/> |
|[<span data-ttu-id="bd305-151">IsUnmodified</span><span class="sxs-lookup"><span data-stu-id="bd305-151">IsUnmodified</span></span>](isunmodified.md) <br/> |<span data-ttu-id="bd305-152">Указывает, были ли изменены элемента.</span><span class="sxs-lookup"><span data-stu-id="bd305-152">Indicates whether the item has been modified.</span></span>  <br/> |
|[<span data-ttu-id="bd305-153">InternetMessageHeaders</span><span class="sxs-lookup"><span data-stu-id="bd305-153">InternetMessageHeaders</span></span>](internetmessageheaders.md) <br/> |<span data-ttu-id="bd305-154">Представляет коллекцию всех заголовков сообщений Интернета, находящихся внутри элемента в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="bd305-154">Represents the collection of all Internet message headers that are contained within an item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="bd305-155">DateTimeSent</span><span class="sxs-lookup"><span data-stu-id="bd305-155">DateTimeSent</span></span>](datetimesent.md) <br/> |<span data-ttu-id="bd305-156">Представляет дату и время отправки элемента в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="bd305-156">Represents the date and time that an item in a mailbox was sent.</span></span>  <br/> |
|[<span data-ttu-id="bd305-157">DateTimeCreated</span><span class="sxs-lookup"><span data-stu-id="bd305-157">DateTimeCreated</span></span>](datetimecreated.md) <br/> |<span data-ttu-id="bd305-158">Представляет дату и время создания данного элемента в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="bd305-158">Represents the date and time that a given item in the mailbox was created.</span></span>  <br/> |
|[<span data-ttu-id="bd305-159">ResponseObjects</span><span class="sxs-lookup"><span data-stu-id="bd305-159">ResponseObjects</span></span>](responseobjects.md) <br/> |<span data-ttu-id="bd305-160">Содержит коллекцию всех объектов ответа, которые связаны с элемента в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="bd305-160">Contains a collection of all the response objects that are associated with an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="bd305-161">ReminderDueBy</span><span class="sxs-lookup"><span data-stu-id="bd305-161">ReminderDueBy</span></span>](reminderdueby.md) <br/> |<span data-ttu-id="bd305-162">Представляет дату и время, когда происходит событие.</span><span class="sxs-lookup"><span data-stu-id="bd305-162">Represents the date and time when the event occurs.</span></span> <span data-ttu-id="bd305-163">Используется в элементе [ReminderMinutesBeforeStart](reminderminutesbeforestart.md) определить, когда отображается оповещение.</span><span class="sxs-lookup"><span data-stu-id="bd305-163">This is used by the [ReminderMinutesBeforeStart](reminderminutesbeforestart.md) element to determine when the reminder is displayed.</span></span>  <br/> |
|[<span data-ttu-id="bd305-164">ReminderIsSet</span><span class="sxs-lookup"><span data-stu-id="bd305-164">ReminderIsSet</span></span>](reminderisset.md) <br/> |<span data-ttu-id="bd305-165">Указывает, установлен ли напоминания для элемента в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="bd305-165">Indicates whether a reminder has been set for an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="bd305-166">ReminderMinutesBeforeStart</span><span class="sxs-lookup"><span data-stu-id="bd305-166">ReminderMinutesBeforeStart</span></span>](reminderminutesbeforestart.md) <br/> |<span data-ttu-id="bd305-167">Представляет число минут и только потом событие, когда отображается напоминание.</span><span class="sxs-lookup"><span data-stu-id="bd305-167">Represents the number of minutes before an event when a reminder is displayed.</span></span>  <br/> |
|[<span data-ttu-id="bd305-168">DisplayCc</span><span class="sxs-lookup"><span data-stu-id="bd305-168">DisplayCc</span></span>](displaycc.md) <br/> |<span data-ttu-id="bd305-169">Строка отображения, который используется для содержимого в поле "Копия".</span><span class="sxs-lookup"><span data-stu-id="bd305-169">Represents the display string that is used for the contents of the Cc box.</span></span> <span data-ttu-id="bd305-170">Это составное строка всех получателей отображаемые имена «копия».</span><span class="sxs-lookup"><span data-stu-id="bd305-170">This is the concatenated string of all Cc recipient display names.</span></span>  <br/> |
|[<span data-ttu-id="bd305-171">DisplayTo</span><span class="sxs-lookup"><span data-stu-id="bd305-171">DisplayTo</span></span>](displayto.md) <br/> |<span data-ttu-id="bd305-172">Строка отображения, который используется для содержимого в поле «Кому».</span><span class="sxs-lookup"><span data-stu-id="bd305-172">Represents the display string that is used for the contents of the To box.</span></span> <span data-ttu-id="bd305-173">Это составное строка всех для получателей отображаемые имена.</span><span class="sxs-lookup"><span data-stu-id="bd305-173">This is the concatenated string of all To recipient display names.</span></span>  <br/> |
|[<span data-ttu-id="bd305-174">HasAttachments</span><span class="sxs-lookup"><span data-stu-id="bd305-174">HasAttachments</span></span>](hasattachments.md) <br/> |<span data-ttu-id="bd305-175">Представляет свойство, которое задано значение **true,** Если элемент содержит вложения по крайней мере один видимым вложения.</span><span class="sxs-lookup"><span data-stu-id="bd305-175">Represents a property that is set to **true** if an item has attachments at least one visible attachment.</span></span> <span data-ttu-id="bd305-176">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="bd305-176">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="bd305-177">ExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="bd305-177">ExtendedProperty</span></span>](extendedproperty.md) <br/> |<span data-ttu-id="bd305-178">Определяет расширенные свойства для папок и элементов.</span><span class="sxs-lookup"><span data-stu-id="bd305-178">Identifies extended properties on folders and items.</span></span>  <br/> |
|[<span data-ttu-id="bd305-179">Язык и региональные параметры</span><span class="sxs-lookup"><span data-stu-id="bd305-179">Culture</span></span>](culture.md) <br/> |<span data-ttu-id="bd305-180">Представляет язык и региональные параметры для заданного элемента в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="bd305-180">Represents the culture for a given item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="bd305-181">EffectiveRights</span><span class="sxs-lookup"><span data-stu-id="bd305-181">EffectiveRights</span></span>](effectiverights.md) <br/> |<span data-ttu-id="bd305-182">Содержит права клиента на основании параметров разрешений для элемента или папки.</span><span class="sxs-lookup"><span data-stu-id="bd305-182">Contains the client's rights based on the permission settings for the item or folder.</span></span> <span data-ttu-id="bd305-183">Этот элемент доступен только для чтения.</span><span class="sxs-lookup"><span data-stu-id="bd305-183">This element is read-only.</span></span>  <br/> |
|[<span data-ttu-id="bd305-184">LastModifiedName</span><span class="sxs-lookup"><span data-stu-id="bd305-184">LastModifiedName</span></span>](lastmodifiedname.md) <br/> |<span data-ttu-id="bd305-185">Содержит отображаемое имя последнего пользователя, чтобы изменить элемент.</span><span class="sxs-lookup"><span data-stu-id="bd305-185">Contains the display name of the last user to modify an item.</span></span>  <br/> |
|[<span data-ttu-id="bd305-186">LastModifiedTime</span><span class="sxs-lookup"><span data-stu-id="bd305-186">LastModifiedTime</span></span>](lastmodifiedtime.md) <br/> |<span data-ttu-id="bd305-187">Указывает время последнего изменения элемента.</span><span class="sxs-lookup"><span data-stu-id="bd305-187">Indicates when an item was last modified.</span></span>  <br/> |
|[<span data-ttu-id="bd305-188">IsAssociated</span><span class="sxs-lookup"><span data-stu-id="bd305-188">IsAssociated</span></span>](isassociated.md) <br/> |<span data-ttu-id="bd305-189">Указывает, является ли элемент связан с папкой.</span><span class="sxs-lookup"><span data-stu-id="bd305-189">Indicates whether the item is associated with a folder.</span></span>  <br/> |
|[<span data-ttu-id="bd305-190">WebClientReadFormQueryString</span><span class="sxs-lookup"><span data-stu-id="bd305-190">WebClientReadFormQueryString</span></span>](webclientreadformquerystring.md) <br/> |<span data-ttu-id="bd305-191">Представляет URL-адрес для присоединения к конечной точке Microsoft Office Outlook Web App для чтения элемента в Outlook Web App.</span><span class="sxs-lookup"><span data-stu-id="bd305-191">Represents a URL to concatenate to the Microsoft Office Outlook Web App endpoint to read an item in Outlook Web App.</span></span>  <br/> |
|[<span data-ttu-id="bd305-192">WebClientEditFormQueryString</span><span class="sxs-lookup"><span data-stu-id="bd305-192">WebClientEditFormQueryString</span></span>](webclienteditformquerystring.md) <br/> |<span data-ttu-id="bd305-193">Представляет URL-адрес для объединения в конечную точку Outlook Web App для редактирования элемента в Outlook Web App.</span><span class="sxs-lookup"><span data-stu-id="bd305-193">Represents a URL to concatenate to the Outlook Web App endpoint to edit an item in Outlook Web App.</span></span>  <br/> |
|[<span data-ttu-id="bd305-194">ConversationId</span><span class="sxs-lookup"><span data-stu-id="bd305-194">ConversationId</span></span>](conversationid.md) <br/> |<span data-ttu-id="bd305-195">Содержит идентификатор элемента или беседы.</span><span class="sxs-lookup"><span data-stu-id="bd305-195">Contains the identifier of an item or conversation.</span></span>  <br/> |
|[<span data-ttu-id="bd305-196">UniqueBody</span><span class="sxs-lookup"><span data-stu-id="bd305-196">UniqueBody</span></span>](uniquebody.md) <br/> |<span data-ttu-id="bd305-197">Представляет фрагмент HTML или обычный текст, который представляет уникальное body эту беседу.</span><span class="sxs-lookup"><span data-stu-id="bd305-197">Represents an HTML fragment or plain text which represents the unique body of this conversation.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="bd305-198">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="bd305-198">Parent elements</span></span>

|<span data-ttu-id="bd305-199">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="bd305-199">**Element**</span></span>|<span data-ttu-id="bd305-200">**Описание**</span><span class="sxs-lookup"><span data-stu-id="bd305-200">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bd305-201">AdjacentMeetings</span><span class="sxs-lookup"><span data-stu-id="bd305-201">AdjacentMeetings</span></span>](adjacentmeetings.md) <br/> |<span data-ttu-id="bd305-202">Описание всех элементов календаря, расположенных на время собрания.</span><span class="sxs-lookup"><span data-stu-id="bd305-202">Describes all calendar items that are adjacent to a meeting time.</span></span>  <br/> |
|[<span data-ttu-id="bd305-203">AppendToItemField</span><span class="sxs-lookup"><span data-stu-id="bd305-203">AppendToItemField</span></span>](appendtoitemfield.md) <br/> |<span data-ttu-id="bd305-204">Указывает данные для добавления к отдельное свойство item/папки во время [операции UpdateItem](updateitem-operation.md).</span><span class="sxs-lookup"><span data-stu-id="bd305-204">Identifies data to append to a single property of an item/folder during an [UpdateItem operation](updateitem-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="bd305-205">ConflictingMeetings</span><span class="sxs-lookup"><span data-stu-id="bd305-205">ConflictingMeetings</span></span>](conflictingmeetings.md) <br/> |<span data-ttu-id="bd305-206">Определяет все элементы, конфликтующие с время собрания.</span><span class="sxs-lookup"><span data-stu-id="bd305-206">Identifies all items that conflict with a meeting time.</span></span>  <br/> |
|[<span data-ttu-id="bd305-207">Создание (ItemSync)</span><span class="sxs-lookup"><span data-stu-id="bd305-207">Create (ItemSync)</span></span>](create-itemsync.md) <br/> |<span data-ttu-id="bd305-208">Определяет один элемент для создания в локальном хранилище клиента.</span><span class="sxs-lookup"><span data-stu-id="bd305-208">Identifies a single item to create in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="bd305-209">ItemAttachment</span><span class="sxs-lookup"><span data-stu-id="bd305-209">ItemAttachment</span></span>](itemattachment.md) <br/> |<span data-ttu-id="bd305-210">Представляет собой элемент Exchange, подключенный к другой элемент Exchange.</span><span class="sxs-lookup"><span data-stu-id="bd305-210">Represents an Exchange item that is attached to another Exchange item.</span></span>  <br/> |
|[<span data-ttu-id="bd305-211">Элементы</span><span class="sxs-lookup"><span data-stu-id="bd305-211">Items</span></span>](items.md) <br/> |<span data-ttu-id="bd305-212">Содержит массив элементов.</span><span class="sxs-lookup"><span data-stu-id="bd305-212">Contains an array of items.</span></span>  <br/> |
|[<span data-ttu-id="bd305-213">Элементы (NonEmptyArrayOfAllItemsType)</span><span class="sxs-lookup"><span data-stu-id="bd305-213">Items (NonEmptyArrayOfAllItemsType)</span></span>](items-nonemptyarrayofallitemstype.md) <br/> |<span data-ttu-id="bd305-214">Содержит массив элементов для создания в папке, указанной с помощью элемента [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) .</span><span class="sxs-lookup"><span data-stu-id="bd305-214">Contains an array of items to create in the folder that is identified by the [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) element.</span></span>  <br/> |
|[<span data-ttu-id="bd305-215">SetItemField</span><span class="sxs-lookup"><span data-stu-id="bd305-215">SetItemField</span></span>](setitemfield.md) <br/> |<span data-ttu-id="bd305-216">Представляет отдельное свойство элемента в [UpdateItem операции](updateitem-operation.md)обновления.</span><span class="sxs-lookup"><span data-stu-id="bd305-216">Represents an update to a single property of an item in an [UpdateItem operation](updateitem-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="bd305-217">Обновление (ItemSync)</span><span class="sxs-lookup"><span data-stu-id="bd305-217">Update (ItemSync)</span></span>](update-itemsync.md) <br/> |<span data-ttu-id="bd305-218">Определяет один элемент для обновления в локальном хранилище клиента.</span><span class="sxs-lookup"><span data-stu-id="bd305-218">Identifies a single item to update in the local client store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="bd305-219">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="bd305-219">Text value</span></span>

<span data-ttu-id="bd305-220">Нет.</span><span class="sxs-lookup"><span data-stu-id="bd305-220">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="bd305-221">Замечания</span><span class="sxs-lookup"><span data-stu-id="bd305-221">Remarks</span></span>

<span data-ttu-id="bd305-222">Важно Обратите внимание, что **ItemType** базовый тип для [задач](task.md), [элемента календаря, имеющего](calendaritem.md), [контакт](contact.md), [DistributionList](distributionlist.md)и [сообщения](message-ex15websvcsotherref.md).</span><span class="sxs-lookup"><span data-stu-id="bd305-222">It is important to note that **ItemType** is the base type for [Task](task.md), [CalendarItem](calendaritem.md), [Contact](contact.md), [DistributionList](distributionlist.md), and [Message](message-ex15websvcsotherref.md).</span></span>
  
<span data-ttu-id="bd305-223">Элементы [сообщения](message-ex15websvcsotherref.md) представляют сообщения электронной почты и другие элементы, которые не строго типизированные схемой веб-служб Exchange (EWS).</span><span class="sxs-lookup"><span data-stu-id="bd305-223">[Message](message-ex15websvcsotherref.md) elements represent e-mail messages and all other items that are not strongly typed by the Exchange Web Services (EWS) schema.</span></span> <span data-ttu-id="bd305-224">Элементы, такие как IPM. Общий доступ и IPM.InfoPath возвращаются в виде элементы **сообщения** .</span><span class="sxs-lookup"><span data-stu-id="bd305-224">Items such as IPM.Sharing and IPM.InfoPath are returned as **Message** elements.</span></span> <span data-ttu-id="bd305-225">Microsoft Exchange Server 2010 не возвращает **базовый элемент** в ответы.</span><span class="sxs-lookup"><span data-stu-id="bd305-225">Microsoft Exchange Server 2010 does not return the base **Item** element in responses.</span></span> 
  
<span data-ttu-id="bd305-226">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="bd305-226">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="bd305-227">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="bd305-227">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="bd305-228">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="bd305-228">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="bd305-229">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="bd305-229">Schema Name</span></span>  <br/> |<span data-ttu-id="bd305-230">Схема Types</span><span class="sxs-lookup"><span data-stu-id="bd305-230">Types schema</span></span>  <br/> |
|<span data-ttu-id="bd305-231">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="bd305-231">Validation File</span></span>  <br/> |<span data-ttu-id="bd305-232">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="bd305-232">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="bd305-233">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="bd305-233">Can be Empty</span></span>  <br/> |<span data-ttu-id="bd305-234">False</span><span class="sxs-lookup"><span data-stu-id="bd305-234">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="bd305-235">См. также</span><span class="sxs-lookup"><span data-stu-id="bd305-235">See also</span></span>



- [<span data-ttu-id="bd305-236">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="bd305-236">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
  
[<span data-ttu-id="bd305-237">Справка по веб-служб Exchange для Exchange</span><span class="sxs-lookup"><span data-stu-id="bd305-237">EWS reference for Exchange</span></span>](ews-reference-for-exchange.md)

