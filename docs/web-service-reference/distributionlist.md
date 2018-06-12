---
title: DistributionList
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DistributionList
api_type:
- schema
ms.assetid: f65aea01-e870-44a2-8571-fa6c001341cc
description: Элемент DistributionList представляет список рассылки.
ms.openlocfilehash: 5edcc83eef6a5b16470e6c290aacd057ceecceb1
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762193"
---
# <a name="distributionlist"></a><span data-ttu-id="68a74-103">DistributionList</span><span class="sxs-lookup"><span data-stu-id="68a74-103">DistributionList</span></span>

<span data-ttu-id="68a74-104">Элемент **DistributionList** представляет список рассылки.</span><span class="sxs-lookup"><span data-stu-id="68a74-104">The **DistributionList** element represents a distribution list.</span></span> 
  
```xml
<DistributionList>
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
   <DisplayName/>
   <FileAs/>
   <ContactSource/>
   <Members/>
</DistributionList>
```

 <span data-ttu-id="68a74-105">**DistributionListType**</span><span class="sxs-lookup"><span data-stu-id="68a74-105">**DistributionListType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="68a74-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="68a74-106">Attributes and elements</span></span>

<span data-ttu-id="68a74-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="68a74-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="68a74-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="68a74-108">Attributes</span></span>

<span data-ttu-id="68a74-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="68a74-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="68a74-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="68a74-110">Child elements</span></span>

