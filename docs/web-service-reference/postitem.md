---
title: PostItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- PostItem
api_type:
- schema
ms.assetid: 7727ed84-9591-4a1c-bb04-12129926499b
description: PostItem элемент представляет элемент post в хранилище Exchange.
ms.openlocfilehash: 3fb6d6cfe334999c93ca0238547dd5aee8150a5f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19834866"
---
# <a name="postitem"></a><span data-ttu-id="0eb2a-103">PostItem</span><span class="sxs-lookup"><span data-stu-id="0eb2a-103">PostItem</span></span>

<span data-ttu-id="0eb2a-104">Элемент **PostItem** представляет элемент post в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="0eb2a-104">The **PostItem** element represents a post item in the Exchange store.</span></span> 
  
```xml
<PostItem>
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
   <ConversationIndex/>
   <ConversationTopic/>
   <From/>
   <InternetMessageId/>
   <IsRead/>
   <PostedTime/>
   <References/>
   <Sender/>
</PostItem>
```

 <span data-ttu-id="0eb2a-105">**PostItemType**</span><span class="sxs-lookup"><span data-stu-id="0eb2a-105">**PostItemType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0eb2a-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="0eb2a-106">Attributes and elements</span></span>

<span data-ttu-id="0eb2a-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="0eb2a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0eb2a-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="0eb2a-108">Attributes</span></span>

<span data-ttu-id="0eb2a-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="0eb2a-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0eb2a-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="0eb2a-110">Child elements</span></span>

