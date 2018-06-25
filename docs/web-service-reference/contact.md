---
title: Контакт
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Contact
api_type:
- schema
ms.assetid: 66bfff50-7a91-4d81-b6a0-610b9962f677
description: Элемент контакта представляет элемента контакта в хранилище Exchange.
ms.openlocfilehash: 7b2e7c0197914c2a0a0ba3815dd05fca52a5f872
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761731"
---
# <a name="contact"></a><span data-ttu-id="64d19-103">Контакт</span><span class="sxs-lookup"><span data-stu-id="64d19-103">Contact</span></span>

<span data-ttu-id="64d19-104">Элемент **контактов** представляет элемента контакта в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="64d19-104">The **Contact** element represents a contact item in the Exchange store.</span></span> 
  
```XML
<Contact>
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
   <FileAs/>
   <FileAsMapping/>
   <DisplayName/>
   <GivenName/>
   <Initials/>
   <MiddleName/>
   <Nickname/>
   <CompleteName/>
   <CompanyName/>
   <EmailAddresses/>
   <PhysicalAddresses/>
   <PhoneNumbers/>
   <AssistantName/>
   <Birthday/>
   <BusinessHomePage/>
   <Children/>
   <Companies/>
   <ContactSource/>
   <Department/>
   <Generation/>
   <ImAddresses/>
   <JobTitle/>
   <Manager/>
   <Mileage/>
   <OfficeLocation/>
   <PostalAddressIndex/>
   <Profession/>
   <SpouseName/>
   <Surname/>
   <WeddingAnniversary/>
   <HasPicture/>
   <PhoneticFullName/>
   <PhoneticFirstName/>
   <PhoneticLastName/>
   <Alias/>
   <Notes/>
   <Photo/>
   <UserSMIMECertificate/>
   <MSExchangeCertificate/>
   <DirectoryId/>
   <ManagerMailbox/>
   <DirectReports/>
</Contact>
```

 <span data-ttu-id="64d19-105">**ContactItemType**</span><span class="sxs-lookup"><span data-stu-id="64d19-105">**ContactItemType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="64d19-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="64d19-106">Attributes and elements</span></span>

<span data-ttu-id="64d19-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="64d19-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="64d19-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="64d19-108">Attributes</span></span>

<span data-ttu-id="64d19-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="64d19-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="64d19-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="64d19-110">Child elements</span></span>

