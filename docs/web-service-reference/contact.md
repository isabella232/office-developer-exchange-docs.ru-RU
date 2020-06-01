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
description: Элемент Contact представляет элемент контакта в хранилище Exchange.
ms.openlocfilehash: b5b4af211815dbbd09449ca2f3c6b6b2dfba6f93
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44445652"
---
# <a name="contact"></a><span data-ttu-id="c30c7-103">Контакт</span><span class="sxs-lookup"><span data-stu-id="c30c7-103">Contact</span></span>

<span data-ttu-id="c30c7-104">Элемент **Contact** представляет элемент контакта в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="c30c7-104">The **Contact** element represents a contact item in the Exchange store.</span></span> 
  
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

 <span data-ttu-id="c30c7-105">**контактитемтипе**</span><span class="sxs-lookup"><span data-stu-id="c30c7-105">**ContactItemType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c30c7-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="c30c7-106">Attributes and elements</span></span>

<span data-ttu-id="c30c7-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="c30c7-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c30c7-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="c30c7-108">Attributes</span></span>

<span data-ttu-id="c30c7-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="c30c7-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c30c7-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="c30c7-110">Child elements</span></span>

|<span data-ttu-id="c30c7-111">**Имя элемента**</span><span class="sxs-lookup"><span data-stu-id="c30c7-111">**Element name**</span></span>|<span data-ttu-id="c30c7-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="c30c7-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c30c7-113">Сохранитьmimecontent</span><span class="sxs-lookup"><span data-stu-id="c30c7-113">MimeContent</span></span>](mimecontent.md) <br/> |<span data-ttu-id="c30c7-114">Содержит собственный многоцелевой поток расширений почты в Интернете (MIME) объекта, представленного в формате base64Binary.</span><span class="sxs-lookup"><span data-stu-id="c30c7-114">Contains the native Multipurpose Internet Mail Extensions (MIME) stream of an object that is represented in base64Binary format.</span></span>  <br/> |
|[<span data-ttu-id="c30c7-115">Идентификатор</span><span class="sxs-lookup"><span data-stu-id="c30c7-115">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="c30c7-116">Содержит уникальный идентификатор и ключ изменения элемента в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="c30c7-116">Contains the unique identifier and change key of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="c30c7-117">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="c30c7-117">ParentFolderId</span></span>](parentfolderid.md) <br/> |<span data-ttu-id="c30c7-118">Представляет идентификатор родительской папки, содержащей элемент или папку.</span><span class="sxs-lookup"><span data-stu-id="c30c7-118">Represents the identifier of the parent folder that contains the item or folder.</span></span>  <br/> |
|[<span data-ttu-id="c30c7-119">ItemClass</span><span class="sxs-lookup"><span data-stu-id="c30c7-119">ItemClass</span></span>](itemclass.md) <br/> |<span data-ttu-id="c30c7-120">Представляет класс сообщения для элемента.</span><span class="sxs-lookup"><span data-stu-id="c30c7-120">Represents the message class of an item.</span></span>  <br/> |
|[<span data-ttu-id="c30c7-121">Тема</span><span class="sxs-lookup"><span data-stu-id="c30c7-121">Subject</span></span>](subject.md) <br/> |<span data-ttu-id="c30c7-122">Представляет тему для элементов хранилища Exchange и объектов ответа.</span><span class="sxs-lookup"><span data-stu-id="c30c7-122">Represents the subject for Exchange store items and response objects.</span></span>  <br/> |
|[<span data-ttu-id="c30c7-123">Sensitivity</span><span class="sxs-lookup"><span data-stu-id="c30c7-123">Sensitivity</span></span>](sensitivity.md) <br/> |<span data-ttu-id="c30c7-124">Указывает уровень конфиденциальности элемента.</span><span class="sxs-lookup"><span data-stu-id="c30c7-124">Indicates the sensitivity level of an item.</span></span>  <br/> |
|[<span data-ttu-id="c30c7-125">Body</span><span class="sxs-lookup"><span data-stu-id="c30c7-125">Body</span></span>](body.md) <br/> |<span data-ttu-id="c30c7-126">Представляет реальное содержимое основного текста сообщения.</span><span class="sxs-lookup"><span data-stu-id="c30c7-126">Represents the actual body content of a message.</span></span>  <br/> |
|[<span data-ttu-id="c30c7-127">Вложения</span><span class="sxs-lookup"><span data-stu-id="c30c7-127">Attachments</span></span>](attachments-ex15websvcsotherref.md) <br/> |<span data-ttu-id="c30c7-128">Содержит элементы или файлы, вложенные в элемент в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="c30c7-128">Contains the items or files that are attached to an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="c30c7-129">DateTimeReceived</span><span class="sxs-lookup"><span data-stu-id="c30c7-129">DateTimeReceived</span></span>](datetimereceived.md) <br/> |<span data-ttu-id="c30c7-130">Представляет дату и время получения элемента в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="c30c7-130">Represents the date and time that an item in a mailbox was received.</span></span>  <br/> |
|[<span data-ttu-id="c30c7-131">Размер</span><span class="sxs-lookup"><span data-stu-id="c30c7-131">Size</span></span>](size.md) <br/> |<span data-ttu-id="c30c7-132">Представляет размер элемента в байтах.</span><span class="sxs-lookup"><span data-stu-id="c30c7-132">Represents the size in bytes of an item.</span></span> <span data-ttu-id="c30c7-133">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c30c7-133">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="c30c7-134">Категории</span><span class="sxs-lookup"><span data-stu-id="c30c7-134">Categories</span></span>](categories-ex15websvcsotherref.md) <br/> |<span data-ttu-id="c30c7-135">Представляет коллекцию строк, определяющих, к каким категориям принадлежит элемент в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="c30c7-135">Represents a collection of strings that identify to which categories an item in the mailbox belongs.</span></span>  <br/> |
|[<span data-ttu-id="c30c7-136">Importance</span><span class="sxs-lookup"><span data-stu-id="c30c7-136">Importance</span></span>](importance.md) <br/> |<span data-ttu-id="c30c7-137">Описывает важность элемента.</span><span class="sxs-lookup"><span data-stu-id="c30c7-137">Describes the importance of an item.</span></span>  <br/> |
|[<span data-ttu-id="c30c7-138">инреплито</span><span class="sxs-lookup"><span data-stu-id="c30c7-138">InReplyTo</span></span>](inreplyto.md) <br/> |<span data-ttu-id="c30c7-139">Представляет идентификатор элемента, который является ответом на этот элемент.</span><span class="sxs-lookup"><span data-stu-id="c30c7-139">Represents the identifier of the item to which this item is a reply.</span></span>  <br/> |
|[<span data-ttu-id="c30c7-140">Отправлено</span><span class="sxs-lookup"><span data-stu-id="c30c7-140">IsSubmitted</span></span>](issubmitted.md) <br/> |<span data-ttu-id="c30c7-141">Указывает, был ли элемент отправлен в папку "Исходящие" по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="c30c7-141">Indicates whether an item has been submitted to the Outbox default folder.</span></span>  <br/> |
|[<span data-ttu-id="c30c7-142">Черновик</span><span class="sxs-lookup"><span data-stu-id="c30c7-142">IsDraft</span></span>](isdraft.md) <br/> |<span data-ttu-id="c30c7-143">Указывает, был ли элемент еще не отправлен.</span><span class="sxs-lookup"><span data-stu-id="c30c7-143">Represents whether an item has not yet been sent.</span></span>  <br/> |
|[<span data-ttu-id="c30c7-144">исфромме</span><span class="sxs-lookup"><span data-stu-id="c30c7-144">IsFromMe</span></span>](isfromme.md) <br/> |<span data-ttu-id="c30c7-145">Указывает, отправил ли пользователь элемент самому себе или самому себе.</span><span class="sxs-lookup"><span data-stu-id="c30c7-145">Indicates whether a user sent an item to himself or herself.</span></span>  <br/> |
|[<span data-ttu-id="c30c7-146">исресенд</span><span class="sxs-lookup"><span data-stu-id="c30c7-146">IsResend</span></span>](isresend.md) <br/> |<span data-ttu-id="c30c7-147">Указывает, был ли ранее отправлен элемент.</span><span class="sxs-lookup"><span data-stu-id="c30c7-147">Indicates whether the item had previously been sent.</span></span>  <br/> |
|[<span data-ttu-id="c30c7-148">исунмодифиед</span><span class="sxs-lookup"><span data-stu-id="c30c7-148">IsUnmodified</span></span>](isunmodified.md) <br/> |<span data-ttu-id="c30c7-149">Указывает, был ли изменен элемент.</span><span class="sxs-lookup"><span data-stu-id="c30c7-149">Indicates whether the item has been modified.</span></span>  <br/> |
|[<span data-ttu-id="c30c7-150">InternetMessageHeaders</span><span class="sxs-lookup"><span data-stu-id="c30c7-150">InternetMessageHeaders</span></span>](internetmessageheaders.md) <br/> |<span data-ttu-id="c30c7-151">Представляет коллекцию всех заголовков сообщений Интернета, которые находятся в элементе почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="c30c7-151">Represents the collection of all Internet message headers that are contained in an item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="c30c7-152">датетимесент</span><span class="sxs-lookup"><span data-stu-id="c30c7-152">DateTimeSent</span></span>](datetimesent.md) <br/> |<span data-ttu-id="c30c7-153">Представляет дату и время отправки элемента в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="c30c7-153">Represents the date and time that an item in a mailbox was sent.</span></span>  <br/> |
|[<span data-ttu-id="c30c7-154">DateTimeCreated</span><span class="sxs-lookup"><span data-stu-id="c30c7-154">DateTimeCreated</span></span>](datetimecreated.md) <br/> |<span data-ttu-id="c30c7-155">Представляет дату и время создания определенного элемента в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="c30c7-155">Represents the date and time that a given item in the mailbox was created.</span></span>  <br/> |
|[<span data-ttu-id="c30c7-156">респонсеобжектс</span><span class="sxs-lookup"><span data-stu-id="c30c7-156">ResponseObjects</span></span>](responseobjects.md) <br/> |<span data-ttu-id="c30c7-157">Содержит коллекцию всех объектов ответа, связанных с элементом в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="c30c7-157">Contains a collection of all the response objects that are associated with an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="c30c7-158">реминдердуеби</span><span class="sxs-lookup"><span data-stu-id="c30c7-158">ReminderDueBy</span></span>](reminderdueby.md) <br/> |<span data-ttu-id="c30c7-159">Представляет дату и время возникновения события.</span><span class="sxs-lookup"><span data-stu-id="c30c7-159">Represents the date and time when the event occurs.</span></span> <span data-ttu-id="c30c7-160">Он используется элементом [реминдерминутесбефорестарт](reminderminutesbeforestart.md) для определения времени отображения напоминания.</span><span class="sxs-lookup"><span data-stu-id="c30c7-160">This is used by the [ReminderMinutesBeforeStart](reminderminutesbeforestart.md) element to determine when the reminder is displayed.</span></span>  <br/> |
|[<span data-ttu-id="c30c7-161">реминдериссет</span><span class="sxs-lookup"><span data-stu-id="c30c7-161">ReminderIsSet</span></span>](reminderisset.md) <br/> |<span data-ttu-id="c30c7-162">Указывает, задано ли напоминание для элемента в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="c30c7-162">Indicates whether a reminder has been set for an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="c30c7-163">ReminderMinutesBeforeStart</span><span class="sxs-lookup"><span data-stu-id="c30c7-163">ReminderMinutesBeforeStart</span></span>](reminderminutesbeforestart.md) <br/> |<span data-ttu-id="c30c7-164">Представляет количество минут до события при отображении напоминания.</span><span class="sxs-lookup"><span data-stu-id="c30c7-164">Represents the number of minutes before an event when a reminder is displayed.</span></span>  <br/> |
|[<span data-ttu-id="c30c7-165">дисплайкк</span><span class="sxs-lookup"><span data-stu-id="c30c7-165">DisplayCc</span></span>](displaycc.md) <br/> |<span data-ttu-id="c30c7-166">Представляет отображаемую строку, используемую для содержимого строки "копия".</span><span class="sxs-lookup"><span data-stu-id="c30c7-166">Represents the display string that is used for the contents of the Cc line.</span></span> <span data-ttu-id="c30c7-167">Это объединенная строка всех отображаемых имен получателей копии.</span><span class="sxs-lookup"><span data-stu-id="c30c7-167">This is the concatenated string of all Cc recipient display names.</span></span>  <br/> |
|[<span data-ttu-id="c30c7-168">дисплайто</span><span class="sxs-lookup"><span data-stu-id="c30c7-168">DisplayTo</span></span>](displayto.md) <br/> |<span data-ttu-id="c30c7-169">Представляет отображаемую строку, используемую для содержимого строки "Кому".</span><span class="sxs-lookup"><span data-stu-id="c30c7-169">Represents the display string that is used for the contents of the To line.</span></span> <span data-ttu-id="c30c7-170">Это объединенная строка для отображаемых имен получателей.</span><span class="sxs-lookup"><span data-stu-id="c30c7-170">This is the concatenated string of all To recipient display names.</span></span>  <br/> |
|[<span data-ttu-id="c30c7-171">HasAttachments</span><span class="sxs-lookup"><span data-stu-id="c30c7-171">HasAttachments</span></span>](hasattachments.md) <br/> |<span data-ttu-id="c30c7-172">Представляет свойство, для которого задано значение **true** , если элемент имеет по крайней мере одно видимое вложение.</span><span class="sxs-lookup"><span data-stu-id="c30c7-172">Represents a property that is set to **true** if an item has at least one visible attachment.</span></span> <span data-ttu-id="c30c7-173">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c30c7-173">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="c30c7-174">ExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="c30c7-174">ExtendedProperty</span></span>](extendedproperty.md) <br/> |<span data-ttu-id="c30c7-175">Определяет расширенные свойства для папок и элементов.</span><span class="sxs-lookup"><span data-stu-id="c30c7-175">Identifies extended properties on folders and items.</span></span>  <br/> |
|[<span data-ttu-id="c30c7-176">Culture</span><span class="sxs-lookup"><span data-stu-id="c30c7-176">Culture</span></span>](culture.md) <br/> |<span data-ttu-id="c30c7-177">Представляет язык и региональные параметры для определенного элемента в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="c30c7-177">Represents the culture for a given item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="c30c7-178">еффективеригхтс</span><span class="sxs-lookup"><span data-stu-id="c30c7-178">EffectiveRights</span></span>](effectiverights.md) <br/> |<span data-ttu-id="c30c7-179">Содержит права клиента на основе параметров разрешений для элемента или папки.</span><span class="sxs-lookup"><span data-stu-id="c30c7-179">Contains the client's rights based on the permission settings for the item or folder.</span></span> <span data-ttu-id="c30c7-180">Этот элемент доступен только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c30c7-180">This element is read-only.</span></span>  <br/> |
|[<span data-ttu-id="c30c7-181">ластмодифиеднаме</span><span class="sxs-lookup"><span data-stu-id="c30c7-181">LastModifiedName</span></span>](lastmodifiedname.md) <br/> |<span data-ttu-id="c30c7-182">Содержит отображаемое имя последнего пользователя для изменения элемента.</span><span class="sxs-lookup"><span data-stu-id="c30c7-182">Contains the display name of the last user to modify an item.</span></span>  <br/> |
|[<span data-ttu-id="c30c7-183">LastModifiedTime</span><span class="sxs-lookup"><span data-stu-id="c30c7-183">LastModifiedTime</span></span>](lastmodifiedtime.md) <br/> |<span data-ttu-id="c30c7-184">Указывает время последнего изменения элемента.</span><span class="sxs-lookup"><span data-stu-id="c30c7-184">Indicates when an item was last modified.</span></span>  <br/> |
|[<span data-ttu-id="c30c7-185">Связанный</span><span class="sxs-lookup"><span data-stu-id="c30c7-185">IsAssociated</span></span>](isassociated.md) <br/> |<span data-ttu-id="c30c7-186">Указывает, связан ли элемент с папкой.</span><span class="sxs-lookup"><span data-stu-id="c30c7-186">Indicates whether the item is associated with a folder.</span></span>  <br/> |
|[<span data-ttu-id="c30c7-187">вебклиентреадформкуеристринг</span><span class="sxs-lookup"><span data-stu-id="c30c7-187">WebClientReadFormQueryString</span></span>](webclientreadformquerystring.md) <br/> |<span data-ttu-id="c30c7-188">Представляет URL-адрес для сцепления с конечной точкой Microsoft Office Outlook Web App для чтения элемента в Outlook Web App.</span><span class="sxs-lookup"><span data-stu-id="c30c7-188">Represents a URL to concatenate to the Microsoft Office Outlook Web App endpoint to read an item in Outlook Web App.</span></span>  <br/> |
|[<span data-ttu-id="c30c7-189">вебклиентедитформкуеристринг</span><span class="sxs-lookup"><span data-stu-id="c30c7-189">WebClientEditFormQueryString</span></span>](webclienteditformquerystring.md) <br/> |<span data-ttu-id="c30c7-190">Представляет URL-адрес для сцепления с конечной точкой Outlook Web App для изменения элемента в Outlook Web App.</span><span class="sxs-lookup"><span data-stu-id="c30c7-190">Represents a URL to concatenate to the Outlook Web App endpoint to edit an item in Outlook Web App.</span></span>  <br/> |
|[<span data-ttu-id="c30c7-191">ConversationId</span><span class="sxs-lookup"><span data-stu-id="c30c7-191">ConversationId</span></span>](conversationid.md) <br/> |<span data-ttu-id="c30c7-192">Содержит идентификатор элемента или беседы.</span><span class="sxs-lookup"><span data-stu-id="c30c7-192">Contains the identifier of an item or conversation.</span></span>  <br/> |
|[<span data-ttu-id="c30c7-193">UniqueBody</span><span class="sxs-lookup"><span data-stu-id="c30c7-193">UniqueBody</span></span>](uniquebody.md) <br/> |<span data-ttu-id="c30c7-194">Представляет фрагмент HTML или обычный текст, представляющий уникальный основной текст этой беседы.</span><span class="sxs-lookup"><span data-stu-id="c30c7-194">Represents an HTML fragment or plain text which represents the unique body of this conversation.</span></span>  <br/> |
|[<span data-ttu-id="c30c7-195">FileAs</span><span class="sxs-lookup"><span data-stu-id="c30c7-195">FileAs</span></span>](fileas.md) <br/> |<span data-ttu-id="c30c7-196">Представляет способ хранения контакта в папке "Контакты".</span><span class="sxs-lookup"><span data-stu-id="c30c7-196">Represents how a contact is filed in the Contacts folder.</span></span>  <br/> |
|[<span data-ttu-id="c30c7-197">филеасмаппинг</span><span class="sxs-lookup"><span data-stu-id="c30c7-197">FileAsMapping</span></span>](fileasmapping.md) <br/> |<span data-ttu-id="c30c7-198">Определяет, как создавать отображаемые сведения о контакте.</span><span class="sxs-lookup"><span data-stu-id="c30c7-198">Defines how to construct what is displayed for a contact.</span></span>  <br/> |
|[<span data-ttu-id="c30c7-199">DisplayName (строка)</span><span class="sxs-lookup"><span data-stu-id="c30c7-199">DisplayName (string)</span></span>](displayname-string.md) <br/> |<span data-ttu-id="c30c7-200">Определяет отображаемое имя контакта.</span><span class="sxs-lookup"><span data-stu-id="c30c7-200">Defines the display name of a contact.</span></span>  <br/> |
|[<span data-ttu-id="c30c7-201">GivenName</span><span class="sxs-lookup"><span data-stu-id="c30c7-201">GivenName</span></span>](givenname.md) <br/> |<span data-ttu-id="c30c7-202">Содержит имя контакта.</span><span class="sxs-lookup"><span data-stu-id="c30c7-202">Contains a contact's given name.</span></span>  <br/> |
|[<span data-ttu-id="c30c7-203">Initials</span><span class="sxs-lookup"><span data-stu-id="c30c7-203">Initials</span></span>](initials.md) <br/> |<span data-ttu-id="c30c7-204">Представляет инициалы контакта.</span><span class="sxs-lookup"><span data-stu-id="c30c7-204">Represents the initials of a contact.</span></span>  <br/> |
|[<span data-ttu-id="c30c7-205">MiddleName</span><span class="sxs-lookup"><span data-stu-id="c30c7-205">MiddleName</span></span>](middlename.md) <br/> |<span data-ttu-id="c30c7-206">Представляет отчество контакта.</span><span class="sxs-lookup"><span data-stu-id="c30c7-206">Represents the middle name of a contact.</span></span>  <br/> |
|[<span data-ttu-id="c30c7-207">Прозвищ</span><span class="sxs-lookup"><span data-stu-id="c30c7-207">Nickname</span></span>](nickname.md) <br/> |<span data-ttu-id="c30c7-208">Представляет псевдоним контакта.</span><span class="sxs-lookup"><span data-stu-id="c30c7-208">Represents the nickname of a contact.</span></span>  <br/> |
|[<span data-ttu-id="c30c7-209">комплетенаме</span><span class="sxs-lookup"><span data-stu-id="c30c7-209">CompleteName</span></span>](completename.md) <br/> |<span data-ttu-id="c30c7-210">Представляет полное имя контакта.</span><span class="sxs-lookup"><span data-stu-id="c30c7-210">Represents the complete name of a contact.</span></span>  <br/> |
|[<span data-ttu-id="c30c7-211">CompanyName</span><span class="sxs-lookup"><span data-stu-id="c30c7-211">CompanyName</span></span>](companyname.md) <br/> |<span data-ttu-id="c30c7-212">Представляет название компании, связанное с контактом.</span><span class="sxs-lookup"><span data-stu-id="c30c7-212">Represents the company name that is associated with a contact.</span></span>  <br/> |
|[<span data-ttu-id="c30c7-213">EmailAddresses</span><span class="sxs-lookup"><span data-stu-id="c30c7-213">EmailAddresses</span></span>](emailaddresses.md) <br/> |<span data-ttu-id="c30c7-214">Представляет коллекцию адресов электронной почты контакта.</span><span class="sxs-lookup"><span data-stu-id="c30c7-214">Represents a collection of e-mail addresses for a contact.</span></span>  <br/> |
|[<span data-ttu-id="c30c7-215">фисикаладдрессес</span><span class="sxs-lookup"><span data-stu-id="c30c7-215">PhysicalAddresses</span></span>](physicaladdresses.md) <br/> |<span data-ttu-id="c30c7-216">Содержит коллекцию физических адресов, связанных с контактом.</span><span class="sxs-lookup"><span data-stu-id="c30c7-216">Contains a collection of physical addresses that are associated with a contact.</span></span>  <br/> |
|[<span data-ttu-id="c30c7-217">PhoneNumbers</span><span class="sxs-lookup"><span data-stu-id="c30c7-217">PhoneNumbers</span></span>](phonenumbers.md) <br/> |<span data-ttu-id="c30c7-218">Представляет коллекцию телефонных номеров контакта.</span><span class="sxs-lookup"><span data-stu-id="c30c7-218">Represents a collection of telephone numbers for a contact.</span></span>  <br/> |
|[<span data-ttu-id="c30c7-219">AssistantName</span><span class="sxs-lookup"><span data-stu-id="c30c7-219">AssistantName</span></span>](assistantname.md) <br/> |<span data-ttu-id="c30c7-220">Представляет помощника для контакта.</span><span class="sxs-lookup"><span data-stu-id="c30c7-220">Represents an assistant to a contact.</span></span>  <br/> |
|[<span data-ttu-id="c30c7-221">Birthday</span><span class="sxs-lookup"><span data-stu-id="c30c7-221">Birthday</span></span>](birthday.md) <br/> |<span data-ttu-id="c30c7-222">Представляет дату рождения контакта.</span><span class="sxs-lookup"><span data-stu-id="c30c7-222">Represents the birth date of a contact.</span></span>  <br/> |
|[<span data-ttu-id="c30c7-223">BusinessHomePage</span><span class="sxs-lookup"><span data-stu-id="c30c7-223">BusinessHomePage</span></span>](businesshomepage.md) <br/> |<span data-ttu-id="c30c7-224">Представляет домашнюю страницу контакта (веб-адрес).</span><span class="sxs-lookup"><span data-stu-id="c30c7-224">Represents the Home page (Web address) for the contact.</span></span>  <br/> |
|[<span data-ttu-id="c30c7-225">Children</span><span class="sxs-lookup"><span data-stu-id="c30c7-225">Children</span></span>](children.md) <br/> |<span data-ttu-id="c30c7-226">Содержит имена потомков контакта.</span><span class="sxs-lookup"><span data-stu-id="c30c7-226">Contains the names of a contact's children.</span></span>  <br/> |
|[<span data-ttu-id="c30c7-227">Companies</span><span class="sxs-lookup"><span data-stu-id="c30c7-227">Companies</span></span>](companies.md) <br/> |<span data-ttu-id="c30c7-228">Представляет коллекцию компаний, связанных с контактом.</span><span class="sxs-lookup"><span data-stu-id="c30c7-228">Represents the collection of companies that are associated with a contact.</span></span>  <br/> |
|[<span data-ttu-id="c30c7-229">контактсаурце</span><span class="sxs-lookup"><span data-stu-id="c30c7-229">ContactSource</span></span>](contactsource.md) <br/> |<span data-ttu-id="c30c7-230">Указывает, находится ли контакт в хранилище Exchange или службе каталогов Active Directory.</span><span class="sxs-lookup"><span data-stu-id="c30c7-230">Describes whether the contact is located in the Exchange store or the Active Directory directory service.</span></span>  <br/> |
|[<span data-ttu-id="c30c7-231">Department</span><span class="sxs-lookup"><span data-stu-id="c30c7-231">Department</span></span>](department.md) <br/> |<span data-ttu-id="c30c7-232">Представляет подразделение контакта на рабочем месте.</span><span class="sxs-lookup"><span data-stu-id="c30c7-232">Represents the contact's department at work.</span></span>  <br/> |
|[<span data-ttu-id="c30c7-233">Generation</span><span class="sxs-lookup"><span data-stu-id="c30c7-233">Generation</span></span>](generation.md) <br/> |<span data-ttu-id="c30c7-234">Представляет сокращенное название, которое соответствует полному имени контакта.</span><span class="sxs-lookup"><span data-stu-id="c30c7-234">Represents a generational abbreviation that follows the full name of a contact.</span></span>  <br/> |
|[<span data-ttu-id="c30c7-235">Адреса</span><span class="sxs-lookup"><span data-stu-id="c30c7-235">ImAddresses</span></span>](imaddresses.md) <br/> |<span data-ttu-id="c30c7-236">Представляет коллекцию адресов обмена мгновенными сообщениями для контакта.</span><span class="sxs-lookup"><span data-stu-id="c30c7-236">Represents a collection of instant messaging addresses for a contact.</span></span>  <br/> |
|[<span data-ttu-id="c30c7-237">JobTitle</span><span class="sxs-lookup"><span data-stu-id="c30c7-237">JobTitle</span></span>](jobtitle.md) <br/> |<span data-ttu-id="c30c7-238">Представляет должность контакта.</span><span class="sxs-lookup"><span data-stu-id="c30c7-238">Represents the job title of a contact.</span></span>  <br/> |
|[<span data-ttu-id="c30c7-239">Manager</span><span class="sxs-lookup"><span data-stu-id="c30c7-239">Manager</span></span>](manager.md) <br/> |<span data-ttu-id="c30c7-240">Представляет руководителя контакта.</span><span class="sxs-lookup"><span data-stu-id="c30c7-240">Represents a contact's manager.</span></span>  <br/> |
|[<span data-ttu-id="c30c7-241">Mileage</span><span class="sxs-lookup"><span data-stu-id="c30c7-241">Mileage</span></span>](mileage.md) <br/> |<span data-ttu-id="c30c7-242">Представляет расстояние для элемента контакта.</span><span class="sxs-lookup"><span data-stu-id="c30c7-242">Represents mileage for a contact item.</span></span>  <br/> |
|[<span data-ttu-id="c30c7-243">OfficeLocation</span><span class="sxs-lookup"><span data-stu-id="c30c7-243">OfficeLocation</span></span>](officelocation.md) <br/> |<span data-ttu-id="c30c7-244">Представляет расположение контакта в офисе.</span><span class="sxs-lookup"><span data-stu-id="c30c7-244">Represents the office location of a contact.</span></span>  <br/> |
|[<span data-ttu-id="c30c7-245">посталаддрессиндекс</span><span class="sxs-lookup"><span data-stu-id="c30c7-245">PostalAddressIndex</span></span>](postaladdressindex.md) <br/> |<span data-ttu-id="c30c7-246">Представляет типы отображения для физических адресов.</span><span class="sxs-lookup"><span data-stu-id="c30c7-246">Represents the display types for physical addresses.</span></span>  <br/> |
|[<span data-ttu-id="c30c7-247">Profession</span><span class="sxs-lookup"><span data-stu-id="c30c7-247">Profession</span></span>](profession.md) <br/> |<span data-ttu-id="c30c7-248">Представляет профессия контакта.</span><span class="sxs-lookup"><span data-stu-id="c30c7-248">Represents the profession of a contact.</span></span>  <br/> |
|[<span data-ttu-id="c30c7-249">спаусенаме</span><span class="sxs-lookup"><span data-stu-id="c30c7-249">SpouseName</span></span>](spousename.md) <br/> |<span data-ttu-id="c30c7-250">Представляет имя супруга/партнера контакта.</span><span class="sxs-lookup"><span data-stu-id="c30c7-250">Represents the name of a contact's spouse/partner.</span></span>  <br/> |
|[<span data-ttu-id="c30c7-251">ФИО</span><span class="sxs-lookup"><span data-stu-id="c30c7-251">Surname</span></span>](surname.md) <br/> |<span data-ttu-id="c30c7-252">Представляет фамилию контакта.</span><span class="sxs-lookup"><span data-stu-id="c30c7-252">Represents the surname of a contact.</span></span>  <br/> |
|[<span data-ttu-id="c30c7-253">веддинганниверсари</span><span class="sxs-lookup"><span data-stu-id="c30c7-253">WeddingAnniversary</span></span>](weddinganniversary.md) <br/> |<span data-ttu-id="c30c7-254">Содержит годовщину свадьбы контакта.</span><span class="sxs-lookup"><span data-stu-id="c30c7-254">Contains the wedding anniversary of a contact.</span></span>  <br/> |
|[<span data-ttu-id="c30c7-255">HasPicture</span><span class="sxs-lookup"><span data-stu-id="c30c7-255">HasPicture</span></span>](haspicture.md) <br/> |<span data-ttu-id="c30c7-256">Указывает, имеет ли элемент контакта вложенный файл, представляющий изображение контакта.</span><span class="sxs-lookup"><span data-stu-id="c30c7-256">Indicates whether the contact item has a file attachment that represents the contact's picture.</span></span>  <br/> |
|[<span data-ttu-id="c30c7-257">фонетикфуллнаме</span><span class="sxs-lookup"><span data-stu-id="c30c7-257">PhoneticFullName</span></span>](phoneticfullname.md) <br/> |<span data-ttu-id="c30c7-258">Содержит полное имя контакта, включая имя и фамилию, введенное в фонетическое имя.</span><span class="sxs-lookup"><span data-stu-id="c30c7-258">Contains the full name of a contact, including the first and last name, spelled phonetically.</span></span>  <br/> |
|[<span data-ttu-id="c30c7-259">фонетикфирстнаме</span><span class="sxs-lookup"><span data-stu-id="c30c7-259">PhoneticFirstName</span></span>](phoneticfirstname.md) <br/> |<span data-ttu-id="c30c7-260">Содержит имя контакта, написанное в фонетическом формате.</span><span class="sxs-lookup"><span data-stu-id="c30c7-260">Contains the first name of a contact, spelled phonetically.</span></span>  <br/> |
|[<span data-ttu-id="c30c7-261">фонетикластнаме</span><span class="sxs-lookup"><span data-stu-id="c30c7-261">PhoneticLastName</span></span>](phoneticlastname.md) <br/> |<span data-ttu-id="c30c7-262">Содержит фамилию контакта с написанием фонетического имени.</span><span class="sxs-lookup"><span data-stu-id="c30c7-262">Contains the last name of a contact, spelled phonetically.</span></span>  <br/> |
|[<span data-ttu-id="c30c7-263">Alias</span><span class="sxs-lookup"><span data-stu-id="c30c7-263">Alias</span></span>](alias.md) <br/> |<span data-ttu-id="c30c7-264">Содержит псевдоним электронной почты контакта.</span><span class="sxs-lookup"><span data-stu-id="c30c7-264">Contains the email alias of a contact.</span></span>  <br/> |
|[<span data-ttu-id="c30c7-265">Примечания (контакт)</span><span class="sxs-lookup"><span data-stu-id="c30c7-265">Notes (Contact)</span></span>](notes-contact.md) <br/> |<span data-ttu-id="c30c7-266">Содержит дополнительную контактную информацию.</span><span class="sxs-lookup"><span data-stu-id="c30c7-266">Contains supplementary contact information.</span></span>  <br/> |
|<span data-ttu-id="c30c7-267">[фотография](photo.md);</span><span class="sxs-lookup"><span data-stu-id="c30c7-267">[Photo](photo.md)</span></span> <br/> |<span data-ttu-id="c30c7-268">Содержит значение, которое кодирует фотографию контакта.</span><span class="sxs-lookup"><span data-stu-id="c30c7-268">Contains a value that encodes the photo of a contact.</span></span>  <br/> |
|[<span data-ttu-id="c30c7-269">UserSMIMECertificate</span><span class="sxs-lookup"><span data-stu-id="c30c7-269">UserSMIMECertificate</span></span>](usersmimecertificate.md) <br/> |<span data-ttu-id="c30c7-270">Содержит значение, которое кодирует сертификат SMIME контакта.</span><span class="sxs-lookup"><span data-stu-id="c30c7-270">Contains a value that encodes the SMIME certificate of a contact.</span></span>  <br/> |
|[<span data-ttu-id="c30c7-271">мсексчанжецертификате</span><span class="sxs-lookup"><span data-stu-id="c30c7-271">MSExchangeCertificate</span></span>](msexchangecertificate.md) <br/> |<span data-ttu-id="c30c7-272">Содержит значение, которое кодирует сертификат Microsoft Exchange контакта.</span><span class="sxs-lookup"><span data-stu-id="c30c7-272">Contains a value that encodes the Microsoft Exchange certificate of a contact.</span></span>  <br/> |
|[<span data-ttu-id="c30c7-273">директорид</span><span class="sxs-lookup"><span data-stu-id="c30c7-273">DirectoryId</span></span>](directoryid.md) <br/> |<span data-ttu-id="c30c7-274">Содержит идентификатор каталога контакта.</span><span class="sxs-lookup"><span data-stu-id="c30c7-274">Contains the directory ID of a contact.</span></span>  <br/> |
|[<span data-ttu-id="c30c7-275">манажермаилбокс</span><span class="sxs-lookup"><span data-stu-id="c30c7-275">ManagerMailbox</span></span>](managermailbox.md) <br/> |<span data-ttu-id="c30c7-276">Содержит данные SMTP, определяющие почтовый ящик руководителя контакта.</span><span class="sxs-lookup"><span data-stu-id="c30c7-276">Contains SMTP information that identifies the manager mailbox of the contact.</span></span>  <br/> |
|[<span data-ttu-id="c30c7-277">DirectReports</span><span class="sxs-lookup"><span data-stu-id="c30c7-277">DirectReports</span></span>](directreports.md) <br/> |<span data-ttu-id="c30c7-278">Содержит сведения об SMTP, которые определяют прямые отчеты о контакте.</span><span class="sxs-lookup"><span data-stu-id="c30c7-278">Contains SMTP information that identifies the direct reports of a contact.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="c30c7-279">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="c30c7-279">Parent elements</span></span>