|<span data-ttu-id="0eb2a-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="0eb2a-111">**Element**</span></span>|<span data-ttu-id="0eb2a-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="0eb2a-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0eb2a-113">MimeContent</span><span class="sxs-lookup"><span data-stu-id="0eb2a-113">MimeContent</span></span>](mimecontent.md) <br/> |<span data-ttu-id="0eb2a-114">Содержит собственный поток Multipurpose Internet Mail Extensions (MIME), представленного в формате base64Binary объекта.</span><span class="sxs-lookup"><span data-stu-id="0eb2a-114">Contains the native Multipurpose Internet Mail Extensions (MIME) stream of an object that is represented in base64Binary format.</span></span>  <br/> |
|[<span data-ttu-id="0eb2a-115">Идентификатор элемента</span><span class="sxs-lookup"><span data-stu-id="0eb2a-115">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="0eb2a-116">Содержит уникальный идентификатор и меняет ключ элемента в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="0eb2a-116">Contains the unique identifier and change key of an item in the Exchange store.</span></span> <span data-ttu-id="0eb2a-117">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0eb2a-117">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="0eb2a-118">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="0eb2a-118">ParentFolderId</span></span>](parentfolderid.md) <br/> |<span data-ttu-id="0eb2a-119">Представляет идентификатор родительской папки, содержащей элемент или папку.</span><span class="sxs-lookup"><span data-stu-id="0eb2a-119">Represents the identifier of the parent folder that contains the item or folder.</span></span> <span data-ttu-id="0eb2a-120">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0eb2a-120">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="0eb2a-121">ItemClass</span><span class="sxs-lookup"><span data-stu-id="0eb2a-121">ItemClass</span></span>](itemclass.md) <br/> |<span data-ttu-id="0eb2a-122">Представляет класс сообщения элемента.</span><span class="sxs-lookup"><span data-stu-id="0eb2a-122">Represents the message class of an item.</span></span>  <br/> |
|[<span data-ttu-id="0eb2a-123">Subject</span><span class="sxs-lookup"><span data-stu-id="0eb2a-123">Subject</span></span>](subject.md) <br/> |<span data-ttu-id="0eb2a-124">Представляет тему для элементов хранилища Exchange и объекты ответа.</span><span class="sxs-lookup"><span data-stu-id="0eb2a-124">Represents the subject for Exchange store items and response objects.</span></span> <span data-ttu-id="0eb2a-125">Тема ограничена 255 символов.</span><span class="sxs-lookup"><span data-stu-id="0eb2a-125">The subject is limited to 255 characters.</span></span>  <br/> |
|[<span data-ttu-id="0eb2a-126">Уровень конфиденциальности сообщения</span><span class="sxs-lookup"><span data-stu-id="0eb2a-126">Sensitivity</span></span>](sensitivity.md) <br/> |<span data-ttu-id="0eb2a-127">Указывает уровень конфиденциальности для элемента.</span><span class="sxs-lookup"><span data-stu-id="0eb2a-127">Indicates the sensitivity level of an item.</span></span>  <br/> |
|[<span data-ttu-id="0eb2a-128">Body</span><span class="sxs-lookup"><span data-stu-id="0eb2a-128">Body</span></span>](body.md) <br/> |<span data-ttu-id="0eb2a-129">Представляет фактическое содержимое основного текста сообщения.</span><span class="sxs-lookup"><span data-stu-id="0eb2a-129">Represents the actual body content of a message.</span></span>  <br/> |
|[<span data-ttu-id="0eb2a-130">Вложения</span><span class="sxs-lookup"><span data-stu-id="0eb2a-130">Attachments</span></span>](attachments-ex15websvcsotherref.md) <br/> |<span data-ttu-id="0eb2a-131">Содержит элементы или файлы, подключенные к элементу в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="0eb2a-131">Contains the items or files that are attached to an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="0eb2a-132">DateTimeReceived</span><span class="sxs-lookup"><span data-stu-id="0eb2a-132">DateTimeReceived</span></span>](datetimereceived.md) <br/> |<span data-ttu-id="0eb2a-133">Представляет дату и время получения элемента в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="0eb2a-133">Represents the date and time that an item in a mailbox was received.</span></span>  <br/> |
|[<span data-ttu-id="0eb2a-134">Размер</span><span class="sxs-lookup"><span data-stu-id="0eb2a-134">Size</span></span>](size.md) <br/> |<span data-ttu-id="0eb2a-135">Представляет размер в байтах элемента.</span><span class="sxs-lookup"><span data-stu-id="0eb2a-135">Represents the size in bytes of an item.</span></span> <span data-ttu-id="0eb2a-136">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0eb2a-136">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="0eb2a-137">Категории</span><span class="sxs-lookup"><span data-stu-id="0eb2a-137">Categories</span></span>](categories-ex15websvcsotherref.md) <br/> |<span data-ttu-id="0eb2a-138">Представляет набор строк, которые определяют категории, к которым принадлежит элемент в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="0eb2a-138">Represents a collection of strings that identify the categories to which an item in the mailbox belongs.</span></span>  <br/> |
|[<span data-ttu-id="0eb2a-139">Важность</span><span class="sxs-lookup"><span data-stu-id="0eb2a-139">Importance</span></span>](importance.md) <br/> |<span data-ttu-id="0eb2a-140">Описывает важность элемента.</span><span class="sxs-lookup"><span data-stu-id="0eb2a-140">Describes the importance of an item.</span></span>  <br/> |
|[<span data-ttu-id="0eb2a-141">InReplyTo</span><span class="sxs-lookup"><span data-stu-id="0eb2a-141">InReplyTo</span></span>](inreplyto.md) <br/> |<span data-ttu-id="0eb2a-142">Представляет идентификатор элемента, к которому этот элемент является ее в ответ.</span><span class="sxs-lookup"><span data-stu-id="0eb2a-142">Represents the identifier of the item to which this item is a reply.</span></span>  <br/> |
|[<span data-ttu-id="0eb2a-143">IsSubmitted</span><span class="sxs-lookup"><span data-stu-id="0eb2a-143">IsSubmitted</span></span>](issubmitted.md) <br/> |<span data-ttu-id="0eb2a-144">Указывает, является ли элемент был отправлен исходящие папке по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="0eb2a-144">Indicates whether an item has been submitted to the Outbox default folder.</span></span>  <br/> |
|[<span data-ttu-id="0eb2a-145">IsDraft</span><span class="sxs-lookup"><span data-stu-id="0eb2a-145">IsDraft</span></span>](isdraft.md) <br/> |<span data-ttu-id="0eb2a-146">Представляет ли элемент еще не были отправлены.</span><span class="sxs-lookup"><span data-stu-id="0eb2a-146">Represents whether an item has not yet been sent.</span></span>  <br/> |
|[<span data-ttu-id="0eb2a-147">IsFromMe</span><span class="sxs-lookup"><span data-stu-id="0eb2a-147">IsFromMe</span></span>](isfromme.md) <br/> |<span data-ttu-id="0eb2a-148">Указывает, отправил ли пользователь элемента для его сами себя.</span><span class="sxs-lookup"><span data-stu-id="0eb2a-148">Indicates whether a user sent an item to him or herself.</span></span>  <br/> |
|[<span data-ttu-id="0eb2a-149">IsResend</span><span class="sxs-lookup"><span data-stu-id="0eb2a-149">IsResend</span></span>](isresend.md) <br/> |<span data-ttu-id="0eb2a-150">Указывает, является ли элемент ранее еще был отправлен.</span><span class="sxs-lookup"><span data-stu-id="0eb2a-150">Indicates whether the item had previously been sent.</span></span>  <br/> |
|[<span data-ttu-id="0eb2a-151">IsUnmodified</span><span class="sxs-lookup"><span data-stu-id="0eb2a-151">IsUnmodified</span></span>](isunmodified.md) <br/> |<span data-ttu-id="0eb2a-152">Указывает, были ли изменены элемента.</span><span class="sxs-lookup"><span data-stu-id="0eb2a-152">Indicates whether the item has been modified.</span></span>  <br/> |
|[<span data-ttu-id="0eb2a-153">InternetMessageHeaders</span><span class="sxs-lookup"><span data-stu-id="0eb2a-153">InternetMessageHeaders</span></span>](internetmessageheaders.md) <br/> |<span data-ttu-id="0eb2a-154">Представляет коллекцию всех заголовков сообщений Интернета, содержащихся в элемента в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="0eb2a-154">Represents the collection of all Internet message headers that are contained in an item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="0eb2a-155">DateTimeSent</span><span class="sxs-lookup"><span data-stu-id="0eb2a-155">DateTimeSent</span></span>](datetimesent.md) <br/> |<span data-ttu-id="0eb2a-156">Представляет дату и время отправки элемента в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="0eb2a-156">Represents the date and time that an item in a mailbox was sent.</span></span>  <br/> |
|[<span data-ttu-id="0eb2a-157">DateTimeCreated</span><span class="sxs-lookup"><span data-stu-id="0eb2a-157">DateTimeCreated</span></span>](datetimecreated.md) <br/> |<span data-ttu-id="0eb2a-158">Представляет дату и время создания данного элемента в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="0eb2a-158">Represents the date and time that a given item in the mailbox was created.</span></span>  <br/> |
|[<span data-ttu-id="0eb2a-159">ResponseObjects</span><span class="sxs-lookup"><span data-stu-id="0eb2a-159">ResponseObjects</span></span>](responseobjects.md) <br/> |<span data-ttu-id="0eb2a-160">Содержит коллекцию всех объектов ответа, которые связаны с элемента в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="0eb2a-160">Contains a collection of all the response objects that are associated with an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="0eb2a-161">ReminderDueBy</span><span class="sxs-lookup"><span data-stu-id="0eb2a-161">ReminderDueBy</span></span>](reminderdueby.md) <br/> |<span data-ttu-id="0eb2a-162">Представляет дату и время, когда происходит событие.</span><span class="sxs-lookup"><span data-stu-id="0eb2a-162">Represents the date and time when the event occurs.</span></span> <span data-ttu-id="0eb2a-163">Используется в элементе [ReminderMinutesBeforeStart](reminderminutesbeforestart.md) определить, когда отображается оповещение.</span><span class="sxs-lookup"><span data-stu-id="0eb2a-163">This is used by the [ReminderMinutesBeforeStart](reminderminutesbeforestart.md) element to determine when the reminder is displayed.</span></span>  <br/> |
|[<span data-ttu-id="0eb2a-164">ReminderIsSet</span><span class="sxs-lookup"><span data-stu-id="0eb2a-164">ReminderIsSet</span></span>](reminderisset.md) <br/> |<span data-ttu-id="0eb2a-165">Указывает, установлен ли напоминания для элемента в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="0eb2a-165">Indicates whether a reminder has been set for an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="0eb2a-166">ReminderMinutesBeforeStart</span><span class="sxs-lookup"><span data-stu-id="0eb2a-166">ReminderMinutesBeforeStart</span></span>](reminderminutesbeforestart.md) <br/> |<span data-ttu-id="0eb2a-167">Представляет число минут и только потом событие, когда отображается напоминание.</span><span class="sxs-lookup"><span data-stu-id="0eb2a-167">Represents the number of minutes before an event when a reminder is displayed.</span></span>  <br/> |
|[<span data-ttu-id="0eb2a-168">DisplayCc</span><span class="sxs-lookup"><span data-stu-id="0eb2a-168">DisplayCc</span></span>](displaycc.md) <br/> |<span data-ttu-id="0eb2a-169">Строка отображения, который используется для содержимого в поле "Копия".</span><span class="sxs-lookup"><span data-stu-id="0eb2a-169">Represents the display string that is used for the contents of the Cc box.</span></span> <span data-ttu-id="0eb2a-170">Это составное строка всех получателей отображаемые имена «копия».</span><span class="sxs-lookup"><span data-stu-id="0eb2a-170">This is the concatenated string of all Cc recipient display names.</span></span>  <br/> |
|[<span data-ttu-id="0eb2a-171">DisplayTo</span><span class="sxs-lookup"><span data-stu-id="0eb2a-171">DisplayTo</span></span>](displayto.md) <br/> |<span data-ttu-id="0eb2a-172">Строка отображения, который используется для содержимого в поле «Кому».</span><span class="sxs-lookup"><span data-stu-id="0eb2a-172">Represents the display string that is used for the contents of the To box.</span></span> <span data-ttu-id="0eb2a-173">Это составное строка всех для получателей отображаемые имена.</span><span class="sxs-lookup"><span data-stu-id="0eb2a-173">This is the concatenated string of all To recipient display names.</span></span>  <br/> |
|[<span data-ttu-id="0eb2a-174">HasAttachments</span><span class="sxs-lookup"><span data-stu-id="0eb2a-174">HasAttachments</span></span>](hasattachments.md) <br/> |<span data-ttu-id="0eb2a-175">Представляет свойство, которое задано значение **true,** Если у элемента есть по крайней мере одного вложения.</span><span class="sxs-lookup"><span data-stu-id="0eb2a-175">Represents a property that is set to **true** if an item has at least one attachment.</span></span> <span data-ttu-id="0eb2a-176">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0eb2a-176">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="0eb2a-177">ExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="0eb2a-177">ExtendedProperty</span></span>](extendedproperty.md) <br/> |<span data-ttu-id="0eb2a-178">Определяет расширенные свойства для папок и элементов.</span><span class="sxs-lookup"><span data-stu-id="0eb2a-178">Identifies extended properties on folders and items.</span></span>  <br/> |
|[<span data-ttu-id="0eb2a-179">Язык и региональные параметры</span><span class="sxs-lookup"><span data-stu-id="0eb2a-179">Culture</span></span>](culture.md) <br/> |<span data-ttu-id="0eb2a-180">Представляет язык и региональные параметры для заданного элемента в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="0eb2a-180">Represents the culture for a given item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="0eb2a-181">EffectiveRights</span><span class="sxs-lookup"><span data-stu-id="0eb2a-181">EffectiveRights</span></span>](effectiverights.md) <br/> |<span data-ttu-id="0eb2a-182">Содержит права клиента на основании параметров разрешений для элемента или папки.</span><span class="sxs-lookup"><span data-stu-id="0eb2a-182">Contains the client's rights based on the permission settings for the item or folder.</span></span> <span data-ttu-id="0eb2a-183">Этот элемент доступен только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0eb2a-183">This element is read-only.</span></span>  <br/> |
|[<span data-ttu-id="0eb2a-184">LastModifiedName</span><span class="sxs-lookup"><span data-stu-id="0eb2a-184">LastModifiedName</span></span>](lastmodifiedname.md) <br/> |<span data-ttu-id="0eb2a-185">Содержит отображаемое имя последнего пользователя, чтобы изменить элемент.</span><span class="sxs-lookup"><span data-stu-id="0eb2a-185">Contains the display name of the last user to modify an item.</span></span>  <br/> |
|[<span data-ttu-id="0eb2a-186">LastModifiedTime</span><span class="sxs-lookup"><span data-stu-id="0eb2a-186">LastModifiedTime</span></span>](lastmodifiedtime.md) <br/> |<span data-ttu-id="0eb2a-187">Указывает время последнего изменения элемента.</span><span class="sxs-lookup"><span data-stu-id="0eb2a-187">Indicates when an item was last modified.</span></span>  <br/> |
|[<span data-ttu-id="0eb2a-188">IsAssociated</span><span class="sxs-lookup"><span data-stu-id="0eb2a-188">IsAssociated</span></span>](isassociated.md) <br/> |<span data-ttu-id="0eb2a-189">Указывает, является ли элемент связан с папкой.</span><span class="sxs-lookup"><span data-stu-id="0eb2a-189">Indicates whether the item is associated with a folder.</span></span>  <br/> |
|[<span data-ttu-id="0eb2a-190">WebClientReadFormQueryString</span><span class="sxs-lookup"><span data-stu-id="0eb2a-190">WebClientReadFormQueryString</span></span>](webclientreadformquerystring.md) <br/> |<span data-ttu-id="0eb2a-191">Представляет URL-адрес для присоединения к конечной точке Microsoft Office Outlook Web App для чтения элемента в Outlook Web App.</span><span class="sxs-lookup"><span data-stu-id="0eb2a-191">Represents a URL to concatenate to the Microsoft Office Outlook Web App endpoint to read an item in Outlook Web App.</span></span>  <br/> |
|[<span data-ttu-id="0eb2a-192">WebClientEditFormQueryString</span><span class="sxs-lookup"><span data-stu-id="0eb2a-192">WebClientEditFormQueryString</span></span>](webclienteditformquerystring.md) <br/> |<span data-ttu-id="0eb2a-193">Представляет URL-адрес для объединения в конечную точку Outlook Web App для редактирования элемента в Outlook Web App.</span><span class="sxs-lookup"><span data-stu-id="0eb2a-193">Represents a URL to concatenate to the Outlook Web App endpoint to edit an item in Outlook Web App.</span></span>  <br/> |
|[<span data-ttu-id="0eb2a-194">ConversationId</span><span class="sxs-lookup"><span data-stu-id="0eb2a-194">ConversationId</span></span>](conversationid.md) <br/> |<span data-ttu-id="0eb2a-195">Содержит идентификатор элемента или беседы.</span><span class="sxs-lookup"><span data-stu-id="0eb2a-195">Contains the identifier of an item or conversation.</span></span>  <br/> |
|[<span data-ttu-id="0eb2a-196">UniqueBody</span><span class="sxs-lookup"><span data-stu-id="0eb2a-196">UniqueBody</span></span>](uniquebody.md) <br/> |<span data-ttu-id="0eb2a-197">Представляет фрагмент HTML или обычный текст, который представляет уникальное body эту беседу.</span><span class="sxs-lookup"><span data-stu-id="0eb2a-197">Represents an HTML fragment or plain text which represents the unique body of this conversation.</span></span>  <br/> |
|[<span data-ttu-id="0eb2a-198">ConversationIndex</span><span class="sxs-lookup"><span data-stu-id="0eb2a-198">ConversationIndex</span></span>](conversationindex.md) <br/> |<span data-ttu-id="0eb2a-199">Содержит двоичные идентификатор, представляющий поток, к которой принадлежит это сообщение.</span><span class="sxs-lookup"><span data-stu-id="0eb2a-199">Contains a binary ID that represents the thread to which this message belongs.</span></span>  <br/> |
|[<span data-ttu-id="0eb2a-200">ConversationTopic</span><span class="sxs-lookup"><span data-stu-id="0eb2a-200">ConversationTopic</span></span>](conversationtopic.md) <br/> |<span data-ttu-id="0eb2a-201">Представляет идентификатор беседы.</span><span class="sxs-lookup"><span data-stu-id="0eb2a-201">Represents the conversation identifier.</span></span>  <br/> |
|[<span data-ttu-id="0eb2a-202">From</span><span class="sxs-lookup"><span data-stu-id="0eb2a-202">From</span></span>](from.md) <br/> |<span data-ttu-id="0eb2a-203">Представляет адрес, с которого было отправлено элемента записи.</span><span class="sxs-lookup"><span data-stu-id="0eb2a-203">Represents the address from which the post item was sent.</span></span> <span data-ttu-id="0eb2a-204">Элемент **из** могут быть установлены только во время создания.</span><span class="sxs-lookup"><span data-stu-id="0eb2a-204">The **From** element can only be set at creation time.</span></span>  <br/> |
|[<span data-ttu-id="0eb2a-205">InternetMessageId</span><span class="sxs-lookup"><span data-stu-id="0eb2a-205">InternetMessageId</span></span>](internetmessageid.md) <br/> |<span data-ttu-id="0eb2a-206">Представляет идентификатор сообщения Интернета элемента.</span><span class="sxs-lookup"><span data-stu-id="0eb2a-206">Represents the Internet message identifier of an item.</span></span>  <br/> |
|[<span data-ttu-id="0eb2a-207">IsRead</span><span class="sxs-lookup"><span data-stu-id="0eb2a-207">IsRead</span></span>](isread.md) <br/> |<span data-ttu-id="0eb2a-208">Указывает, имеет ли чтение сообщения.</span><span class="sxs-lookup"><span data-stu-id="0eb2a-208">Indicates whether a message has been read.</span></span>  <br/> |
|[<span data-ttu-id="0eb2a-209">PostedTime</span><span class="sxs-lookup"><span data-stu-id="0eb2a-209">PostedTime</span></span>](postedtime.md) <br/> |<span data-ttu-id="0eb2a-210">Представляет время, добавившего [PostItem](postitem.md) .</span><span class="sxs-lookup"><span data-stu-id="0eb2a-210">Represents the time that a [PostItem](postitem.md) was posted.</span></span>  <br/> |
|[<span data-ttu-id="0eb2a-211">Справочные материалы</span><span class="sxs-lookup"><span data-stu-id="0eb2a-211">References</span></span>](references.md) <br/> |<span data-ttu-id="0eb2a-212">Представляет заголовок групп, используемый для связи ответов с исходного сообщения.</span><span class="sxs-lookup"><span data-stu-id="0eb2a-212">Represents the Usenet header that is used to associate replies with the original messages.</span></span>  <br/> |
|[<span data-ttu-id="0eb2a-213">Отправитель</span><span class="sxs-lookup"><span data-stu-id="0eb2a-213">Sender</span></span>](sender.md) <br/> |<span data-ttu-id="0eb2a-214">Идентифицирует отправителя элемента.</span><span class="sxs-lookup"><span data-stu-id="0eb2a-214">Identifies the sender of an item.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="0eb2a-215">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="0eb2a-215">Parent elements</span></span>