|<span data-ttu-id="64d19-111">**Имя элемента**</span><span class="sxs-lookup"><span data-stu-id="64d19-111">**Element name**</span></span>|<span data-ttu-id="64d19-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="64d19-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="64d19-113">MimeContent</span><span class="sxs-lookup"><span data-stu-id="64d19-113">MimeContent</span></span>](mimecontent.md) <br/> |<span data-ttu-id="64d19-114">Содержит собственный поток Multipurpose Internet Mail Extensions (MIME), представленного в формате base64Binary объекта.</span><span class="sxs-lookup"><span data-stu-id="64d19-114">Contains the native Multipurpose Internet Mail Extensions (MIME) stream of an object that is represented in base64Binary format.</span></span>  <br/> |
|[<span data-ttu-id="64d19-115">Идентификатор элемента</span><span class="sxs-lookup"><span data-stu-id="64d19-115">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="64d19-116">Содержит уникальный идентификатор и меняет ключ элемента в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="64d19-116">Contains the unique identifier and change key of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="64d19-117">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="64d19-117">ParentFolderId</span></span>](parentfolderid.md) <br/> |<span data-ttu-id="64d19-118">Представляет идентификатор родительской папки, содержащей элемент или папку.</span><span class="sxs-lookup"><span data-stu-id="64d19-118">Represents the identifier of the parent folder that contains the item or folder.</span></span>  <br/> |
|[<span data-ttu-id="64d19-119">ItemClass</span><span class="sxs-lookup"><span data-stu-id="64d19-119">ItemClass</span></span>](itemclass.md) <br/> |<span data-ttu-id="64d19-120">Представляет класс сообщения элемента.</span><span class="sxs-lookup"><span data-stu-id="64d19-120">Represents the message class of an item.</span></span>  <br/> |
|[<span data-ttu-id="64d19-121">Subject</span><span class="sxs-lookup"><span data-stu-id="64d19-121">Subject</span></span>](subject.md) <br/> |<span data-ttu-id="64d19-122">Представляет тему для элементов хранилища Exchange и объекты ответа.</span><span class="sxs-lookup"><span data-stu-id="64d19-122">Represents the subject for Exchange store items and response objects.</span></span>  <br/> |
|[<span data-ttu-id="64d19-123">Уровень конфиденциальности сообщения</span><span class="sxs-lookup"><span data-stu-id="64d19-123">Sensitivity</span></span>](sensitivity.md) <br/> |<span data-ttu-id="64d19-124">Указывает уровень конфиденциальности для элемента.</span><span class="sxs-lookup"><span data-stu-id="64d19-124">Indicates the sensitivity level of an item.</span></span>  <br/> |
|[<span data-ttu-id="64d19-125">Body</span><span class="sxs-lookup"><span data-stu-id="64d19-125">Body</span></span>](body.md) <br/> |<span data-ttu-id="64d19-126">Представляет фактическое содержимое основного текста сообщения.</span><span class="sxs-lookup"><span data-stu-id="64d19-126">Represents the actual body content of a message.</span></span>  <br/> |
|[<span data-ttu-id="64d19-127">Вложения</span><span class="sxs-lookup"><span data-stu-id="64d19-127">Attachments</span></span>](attachments-ex15websvcsotherref.md) <br/> |<span data-ttu-id="64d19-128">Содержит элементы или файлы, подключенные к элементу в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="64d19-128">Contains the items or files that are attached to an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="64d19-129">DateTimeReceived</span><span class="sxs-lookup"><span data-stu-id="64d19-129">DateTimeReceived</span></span>](datetimereceived.md) <br/> |<span data-ttu-id="64d19-130">Представляет дату и время получения элемента в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="64d19-130">Represents the date and time that an item in a mailbox was received.</span></span>  <br/> |
|[<span data-ttu-id="64d19-131">Размер</span><span class="sxs-lookup"><span data-stu-id="64d19-131">Size</span></span>](size.md) <br/> |<span data-ttu-id="64d19-132">Представляет размер в байтах элемента.</span><span class="sxs-lookup"><span data-stu-id="64d19-132">Represents the size in bytes of an item.</span></span> <span data-ttu-id="64d19-133">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="64d19-133">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="64d19-134">Категории</span><span class="sxs-lookup"><span data-stu-id="64d19-134">Categories</span></span>](categories-ex15websvcsotherref.md) <br/> |<span data-ttu-id="64d19-135">Представляет набор строк, чтобы указать, к какой категории относится элемент в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="64d19-135">Represents a collection of strings that identify to which categories an item in the mailbox belongs.</span></span>  <br/> |
|[<span data-ttu-id="64d19-136">Важность</span><span class="sxs-lookup"><span data-stu-id="64d19-136">Importance</span></span>](importance.md) <br/> |<span data-ttu-id="64d19-137">Описывает важность элемента.</span><span class="sxs-lookup"><span data-stu-id="64d19-137">Describes the importance of an item.</span></span>  <br/> |
|[<span data-ttu-id="64d19-138">InReplyTo</span><span class="sxs-lookup"><span data-stu-id="64d19-138">InReplyTo</span></span>](inreplyto.md) <br/> |<span data-ttu-id="64d19-139">Представляет идентификатор элемента, к которому этот элемент является ее в ответ.</span><span class="sxs-lookup"><span data-stu-id="64d19-139">Represents the identifier of the item to which this item is a reply.</span></span>  <br/> |
|[<span data-ttu-id="64d19-140">IsSubmitted</span><span class="sxs-lookup"><span data-stu-id="64d19-140">IsSubmitted</span></span>](issubmitted.md) <br/> |<span data-ttu-id="64d19-141">Указывает, является ли элемент был отправлен исходящие папке по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="64d19-141">Indicates whether an item has been submitted to the Outbox default folder.</span></span>  <br/> |
|[<span data-ttu-id="64d19-142">IsDraft</span><span class="sxs-lookup"><span data-stu-id="64d19-142">IsDraft</span></span>](isdraft.md) <br/> |<span data-ttu-id="64d19-143">Представляет ли элемент еще не были отправлены.</span><span class="sxs-lookup"><span data-stu-id="64d19-143">Represents whether an item has not yet been sent.</span></span>  <br/> |
|[<span data-ttu-id="64d19-144">IsFromMe</span><span class="sxs-lookup"><span data-stu-id="64d19-144">IsFromMe</span></span>](isfromme.md) <br/> |<span data-ttu-id="64d19-145">Показывает пользователя отправить элемент в себе.</span><span class="sxs-lookup"><span data-stu-id="64d19-145">Indicates whether a user sent an item to himself or herself.</span></span>  <br/> |
|[<span data-ttu-id="64d19-146">IsResend</span><span class="sxs-lookup"><span data-stu-id="64d19-146">IsResend</span></span>](isresend.md) <br/> |<span data-ttu-id="64d19-147">Указывает, является ли элемент ранее еще был отправлен.</span><span class="sxs-lookup"><span data-stu-id="64d19-147">Indicates whether the item had previously been sent.</span></span>  <br/> |
|[<span data-ttu-id="64d19-148">IsUnmodified</span><span class="sxs-lookup"><span data-stu-id="64d19-148">IsUnmodified</span></span>](isunmodified.md) <br/> |<span data-ttu-id="64d19-149">Указывает, были ли изменены элемента.</span><span class="sxs-lookup"><span data-stu-id="64d19-149">Indicates whether the item has been modified.</span></span>  <br/> |
|[<span data-ttu-id="64d19-150">InternetMessageHeaders</span><span class="sxs-lookup"><span data-stu-id="64d19-150">InternetMessageHeaders</span></span>](internetmessageheaders.md) <br/> |<span data-ttu-id="64d19-151">Представляет коллекцию всех заголовков сообщений Интернета, содержащихся в элемента в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="64d19-151">Represents the collection of all Internet message headers that are contained in an item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="64d19-152">DateTimeSent</span><span class="sxs-lookup"><span data-stu-id="64d19-152">DateTimeSent</span></span>](datetimesent.md) <br/> |<span data-ttu-id="64d19-153">Представляет дату и время отправки элемента в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="64d19-153">Represents the date and time that an item in a mailbox was sent.</span></span>  <br/> |
|[<span data-ttu-id="64d19-154">DateTimeCreated</span><span class="sxs-lookup"><span data-stu-id="64d19-154">DateTimeCreated</span></span>](datetimecreated.md) <br/> |<span data-ttu-id="64d19-155">Представляет дату и время создания данного элемента в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="64d19-155">Represents the date and time that a given item in the mailbox was created.</span></span>  <br/> |
|[<span data-ttu-id="64d19-156">ResponseObjects</span><span class="sxs-lookup"><span data-stu-id="64d19-156">ResponseObjects</span></span>](responseobjects.md) <br/> |<span data-ttu-id="64d19-157">Содержит коллекцию всех объектов ответа, которые связаны с элемента в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="64d19-157">Contains a collection of all the response objects that are associated with an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="64d19-158">ReminderDueBy</span><span class="sxs-lookup"><span data-stu-id="64d19-158">ReminderDueBy</span></span>](reminderdueby.md) <br/> |<span data-ttu-id="64d19-159">Представляет дату и время, когда происходит событие.</span><span class="sxs-lookup"><span data-stu-id="64d19-159">Represents the date and time when the event occurs.</span></span> <span data-ttu-id="64d19-160">Используется в элементе [ReminderMinutesBeforeStart](reminderminutesbeforestart.md) определить, когда отображается оповещение.</span><span class="sxs-lookup"><span data-stu-id="64d19-160">This is used by the [ReminderMinutesBeforeStart](reminderminutesbeforestart.md) element to determine when the reminder is displayed.</span></span>  <br/> |
|[<span data-ttu-id="64d19-161">ReminderIsSet</span><span class="sxs-lookup"><span data-stu-id="64d19-161">ReminderIsSet</span></span>](reminderisset.md) <br/> |<span data-ttu-id="64d19-162">Указывает, установлен ли напоминания для элемента в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="64d19-162">Indicates whether a reminder has been set for an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="64d19-163">ReminderMinutesBeforeStart</span><span class="sxs-lookup"><span data-stu-id="64d19-163">ReminderMinutesBeforeStart</span></span>](reminderminutesbeforestart.md) <br/> |<span data-ttu-id="64d19-164">Представляет число минут и только потом событие, когда отображается напоминание.</span><span class="sxs-lookup"><span data-stu-id="64d19-164">Represents the number of minutes before an event when a reminder is displayed.</span></span>  <br/> |
|[<span data-ttu-id="64d19-165">DisplayCc</span><span class="sxs-lookup"><span data-stu-id="64d19-165">DisplayCc</span></span>](displaycc.md) <br/> |<span data-ttu-id="64d19-166">Строка отображения, который используется для содержимого строку "Копия".</span><span class="sxs-lookup"><span data-stu-id="64d19-166">Represents the display string that is used for the contents of the Cc line.</span></span> <span data-ttu-id="64d19-167">Это составное строка всех получателей отображаемые имена «копия».</span><span class="sxs-lookup"><span data-stu-id="64d19-167">This is the concatenated string of all Cc recipient display names.</span></span>  <br/> |
|[<span data-ttu-id="64d19-168">DisplayTo</span><span class="sxs-lookup"><span data-stu-id="64d19-168">DisplayTo</span></span>](displayto.md) <br/> |<span data-ttu-id="64d19-169">Строка отображения, который используется для содержимого строке.</span><span class="sxs-lookup"><span data-stu-id="64d19-169">Represents the display string that is used for the contents of the To line.</span></span> <span data-ttu-id="64d19-170">Это составное строка всех для получателей отображаемые имена.</span><span class="sxs-lookup"><span data-stu-id="64d19-170">This is the concatenated string of all To recipient display names.</span></span>  <br/> |
|[<span data-ttu-id="64d19-171">HasAttachments</span><span class="sxs-lookup"><span data-stu-id="64d19-171">HasAttachments</span></span>](hasattachments.md) <br/> |<span data-ttu-id="64d19-172">Представляет свойство, которое задано значение **true,** Если у элемента есть по крайней мере один видимым вложения.</span><span class="sxs-lookup"><span data-stu-id="64d19-172">Represents a property that is set to **true** if an item has at least one visible attachment.</span></span> <span data-ttu-id="64d19-173">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="64d19-173">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="64d19-174">ExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="64d19-174">ExtendedProperty</span></span>](extendedproperty.md) <br/> |<span data-ttu-id="64d19-175">Определяет расширенные свойства для папок и элементов.</span><span class="sxs-lookup"><span data-stu-id="64d19-175">Identifies extended properties on folders and items.</span></span>  <br/> |
|[<span data-ttu-id="64d19-176">Язык и региональные параметры</span><span class="sxs-lookup"><span data-stu-id="64d19-176">Culture</span></span>](culture.md) <br/> |<span data-ttu-id="64d19-177">Представляет язык и региональные параметры для заданного элемента в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="64d19-177">Represents the culture for a given item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="64d19-178">EffectiveRights</span><span class="sxs-lookup"><span data-stu-id="64d19-178">EffectiveRights</span></span>](effectiverights.md) <br/> |<span data-ttu-id="64d19-179">Содержит права клиента на основании параметров разрешений для элемента или папки.</span><span class="sxs-lookup"><span data-stu-id="64d19-179">Contains the client's rights based on the permission settings for the item or folder.</span></span> <span data-ttu-id="64d19-180">Этот элемент доступен только для чтения.</span><span class="sxs-lookup"><span data-stu-id="64d19-180">This element is read-only.</span></span>  <br/> |
|[<span data-ttu-id="64d19-181">LastModifiedName</span><span class="sxs-lookup"><span data-stu-id="64d19-181">LastModifiedName</span></span>](lastmodifiedname.md) <br/> |<span data-ttu-id="64d19-182">Содержит отображаемое имя последнего пользователя, чтобы изменить элемент.</span><span class="sxs-lookup"><span data-stu-id="64d19-182">Contains the display name of the last user to modify an item.</span></span>  <br/> |
|[<span data-ttu-id="64d19-183">LastModifiedTime</span><span class="sxs-lookup"><span data-stu-id="64d19-183">LastModifiedTime</span></span>](lastmodifiedtime.md) <br/> |<span data-ttu-id="64d19-184">Указывает время последнего изменения элемента.</span><span class="sxs-lookup"><span data-stu-id="64d19-184">Indicates when an item was last modified.</span></span>  <br/> |
|[<span data-ttu-id="64d19-185">IsAssociated</span><span class="sxs-lookup"><span data-stu-id="64d19-185">IsAssociated</span></span>](isassociated.md) <br/> |<span data-ttu-id="64d19-186">Указывает, является ли элемент связан с папкой.</span><span class="sxs-lookup"><span data-stu-id="64d19-186">Indicates whether the item is associated with a folder.</span></span>  <br/> |
|[<span data-ttu-id="64d19-187">WebClientReadFormQueryString</span><span class="sxs-lookup"><span data-stu-id="64d19-187">WebClientReadFormQueryString</span></span>](webclientreadformquerystring.md) <br/> |<span data-ttu-id="64d19-188">Представляет URL-адрес для присоединения к конечной точке Microsoft Office Outlook Web App для чтения элемента в Outlook Web App.</span><span class="sxs-lookup"><span data-stu-id="64d19-188">Represents a URL to concatenate to the Microsoft Office Outlook Web App endpoint to read an item in Outlook Web App.</span></span>  <br/> |
|[<span data-ttu-id="64d19-189">WebClientEditFormQueryString</span><span class="sxs-lookup"><span data-stu-id="64d19-189">WebClientEditFormQueryString</span></span>](webclienteditformquerystring.md) <br/> |<span data-ttu-id="64d19-190">Представляет URL-адрес для объединения в конечную точку Outlook Web App для редактирования элемента в Outlook Web App.</span><span class="sxs-lookup"><span data-stu-id="64d19-190">Represents a URL to concatenate to the Outlook Web App endpoint to edit an item in Outlook Web App.</span></span>  <br/> |
|[<span data-ttu-id="64d19-191">ConversationId</span><span class="sxs-lookup"><span data-stu-id="64d19-191">ConversationId</span></span>](conversationid.md) <br/> |<span data-ttu-id="64d19-192">Содержит идентификатор элемента или беседы.</span><span class="sxs-lookup"><span data-stu-id="64d19-192">Contains the identifier of an item or conversation.</span></span>  <br/> |
|[<span data-ttu-id="64d19-193">UniqueBody</span><span class="sxs-lookup"><span data-stu-id="64d19-193">UniqueBody</span></span>](uniquebody.md) <br/> |<span data-ttu-id="64d19-194">Представляет фрагмент HTML или обычный текст, который представляет уникальное body эту беседу.</span><span class="sxs-lookup"><span data-stu-id="64d19-194">Represents an HTML fragment or plain text which represents the unique body of this conversation.</span></span>  <br/> |
|[<span data-ttu-id="64d19-195">FileAs</span><span class="sxs-lookup"><span data-stu-id="64d19-195">FileAs</span></span>](fileas.md) <br/> |<span data-ttu-id="64d19-196">Представляет, как оформлена контакт в папке «Контакты».</span><span class="sxs-lookup"><span data-stu-id="64d19-196">Represents how a contact is filed in the Contacts folder.</span></span>  <br/> |
|[<span data-ttu-id="64d19-197">FileAsMapping</span><span class="sxs-lookup"><span data-stu-id="64d19-197">FileAsMapping</span></span>](fileasmapping.md) <br/> |<span data-ttu-id="64d19-198">Определяет порядок создания, отображаемых для контакта.</span><span class="sxs-lookup"><span data-stu-id="64d19-198">Defines how to construct what is displayed for a contact.</span></span>  <br/> |
|[<span data-ttu-id="64d19-199">Отображаемое имя (строка)</span><span class="sxs-lookup"><span data-stu-id="64d19-199">DisplayName (string)</span></span>](displayname-string.md) <br/> |<span data-ttu-id="64d19-200">Задает отображаемое имя контакта.</span><span class="sxs-lookup"><span data-stu-id="64d19-200">Defines the display name of a contact.</span></span>  <br/> |
|[<span data-ttu-id="64d19-201">GivenName</span><span class="sxs-lookup"><span data-stu-id="64d19-201">GivenName</span></span>](givenname.md) <br/> |<span data-ttu-id="64d19-202">Содержит имя контакта.</span><span class="sxs-lookup"><span data-stu-id="64d19-202">Contains a contact's given name.</span></span>  <br/> |
|[<span data-ttu-id="64d19-203">Инициалы</span><span class="sxs-lookup"><span data-stu-id="64d19-203">Initials</span></span>](initials.md) <br/> |<span data-ttu-id="64d19-204">Представляет отчество контакта.</span><span class="sxs-lookup"><span data-stu-id="64d19-204">Represents the initials of a contact.</span></span>  <br/> |
|[<span data-ttu-id="64d19-205">Отчество</span><span class="sxs-lookup"><span data-stu-id="64d19-205">MiddleName</span></span>](middlename.md) <br/> |<span data-ttu-id="64d19-206">Представляет отчество контакта.</span><span class="sxs-lookup"><span data-stu-id="64d19-206">Represents the middle name of a contact.</span></span>  <br/> |
|[<span data-ttu-id="64d19-207">Понятное имя</span><span class="sxs-lookup"><span data-stu-id="64d19-207">Nickname</span></span>](nickname.md) <br/> |<span data-ttu-id="64d19-208">Представляет псевдоним контакта.</span><span class="sxs-lookup"><span data-stu-id="64d19-208">Represents the nickname of a contact.</span></span>  <br/> |
|[<span data-ttu-id="64d19-209">CompleteName</span><span class="sxs-lookup"><span data-stu-id="64d19-209">CompleteName</span></span>](completename.md) <br/> |<span data-ttu-id="64d19-210">Представляет полное имя контакта.</span><span class="sxs-lookup"><span data-stu-id="64d19-210">Represents the complete name of a contact.</span></span>  <br/> |
|[<span data-ttu-id="64d19-211">Название организации</span><span class="sxs-lookup"><span data-stu-id="64d19-211">CompanyName</span></span>](companyname.md) <br/> |<span data-ttu-id="64d19-212">Представляет имя компании, связанное с контактом.</span><span class="sxs-lookup"><span data-stu-id="64d19-212">Represents the company name that is associated with a contact.</span></span>  <br/> |
|[<span data-ttu-id="64d19-213">EmailAddresses</span><span class="sxs-lookup"><span data-stu-id="64d19-213">EmailAddresses</span></span>](emailaddresses.md) <br/> |<span data-ttu-id="64d19-214">Представляет коллекцию адреса электронной почты контакта.</span><span class="sxs-lookup"><span data-stu-id="64d19-214">Represents a collection of e-mail addresses for a contact.</span></span>  <br/> |
|[<span data-ttu-id="64d19-215">PhysicalAddresses</span><span class="sxs-lookup"><span data-stu-id="64d19-215">PhysicalAddresses</span></span>](physicaladdresses.md) <br/> |<span data-ttu-id="64d19-216">Содержит коллекцию физических адресов, связанные с контактом.</span><span class="sxs-lookup"><span data-stu-id="64d19-216">Contains a collection of physical addresses that are associated with a contact.</span></span>  <br/> |
|[<span data-ttu-id="64d19-217">PhoneNumbers</span><span class="sxs-lookup"><span data-stu-id="64d19-217">PhoneNumbers</span></span>](phonenumbers.md) <br/> |<span data-ttu-id="64d19-218">Представляет коллекцию телефонных номеров контакта.</span><span class="sxs-lookup"><span data-stu-id="64d19-218">Represents a collection of telephone numbers for a contact.</span></span>  <br/> |
|[<span data-ttu-id="64d19-219">AssistantName</span><span class="sxs-lookup"><span data-stu-id="64d19-219">AssistantName</span></span>](assistantname.md) <br/> |<span data-ttu-id="64d19-220">Представляет помощника контакта.</span><span class="sxs-lookup"><span data-stu-id="64d19-220">Represents an assistant to a contact.</span></span>  <br/> |
|[<span data-ttu-id="64d19-221">День рождения</span><span class="sxs-lookup"><span data-stu-id="64d19-221">Birthday</span></span>](birthday.md) <br/> |<span data-ttu-id="64d19-222">Представляет Дата рождения контакта.</span><span class="sxs-lookup"><span data-stu-id="64d19-222">Represents the birth date of a contact.</span></span>  <br/> |
|[<span data-ttu-id="64d19-223">BusinessHomePage</span><span class="sxs-lookup"><span data-stu-id="64d19-223">BusinessHomePage</span></span>](businesshomepage.md) <br/> |<span data-ttu-id="64d19-224">Представляет Домашняя страница (веб-адрес) для этого контакта.</span><span class="sxs-lookup"><span data-stu-id="64d19-224">Represents the Home page (Web address) for the contact.</span></span>  <br/> |
|[<span data-ttu-id="64d19-225">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="64d19-225">Children</span></span>](children.md) <br/> |<span data-ttu-id="64d19-226">Содержит имена дочерних элементов контакта.</span><span class="sxs-lookup"><span data-stu-id="64d19-226">Contains the names of a contact's children.</span></span>  <br/> |
|[<span data-ttu-id="64d19-227">Компании</span><span class="sxs-lookup"><span data-stu-id="64d19-227">Companies</span></span>](companies.md) <br/> |<span data-ttu-id="64d19-228">Представляет коллекцию компании, связанные с контактом.</span><span class="sxs-lookup"><span data-stu-id="64d19-228">Represents the collection of companies that are associated with a contact.</span></span>  <br/> |
|[<span data-ttu-id="64d19-229">ContactSource</span><span class="sxs-lookup"><span data-stu-id="64d19-229">ContactSource</span></span>](contactsource.md) <br/> |<span data-ttu-id="64d19-230">Описание, находится ли контакт в хранилище Exchange или службе каталогов Active Directory.</span><span class="sxs-lookup"><span data-stu-id="64d19-230">Describes whether the contact is located in the Exchange store or the Active Directory directory service.</span></span>  <br/> |
|[<span data-ttu-id="64d19-231">Отдел</span><span class="sxs-lookup"><span data-stu-id="64d19-231">Department</span></span>](department.md) <br/> |<span data-ttu-id="64d19-232">Представляет отдел контакта на работе.</span><span class="sxs-lookup"><span data-stu-id="64d19-232">Represents the contact's department at work.</span></span>  <br/> |
|[<span data-ttu-id="64d19-233">Создание</span><span class="sxs-lookup"><span data-stu-id="64d19-233">Generation</span></span>](generation.md) <br/> |<span data-ttu-id="64d19-234">Представляет поколениям аббревиатура, исходя из полного имени контакта.</span><span class="sxs-lookup"><span data-stu-id="64d19-234">Represents a generational abbreviation that follows the full name of a contact.</span></span>  <br/> |
|[<span data-ttu-id="64d19-235">ImAddresses</span><span class="sxs-lookup"><span data-stu-id="64d19-235">ImAddresses</span></span>](imaddresses.md) <br/> |<span data-ttu-id="64d19-236">Представляет коллекцию мгновенного обмена сообщениями адресов для контакта.</span><span class="sxs-lookup"><span data-stu-id="64d19-236">Represents a collection of instant messaging addresses for a contact.</span></span>  <br/> |
|[<span data-ttu-id="64d19-237">Название должности</span><span class="sxs-lookup"><span data-stu-id="64d19-237">JobTitle</span></span>](jobtitle.md) <br/> |<span data-ttu-id="64d19-238">Представляет должность контакта.</span><span class="sxs-lookup"><span data-stu-id="64d19-238">Represents the job title of a contact.</span></span>  <br/> |
|[<span data-ttu-id="64d19-239">Руководитель</span><span class="sxs-lookup"><span data-stu-id="64d19-239">Manager</span></span>](manager.md) <br/> |<span data-ttu-id="64d19-240">Представляет диспетчера контактов.</span><span class="sxs-lookup"><span data-stu-id="64d19-240">Represents a contact's manager.</span></span>  <br/> |
|[<span data-ttu-id="64d19-241">Расстояние</span><span class="sxs-lookup"><span data-stu-id="64d19-241">Mileage</span></span>](mileage.md) <br/> |<span data-ttu-id="64d19-242">Представляет расстояние для элемента контакта.</span><span class="sxs-lookup"><span data-stu-id="64d19-242">Represents mileage for a contact item.</span></span>  <br/> |
|[<span data-ttu-id="64d19-243">Расположение компании</span><span class="sxs-lookup"><span data-stu-id="64d19-243">OfficeLocation</span></span>](officelocation.md) <br/> |<span data-ttu-id="64d19-244">Представляет расположение комнаты контакта.</span><span class="sxs-lookup"><span data-stu-id="64d19-244">Represents the office location of a contact.</span></span>  <br/> |
|[<span data-ttu-id="64d19-245">PostalAddressIndex</span><span class="sxs-lookup"><span data-stu-id="64d19-245">PostalAddressIndex</span></span>](postaladdressindex.md) <br/> |<span data-ttu-id="64d19-246">Представляет типов отображения физических адресов.</span><span class="sxs-lookup"><span data-stu-id="64d19-246">Represents the display types for physical addresses.</span></span>  <br/> |
|[<span data-ttu-id="64d19-247">Род занятий</span><span class="sxs-lookup"><span data-stu-id="64d19-247">Profession</span></span>](profession.md) <br/> |<span data-ttu-id="64d19-248">Представляет род занятий контакта.</span><span class="sxs-lookup"><span data-stu-id="64d19-248">Represents the profession of a contact.</span></span>  <br/> |
|[<span data-ttu-id="64d19-249">SpouseName</span><span class="sxs-lookup"><span data-stu-id="64d19-249">SpouseName</span></span>](spousename.md) <br/> |<span data-ttu-id="64d19-250">Представляет имя контакта супруга/партнера.</span><span class="sxs-lookup"><span data-stu-id="64d19-250">Represents the name of a contact's spouse/partner.</span></span>  <br/> |
|[<span data-ttu-id="64d19-251">Фамилия</span><span class="sxs-lookup"><span data-stu-id="64d19-251">Surname</span></span>](surname.md) <br/> |<span data-ttu-id="64d19-252">Представляет фамилию контакта.</span><span class="sxs-lookup"><span data-stu-id="64d19-252">Represents the surname of a contact.</span></span>  <br/> |
|[<span data-ttu-id="64d19-253">WeddingAnniversary</span><span class="sxs-lookup"><span data-stu-id="64d19-253">WeddingAnniversary</span></span>](weddinganniversary.md) <br/> |<span data-ttu-id="64d19-254">Содержит Годовщина свадьбы контакта.</span><span class="sxs-lookup"><span data-stu-id="64d19-254">Contains the wedding anniversary of a contact.</span></span>  <br/> |
|[<span data-ttu-id="64d19-255">HasPicture</span><span class="sxs-lookup"><span data-stu-id="64d19-255">HasPicture</span></span>](haspicture.md) <br/> |<span data-ttu-id="64d19-256">Указывает, имеет ли элемент контактов вложенный файл, который представляет на изображение контакта.</span><span class="sxs-lookup"><span data-stu-id="64d19-256">Indicates whether the contact item has a file attachment that represents the contact's picture.</span></span>  <br/> |
|[<span data-ttu-id="64d19-257">PhoneticFullName</span><span class="sxs-lookup"><span data-stu-id="64d19-257">PhoneticFullName</span></span>](phoneticfullname.md) <br/> |<span data-ttu-id="64d19-258">Содержит полное имя контакта, включая имя и фамилию, фонетически.</span><span class="sxs-lookup"><span data-stu-id="64d19-258">Contains the full name of a contact, including the first and last name, spelled phonetically.</span></span>  <br/> |
|[<span data-ttu-id="64d19-259">PhoneticFirstName</span><span class="sxs-lookup"><span data-stu-id="64d19-259">PhoneticFirstName</span></span>](phoneticfirstname.md) <br/> |<span data-ttu-id="64d19-260">Содержит имя контакта, фонетически.</span><span class="sxs-lookup"><span data-stu-id="64d19-260">Contains the first name of a contact, spelled phonetically.</span></span>  <br/> |
|[<span data-ttu-id="64d19-261">PhoneticLastName</span><span class="sxs-lookup"><span data-stu-id="64d19-261">PhoneticLastName</span></span>](phoneticlastname.md) <br/> |<span data-ttu-id="64d19-262">Содержит фамилию контакта, фонетически.</span><span class="sxs-lookup"><span data-stu-id="64d19-262">Contains the last name of a contact, spelled phonetically.</span></span>  <br/> |
|[<span data-ttu-id="64d19-263">Псевдоним</span><span class="sxs-lookup"><span data-stu-id="64d19-263">Alias</span></span>](alias.md) <br/> |<span data-ttu-id="64d19-264">Содержит псевдоним электронной почты контакта.</span><span class="sxs-lookup"><span data-stu-id="64d19-264">Contains the email alias of a contact.</span></span>  <br/> |
|[<span data-ttu-id="64d19-265">Примечания (контактов)</span><span class="sxs-lookup"><span data-stu-id="64d19-265">Notes (Contact)</span></span>](notes-contact.md) <br/> |<span data-ttu-id="64d19-266">Содержит дополнительные контактные сведения.</span><span class="sxs-lookup"><span data-stu-id="64d19-266">Contains supplementary contact information.</span></span>  <br/> |
|[<span data-ttu-id="64d19-267">Photo</span><span class="sxs-lookup"><span data-stu-id="64d19-267">Photo</span></span>](photo.md) <br/> |<span data-ttu-id="64d19-268">Содержит значение, которое кодирует фотографии контакта.</span><span class="sxs-lookup"><span data-stu-id="64d19-268">Contains a value that encodes the photo of a contact.</span></span>  <br/> |
|[<span data-ttu-id="64d19-269">UserSMIMECertificate</span><span class="sxs-lookup"><span data-stu-id="64d19-269">UserSMIMECertificate</span></span>](usersmimecertificate.md) <br/> |<span data-ttu-id="64d19-270">Содержит значение, которое кодирует сертификат SMIME контакта.</span><span class="sxs-lookup"><span data-stu-id="64d19-270">Contains a value that encodes the SMIME certificate of a contact.</span></span>  <br/> |
|[<span data-ttu-id="64d19-271">MSExchangeCertificate</span><span class="sxs-lookup"><span data-stu-id="64d19-271">MSExchangeCertificate</span></span>](msexchangecertificate.md) <br/> |<span data-ttu-id="64d19-272">Содержит значение, которое кодирует сертификата Microsoft Exchange контакта.</span><span class="sxs-lookup"><span data-stu-id="64d19-272">Contains a value that encodes the Microsoft Exchange certificate of a contact.</span></span>  <br/> |
|[<span data-ttu-id="64d19-273">DirectoryId</span><span class="sxs-lookup"><span data-stu-id="64d19-273">DirectoryId</span></span>](directoryid.md) <br/> |<span data-ttu-id="64d19-274">Содержит идентификатор каталога контакта.</span><span class="sxs-lookup"><span data-stu-id="64d19-274">Contains the directory ID of a contact.</span></span>  <br/> |
|[<span data-ttu-id="64d19-275">ManagerMailbox</span><span class="sxs-lookup"><span data-stu-id="64d19-275">ManagerMailbox</span></span>](managermailbox.md) <br/> |<span data-ttu-id="64d19-276">Содержит сведения SMTP, который идентифицирует почтовый ящик диспетчера контакта.</span><span class="sxs-lookup"><span data-stu-id="64d19-276">Contains SMTP information that identifies the manager mailbox of the contact.</span></span>  <br/> |
|[<span data-ttu-id="64d19-277">DirectReports</span><span class="sxs-lookup"><span data-stu-id="64d19-277">DirectReports</span></span>](directreports.md) <br/> |<span data-ttu-id="64d19-278">Содержит SMTP идентификационные сведения о прямых отчетов контакта.</span><span class="sxs-lookup"><span data-stu-id="64d19-278">Contains SMTP information that identifies the direct reports of a contact.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="64d19-279">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="64d19-279">Parent elements</span></span>