|<span data-ttu-id="68a74-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="68a74-111">**Element**</span></span>|<span data-ttu-id="68a74-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="68a74-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="68a74-113">MimeContent</span><span class="sxs-lookup"><span data-stu-id="68a74-113">MimeContent</span></span>](mimecontent.md) <br/> |<span data-ttu-id="68a74-114">Содержит собственный поток MIME объекта, представленного в формате base64Binary.</span><span class="sxs-lookup"><span data-stu-id="68a74-114">Contains the native MIME stream of an object represented in base64Binary format.</span></span>  <br/> |
|[<span data-ttu-id="68a74-115">Идентификатор элемента</span><span class="sxs-lookup"><span data-stu-id="68a74-115">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="68a74-116">Содержит уникальный идентификатор и меняет ключ элемента списка рассылки в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="68a74-116">Contains the unique identifier and change key of a distribution list item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="68a74-117">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="68a74-117">ParentFolderId</span></span>](parentfolderid.md) <br/> |<span data-ttu-id="68a74-118">Представляет идентификатор родительской папки, содержащей элемент списка рассылки.</span><span class="sxs-lookup"><span data-stu-id="68a74-118">Represents the identifier of the parent folder that contains the distribution list item.</span></span>  <br/> |
|[<span data-ttu-id="68a74-119">ItemClass</span><span class="sxs-lookup"><span data-stu-id="68a74-119">ItemClass</span></span>](itemclass.md) <br/> |<span data-ttu-id="68a74-120">Представляет класс сообщения элемента списка рассылки.</span><span class="sxs-lookup"><span data-stu-id="68a74-120">Represents the message class of a distribution list item.</span></span>  <br/> |
|[<span data-ttu-id="68a74-121">Subject</span><span class="sxs-lookup"><span data-stu-id="68a74-121">Subject</span></span>](subject.md) <br/> |<span data-ttu-id="68a74-122">Представляет тему для элементов хранилища Exchange и объекты ответа.</span><span class="sxs-lookup"><span data-stu-id="68a74-122">Represents the subject for Exchange store items and response objects.</span></span>  <br/> |
|[<span data-ttu-id="68a74-123">Уровень конфиденциальности сообщения</span><span class="sxs-lookup"><span data-stu-id="68a74-123">Sensitivity</span></span>](sensitivity.md) <br/> |<span data-ttu-id="68a74-124">Содержит сведения о состоянии чувствительность элемента списка рассылки.</span><span class="sxs-lookup"><span data-stu-id="68a74-124">Contains the status for a distribution list item's sensitivity.</span></span>  <br/> |
|[<span data-ttu-id="68a74-125">Body</span><span class="sxs-lookup"><span data-stu-id="68a74-125">Body</span></span>](body.md) <br/> |<span data-ttu-id="68a74-126">Представляет фактическое содержимое основного текста элемента списка рассылки.</span><span class="sxs-lookup"><span data-stu-id="68a74-126">Represents the actual body content of a distribution list item.</span></span>  <br/> |
|[<span data-ttu-id="68a74-127">Вложения</span><span class="sxs-lookup"><span data-stu-id="68a74-127">Attachments</span></span>](attachments-ex15websvcsotherref.md) <br/> |<span data-ttu-id="68a74-128">Содержит элементы или файлы, подключенные к элементу списка рассылки в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="68a74-128">Contains the items or files that are attached to a distribution list item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="68a74-129">DateTimeReceived</span><span class="sxs-lookup"><span data-stu-id="68a74-129">DateTimeReceived</span></span>](datetimereceived.md) <br/> |<span data-ttu-id="68a74-130">Представляет дату и время, которое было получено элемента списка рассылки в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="68a74-130">Represents the date and time that a distribution list item in a mailbox was received.</span></span>  <br/> |
|[<span data-ttu-id="68a74-131">Размер</span><span class="sxs-lookup"><span data-stu-id="68a74-131">Size</span></span>](size.md) <br/> |<span data-ttu-id="68a74-132">Представляет размер в байтах, элемента списка рассылки.</span><span class="sxs-lookup"><span data-stu-id="68a74-132">Represents the size, in bytes, of a distribution list item.</span></span> <span data-ttu-id="68a74-133">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="68a74-133">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="68a74-134">Категории</span><span class="sxs-lookup"><span data-stu-id="68a74-134">Categories</span></span>](categories-ex15websvcsotherref.md) <br/> |<span data-ttu-id="68a74-135">Представляет набор строк, чтобы указать, к какой категории принадлежит элемент списка рассылки в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="68a74-135">Represents a collection of strings that identify to which categories a distribution list item in the mailbox belongs.</span></span>  <br/> |
|[<span data-ttu-id="68a74-136">Важность</span><span class="sxs-lookup"><span data-stu-id="68a74-136">Importance</span></span>](importance.md) <br/> |<span data-ttu-id="68a74-137">Описывает важность элемента списка рассылки.</span><span class="sxs-lookup"><span data-stu-id="68a74-137">Describes the importance of a distribution list item.</span></span>  <br/> |
|[<span data-ttu-id="68a74-138">InReplyTo</span><span class="sxs-lookup"><span data-stu-id="68a74-138">InReplyTo</span></span>](inreplyto.md) <br/> |<span data-ttu-id="68a74-139">Представляет идентификатор элемента, который этот элемент является ее в ответ.</span><span class="sxs-lookup"><span data-stu-id="68a74-139">Represents the identifier of the item which this item is a reply.</span></span>  <br/> |
|[<span data-ttu-id="68a74-140">IsSubmitted</span><span class="sxs-lookup"><span data-stu-id="68a74-140">IsSubmitted</span></span>](issubmitted.md) <br/> |<span data-ttu-id="68a74-141">Указывает, является ли элемент был отправлен исходящие папке по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="68a74-141">Indicates whether an item has been submitted to the Outbox default folder.</span></span>  <br/> |
|[<span data-ttu-id="68a74-142">IsDraft</span><span class="sxs-lookup"><span data-stu-id="68a74-142">IsDraft</span></span>](isdraft.md) <br/> |<span data-ttu-id="68a74-143">Представляет ли элемент еще не были отправлены.</span><span class="sxs-lookup"><span data-stu-id="68a74-143">Represents whether an item has not yet been sent.</span></span>  <br/> |
|[<span data-ttu-id="68a74-144">IsFromMe</span><span class="sxs-lookup"><span data-stu-id="68a74-144">IsFromMe</span></span>](isfromme.md) <br/> |<span data-ttu-id="68a74-145">Показывает пользователя отправить элемент на себя.</span><span class="sxs-lookup"><span data-stu-id="68a74-145">Indicates whether a user sent an item to itself.</span></span>  <br/> |
|[<span data-ttu-id="68a74-146">IsResend</span><span class="sxs-lookup"><span data-stu-id="68a74-146">IsResend</span></span>](isresend.md) <br/> |<span data-ttu-id="68a74-147">Указывает, является ли элемент ранее еще был отправлен.</span><span class="sxs-lookup"><span data-stu-id="68a74-147">Indicates whether the item had previously been sent.</span></span>  <br/> |
|[<span data-ttu-id="68a74-148">IsUnmodified</span><span class="sxs-lookup"><span data-stu-id="68a74-148">IsUnmodified</span></span>](isunmodified.md) <br/> |<span data-ttu-id="68a74-149">Указывает, были ли изменены элемента.</span><span class="sxs-lookup"><span data-stu-id="68a74-149">Indicates whether the item has been modified.</span></span>  <br/> |
|[<span data-ttu-id="68a74-150">InternetMessageHeaders</span><span class="sxs-lookup"><span data-stu-id="68a74-150">InternetMessageHeaders</span></span>](internetmessageheaders.md) <br/> |<span data-ttu-id="68a74-151">Представляет коллекцию всех заголовков сообщений Интернета, содержащиеся внутри элемента в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="68a74-151">Represents the collection of all Internet message headers contained within an item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="68a74-152">DateTimeSent</span><span class="sxs-lookup"><span data-stu-id="68a74-152">DateTimeSent</span></span>](datetimesent.md) <br/> |<span data-ttu-id="68a74-153">Представляет дату и время отправки элемента в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="68a74-153">Represents the date and time that an item in a mailbox was sent.</span></span>  <br/> |
|[<span data-ttu-id="68a74-154">DateTimeCreated</span><span class="sxs-lookup"><span data-stu-id="68a74-154">DateTimeCreated</span></span>](datetimecreated.md) <br/> |<span data-ttu-id="68a74-155">Представляет дату и время создания данного элемента в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="68a74-155">Represents the date and time that a given item in the mailbox was created.</span></span>  <br/> |
|[<span data-ttu-id="68a74-156">ResponseObjects</span><span class="sxs-lookup"><span data-stu-id="68a74-156">ResponseObjects</span></span>](responseobjects.md) <br/> |<span data-ttu-id="68a74-157">Содержит коллекцию всех объектов ответа, которые связаны с элемента в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="68a74-157">Contains a collection of all the response objects that are associated with an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="68a74-158">ReminderDueBy</span><span class="sxs-lookup"><span data-stu-id="68a74-158">ReminderDueBy</span></span>](reminderdueby.md) <br/> |<span data-ttu-id="68a74-159">Представляет дату и время, когда происходит событие.</span><span class="sxs-lookup"><span data-stu-id="68a74-159">Represents the date and time when the event occurs.</span></span> <span data-ttu-id="68a74-160">Используется в элементе [ReminderMinutesBeforeStart](reminderminutesbeforestart.md) определить, когда отображается оповещение.</span><span class="sxs-lookup"><span data-stu-id="68a74-160">This is used by the [ReminderMinutesBeforeStart](reminderminutesbeforestart.md) element to determine when the reminder is displayed.</span></span>  <br/> |
|[<span data-ttu-id="68a74-161">ReminderIsSet</span><span class="sxs-lookup"><span data-stu-id="68a74-161">ReminderIsSet</span></span>](reminderisset.md) <br/> |<span data-ttu-id="68a74-162">Указывает, установлен ли напоминания для элемента в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="68a74-162">Indicates whether a reminder has been set for an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="68a74-163">ReminderMinutesBeforeStart</span><span class="sxs-lookup"><span data-stu-id="68a74-163">ReminderMinutesBeforeStart</span></span>](reminderminutesbeforestart.md) <br/> |<span data-ttu-id="68a74-164">Представляет число минут и только потом событие, когда отображается напоминание.</span><span class="sxs-lookup"><span data-stu-id="68a74-164">Represents the number of minutes before an event when a reminder is displayed.</span></span>  <br/> |
|[<span data-ttu-id="68a74-165">DisplayCc</span><span class="sxs-lookup"><span data-stu-id="68a74-165">DisplayCc</span></span>](displaycc.md) <br/> |<span data-ttu-id="68a74-166">Строка отображения, который используется для содержимого строку "Копия".</span><span class="sxs-lookup"><span data-stu-id="68a74-166">Represents the display string that is used for the contents of the Cc line.</span></span> <span data-ttu-id="68a74-167">Это составное строка всех получателей отображаемые имена «копия».</span><span class="sxs-lookup"><span data-stu-id="68a74-167">This is the concatenated string of all Cc recipient display names.</span></span>  <br/> |
|[<span data-ttu-id="68a74-168">DisplayTo</span><span class="sxs-lookup"><span data-stu-id="68a74-168">DisplayTo</span></span>](displayto.md) <br/> |<span data-ttu-id="68a74-169">Строка отображения, который используется для содержимого строке.</span><span class="sxs-lookup"><span data-stu-id="68a74-169">Represents the display string that is used for the contents of the To line.</span></span> <span data-ttu-id="68a74-170">Это составное строка всех для получателей отображаемые имена.</span><span class="sxs-lookup"><span data-stu-id="68a74-170">This is the concatenated string of all To recipient display names.</span></span>  <br/> |
|[<span data-ttu-id="68a74-171">HasAttachments</span><span class="sxs-lookup"><span data-stu-id="68a74-171">HasAttachments</span></span>](hasattachments.md) <br/> |<span data-ttu-id="68a74-172">Представляет свойство, которое задано значение **true,** Если у элемента есть по крайней мере один видимым вложения.</span><span class="sxs-lookup"><span data-stu-id="68a74-172">Represents a property that is set to **true** if an item has at least one visible attachment.</span></span> <span data-ttu-id="68a74-173">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="68a74-173">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="68a74-174">ExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="68a74-174">ExtendedProperty</span></span>](extendedproperty.md) <br/> |<span data-ttu-id="68a74-175">Определяет расширенные свойства элемента списка рассылки.</span><span class="sxs-lookup"><span data-stu-id="68a74-175">Identifies extended properties on a distribution list item.</span></span>  <br/> |
|[<span data-ttu-id="68a74-176">Язык и региональные параметры</span><span class="sxs-lookup"><span data-stu-id="68a74-176">Culture</span></span>](culture.md) <br/> |<span data-ttu-id="68a74-177">Представляет язык и региональные параметры для элемента списка рассылки в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="68a74-177">Represents the culture for a distribution list item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="68a74-178">EffectiveRights</span><span class="sxs-lookup"><span data-stu-id="68a74-178">EffectiveRights</span></span>](effectiverights.md) <br/> |<span data-ttu-id="68a74-179">Содержит права клиента на основании параметров разрешений для элемента или папки.</span><span class="sxs-lookup"><span data-stu-id="68a74-179">Contains the client's rights based on the permission settings for the item or folder.</span></span> <span data-ttu-id="68a74-180">Этот элемент доступен только для чтения.</span><span class="sxs-lookup"><span data-stu-id="68a74-180">This element is read-only.</span></span>  <br/> |
|[<span data-ttu-id="68a74-181">LastModifiedName</span><span class="sxs-lookup"><span data-stu-id="68a74-181">LastModifiedName</span></span>](lastmodifiedname.md) <br/> |<span data-ttu-id="68a74-182">Содержит отображаемое имя последнего пользователя, чтобы изменить элемент.</span><span class="sxs-lookup"><span data-stu-id="68a74-182">Contains the display name of the last user to modify an item.</span></span>  <br/> |
|[<span data-ttu-id="68a74-183">LastModifiedTime</span><span class="sxs-lookup"><span data-stu-id="68a74-183">LastModifiedTime</span></span>](lastmodifiedtime.md) <br/> |<span data-ttu-id="68a74-184">Указывает время последнего изменения элемента.</span><span class="sxs-lookup"><span data-stu-id="68a74-184">Indicates when an item was last modified.</span></span>  <br/> |
|[<span data-ttu-id="68a74-185">IsAssociated</span><span class="sxs-lookup"><span data-stu-id="68a74-185">IsAssociated</span></span>](isassociated.md) <br/> |<span data-ttu-id="68a74-186">Указывает, является ли элемент связан с папкой.</span><span class="sxs-lookup"><span data-stu-id="68a74-186">Indicates whether the item is associated with a folder.</span></span>  <br/> |
|[<span data-ttu-id="68a74-187">WebClientReadFormQueryString</span><span class="sxs-lookup"><span data-stu-id="68a74-187">WebClientReadFormQueryString</span></span>](webclientreadformquerystring.md) <br/> |<span data-ttu-id="68a74-188">Представляет URL-адрес для присоединения к конечной точке Microsoft Office Outlook Web App для чтения элемента в Outlook Web App.</span><span class="sxs-lookup"><span data-stu-id="68a74-188">Represents a URL to concatenate to the Microsoft Office Outlook Web App endpoint to read an item in Outlook Web App.</span></span>  <br/> |
|[<span data-ttu-id="68a74-189">WebClientEditFormQueryString</span><span class="sxs-lookup"><span data-stu-id="68a74-189">WebClientEditFormQueryString</span></span>](webclienteditformquerystring.md) <br/> |<span data-ttu-id="68a74-190">Представляет URL-адрес для объединения в конечную точку Outlook Web App для редактирования элемента в Outlook Web App.</span><span class="sxs-lookup"><span data-stu-id="68a74-190">Represents a URL to concatenate to the Outlook Web App endpoint to edit an item in Outlook Web App.</span></span>  <br/> |
|[<span data-ttu-id="68a74-191">ConversationId</span><span class="sxs-lookup"><span data-stu-id="68a74-191">ConversationId</span></span>](conversationid.md) <br/> |<span data-ttu-id="68a74-192">Содержит идентификатор элемента или беседы.</span><span class="sxs-lookup"><span data-stu-id="68a74-192">Contains the identifier of an item or conversation.</span></span>  <br/> |
|[<span data-ttu-id="68a74-193">UniqueBody</span><span class="sxs-lookup"><span data-stu-id="68a74-193">UniqueBody</span></span>](uniquebody.md) <br/> |<span data-ttu-id="68a74-194">Представляет фрагмент HTML или обычный текст, который представляет уникальное body эту беседу.</span><span class="sxs-lookup"><span data-stu-id="68a74-194">Represents an HTML fragment or plain text which represents the unique body of this conversation.</span></span>  <br/> |
|[<span data-ttu-id="68a74-195">Отображаемое имя (строка)</span><span class="sxs-lookup"><span data-stu-id="68a74-195">DisplayName (string)</span></span>](displayname-string.md) <br/> |<span data-ttu-id="68a74-196">Задает отображаемое имя списка рассылки.</span><span class="sxs-lookup"><span data-stu-id="68a74-196">Defines the display name of a distribution list.</span></span>  <br/> |
|[<span data-ttu-id="68a74-197">FileAs</span><span class="sxs-lookup"><span data-stu-id="68a74-197">FileAs</span></span>](fileas.md) <br/> |<span data-ttu-id="68a74-198">Представляет, как оформлена в список рассылки в папке «Контакты».</span><span class="sxs-lookup"><span data-stu-id="68a74-198">Represents how a distribution list is filed in the Contacts folder.</span></span>  <br/> |
|[<span data-ttu-id="68a74-199">ContactSource</span><span class="sxs-lookup"><span data-stu-id="68a74-199">ContactSource</span></span>](contactsource.md) <br/> |<span data-ttu-id="68a74-200">Описание, находится ли контакт в хранилище Exchange или в доменных службах Active Directory (AD DS).</span><span class="sxs-lookup"><span data-stu-id="68a74-200">Describes whether the contact is located in the Exchange store or in Active Directory Domain Services (AD DS).</span></span>  <br/> |
|[<span data-ttu-id="68a74-201">Члены (MemberListType)</span><span class="sxs-lookup"><span data-stu-id="68a74-201">Members (MemberListType)</span></span>](members-memberlisttype.md) <br/> |<span data-ttu-id="68a74-202">Содержит список членов списка рассылки.</span><span class="sxs-lookup"><span data-stu-id="68a74-202">Contains a list of members of the distribution list.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="68a74-203">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="68a74-203">Parent elements</span></span>