|<span data-ttu-id="0eb2a-216">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="0eb2a-216">**Element**</span></span>|<span data-ttu-id="0eb2a-217">**Описание**</span><span class="sxs-lookup"><span data-stu-id="0eb2a-217">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0eb2a-218">SetItemField</span><span class="sxs-lookup"><span data-stu-id="0eb2a-218">SetItemField</span></span>](setitemfield.md) <br/> |<span data-ttu-id="0eb2a-219">Представляет обновление для одного свойства элемента в рамках одной операции UpdateItem.</span><span class="sxs-lookup"><span data-stu-id="0eb2a-219">Represents an update to a single property of an item in an UpdateItem operation.</span></span>  <br/> |
|[<span data-ttu-id="0eb2a-220">AppendToItemField</span><span class="sxs-lookup"><span data-stu-id="0eb2a-220">AppendToItemField</span></span>](appendtoitemfield.md) <br/> |<span data-ttu-id="0eb2a-221">Указывает данные для добавления во время [операции UpdateItem](updateitem-operation.md)отдельное свойство элемента или папки.</span><span class="sxs-lookup"><span data-stu-id="0eb2a-221">Identifies data to append to a single property of an item or folder during an [UpdateItem operation](updateitem-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="0eb2a-222">ItemAttachment</span><span class="sxs-lookup"><span data-stu-id="0eb2a-222">ItemAttachment</span></span>](itemattachment.md) <br/> |<span data-ttu-id="0eb2a-223">Представляет собой элемент Exchange, подключенный к другой элемент Exchange.</span><span class="sxs-lookup"><span data-stu-id="0eb2a-223">Represents an Exchange item that is attached to another Exchange item.</span></span>  <br/> |
|[<span data-ttu-id="0eb2a-224">Создание (ItemSync)</span><span class="sxs-lookup"><span data-stu-id="0eb2a-224">Create (ItemSync)</span></span>](create-itemsync.md) <br/> |<span data-ttu-id="0eb2a-225">Определяет один элемент для создания в локальном хранилище клиента.</span><span class="sxs-lookup"><span data-stu-id="0eb2a-225">Identifies a single item to create in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="0eb2a-226">Обновление (ItemSync)</span><span class="sxs-lookup"><span data-stu-id="0eb2a-226">Update (ItemSync)</span></span>](update-itemsync.md) <br/> |<span data-ttu-id="0eb2a-227">Определяет один элемент для обновления в локальном хранилище клиента.</span><span class="sxs-lookup"><span data-stu-id="0eb2a-227">Identifies a single item to update in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="0eb2a-228">ReadFlagChange</span><span class="sxs-lookup"><span data-stu-id="0eb2a-228">ReadFlagChange</span></span>](readflagchange.md) <br/> |<span data-ttu-id="0eb2a-229">Возвращаются в ответы [SyncFolderItems](syncfolderitems.md) прочтении элемента.</span><span class="sxs-lookup"><span data-stu-id="0eb2a-229">Returned in [SyncFolderItems](syncfolderitems.md) responses when an item has been read.</span></span> <span data-ttu-id="0eb2a-230">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0eb2a-230">This property is read-only.</span></span> <span data-ttu-id="0eb2a-231">Этот элемент появился в Exchange 2007 с пакетом обновления 1.</span><span class="sxs-lookup"><span data-stu-id="0eb2a-231">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="0eb2a-232">Элементы</span><span class="sxs-lookup"><span data-stu-id="0eb2a-232">Items</span></span>](items.md) <br/> |<span data-ttu-id="0eb2a-233">Содержит массив элементов.</span><span class="sxs-lookup"><span data-stu-id="0eb2a-233">Contains an array of items.</span></span>  <br/> |
|[<span data-ttu-id="0eb2a-234">ConflictingMeetings</span><span class="sxs-lookup"><span data-stu-id="0eb2a-234">ConflictingMeetings</span></span>](conflictingmeetings.md) <br/> |<span data-ttu-id="0eb2a-235">Определяет все элементы, конфликтующие с время собрания.</span><span class="sxs-lookup"><span data-stu-id="0eb2a-235">Identifies all items that conflict with a meeting time.</span></span>  <br/> |
|[<span data-ttu-id="0eb2a-236">AdjacentMeetings</span><span class="sxs-lookup"><span data-stu-id="0eb2a-236">AdjacentMeetings</span></span>](adjacentmeetings.md) <br/> |<span data-ttu-id="0eb2a-237">Описание всех элементов календаря, расположенных на время собрания.</span><span class="sxs-lookup"><span data-stu-id="0eb2a-237">Describes all calendar items that are adjacent to a meeting time.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="0eb2a-238">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="0eb2a-238">Text value</span></span>

