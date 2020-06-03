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
description: Элемент "i Item" представляет элемент POST в хранилище Exchange.
ms.openlocfilehash: 5fba1a9a6a3abc95ea2ce65cafa2b62bc7423f28
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44528869"
---
# <a name="postitem"></a><span data-ttu-id="472fb-103">PostItem</span><span class="sxs-lookup"><span data-stu-id="472fb-103">PostItem</span></span>

<span data-ttu-id="472fb-104">Элемент "i **Item** " представляет элемент POST в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="472fb-104">The **PostItem** element represents a post item in the Exchange store.</span></span> 
  
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

 <span data-ttu-id="472fb-105">**Неitemtype**</span><span class="sxs-lookup"><span data-stu-id="472fb-105">**PostItemType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="472fb-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="472fb-106">Attributes and elements</span></span>

<span data-ttu-id="472fb-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="472fb-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="472fb-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="472fb-108">Attributes</span></span>

<span data-ttu-id="472fb-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="472fb-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="472fb-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="472fb-110">Child elements</span></span>

|<span data-ttu-id="472fb-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="472fb-111">**Element**</span></span>|<span data-ttu-id="472fb-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="472fb-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="472fb-113">Сохранитьmimecontent</span><span class="sxs-lookup"><span data-stu-id="472fb-113">MimeContent</span></span>](mimecontent.md) <br/> |<span data-ttu-id="472fb-114">Содержит собственный многоцелевой поток расширений почты в Интернете (MIME) объекта, представленного в формате base64Binary.</span><span class="sxs-lookup"><span data-stu-id="472fb-114">Contains the native Multipurpose Internet Mail Extensions (MIME) stream of an object that is represented in base64Binary format.</span></span>  <br/> |
|[<span data-ttu-id="472fb-115">Идентификатор</span><span class="sxs-lookup"><span data-stu-id="472fb-115">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="472fb-116">Содержит уникальный идентификатор и ключ изменения элемента в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="472fb-116">Contains the unique identifier and change key of an item in the Exchange store.</span></span> <span data-ttu-id="472fb-117">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="472fb-117">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="472fb-118">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="472fb-118">ParentFolderId</span></span>](parentfolderid.md) <br/> |<span data-ttu-id="472fb-119">Представляет идентификатор родительской папки, содержащей элемент или папку.</span><span class="sxs-lookup"><span data-stu-id="472fb-119">Represents the identifier of the parent folder that contains the item or folder.</span></span> <span data-ttu-id="472fb-120">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="472fb-120">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="472fb-121">ItemClass</span><span class="sxs-lookup"><span data-stu-id="472fb-121">ItemClass</span></span>](itemclass.md) <br/> |<span data-ttu-id="472fb-122">Представляет класс сообщения для элемента.</span><span class="sxs-lookup"><span data-stu-id="472fb-122">Represents the message class of an item.</span></span>  <br/> |
|[<span data-ttu-id="472fb-123">Тема</span><span class="sxs-lookup"><span data-stu-id="472fb-123">Subject</span></span>](subject.md) <br/> |<span data-ttu-id="472fb-124">Представляет тему для элементов хранилища Exchange и объектов ответа.</span><span class="sxs-lookup"><span data-stu-id="472fb-124">Represents the subject for Exchange store items and response objects.</span></span> <span data-ttu-id="472fb-125">Тема может иметь не более 255 символов.</span><span class="sxs-lookup"><span data-stu-id="472fb-125">The subject is limited to 255 characters.</span></span>  <br/> |
|[<span data-ttu-id="472fb-126">Sensitivity</span><span class="sxs-lookup"><span data-stu-id="472fb-126">Sensitivity</span></span>](sensitivity.md) <br/> |<span data-ttu-id="472fb-127">Указывает уровень конфиденциальности элемента.</span><span class="sxs-lookup"><span data-stu-id="472fb-127">Indicates the sensitivity level of an item.</span></span>  <br/> |
|[<span data-ttu-id="472fb-128">Body</span><span class="sxs-lookup"><span data-stu-id="472fb-128">Body</span></span>](body.md) <br/> |<span data-ttu-id="472fb-129">Представляет реальное содержимое основного текста сообщения.</span><span class="sxs-lookup"><span data-stu-id="472fb-129">Represents the actual body content of a message.</span></span>  <br/> |
|[<span data-ttu-id="472fb-130">Вложения</span><span class="sxs-lookup"><span data-stu-id="472fb-130">Attachments</span></span>](attachments-ex15websvcsotherref.md) <br/> |<span data-ttu-id="472fb-131">Содержит элементы или файлы, вложенные в элемент в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="472fb-131">Contains the items or files that are attached to an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="472fb-132">DateTimeReceived</span><span class="sxs-lookup"><span data-stu-id="472fb-132">DateTimeReceived</span></span>](datetimereceived.md) <br/> |<span data-ttu-id="472fb-133">Представляет дату и время получения элемента в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="472fb-133">Represents the date and time that an item in a mailbox was received.</span></span>  <br/> |
|[<span data-ttu-id="472fb-134">Размер</span><span class="sxs-lookup"><span data-stu-id="472fb-134">Size</span></span>](size.md) <br/> |<span data-ttu-id="472fb-135">Представляет размер элемента в байтах.</span><span class="sxs-lookup"><span data-stu-id="472fb-135">Represents the size in bytes of an item.</span></span> <span data-ttu-id="472fb-136">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="472fb-136">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="472fb-137">Категории</span><span class="sxs-lookup"><span data-stu-id="472fb-137">Categories</span></span>](categories-ex15websvcsotherref.md) <br/> |<span data-ttu-id="472fb-138">Представляет коллекцию строк, определяющих категории, к которым относится элемент в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="472fb-138">Represents a collection of strings that identify the categories to which an item in the mailbox belongs.</span></span>  <br/> |
|[<span data-ttu-id="472fb-139">Importance</span><span class="sxs-lookup"><span data-stu-id="472fb-139">Importance</span></span>](importance.md) <br/> |<span data-ttu-id="472fb-140">Описывает важность элемента.</span><span class="sxs-lookup"><span data-stu-id="472fb-140">Describes the importance of an item.</span></span>  <br/> |
|[<span data-ttu-id="472fb-141">инреплито</span><span class="sxs-lookup"><span data-stu-id="472fb-141">InReplyTo</span></span>](inreplyto.md) <br/> |<span data-ttu-id="472fb-142">Представляет идентификатор элемента, который является ответом на этот элемент.</span><span class="sxs-lookup"><span data-stu-id="472fb-142">Represents the identifier of the item to which this item is a reply.</span></span>  <br/> |
|[<span data-ttu-id="472fb-143">Отправлено</span><span class="sxs-lookup"><span data-stu-id="472fb-143">IsSubmitted</span></span>](issubmitted.md) <br/> |<span data-ttu-id="472fb-144">Указывает, был ли элемент отправлен в папку "Исходящие" по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="472fb-144">Indicates whether an item has been submitted to the Outbox default folder.</span></span>  <br/> |
|[<span data-ttu-id="472fb-145">Черновик</span><span class="sxs-lookup"><span data-stu-id="472fb-145">IsDraft</span></span>](isdraft.md) <br/> |<span data-ttu-id="472fb-146">Указывает, был ли элемент еще не отправлен.</span><span class="sxs-lookup"><span data-stu-id="472fb-146">Represents whether an item has not yet been sent.</span></span>  <br/> |
|[<span data-ttu-id="472fb-147">исфромме</span><span class="sxs-lookup"><span data-stu-id="472fb-147">IsFromMe</span></span>](isfromme.md) <br/> |<span data-ttu-id="472fb-148">Указывает, отправляет ли пользователь элемент.</span><span class="sxs-lookup"><span data-stu-id="472fb-148">Indicates whether a user sent an item to him or herself.</span></span>  <br/> |
|[<span data-ttu-id="472fb-149">исресенд</span><span class="sxs-lookup"><span data-stu-id="472fb-149">IsResend</span></span>](isresend.md) <br/> |<span data-ttu-id="472fb-150">Указывает, был ли ранее отправлен элемент.</span><span class="sxs-lookup"><span data-stu-id="472fb-150">Indicates whether the item had previously been sent.</span></span>  <br/> |
|[<span data-ttu-id="472fb-151">исунмодифиед</span><span class="sxs-lookup"><span data-stu-id="472fb-151">IsUnmodified</span></span>](isunmodified.md) <br/> |<span data-ttu-id="472fb-152">Указывает, был ли изменен элемент.</span><span class="sxs-lookup"><span data-stu-id="472fb-152">Indicates whether the item has been modified.</span></span>  <br/> |
|[<span data-ttu-id="472fb-153">InternetMessageHeaders</span><span class="sxs-lookup"><span data-stu-id="472fb-153">InternetMessageHeaders</span></span>](internetmessageheaders.md) <br/> |<span data-ttu-id="472fb-154">Представляет коллекцию всех заголовков сообщений Интернета, которые находятся в элементе почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="472fb-154">Represents the collection of all Internet message headers that are contained in an item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="472fb-155">датетимесент</span><span class="sxs-lookup"><span data-stu-id="472fb-155">DateTimeSent</span></span>](datetimesent.md) <br/> |<span data-ttu-id="472fb-156">Представляет дату и время отправки элемента в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="472fb-156">Represents the date and time that an item in a mailbox was sent.</span></span>  <br/> |
|[<span data-ttu-id="472fb-157">DateTimeCreated</span><span class="sxs-lookup"><span data-stu-id="472fb-157">DateTimeCreated</span></span>](datetimecreated.md) <br/> |<span data-ttu-id="472fb-158">Представляет дату и время создания определенного элемента в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="472fb-158">Represents the date and time that a given item in the mailbox was created.</span></span>  <br/> |
|[<span data-ttu-id="472fb-159">респонсеобжектс</span><span class="sxs-lookup"><span data-stu-id="472fb-159">ResponseObjects</span></span>](responseobjects.md) <br/> |<span data-ttu-id="472fb-160">Содержит коллекцию всех объектов ответа, связанных с элементом в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="472fb-160">Contains a collection of all the response objects that are associated with an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="472fb-161">реминдердуеби</span><span class="sxs-lookup"><span data-stu-id="472fb-161">ReminderDueBy</span></span>](reminderdueby.md) <br/> |<span data-ttu-id="472fb-162">Представляет дату и время возникновения события.</span><span class="sxs-lookup"><span data-stu-id="472fb-162">Represents the date and time when the event occurs.</span></span> <span data-ttu-id="472fb-163">Он используется элементом [реминдерминутесбефорестарт](reminderminutesbeforestart.md) для определения времени отображения напоминания.</span><span class="sxs-lookup"><span data-stu-id="472fb-163">This is used by the [ReminderMinutesBeforeStart](reminderminutesbeforestart.md) element to determine when the reminder is displayed.</span></span>  <br/> |
|[<span data-ttu-id="472fb-164">реминдериссет</span><span class="sxs-lookup"><span data-stu-id="472fb-164">ReminderIsSet</span></span>](reminderisset.md) <br/> |<span data-ttu-id="472fb-165">Указывает, задано ли напоминание для элемента в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="472fb-165">Indicates whether a reminder has been set for an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="472fb-166">ReminderMinutesBeforeStart</span><span class="sxs-lookup"><span data-stu-id="472fb-166">ReminderMinutesBeforeStart</span></span>](reminderminutesbeforestart.md) <br/> |<span data-ttu-id="472fb-167">Представляет количество минут до события при отображении напоминания.</span><span class="sxs-lookup"><span data-stu-id="472fb-167">Represents the number of minutes before an event when a reminder is displayed.</span></span>  <br/> |
|[<span data-ttu-id="472fb-168">дисплайкк</span><span class="sxs-lookup"><span data-stu-id="472fb-168">DisplayCc</span></span>](displaycc.md) <br/> |<span data-ttu-id="472fb-169">Представляет отображаемую строку, используемую для содержимого поля "копия".</span><span class="sxs-lookup"><span data-stu-id="472fb-169">Represents the display string that is used for the contents of the Cc box.</span></span> <span data-ttu-id="472fb-170">Это объединенная строка всех отображаемых имен получателей копии.</span><span class="sxs-lookup"><span data-stu-id="472fb-170">This is the concatenated string of all Cc recipient display names.</span></span>  <br/> |
|[<span data-ttu-id="472fb-171">дисплайто</span><span class="sxs-lookup"><span data-stu-id="472fb-171">DisplayTo</span></span>](displayto.md) <br/> |<span data-ttu-id="472fb-172">Представляет отображаемую строку, используемую для содержимого поля "Кому".</span><span class="sxs-lookup"><span data-stu-id="472fb-172">Represents the display string that is used for the contents of the To box.</span></span> <span data-ttu-id="472fb-173">Это объединенная строка для отображаемых имен получателей.</span><span class="sxs-lookup"><span data-stu-id="472fb-173">This is the concatenated string of all To recipient display names.</span></span>  <br/> |
|[<span data-ttu-id="472fb-174">HasAttachments</span><span class="sxs-lookup"><span data-stu-id="472fb-174">HasAttachments</span></span>](hasattachments.md) <br/> |<span data-ttu-id="472fb-175">Представляет свойство, которое имеет значение **true** , если элемент имеет по крайней мере одно вложение.</span><span class="sxs-lookup"><span data-stu-id="472fb-175">Represents a property that is set to **true** if an item has at least one attachment.</span></span> <span data-ttu-id="472fb-176">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="472fb-176">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="472fb-177">ExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="472fb-177">ExtendedProperty</span></span>](extendedproperty.md) <br/> |<span data-ttu-id="472fb-178">Определяет расширенные свойства для папок и элементов.</span><span class="sxs-lookup"><span data-stu-id="472fb-178">Identifies extended properties on folders and items.</span></span>  <br/> |
|[<span data-ttu-id="472fb-179">Culture</span><span class="sxs-lookup"><span data-stu-id="472fb-179">Culture</span></span>](culture.md) <br/> |<span data-ttu-id="472fb-180">Представляет язык и региональные параметры для определенного элемента в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="472fb-180">Represents the culture for a given item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="472fb-181">еффективеригхтс</span><span class="sxs-lookup"><span data-stu-id="472fb-181">EffectiveRights</span></span>](effectiverights.md) <br/> |<span data-ttu-id="472fb-182">Содержит права клиента на основе параметров разрешений для элемента или папки.</span><span class="sxs-lookup"><span data-stu-id="472fb-182">Contains the client's rights based on the permission settings for the item or folder.</span></span> <span data-ttu-id="472fb-183">Этот элемент доступен только для чтения.</span><span class="sxs-lookup"><span data-stu-id="472fb-183">This element is read-only.</span></span>  <br/> |
|[<span data-ttu-id="472fb-184">ластмодифиеднаме</span><span class="sxs-lookup"><span data-stu-id="472fb-184">LastModifiedName</span></span>](lastmodifiedname.md) <br/> |<span data-ttu-id="472fb-185">Содержит отображаемое имя последнего пользователя для изменения элемента.</span><span class="sxs-lookup"><span data-stu-id="472fb-185">Contains the display name of the last user to modify an item.</span></span>  <br/> |
|[<span data-ttu-id="472fb-186">LastModifiedTime</span><span class="sxs-lookup"><span data-stu-id="472fb-186">LastModifiedTime</span></span>](lastmodifiedtime.md) <br/> |<span data-ttu-id="472fb-187">Указывает время последнего изменения элемента.</span><span class="sxs-lookup"><span data-stu-id="472fb-187">Indicates when an item was last modified.</span></span>  <br/> |
|[<span data-ttu-id="472fb-188">Связанный</span><span class="sxs-lookup"><span data-stu-id="472fb-188">IsAssociated</span></span>](isassociated.md) <br/> |<span data-ttu-id="472fb-189">Указывает, связан ли элемент с папкой.</span><span class="sxs-lookup"><span data-stu-id="472fb-189">Indicates whether the item is associated with a folder.</span></span>  <br/> |
|[<span data-ttu-id="472fb-190">вебклиентреадформкуеристринг</span><span class="sxs-lookup"><span data-stu-id="472fb-190">WebClientReadFormQueryString</span></span>](webclientreadformquerystring.md) <br/> |<span data-ttu-id="472fb-191">Представляет URL-адрес для сцепления с конечной точкой Microsoft Office Outlook Web App для чтения элемента в Outlook Web App.</span><span class="sxs-lookup"><span data-stu-id="472fb-191">Represents a URL to concatenate to the Microsoft Office Outlook Web App endpoint to read an item in Outlook Web App.</span></span>  <br/> |
|[<span data-ttu-id="472fb-192">вебклиентедитформкуеристринг</span><span class="sxs-lookup"><span data-stu-id="472fb-192">WebClientEditFormQueryString</span></span>](webclienteditformquerystring.md) <br/> |<span data-ttu-id="472fb-193">Представляет URL-адрес для сцепления с конечной точкой Outlook Web App для изменения элемента в Outlook Web App.</span><span class="sxs-lookup"><span data-stu-id="472fb-193">Represents a URL to concatenate to the Outlook Web App endpoint to edit an item in Outlook Web App.</span></span>  <br/> |
|[<span data-ttu-id="472fb-194">ConversationId</span><span class="sxs-lookup"><span data-stu-id="472fb-194">ConversationId</span></span>](conversationid.md) <br/> |<span data-ttu-id="472fb-195">Содержит идентификатор элемента или беседы.</span><span class="sxs-lookup"><span data-stu-id="472fb-195">Contains the identifier of an item or conversation.</span></span>  <br/> |
|[<span data-ttu-id="472fb-196">UniqueBody</span><span class="sxs-lookup"><span data-stu-id="472fb-196">UniqueBody</span></span>](uniquebody.md) <br/> |<span data-ttu-id="472fb-197">Представляет фрагмент HTML или обычный текст, представляющий уникальный основной текст этой беседы.</span><span class="sxs-lookup"><span data-stu-id="472fb-197">Represents an HTML fragment or plain text which represents the unique body of this conversation.</span></span>  <br/> |
|[<span data-ttu-id="472fb-198">ConversationIndex</span><span class="sxs-lookup"><span data-stu-id="472fb-198">ConversationIndex</span></span>](conversationindex.md) <br/> |<span data-ttu-id="472fb-199">Содержит двоичный код, представляющий поток, к которому относится сообщение.</span><span class="sxs-lookup"><span data-stu-id="472fb-199">Contains a binary ID that represents the thread to which this message belongs.</span></span>  <br/> |
|[<span data-ttu-id="472fb-200">ConversationTopic</span><span class="sxs-lookup"><span data-stu-id="472fb-200">ConversationTopic</span></span>](conversationtopic.md) <br/> |<span data-ttu-id="472fb-201">Представляет идентификатор беседы.</span><span class="sxs-lookup"><span data-stu-id="472fb-201">Represents the conversation identifier.</span></span>  <br/> |
|[<span data-ttu-id="472fb-202">From</span><span class="sxs-lookup"><span data-stu-id="472fb-202">From</span></span>](from.md) <br/> |<span data-ttu-id="472fb-203">Представляет адрес, с которого отправлен элемент POST.</span><span class="sxs-lookup"><span data-stu-id="472fb-203">Represents the address from which the post item was sent.</span></span> <span data-ttu-id="472fb-204">Элемент **from** можно задать только во время создания.</span><span class="sxs-lookup"><span data-stu-id="472fb-204">The **From** element can only be set at creation time.</span></span>  <br/> |
|[<span data-ttu-id="472fb-205">InternetMessageId</span><span class="sxs-lookup"><span data-stu-id="472fb-205">InternetMessageId</span></span>](internetmessageid.md) <br/> |<span data-ttu-id="472fb-206">Представляет идентификатор сообщения Интернета для элемента.</span><span class="sxs-lookup"><span data-stu-id="472fb-206">Represents the Internet message identifier of an item.</span></span>  <br/> |
|[<span data-ttu-id="472fb-207">IsRead</span><span class="sxs-lookup"><span data-stu-id="472fb-207">IsRead</span></span>](isread.md) <br/> |<span data-ttu-id="472fb-208">Указывает, было ли Прочитано сообщение.</span><span class="sxs-lookup"><span data-stu-id="472fb-208">Indicates whether a message has been read.</span></span>  <br/> |
|[<span data-ttu-id="472fb-209">постедтиме</span><span class="sxs-lookup"><span data-stu-id="472fb-209">PostedTime</span></span>](postedtime.md) <br/> |<span data-ttu-id="472fb-210">Представляет время отправки почтового [элемента](postitem.md) .</span><span class="sxs-lookup"><span data-stu-id="472fb-210">Represents the time that a [PostItem](postitem.md) was posted.</span></span>  <br/> |
|[<span data-ttu-id="472fb-211">References</span><span class="sxs-lookup"><span data-stu-id="472fb-211">References</span></span>](references.md) <br/> |<span data-ttu-id="472fb-212">Представляет заголовок Usenet, используемый для связывания ответов с исходными сообщениями.</span><span class="sxs-lookup"><span data-stu-id="472fb-212">Represents the Usenet header that is used to associate replies with the original messages.</span></span>  <br/> |
|[<span data-ttu-id="472fb-213">Sender</span><span class="sxs-lookup"><span data-stu-id="472fb-213">Sender</span></span>](sender.md) <br/> |<span data-ttu-id="472fb-214">Определяет отправителя элемента.</span><span class="sxs-lookup"><span data-stu-id="472fb-214">Identifies the sender of an item.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="472fb-215">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="472fb-215">Parent elements</span></span>

