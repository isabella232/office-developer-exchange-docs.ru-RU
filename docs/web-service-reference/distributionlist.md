---
title: дистрибутионлист
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
description: Элемент Дистрибутионлист представляет список рассылки.
ms.openlocfilehash: 5eb97bef349ca02848f65fa58370b9c81c6653d0
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457006"
---
# <a name="distributionlist"></a><span data-ttu-id="77c4e-103">дистрибутионлист</span><span class="sxs-lookup"><span data-stu-id="77c4e-103">DistributionList</span></span>

<span data-ttu-id="77c4e-104">Элемент **дистрибутионлист** представляет список рассылки.</span><span class="sxs-lookup"><span data-stu-id="77c4e-104">The **DistributionList** element represents a distribution list.</span></span> 
  
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

 <span data-ttu-id="77c4e-105">**дистрибутионлисттипе**</span><span class="sxs-lookup"><span data-stu-id="77c4e-105">**DistributionListType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="77c4e-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="77c4e-106">Attributes and elements</span></span>

<span data-ttu-id="77c4e-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="77c4e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="77c4e-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="77c4e-108">Attributes</span></span>

<span data-ttu-id="77c4e-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="77c4e-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="77c4e-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="77c4e-110">Child elements</span></span>

|<span data-ttu-id="77c4e-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="77c4e-111">**Element**</span></span>|<span data-ttu-id="77c4e-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="77c4e-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="77c4e-113">Сохранитьmimecontent</span><span class="sxs-lookup"><span data-stu-id="77c4e-113">MimeContent</span></span>](mimecontent.md) <br/> |<span data-ttu-id="77c4e-114">Содержит собственный поток MIME объекта, представленный в формате base64Binary.</span><span class="sxs-lookup"><span data-stu-id="77c4e-114">Contains the native MIME stream of an object represented in base64Binary format.</span></span>  <br/> |
|[<span data-ttu-id="77c4e-115">Идентификатор</span><span class="sxs-lookup"><span data-stu-id="77c4e-115">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="77c4e-116">Содержит уникальный идентификатор и ключ изменения элемента списка рассылки в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="77c4e-116">Contains the unique identifier and change key of a distribution list item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="77c4e-117">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="77c4e-117">ParentFolderId</span></span>](parentfolderid.md) <br/> |<span data-ttu-id="77c4e-118">Представляет идентификатор родительской папки, содержащей элемент списка рассылки.</span><span class="sxs-lookup"><span data-stu-id="77c4e-118">Represents the identifier of the parent folder that contains the distribution list item.</span></span>  <br/> |
|[<span data-ttu-id="77c4e-119">ItemClass</span><span class="sxs-lookup"><span data-stu-id="77c4e-119">ItemClass</span></span>](itemclass.md) <br/> |<span data-ttu-id="77c4e-120">Представляет класс сообщения для элемента списка рассылки.</span><span class="sxs-lookup"><span data-stu-id="77c4e-120">Represents the message class of a distribution list item.</span></span>  <br/> |
|[<span data-ttu-id="77c4e-121">Тема</span><span class="sxs-lookup"><span data-stu-id="77c4e-121">Subject</span></span>](subject.md) <br/> |<span data-ttu-id="77c4e-122">Представляет тему для элементов хранилища Exchange и объектов ответа.</span><span class="sxs-lookup"><span data-stu-id="77c4e-122">Represents the subject for Exchange store items and response objects.</span></span>  <br/> |
|[<span data-ttu-id="77c4e-123">Sensitivity</span><span class="sxs-lookup"><span data-stu-id="77c4e-123">Sensitivity</span></span>](sensitivity.md) <br/> |<span data-ttu-id="77c4e-124">Содержит состояние чувствительности элемента списка рассылки.</span><span class="sxs-lookup"><span data-stu-id="77c4e-124">Contains the status for a distribution list item's sensitivity.</span></span>  <br/> |
|[<span data-ttu-id="77c4e-125">Body</span><span class="sxs-lookup"><span data-stu-id="77c4e-125">Body</span></span>](body.md) <br/> |<span data-ttu-id="77c4e-126">Представляет фактический основной контент элемента списка рассылки.</span><span class="sxs-lookup"><span data-stu-id="77c4e-126">Represents the actual body content of a distribution list item.</span></span>  <br/> |
|[<span data-ttu-id="77c4e-127">Вложения</span><span class="sxs-lookup"><span data-stu-id="77c4e-127">Attachments</span></span>](attachments-ex15websvcsotherref.md) <br/> |<span data-ttu-id="77c4e-128">Содержит элементы или файлы, вложенные в элемент списка рассылки в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="77c4e-128">Contains the items or files that are attached to a distribution list item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="77c4e-129">DateTimeReceived</span><span class="sxs-lookup"><span data-stu-id="77c4e-129">DateTimeReceived</span></span>](datetimereceived.md) <br/> |<span data-ttu-id="77c4e-130">Представляет дату и время получения элемента списка рассылки в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="77c4e-130">Represents the date and time that a distribution list item in a mailbox was received.</span></span>  <br/> |
|[<span data-ttu-id="77c4e-131">Размер</span><span class="sxs-lookup"><span data-stu-id="77c4e-131">Size</span></span>](size.md) <br/> |<span data-ttu-id="77c4e-132">Представляет размер элемента списка рассылки (в байтах).</span><span class="sxs-lookup"><span data-stu-id="77c4e-132">Represents the size, in bytes, of a distribution list item.</span></span> <span data-ttu-id="77c4e-133">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="77c4e-133">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="77c4e-134">Категории</span><span class="sxs-lookup"><span data-stu-id="77c4e-134">Categories</span></span>](categories-ex15websvcsotherref.md) <br/> |<span data-ttu-id="77c4e-135">Представляет коллекцию строк, указывающих, к каким категориям принадлежит элемент списка рассылки в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="77c4e-135">Represents a collection of strings that identify to which categories a distribution list item in the mailbox belongs.</span></span>  <br/> |
|[<span data-ttu-id="77c4e-136">Importance</span><span class="sxs-lookup"><span data-stu-id="77c4e-136">Importance</span></span>](importance.md) <br/> |<span data-ttu-id="77c4e-137">Описывает важность элемента списка рассылки.</span><span class="sxs-lookup"><span data-stu-id="77c4e-137">Describes the importance of a distribution list item.</span></span>  <br/> |
|[<span data-ttu-id="77c4e-138">инреплито</span><span class="sxs-lookup"><span data-stu-id="77c4e-138">InReplyTo</span></span>](inreplyto.md) <br/> |<span data-ttu-id="77c4e-139">Представляет идентификатор элемента, который является ответом для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="77c4e-139">Represents the identifier of the item which this item is a reply.</span></span>  <br/> |
|[<span data-ttu-id="77c4e-140">Отправлено</span><span class="sxs-lookup"><span data-stu-id="77c4e-140">IsSubmitted</span></span>](issubmitted.md) <br/> |<span data-ttu-id="77c4e-141">Указывает, был ли элемент отправлен в папку "Исходящие" по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="77c4e-141">Indicates whether an item has been submitted to the Outbox default folder.</span></span>  <br/> |
|[<span data-ttu-id="77c4e-142">Черновик</span><span class="sxs-lookup"><span data-stu-id="77c4e-142">IsDraft</span></span>](isdraft.md) <br/> |<span data-ttu-id="77c4e-143">Указывает, был ли элемент еще не отправлен.</span><span class="sxs-lookup"><span data-stu-id="77c4e-143">Represents whether an item has not yet been sent.</span></span>  <br/> |
|[<span data-ttu-id="77c4e-144">исфромме</span><span class="sxs-lookup"><span data-stu-id="77c4e-144">IsFromMe</span></span>](isfromme.md) <br/> |<span data-ttu-id="77c4e-145">Указывает, отправил ли пользователь элемент самому себе.</span><span class="sxs-lookup"><span data-stu-id="77c4e-145">Indicates whether a user sent an item to itself.</span></span>  <br/> |
|[<span data-ttu-id="77c4e-146">исресенд</span><span class="sxs-lookup"><span data-stu-id="77c4e-146">IsResend</span></span>](isresend.md) <br/> |<span data-ttu-id="77c4e-147">Указывает, был ли ранее отправлен элемент.</span><span class="sxs-lookup"><span data-stu-id="77c4e-147">Indicates whether the item had previously been sent.</span></span>  <br/> |
|[<span data-ttu-id="77c4e-148">исунмодифиед</span><span class="sxs-lookup"><span data-stu-id="77c4e-148">IsUnmodified</span></span>](isunmodified.md) <br/> |<span data-ttu-id="77c4e-149">Указывает, был ли изменен элемент.</span><span class="sxs-lookup"><span data-stu-id="77c4e-149">Indicates whether the item has been modified.</span></span>  <br/> |
|[<span data-ttu-id="77c4e-150">InternetMessageHeaders</span><span class="sxs-lookup"><span data-stu-id="77c4e-150">InternetMessageHeaders</span></span>](internetmessageheaders.md) <br/> |<span data-ttu-id="77c4e-151">Представляет коллекцию всех заголовков сообщений Интернета, содержащихся в элементе почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="77c4e-151">Represents the collection of all Internet message headers contained within an item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="77c4e-152">датетимесент</span><span class="sxs-lookup"><span data-stu-id="77c4e-152">DateTimeSent</span></span>](datetimesent.md) <br/> |<span data-ttu-id="77c4e-153">Представляет дату и время отправки элемента в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="77c4e-153">Represents the date and time that an item in a mailbox was sent.</span></span>  <br/> |
|[<span data-ttu-id="77c4e-154">DateTimeCreated</span><span class="sxs-lookup"><span data-stu-id="77c4e-154">DateTimeCreated</span></span>](datetimecreated.md) <br/> |<span data-ttu-id="77c4e-155">Представляет дату и время создания определенного элемента в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="77c4e-155">Represents the date and time that a given item in the mailbox was created.</span></span>  <br/> |
|[<span data-ttu-id="77c4e-156">респонсеобжектс</span><span class="sxs-lookup"><span data-stu-id="77c4e-156">ResponseObjects</span></span>](responseobjects.md) <br/> |<span data-ttu-id="77c4e-157">Содержит коллекцию всех объектов ответа, связанных с элементом в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="77c4e-157">Contains a collection of all the response objects that are associated with an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="77c4e-158">реминдердуеби</span><span class="sxs-lookup"><span data-stu-id="77c4e-158">ReminderDueBy</span></span>](reminderdueby.md) <br/> |<span data-ttu-id="77c4e-159">Представляет дату и время возникновения события.</span><span class="sxs-lookup"><span data-stu-id="77c4e-159">Represents the date and time when the event occurs.</span></span> <span data-ttu-id="77c4e-160">Он используется элементом [реминдерминутесбефорестарт](reminderminutesbeforestart.md) для определения времени отображения напоминания.</span><span class="sxs-lookup"><span data-stu-id="77c4e-160">This is used by the [ReminderMinutesBeforeStart](reminderminutesbeforestart.md) element to determine when the reminder is displayed.</span></span>  <br/> |
|[<span data-ttu-id="77c4e-161">реминдериссет</span><span class="sxs-lookup"><span data-stu-id="77c4e-161">ReminderIsSet</span></span>](reminderisset.md) <br/> |<span data-ttu-id="77c4e-162">Указывает, задано ли напоминание для элемента в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="77c4e-162">Indicates whether a reminder has been set for an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="77c4e-163">ReminderMinutesBeforeStart</span><span class="sxs-lookup"><span data-stu-id="77c4e-163">ReminderMinutesBeforeStart</span></span>](reminderminutesbeforestart.md) <br/> |<span data-ttu-id="77c4e-164">Представляет количество минут до события при отображении напоминания.</span><span class="sxs-lookup"><span data-stu-id="77c4e-164">Represents the number of minutes before an event when a reminder is displayed.</span></span>  <br/> |
|[<span data-ttu-id="77c4e-165">дисплайкк</span><span class="sxs-lookup"><span data-stu-id="77c4e-165">DisplayCc</span></span>](displaycc.md) <br/> |<span data-ttu-id="77c4e-166">Представляет отображаемую строку, используемую для содержимого строки "копия".</span><span class="sxs-lookup"><span data-stu-id="77c4e-166">Represents the display string that is used for the contents of the Cc line.</span></span> <span data-ttu-id="77c4e-167">Это объединенная строка всех отображаемых имен получателей копии.</span><span class="sxs-lookup"><span data-stu-id="77c4e-167">This is the concatenated string of all Cc recipient display names.</span></span>  <br/> |
|[<span data-ttu-id="77c4e-168">дисплайто</span><span class="sxs-lookup"><span data-stu-id="77c4e-168">DisplayTo</span></span>](displayto.md) <br/> |<span data-ttu-id="77c4e-169">Представляет отображаемую строку, используемую для содержимого строки "Кому".</span><span class="sxs-lookup"><span data-stu-id="77c4e-169">Represents the display string that is used for the contents of the To line.</span></span> <span data-ttu-id="77c4e-170">Это объединенная строка для отображаемых имен получателей.</span><span class="sxs-lookup"><span data-stu-id="77c4e-170">This is the concatenated string of all To recipient display names.</span></span>  <br/> |
|[<span data-ttu-id="77c4e-171">HasAttachments</span><span class="sxs-lookup"><span data-stu-id="77c4e-171">HasAttachments</span></span>](hasattachments.md) <br/> |<span data-ttu-id="77c4e-172">Представляет свойство, для которого задано значение **true** , если элемент имеет по крайней мере одно видимое вложение.</span><span class="sxs-lookup"><span data-stu-id="77c4e-172">Represents a property that is set to **true** if an item has at least one visible attachment.</span></span> <span data-ttu-id="77c4e-173">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="77c4e-173">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="77c4e-174">ExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="77c4e-174">ExtendedProperty</span></span>](extendedproperty.md) <br/> |<span data-ttu-id="77c4e-175">Определяет расширенные свойства для элемента списка рассылки.</span><span class="sxs-lookup"><span data-stu-id="77c4e-175">Identifies extended properties on a distribution list item.</span></span>  <br/> |
|[<span data-ttu-id="77c4e-176">Culture</span><span class="sxs-lookup"><span data-stu-id="77c4e-176">Culture</span></span>](culture.md) <br/> |<span data-ttu-id="77c4e-177">Представляет язык и региональные параметры для элемента списка рассылки в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="77c4e-177">Represents the culture for a distribution list item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="77c4e-178">еффективеригхтс</span><span class="sxs-lookup"><span data-stu-id="77c4e-178">EffectiveRights</span></span>](effectiverights.md) <br/> |<span data-ttu-id="77c4e-179">Содержит права клиента на основе параметров разрешений для элемента или папки.</span><span class="sxs-lookup"><span data-stu-id="77c4e-179">Contains the client's rights based on the permission settings for the item or folder.</span></span> <span data-ttu-id="77c4e-180">Этот элемент доступен только для чтения.</span><span class="sxs-lookup"><span data-stu-id="77c4e-180">This element is read-only.</span></span>  <br/> |
|[<span data-ttu-id="77c4e-181">ластмодифиеднаме</span><span class="sxs-lookup"><span data-stu-id="77c4e-181">LastModifiedName</span></span>](lastmodifiedname.md) <br/> |<span data-ttu-id="77c4e-182">Содержит отображаемое имя последнего пользователя для изменения элемента.</span><span class="sxs-lookup"><span data-stu-id="77c4e-182">Contains the display name of the last user to modify an item.</span></span>  <br/> |
|[<span data-ttu-id="77c4e-183">LastModifiedTime</span><span class="sxs-lookup"><span data-stu-id="77c4e-183">LastModifiedTime</span></span>](lastmodifiedtime.md) <br/> |<span data-ttu-id="77c4e-184">Указывает время последнего изменения элемента.</span><span class="sxs-lookup"><span data-stu-id="77c4e-184">Indicates when an item was last modified.</span></span>  <br/> |
|[<span data-ttu-id="77c4e-185">Связанный</span><span class="sxs-lookup"><span data-stu-id="77c4e-185">IsAssociated</span></span>](isassociated.md) <br/> |<span data-ttu-id="77c4e-186">Указывает, связан ли элемент с папкой.</span><span class="sxs-lookup"><span data-stu-id="77c4e-186">Indicates whether the item is associated with a folder.</span></span>  <br/> |
|[<span data-ttu-id="77c4e-187">вебклиентреадформкуеристринг</span><span class="sxs-lookup"><span data-stu-id="77c4e-187">WebClientReadFormQueryString</span></span>](webclientreadformquerystring.md) <br/> |<span data-ttu-id="77c4e-188">Представляет URL-адрес для сцепления с конечной точкой Microsoft Office Outlook Web App для чтения элемента в Outlook Web App.</span><span class="sxs-lookup"><span data-stu-id="77c4e-188">Represents a URL to concatenate to the Microsoft Office Outlook Web App endpoint to read an item in Outlook Web App.</span></span>  <br/> |
|[<span data-ttu-id="77c4e-189">вебклиентедитформкуеристринг</span><span class="sxs-lookup"><span data-stu-id="77c4e-189">WebClientEditFormQueryString</span></span>](webclienteditformquerystring.md) <br/> |<span data-ttu-id="77c4e-190">Представляет URL-адрес для сцепления с конечной точкой Outlook Web App для изменения элемента в Outlook Web App.</span><span class="sxs-lookup"><span data-stu-id="77c4e-190">Represents a URL to concatenate to the Outlook Web App endpoint to edit an item in Outlook Web App.</span></span>  <br/> |
|[<span data-ttu-id="77c4e-191">ConversationId</span><span class="sxs-lookup"><span data-stu-id="77c4e-191">ConversationId</span></span>](conversationid.md) <br/> |<span data-ttu-id="77c4e-192">Содержит идентификатор элемента или беседы.</span><span class="sxs-lookup"><span data-stu-id="77c4e-192">Contains the identifier of an item or conversation.</span></span>  <br/> |
|[<span data-ttu-id="77c4e-193">UniqueBody</span><span class="sxs-lookup"><span data-stu-id="77c4e-193">UniqueBody</span></span>](uniquebody.md) <br/> |<span data-ttu-id="77c4e-194">Представляет фрагмент HTML или обычный текст, представляющий уникальный основной текст этой беседы.</span><span class="sxs-lookup"><span data-stu-id="77c4e-194">Represents an HTML fragment or plain text which represents the unique body of this conversation.</span></span>  <br/> |
|[<span data-ttu-id="77c4e-195">DisplayName (строка)</span><span class="sxs-lookup"><span data-stu-id="77c4e-195">DisplayName (string)</span></span>](displayname-string.md) <br/> |<span data-ttu-id="77c4e-196">Определяет отображаемое имя списка рассылки.</span><span class="sxs-lookup"><span data-stu-id="77c4e-196">Defines the display name of a distribution list.</span></span>  <br/> |
|[<span data-ttu-id="77c4e-197">FileAs</span><span class="sxs-lookup"><span data-stu-id="77c4e-197">FileAs</span></span>](fileas.md) <br/> |<span data-ttu-id="77c4e-198">Представляет способ хранения списка рассылки в папке "Контакты".</span><span class="sxs-lookup"><span data-stu-id="77c4e-198">Represents how a distribution list is filed in the Contacts folder.</span></span>  <br/> |
|[<span data-ttu-id="77c4e-199">контактсаурце</span><span class="sxs-lookup"><span data-stu-id="77c4e-199">ContactSource</span></span>](contactsource.md) <br/> |<span data-ttu-id="77c4e-200">Указывает, находится ли контакт в хранилище Exchange или в доменных службах Active Directory (AD DS).</span><span class="sxs-lookup"><span data-stu-id="77c4e-200">Describes whether the contact is located in the Exchange store or in Active Directory Domain Services (AD DS).</span></span>  <br/> |
|[<span data-ttu-id="77c4e-201">Members (Мемберлисттипе)</span><span class="sxs-lookup"><span data-stu-id="77c4e-201">Members (MemberListType)</span></span>](members-memberlisttype.md) <br/> |<span data-ttu-id="77c4e-202">Содержит список членов списка рассылки.</span><span class="sxs-lookup"><span data-stu-id="77c4e-202">Contains a list of members of the distribution list.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="77c4e-203">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="77c4e-203">Parent elements</span></span>