<span data-ttu-id="0eb2a-239">Нет.</span><span class="sxs-lookup"><span data-stu-id="0eb2a-239">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="0eb2a-240">Замечания</span><span class="sxs-lookup"><span data-stu-id="0eb2a-240">Remarks</span></span>

<span data-ttu-id="0eb2a-241">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="0eb2a-241">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0eb2a-242">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="0eb2a-242">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0eb2a-243">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="0eb2a-243">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="0eb2a-244">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="0eb2a-244">Schema Name</span></span>  <br/> |<span data-ttu-id="0eb2a-245">Схема Types</span><span class="sxs-lookup"><span data-stu-id="0eb2a-245">Types schema</span></span>  <br/> |
|<span data-ttu-id="0eb2a-246">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="0eb2a-246">Validation File</span></span>  <br/> |<span data-ttu-id="0eb2a-247">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="0eb2a-247">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="0eb2a-248">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="0eb2a-248">Can be Empty</span></span>  <br/> |<span data-ttu-id="0eb2a-249">False</span><span class="sxs-lookup"><span data-stu-id="0eb2a-249">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0eb2a-250">См. также</span><span class="sxs-lookup"><span data-stu-id="0eb2a-250">See also</span></span>



- [<span data-ttu-id="0eb2a-251">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="0eb2a-251">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