|<span data-ttu-id="68a74-204">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="68a74-204">**Element**</span></span>|<span data-ttu-id="68a74-205">**Описание**</span><span class="sxs-lookup"><span data-stu-id="68a74-205">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="68a74-206">AdjacentMeetings</span><span class="sxs-lookup"><span data-stu-id="68a74-206">AdjacentMeetings</span></span>](adjacentmeetings.md) <br/> |<span data-ttu-id="68a74-207">Описание всех элементов календаря, расположенных на время собрания.</span><span class="sxs-lookup"><span data-stu-id="68a74-207">Describes all calendar items that are adjacent to a meeting time.</span></span>  <br/> |
|[<span data-ttu-id="68a74-208">AppendToItemField</span><span class="sxs-lookup"><span data-stu-id="68a74-208">AppendToItemField</span></span>](appendtoitemfield.md) <br/> |<span data-ttu-id="68a74-209">Указывает данные для добавления к одному свойству списка рассылки во время [операции UpdateItem](updateitem-operation.md).</span><span class="sxs-lookup"><span data-stu-id="68a74-209">Identifies data to append to a single property of a distribution list during an [UpdateItem operation](updateitem-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="68a74-210">ConflictingMeetings</span><span class="sxs-lookup"><span data-stu-id="68a74-210">ConflictingMeetings</span></span>](conflictingmeetings.md) <br/> |<span data-ttu-id="68a74-211">Определяет все элементы, конфликтующие с время собрания.</span><span class="sxs-lookup"><span data-stu-id="68a74-211">Identifies all items that conflict with a meeting time.</span></span>  <br/> |
|[<span data-ttu-id="68a74-212">Создание (ItemSync)</span><span class="sxs-lookup"><span data-stu-id="68a74-212">Create (ItemSync)</span></span>](create-itemsync.md) <br/> |<span data-ttu-id="68a74-213">Определяет один список для создания в локальном хранилище клиента.</span><span class="sxs-lookup"><span data-stu-id="68a74-213">Identifies a single distribution list to create in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="68a74-214">Обновление (ItemSync)</span><span class="sxs-lookup"><span data-stu-id="68a74-214">Update (ItemSync)</span></span>](update-itemsync.md) <br/> |<span data-ttu-id="68a74-215">Определяет один список для обновления в локальном хранилище клиента.</span><span class="sxs-lookup"><span data-stu-id="68a74-215">Identifies a single distribution list to update in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="68a74-216">Элементы</span><span class="sxs-lookup"><span data-stu-id="68a74-216">Items</span></span>](items.md) <br/> |<span data-ttu-id="68a74-217">Содержит массив элементов.</span><span class="sxs-lookup"><span data-stu-id="68a74-217">Contains an array of items.</span></span>  <br/> |
|[<span data-ttu-id="68a74-218">Элементы (NonEmptyArrayOfAllItemsType)</span><span class="sxs-lookup"><span data-stu-id="68a74-218">Items (NonEmptyArrayOfAllItemsType)</span></span>](items-nonemptyarrayofallitemstype.md) <br/> |<span data-ttu-id="68a74-219">Содержит массив элементов для создания в папку, указанную в элементе [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) .</span><span class="sxs-lookup"><span data-stu-id="68a74-219">Contains an array of items to create in the folder identified by the [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) element.</span></span>  <br/> |
|[<span data-ttu-id="68a74-220">SetItemField</span><span class="sxs-lookup"><span data-stu-id="68a74-220">SetItemField</span></span>](setitemfield.md) <br/> |<span data-ttu-id="68a74-221">Представляет обновление для одного свойства элемента списка рассылки в рамках одной [операции UpdateItem](updateitem-operation.md).</span><span class="sxs-lookup"><span data-stu-id="68a74-221">Represents an update to a single property of a distribution list item in an [UpdateItem operation](updateitem-operation.md).</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="68a74-222">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="68a74-222">Text value</span></span>

<span data-ttu-id="68a74-223">Нет.</span><span class="sxs-lookup"><span data-stu-id="68a74-223">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="68a74-224">Замечания</span><span class="sxs-lookup"><span data-stu-id="68a74-224">Remarks</span></span>

<span data-ttu-id="68a74-225">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="68a74-225">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="68a74-226">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="68a74-226">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="68a74-227">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="68a74-227">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="68a74-228">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="68a74-228">Schema Name</span></span>  <br/> |<span data-ttu-id="68a74-229">Схема Types</span><span class="sxs-lookup"><span data-stu-id="68a74-229">Types schema</span></span>  <br/> |
|<span data-ttu-id="68a74-230">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="68a74-230">Validation File</span></span>  <br/> |<span data-ttu-id="68a74-231">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="68a74-231">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="68a74-232">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="68a74-232">Can be Empty</span></span>  <br/> |<span data-ttu-id="68a74-233">False</span><span class="sxs-lookup"><span data-stu-id="68a74-233">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="68a74-234">См. также</span><span class="sxs-lookup"><span data-stu-id="68a74-234">See also</span></span>

- [<span data-ttu-id="68a74-235">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="68a74-235">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