|<span data-ttu-id="77c4e-204">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="77c4e-204">**Element**</span></span>|<span data-ttu-id="77c4e-205">**Описание**</span><span class="sxs-lookup"><span data-stu-id="77c4e-205">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="77c4e-206">аджацентмитингс</span><span class="sxs-lookup"><span data-stu-id="77c4e-206">AdjacentMeetings</span></span>](adjacentmeetings.md) <br/> |<span data-ttu-id="77c4e-207">Описывает все элементы календаря, смежные с временем собрания.</span><span class="sxs-lookup"><span data-stu-id="77c4e-207">Describes all calendar items that are adjacent to a meeting time.</span></span>  <br/> |
|[<span data-ttu-id="77c4e-208">аппендтоитемфиелд</span><span class="sxs-lookup"><span data-stu-id="77c4e-208">AppendToItemField</span></span>](appendtoitemfield.md) <br/> |<span data-ttu-id="77c4e-209">Определяет данные, добавляемые к одному свойству списка рассылки во время [операции UpdateItem](updateitem-operation.md).</span><span class="sxs-lookup"><span data-stu-id="77c4e-209">Identifies data to append to a single property of a distribution list during an [UpdateItem operation](updateitem-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="77c4e-210">конфликтингмитингс</span><span class="sxs-lookup"><span data-stu-id="77c4e-210">ConflictingMeetings</span></span>](conflictingmeetings.md) <br/> |<span data-ttu-id="77c4e-211">Определяет все элементы, которые конфликтуют с временем собрания.</span><span class="sxs-lookup"><span data-stu-id="77c4e-211">Identifies all items that conflict with a meeting time.</span></span>  <br/> |
|[<span data-ttu-id="77c4e-212">Create (Итемсинк)</span><span class="sxs-lookup"><span data-stu-id="77c4e-212">Create (ItemSync)</span></span>](create-itemsync.md) <br/> |<span data-ttu-id="77c4e-213">Определяет один список рассылки для создания в локальном хранилище клиента.</span><span class="sxs-lookup"><span data-stu-id="77c4e-213">Identifies a single distribution list to create in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="77c4e-214">Обновление (Итемсинк)</span><span class="sxs-lookup"><span data-stu-id="77c4e-214">Update (ItemSync)</span></span>](update-itemsync.md) <br/> |<span data-ttu-id="77c4e-215">Определяет один список рассылки для обновления в локальном хранилище клиента.</span><span class="sxs-lookup"><span data-stu-id="77c4e-215">Identifies a single distribution list to update in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="77c4e-216">Items</span><span class="sxs-lookup"><span data-stu-id="77c4e-216">Items</span></span>](items.md) <br/> |<span data-ttu-id="77c4e-217">Содержит массив элементов.</span><span class="sxs-lookup"><span data-stu-id="77c4e-217">Contains an array of items.</span></span>  <br/> |
|[<span data-ttu-id="77c4e-218">Элементы (Нонемптяррайофаллитемстипе)</span><span class="sxs-lookup"><span data-stu-id="77c4e-218">Items (NonEmptyArrayOfAllItemsType)</span></span>](items-nonemptyarrayofallitemstype.md) <br/> |<span data-ttu-id="77c4e-219">Содержит массив элементов для создания в папке, определенной элементом [ParentFolderId (таржетфолдеридтипе)](parentfolderid-targetfolderidtype.md) .</span><span class="sxs-lookup"><span data-stu-id="77c4e-219">Contains an array of items to create in the folder identified by the [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) element.</span></span>  <br/> |
|[<span data-ttu-id="77c4e-220">сетитемфиелд</span><span class="sxs-lookup"><span data-stu-id="77c4e-220">SetItemField</span></span>](setitemfield.md) <br/> |<span data-ttu-id="77c4e-221">Представляет обновление одного свойства элемента списка рассылки в [операции UpdateItem](updateitem-operation.md).</span><span class="sxs-lookup"><span data-stu-id="77c4e-221">Represents an update to a single property of a distribution list item in an [UpdateItem operation](updateitem-operation.md).</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="77c4e-222">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="77c4e-222">Text value</span></span>

<span data-ttu-id="77c4e-223">Нет.</span><span class="sxs-lookup"><span data-stu-id="77c4e-223">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="77c4e-224">Примечания</span><span class="sxs-lookup"><span data-stu-id="77c4e-224">Remarks</span></span>

<span data-ttu-id="77c4e-225">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="77c4e-225">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="77c4e-226">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="77c4e-226">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="77c4e-227">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="77c4e-227">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="77c4e-228">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="77c4e-228">Schema Name</span></span>  <br/> |<span data-ttu-id="77c4e-229">Схема Types</span><span class="sxs-lookup"><span data-stu-id="77c4e-229">Types schema</span></span>  <br/> |
|<span data-ttu-id="77c4e-230">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="77c4e-230">Validation File</span></span>  <br/> |<span data-ttu-id="77c4e-231">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="77c4e-231">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="77c4e-232">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="77c4e-232">Can be Empty</span></span>  <br/> |<span data-ttu-id="77c4e-233">False</span><span class="sxs-lookup"><span data-stu-id="77c4e-233">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="77c4e-234">См. также</span><span class="sxs-lookup"><span data-stu-id="77c4e-234">See also</span></span>

- [<span data-ttu-id="77c4e-235">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="77c4e-235">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