|<span data-ttu-id="64d19-280">**Имя элемента**</span><span class="sxs-lookup"><span data-stu-id="64d19-280">**Element name**</span></span>|<span data-ttu-id="64d19-281">**Описание**</span><span class="sxs-lookup"><span data-stu-id="64d19-281">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="64d19-282">AdjacentMeetings</span><span class="sxs-lookup"><span data-stu-id="64d19-282">AdjacentMeetings</span></span>](adjacentmeetings.md) <br/> |<span data-ttu-id="64d19-283">Описание всех элементов календаря, расположенных на время собрания.</span><span class="sxs-lookup"><span data-stu-id="64d19-283">Describes all calendar items that are adjacent to a meeting time.</span></span>  <br/> |
|[<span data-ttu-id="64d19-284">AppendToItemField</span><span class="sxs-lookup"><span data-stu-id="64d19-284">AppendToItemField</span></span>](appendtoitemfield.md) <br/> |<span data-ttu-id="64d19-285">Указывает данные для добавления во время [операции UpdateItem](updateitem-operation.md)отдельное свойство элемента или папки.</span><span class="sxs-lookup"><span data-stu-id="64d19-285">Identifies data to append to a single property of an item or folder during an [UpdateItem operation](updateitem-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="64d19-286">ConflictingMeetings</span><span class="sxs-lookup"><span data-stu-id="64d19-286">ConflictingMeetings</span></span>](conflictingmeetings.md) <br/> |<span data-ttu-id="64d19-287">Определяет все элементы, конфликтующие с время собрания</span><span class="sxs-lookup"><span data-stu-id="64d19-287">Identifies all items that conflict with a meeting time</span></span>  <br/> |
|[<span data-ttu-id="64d19-288">Создание (ItemSync)</span><span class="sxs-lookup"><span data-stu-id="64d19-288">Create (ItemSync)</span></span>](create-itemsync.md) <br/> |<span data-ttu-id="64d19-289">Определяет одну папку для создания в локальном хранилище клиента.</span><span class="sxs-lookup"><span data-stu-id="64d19-289">Identifies a single folder to create in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="64d19-290">ItemAttachment</span><span class="sxs-lookup"><span data-stu-id="64d19-290">ItemAttachment</span></span>](itemattachment.md) <br/> |<span data-ttu-id="64d19-291">Представляет собой элемент Exchange, подключенный к другой элемент Exchange.</span><span class="sxs-lookup"><span data-stu-id="64d19-291">Represents an Exchange item that is attached to another Exchange item.</span></span>  <br/> |
|[<span data-ttu-id="64d19-292">Элементы</span><span class="sxs-lookup"><span data-stu-id="64d19-292">Items</span></span>](items.md) <br/> |<span data-ttu-id="64d19-293">Содержит массив элементов.</span><span class="sxs-lookup"><span data-stu-id="64d19-293">Contains an array of items.</span></span>  <br/> |
|[<span data-ttu-id="64d19-294">Элементы (NonEmptyArrayOfAllItemsType)</span><span class="sxs-lookup"><span data-stu-id="64d19-294">Items (NonEmptyArrayOfAllItemsType)</span></span>](items-nonemptyarrayofallitemstype.md) <br/> |<span data-ttu-id="64d19-295">Содержит массив элементов для создания в папке, указанной с помощью элемента [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) .</span><span class="sxs-lookup"><span data-stu-id="64d19-295">Contains an array of items to create in the folder that is identified by the [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) element.</span></span>  <br/> |
|[<span data-ttu-id="64d19-296">Решение</span><span class="sxs-lookup"><span data-stu-id="64d19-296">Resolution</span></span>](resolution.md) <br/> |<span data-ttu-id="64d19-297">Содержит одного объекта разрешения.</span><span class="sxs-lookup"><span data-stu-id="64d19-297">Contains a single resolved entity.</span></span>  <br/> |
|[<span data-ttu-id="64d19-298">SetItemField</span><span class="sxs-lookup"><span data-stu-id="64d19-298">SetItemField</span></span>](setitemfield.md) <br/> |<span data-ttu-id="64d19-299">Представляет отдельное свойство элемента в [UpdateItem операции](updateitem-operation.md)обновления.</span><span class="sxs-lookup"><span data-stu-id="64d19-299">Represents an update to a single property of an item in an [UpdateItem operation](updateitem-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="64d19-300">Обновление (ItemSync)</span><span class="sxs-lookup"><span data-stu-id="64d19-300">Update (ItemSync)</span></span>](update-itemsync.md) <br/> |<span data-ttu-id="64d19-301">Определяет один элемент для обновления в локальном хранилище клиента.</span><span class="sxs-lookup"><span data-stu-id="64d19-301">Identifies a single item to update in the local client store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="64d19-302">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="64d19-302">Text value</span></span>