|<span data-ttu-id="472fb-216">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="472fb-216">**Element**</span></span>|<span data-ttu-id="472fb-217">**Описание**</span><span class="sxs-lookup"><span data-stu-id="472fb-217">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="472fb-218">сетитемфиелд</span><span class="sxs-lookup"><span data-stu-id="472fb-218">SetItemField</span></span>](setitemfield.md) <br/> |<span data-ttu-id="472fb-219">Представляет обновление одного свойства элемента в операции UpdateItem.</span><span class="sxs-lookup"><span data-stu-id="472fb-219">Represents an update to a single property of an item in an UpdateItem operation.</span></span>  <br/> |
|[<span data-ttu-id="472fb-220">аппендтоитемфиелд</span><span class="sxs-lookup"><span data-stu-id="472fb-220">AppendToItemField</span></span>](appendtoitemfield.md) <br/> |<span data-ttu-id="472fb-221">Определяет данные, добавляемые к одному свойству элемента или папки во время [операции UpdateItem](updateitem-operation.md).</span><span class="sxs-lookup"><span data-stu-id="472fb-221">Identifies data to append to a single property of an item or folder during an [UpdateItem operation](updateitem-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="472fb-222">ItemAttachment</span><span class="sxs-lookup"><span data-stu-id="472fb-222">ItemAttachment</span></span>](itemattachment.md) <br/> |<span data-ttu-id="472fb-223">Представляет элемент Exchange, присоединенный к другому элементу Exchange.</span><span class="sxs-lookup"><span data-stu-id="472fb-223">Represents an Exchange item that is attached to another Exchange item.</span></span>  <br/> |
|[<span data-ttu-id="472fb-224">Create (Итемсинк)</span><span class="sxs-lookup"><span data-stu-id="472fb-224">Create (ItemSync)</span></span>](create-itemsync.md) <br/> |<span data-ttu-id="472fb-225">Определяет один элемент, который необходимо создать в локальном хранилище клиента.</span><span class="sxs-lookup"><span data-stu-id="472fb-225">Identifies a single item to create in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="472fb-226">Обновление (Итемсинк)</span><span class="sxs-lookup"><span data-stu-id="472fb-226">Update (ItemSync)</span></span>](update-itemsync.md) <br/> |<span data-ttu-id="472fb-227">Определяет один элемент для обновления в локальном хранилище клиента.</span><span class="sxs-lookup"><span data-stu-id="472fb-227">Identifies a single item to update in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="472fb-228">реадфлагчанже</span><span class="sxs-lookup"><span data-stu-id="472fb-228">ReadFlagChange</span></span>](readflagchange.md) <br/> |<span data-ttu-id="472fb-229">Возвращается в ответах [SyncFolderItems](syncfolderitems.md) при чтении элемента.</span><span class="sxs-lookup"><span data-stu-id="472fb-229">Returned in [SyncFolderItems](syncfolderitems.md) responses when an item has been read.</span></span> <span data-ttu-id="472fb-230">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="472fb-230">This property is read-only.</span></span> <span data-ttu-id="472fb-231">Этот элемент появился в Exchange 2007 с пакетом обновления 1.</span><span class="sxs-lookup"><span data-stu-id="472fb-231">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="472fb-232">Items</span><span class="sxs-lookup"><span data-stu-id="472fb-232">Items</span></span>](items.md) <br/> |<span data-ttu-id="472fb-233">Содержит массив элементов.</span><span class="sxs-lookup"><span data-stu-id="472fb-233">Contains an array of items.</span></span>  <br/> |
|[<span data-ttu-id="472fb-234">конфликтингмитингс</span><span class="sxs-lookup"><span data-stu-id="472fb-234">ConflictingMeetings</span></span>](conflictingmeetings.md) <br/> |<span data-ttu-id="472fb-235">Определяет все элементы, которые конфликтуют с временем собрания.</span><span class="sxs-lookup"><span data-stu-id="472fb-235">Identifies all items that conflict with a meeting time.</span></span>  <br/> |
|[<span data-ttu-id="472fb-236">аджацентмитингс</span><span class="sxs-lookup"><span data-stu-id="472fb-236">AdjacentMeetings</span></span>](adjacentmeetings.md) <br/> |<span data-ttu-id="472fb-237">Описывает все элементы календаря, смежные с временем собрания.</span><span class="sxs-lookup"><span data-stu-id="472fb-237">Describes all calendar items that are adjacent to a meeting time.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="472fb-238">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="472fb-238">Text value</span></span>

<span data-ttu-id="472fb-239">Нет.</span><span class="sxs-lookup"><span data-stu-id="472fb-239">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="472fb-240">Примечания</span><span class="sxs-lookup"><span data-stu-id="472fb-240">Remarks</span></span>

<span data-ttu-id="472fb-241">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="472fb-241">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="472fb-242">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="472fb-242">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="472fb-243">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="472fb-243">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="472fb-244">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="472fb-244">Schema Name</span></span>  <br/> |<span data-ttu-id="472fb-245">Схема Types</span><span class="sxs-lookup"><span data-stu-id="472fb-245">Types schema</span></span>  <br/> |
|<span data-ttu-id="472fb-246">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="472fb-246">Validation File</span></span>  <br/> |<span data-ttu-id="472fb-247">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="472fb-247">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="472fb-248">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="472fb-248">Can be Empty</span></span>  <br/> |<span data-ttu-id="472fb-249">False</span><span class="sxs-lookup"><span data-stu-id="472fb-249">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="472fb-250">См. также</span><span class="sxs-lookup"><span data-stu-id="472fb-250">See also</span></span>



- [<span data-ttu-id="472fb-251">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="472fb-251">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