|<span data-ttu-id="c30c7-280">**Имя элемента**</span><span class="sxs-lookup"><span data-stu-id="c30c7-280">**Element name**</span></span>|<span data-ttu-id="c30c7-281">**Описание**</span><span class="sxs-lookup"><span data-stu-id="c30c7-281">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c30c7-282">аджацентмитингс</span><span class="sxs-lookup"><span data-stu-id="c30c7-282">AdjacentMeetings</span></span>](adjacentmeetings.md) <br/> |<span data-ttu-id="c30c7-283">Описывает все элементы календаря, смежные с временем собрания.</span><span class="sxs-lookup"><span data-stu-id="c30c7-283">Describes all calendar items that are adjacent to a meeting time.</span></span>  <br/> |
|[<span data-ttu-id="c30c7-284">аппендтоитемфиелд</span><span class="sxs-lookup"><span data-stu-id="c30c7-284">AppendToItemField</span></span>](appendtoitemfield.md) <br/> |<span data-ttu-id="c30c7-285">Определяет данные, добавляемые к одному свойству элемента или папки во время [операции UpdateItem](updateitem-operation.md).</span><span class="sxs-lookup"><span data-stu-id="c30c7-285">Identifies data to append to a single property of an item or folder during an [UpdateItem operation](updateitem-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="c30c7-286">конфликтингмитингс</span><span class="sxs-lookup"><span data-stu-id="c30c7-286">ConflictingMeetings</span></span>](conflictingmeetings.md) <br/> |<span data-ttu-id="c30c7-287">Определяет все элементы, которые конфликтуют с временем собрания</span><span class="sxs-lookup"><span data-stu-id="c30c7-287">Identifies all items that conflict with a meeting time</span></span>  <br/> |
|[<span data-ttu-id="c30c7-288">Create (Итемсинк)</span><span class="sxs-lookup"><span data-stu-id="c30c7-288">Create (ItemSync)</span></span>](create-itemsync.md) <br/> |<span data-ttu-id="c30c7-289">Определяет одну папку для создания в локальном хранилище клиента.</span><span class="sxs-lookup"><span data-stu-id="c30c7-289">Identifies a single folder to create in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="c30c7-290">ItemAttachment</span><span class="sxs-lookup"><span data-stu-id="c30c7-290">ItemAttachment</span></span>](itemattachment.md) <br/> |<span data-ttu-id="c30c7-291">Представляет элемент Exchange, присоединенный к другому элементу Exchange.</span><span class="sxs-lookup"><span data-stu-id="c30c7-291">Represents an Exchange item that is attached to another Exchange item.</span></span>  <br/> |
|[<span data-ttu-id="c30c7-292">Items</span><span class="sxs-lookup"><span data-stu-id="c30c7-292">Items</span></span>](items.md) <br/> |<span data-ttu-id="c30c7-293">Содержит массив элементов.</span><span class="sxs-lookup"><span data-stu-id="c30c7-293">Contains an array of items.</span></span>  <br/> |
|[<span data-ttu-id="c30c7-294">Элементы (Нонемптяррайофаллитемстипе)</span><span class="sxs-lookup"><span data-stu-id="c30c7-294">Items (NonEmptyArrayOfAllItemsType)</span></span>](items-nonemptyarrayofallitemstype.md) <br/> |<span data-ttu-id="c30c7-295">Содержит массив элементов для создания в папке, определяемой элементом [ParentFolderId (таржетфолдеридтипе)](parentfolderid-targetfolderidtype.md) .</span><span class="sxs-lookup"><span data-stu-id="c30c7-295">Contains an array of items to create in the folder that is identified by the [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) element.</span></span>  <br/> |
|[<span data-ttu-id="c30c7-296">Resolution</span><span class="sxs-lookup"><span data-stu-id="c30c7-296">Resolution</span></span>](resolution.md) <br/> |<span data-ttu-id="c30c7-297">Содержит одну разрешенную сущность.</span><span class="sxs-lookup"><span data-stu-id="c30c7-297">Contains a single resolved entity.</span></span>  <br/> |
|[<span data-ttu-id="c30c7-298">сетитемфиелд</span><span class="sxs-lookup"><span data-stu-id="c30c7-298">SetItemField</span></span>](setitemfield.md) <br/> |<span data-ttu-id="c30c7-299">Представляет обновление одного свойства элемента в [операции UpdateItem](updateitem-operation.md).</span><span class="sxs-lookup"><span data-stu-id="c30c7-299">Represents an update to a single property of an item in an [UpdateItem operation](updateitem-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="c30c7-300">Обновление (Итемсинк)</span><span class="sxs-lookup"><span data-stu-id="c30c7-300">Update (ItemSync)</span></span>](update-itemsync.md) <br/> |<span data-ttu-id="c30c7-301">Определяет один элемент для обновления в локальном хранилище клиента.</span><span class="sxs-lookup"><span data-stu-id="c30c7-301">Identifies a single item to update in the local client store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="c30c7-302">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="c30c7-302">Text value</span></span>