<span data-ttu-id="64d19-303">Нет.</span><span class="sxs-lookup"><span data-stu-id="64d19-303">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="64d19-304">Замечания</span><span class="sxs-lookup"><span data-stu-id="64d19-304">Remarks</span></span>

<span data-ttu-id="64d19-305">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="64d19-305">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="64d19-306">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="64d19-306">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="64d19-307">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="64d19-307">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="64d19-308">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="64d19-308">Schema name</span></span>  <br/> |<span data-ttu-id="64d19-309">Схема Types</span><span class="sxs-lookup"><span data-stu-id="64d19-309">Types schema</span></span>  <br/> |
|<span data-ttu-id="64d19-310">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="64d19-310">Validation file</span></span>  <br/> |<span data-ttu-id="64d19-311">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="64d19-311">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="64d19-312">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="64d19-312">Can be empty</span></span>  <br/> |<span data-ttu-id="64d19-313">False</span><span class="sxs-lookup"><span data-stu-id="64d19-313">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="64d19-314">См. также</span><span class="sxs-lookup"><span data-stu-id="64d19-314">See also</span></span>



- [<span data-ttu-id="64d19-315">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="64d19-315">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="64d19-316">Создание контактов (веб-служб Exchange)</span><span class="sxs-lookup"><span data-stu-id="64d19-316">Creating Contacts (Exchange Web Services)</span></span>](http://msdn.microsoft.com/library/4845917e-70d1-481c-bbd7-011ec6571789%28Office.15%29.aspx)
  
[<span data-ttu-id="64d19-317">Обновление контактов</span><span class="sxs-lookup"><span data-stu-id="64d19-317">Updating Contacts</span></span>](http://msdn.microsoft.com/library/9a865953-b94a-4229-b632-2dee433314be%28Office.15%29.aspx)
  
[<span data-ttu-id="64d19-318">Удаление контактов</span><span class="sxs-lookup"><span data-stu-id="64d19-318">Deleting Contacts</span></span>](http://msdn.microsoft.com/library/fcc3dc84-cd3e-455e-a1a7-ae6921c9b588%28Office.15%29.aspx)