<span data-ttu-id="c30c7-303">Нет.</span><span class="sxs-lookup"><span data-stu-id="c30c7-303">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="c30c7-304">Примечания</span><span class="sxs-lookup"><span data-stu-id="c30c7-304">Remarks</span></span>

<span data-ttu-id="c30c7-305">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="c30c7-305">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c30c7-306">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="c30c7-306">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c30c7-307">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="c30c7-307">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="c30c7-308">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="c30c7-308">Schema name</span></span>  <br/> |<span data-ttu-id="c30c7-309">Схема Types</span><span class="sxs-lookup"><span data-stu-id="c30c7-309">Types schema</span></span>  <br/> |
|<span data-ttu-id="c30c7-310">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="c30c7-310">Validation file</span></span>  <br/> |<span data-ttu-id="c30c7-311">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="c30c7-311">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="c30c7-312">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="c30c7-312">Can be empty</span></span>  <br/> |<span data-ttu-id="c30c7-313">False</span><span class="sxs-lookup"><span data-stu-id="c30c7-313">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c30c7-314">См. также</span><span class="sxs-lookup"><span data-stu-id="c30c7-314">See also</span></span>



- [<span data-ttu-id="c30c7-315">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="c30c7-315">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="c30c7-316">Создание контактов (веб-службы Exchange)</span><span class="sxs-lookup"><span data-stu-id="c30c7-316">Creating Contacts (Exchange Web Services)</span></span>](https://msdn.microsoft.com/library/4845917e-70d1-481c-bbd7-011ec6571789%28Office.15%29.aspx)
  
[<span data-ttu-id="c30c7-317">Обновление контактов</span><span class="sxs-lookup"><span data-stu-id="c30c7-317">Updating Contacts</span></span>](https://msdn.microsoft.com/library/9a865953-b94a-4229-b632-2dee433314be%28Office.15%29.aspx)
  
[<span data-ttu-id="c30c7-318">Удаление контактов</span><span class="sxs-lookup"><span data-stu-id="c30c7-318">Deleting Contacts</span></span>](https://msdn.microsoft.com/library/fcc3dc84-cd3e-455e-a1a7-ae6921c9b588%28Office.15%29.aspx)

