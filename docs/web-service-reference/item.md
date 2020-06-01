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
description: Элемент Item представляет общий элемент в хранилище Exchange.
ms.openlocfilehash: 72d8b1344bea3bcd105a0e293365b17f37193ac3
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460318"
---
# <a name="item"></a><span data-ttu-id="5dd2b-103">Элемент</span><span class="sxs-lookup"><span data-stu-id="5dd2b-103">Item</span></span>

<span data-ttu-id="5dd2b-104">Элемент **Item** представляет общий элемент в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="5dd2b-104">The **Item** element represents a generic item in the Exchange store.</span></span> 
  
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

 <span data-ttu-id="5dd2b-105">**ItemType**</span><span class="sxs-lookup"><span data-stu-id="5dd2b-105">**ItemType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5dd2b-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="5dd2b-106">Attributes and elements</span></span>

<span data-ttu-id="5dd2b-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="5dd2b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5dd2b-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="5dd2b-108">Attributes</span></span>

<span data-ttu-id="5dd2b-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="5dd2b-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5dd2b-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="5dd2b-110">Child elements</span></span>

|<span data-ttu-id="5dd2b-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="5dd2b-111">**Element**</span></span>|<span data-ttu-id="5dd2b-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="5dd2b-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5dd2b-113">Сохранитьmimecontent</span><span class="sxs-lookup"><span data-stu-id="5dd2b-113">MimeContent</span></span>](mimecontent.md) <br/> |<span data-ttu-id="5dd2b-114">Содержит собственный многоцелевой поток расширений почты в Интернете (MIME) объекта, представленного в формате base64Binary.</span><span class="sxs-lookup"><span data-stu-id="5dd2b-114">Contains the native Multipurpose Internet Mail Extensions (MIME) stream of an object that is represented in base64Binary format.</span></span>  <br/> |
|[<span data-ttu-id="5dd2b-115">Идентификатор</span><span class="sxs-lookup"><span data-stu-id="5dd2b-115">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="5dd2b-116">Содержит уникальный идентификатор и ключ изменения элемента в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="5dd2b-116">Contains the unique identifier and change key of an item in the Exchange store.</span></span> <span data-ttu-id="5dd2b-117">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5dd2b-117">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="5dd2b-118">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="5dd2b-118">ParentFolderId</span></span>](parentfolderid.md) <br/> |<span data-ttu-id="5dd2b-119">Представляет идентификатор родительской папки, содержащей элемент или папку.</span><span class="sxs-lookup"><span data-stu-id="5dd2b-119">Represents the identifier of the parent folder that contains the item or folder.</span></span> <span data-ttu-id="5dd2b-120">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5dd2b-120">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="5dd2b-121">ItemClass</span><span class="sxs-lookup"><span data-stu-id="5dd2b-121">ItemClass</span></span>](itemclass.md) <br/> |<span data-ttu-id="5dd2b-122">Представляет класс сообщения для элемента.</span><span class="sxs-lookup"><span data-stu-id="5dd2b-122">Represents the message class of an item.</span></span>  <br/> |
|[<span data-ttu-id="5dd2b-123">Тема</span><span class="sxs-lookup"><span data-stu-id="5dd2b-123">Subject</span></span>](subject.md) <br/> |<span data-ttu-id="5dd2b-124">Представляет тему для элементов хранилища Exchange и объектов ответа.</span><span class="sxs-lookup"><span data-stu-id="5dd2b-124">Represents the subject for Exchange store items and response objects.</span></span> <span data-ttu-id="5dd2b-125">Тема может иметь не более 255 символов.</span><span class="sxs-lookup"><span data-stu-id="5dd2b-125">The subject is limited to 255 characters.</span></span>  <br/> |
|[<span data-ttu-id="5dd2b-126">Sensitivity</span><span class="sxs-lookup"><span data-stu-id="5dd2b-126">Sensitivity</span></span>](sensitivity.md) <br/> |<span data-ttu-id="5dd2b-127">Указывает уровень конфиденциальности элемента.</span><span class="sxs-lookup"><span data-stu-id="5dd2b-127">Indicates the sensitivity level of an item.</span></span>  <br/> |
|[<span data-ttu-id="5dd2b-128">Body</span><span class="sxs-lookup"><span data-stu-id="5dd2b-128">Body</span></span>](body.md) <br/> |<span data-ttu-id="5dd2b-129">Представляет реальное содержимое основного текста сообщения.</span><span class="sxs-lookup"><span data-stu-id="5dd2b-129">Represents the actual body content of a message.</span></span>  <br/> |
|[<span data-ttu-id="5dd2b-130">Вложения</span><span class="sxs-lookup"><span data-stu-id="5dd2b-130">Attachments</span></span>](attachments-ex15websvcsotherref.md) <br/> |<span data-ttu-id="5dd2b-131">Содержит элементы или файлы, вложенные в элемент в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="5dd2b-131">Contains the items or files that are attached to an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="5dd2b-132">DateTimeReceived</span><span class="sxs-lookup"><span data-stu-id="5dd2b-132">DateTimeReceived</span></span>](datetimereceived.md) <br/> |<span data-ttu-id="5dd2b-133">Представляет дату и время получения элемента в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="5dd2b-133">Represents the date and time that an item in a mailbox was received.</span></span>  <br/> |
|[<span data-ttu-id="5dd2b-134">Размер</span><span class="sxs-lookup"><span data-stu-id="5dd2b-134">Size</span></span>](size.md) <br/> |<span data-ttu-id="5dd2b-135">Представляет размер элемента в байтах.</span><span class="sxs-lookup"><span data-stu-id="5dd2b-135">Represents the size in bytes of an item.</span></span> <span data-ttu-id="5dd2b-136">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5dd2b-136">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="5dd2b-137">Категории</span><span class="sxs-lookup"><span data-stu-id="5dd2b-137">Categories</span></span>](categories-ex15websvcsotherref.md) <br/> |<span data-ttu-id="5dd2b-138">Представляет коллекцию строк, определяющих, к каким категориям принадлежит элемент в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="5dd2b-138">Represents a collection of strings that identify to which categories an item in the mailbox belongs.</span></span>  <br/> |
|[<span data-ttu-id="5dd2b-139">Importance</span><span class="sxs-lookup"><span data-stu-id="5dd2b-139">Importance</span></span>](importance.md) <br/> |<span data-ttu-id="5dd2b-140">Описывает важность элемента.</span><span class="sxs-lookup"><span data-stu-id="5dd2b-140">Describes the importance of an item.</span></span>  <br/> |
|[<span data-ttu-id="5dd2b-141">инреплито</span><span class="sxs-lookup"><span data-stu-id="5dd2b-141">InReplyTo</span></span>](inreplyto.md) <br/> |<span data-ttu-id="5dd2b-142">Представляет идентификатор элемента, который является ответом на этот элемент.</span><span class="sxs-lookup"><span data-stu-id="5dd2b-142">Represents the identifier of the item to which this item is a reply.</span></span>  <br/> |
|[<span data-ttu-id="5dd2b-143">Отправлено</span><span class="sxs-lookup"><span data-stu-id="5dd2b-143">IsSubmitted</span></span>](issubmitted.md) <br/> |<span data-ttu-id="5dd2b-144">Указывает, был ли элемент отправлен в папку "Исходящие" по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="5dd2b-144">Indicates whether an item has been submitted to the Outbox default folder.</span></span>  <br/> |
|[<span data-ttu-id="5dd2b-145">Черновик</span><span class="sxs-lookup"><span data-stu-id="5dd2b-145">IsDraft</span></span>](isdraft.md) <br/> |<span data-ttu-id="5dd2b-146">Указывает, был ли элемент еще не отправлен.</span><span class="sxs-lookup"><span data-stu-id="5dd2b-146">Represents whether an item has not yet been sent.</span></span>  <br/> |
|[<span data-ttu-id="5dd2b-147">исфромме</span><span class="sxs-lookup"><span data-stu-id="5dd2b-147">IsFromMe</span></span>](isfromme.md) <br/> |<span data-ttu-id="5dd2b-148">Указывает, отправил ли пользователь элемент самому себе.</span><span class="sxs-lookup"><span data-stu-id="5dd2b-148">Indicates whether a user sent an item to itself.</span></span>  <br/> |
|[<span data-ttu-id="5dd2b-149">исресенд</span><span class="sxs-lookup"><span data-stu-id="5dd2b-149">IsResend</span></span>](isresend.md) <br/> |<span data-ttu-id="5dd2b-150">Указывает, был ли ранее отправлен элемент.</span><span class="sxs-lookup"><span data-stu-id="5dd2b-150">Indicates whether the item had previously been sent.</span></span>  <br/> |
|[<span data-ttu-id="5dd2b-151">исунмодифиед</span><span class="sxs-lookup"><span data-stu-id="5dd2b-151">IsUnmodified</span></span>](isunmodified.md) <br/> |<span data-ttu-id="5dd2b-152">Указывает, был ли изменен элемент.</span><span class="sxs-lookup"><span data-stu-id="5dd2b-152">Indicates whether the item has been modified.</span></span>  <br/> |
|[<span data-ttu-id="5dd2b-153">InternetMessageHeaders</span><span class="sxs-lookup"><span data-stu-id="5dd2b-153">InternetMessageHeaders</span></span>](internetmessageheaders.md) <br/> |<span data-ttu-id="5dd2b-154">Представляет коллекцию всех заголовков сообщений Интернета, содержащихся в элементе почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="5dd2b-154">Represents the collection of all Internet message headers that are contained within an item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="5dd2b-155">датетимесент</span><span class="sxs-lookup"><span data-stu-id="5dd2b-155">DateTimeSent</span></span>](datetimesent.md) <br/> |<span data-ttu-id="5dd2b-156">Представляет дату и время отправки элемента в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="5dd2b-156">Represents the date and time that an item in a mailbox was sent.</span></span>  <br/> |
|[<span data-ttu-id="5dd2b-157">DateTimeCreated</span><span class="sxs-lookup"><span data-stu-id="5dd2b-157">DateTimeCreated</span></span>](datetimecreated.md) <br/> |<span data-ttu-id="5dd2b-158">Представляет дату и время создания определенного элемента в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="5dd2b-158">Represents the date and time that a given item in the mailbox was created.</span></span>  <br/> |
|[<span data-ttu-id="5dd2b-159">респонсеобжектс</span><span class="sxs-lookup"><span data-stu-id="5dd2b-159">ResponseObjects</span></span>](responseobjects.md) <br/> |<span data-ttu-id="5dd2b-160">Содержит коллекцию всех объектов ответа, связанных с элементом в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="5dd2b-160">Contains a collection of all the response objects that are associated with an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="5dd2b-161">реминдердуеби</span><span class="sxs-lookup"><span data-stu-id="5dd2b-161">ReminderDueBy</span></span>](reminderdueby.md) <br/> |<span data-ttu-id="5dd2b-162">Представляет дату и время возникновения события.</span><span class="sxs-lookup"><span data-stu-id="5dd2b-162">Represents the date and time when the event occurs.</span></span> <span data-ttu-id="5dd2b-163">Он используется элементом [реминдерминутесбефорестарт](reminderminutesbeforestart.md) для определения времени отображения напоминания.</span><span class="sxs-lookup"><span data-stu-id="5dd2b-163">This is used by the [ReminderMinutesBeforeStart](reminderminutesbeforestart.md) element to determine when the reminder is displayed.</span></span>  <br/> |
|[<span data-ttu-id="5dd2b-164">реминдериссет</span><span class="sxs-lookup"><span data-stu-id="5dd2b-164">ReminderIsSet</span></span>](reminderisset.md) <br/> |<span data-ttu-id="5dd2b-165">Указывает, задано ли напоминание для элемента в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="5dd2b-165">Indicates whether a reminder has been set for an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="5dd2b-166">ReminderMinutesBeforeStart</span><span class="sxs-lookup"><span data-stu-id="5dd2b-166">ReminderMinutesBeforeStart</span></span>](reminderminutesbeforestart.md) <br/> |<span data-ttu-id="5dd2b-167">Представляет количество минут до события при отображении напоминания.</span><span class="sxs-lookup"><span data-stu-id="5dd2b-167">Represents the number of minutes before an event when a reminder is displayed.</span></span>  <br/> |
|[<span data-ttu-id="5dd2b-168">дисплайкк</span><span class="sxs-lookup"><span data-stu-id="5dd2b-168">DisplayCc</span></span>](displaycc.md) <br/> |<span data-ttu-id="5dd2b-169">Представляет отображаемую строку, используемую для содержимого поля "копия".</span><span class="sxs-lookup"><span data-stu-id="5dd2b-169">Represents the display string that is used for the contents of the Cc box.</span></span> <span data-ttu-id="5dd2b-170">Это объединенная строка всех отображаемых имен получателей копии.</span><span class="sxs-lookup"><span data-stu-id="5dd2b-170">This is the concatenated string of all Cc recipient display names.</span></span>  <br/> |
|[<span data-ttu-id="5dd2b-171">дисплайто</span><span class="sxs-lookup"><span data-stu-id="5dd2b-171">DisplayTo</span></span>](displayto.md) <br/> |<span data-ttu-id="5dd2b-172">Представляет отображаемую строку, используемую для содержимого поля "Кому".</span><span class="sxs-lookup"><span data-stu-id="5dd2b-172">Represents the display string that is used for the contents of the To box.</span></span> <span data-ttu-id="5dd2b-173">Это объединенная строка для отображаемых имен получателей.</span><span class="sxs-lookup"><span data-stu-id="5dd2b-173">This is the concatenated string of all To recipient display names.</span></span>  <br/> |
|[<span data-ttu-id="5dd2b-174">HasAttachments</span><span class="sxs-lookup"><span data-stu-id="5dd2b-174">HasAttachments</span></span>](hasattachments.md) <br/> |<span data-ttu-id="5dd2b-175">Представляет свойство, для которого установлено значение **true** , если элемент имеет вложения по крайней мере с одним видимым вложением.</span><span class="sxs-lookup"><span data-stu-id="5dd2b-175">Represents a property that is set to **true** if an item has attachments at least one visible attachment.</span></span> <span data-ttu-id="5dd2b-176">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5dd2b-176">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="5dd2b-177">ExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="5dd2b-177">ExtendedProperty</span></span>](extendedproperty.md) <br/> |<span data-ttu-id="5dd2b-178">Определяет расширенные свойства для папок и элементов.</span><span class="sxs-lookup"><span data-stu-id="5dd2b-178">Identifies extended properties on folders and items.</span></span>  <br/> |
|[<span data-ttu-id="5dd2b-179">Culture</span><span class="sxs-lookup"><span data-stu-id="5dd2b-179">Culture</span></span>](culture.md) <br/> |<span data-ttu-id="5dd2b-180">Представляет язык и региональные параметры для определенного элемента в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="5dd2b-180">Represents the culture for a given item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="5dd2b-181">еффективеригхтс</span><span class="sxs-lookup"><span data-stu-id="5dd2b-181">EffectiveRights</span></span>](effectiverights.md) <br/> |<span data-ttu-id="5dd2b-182">Содержит права клиента на основе параметров разрешений для элемента или папки.</span><span class="sxs-lookup"><span data-stu-id="5dd2b-182">Contains the client's rights based on the permission settings for the item or folder.</span></span> <span data-ttu-id="5dd2b-183">Этот элемент доступен только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5dd2b-183">This element is read-only.</span></span>  <br/> |
|[<span data-ttu-id="5dd2b-184">ластмодифиеднаме</span><span class="sxs-lookup"><span data-stu-id="5dd2b-184">LastModifiedName</span></span>](lastmodifiedname.md) <br/> |<span data-ttu-id="5dd2b-185">Содержит отображаемое имя последнего пользователя для изменения элемента.</span><span class="sxs-lookup"><span data-stu-id="5dd2b-185">Contains the display name of the last user to modify an item.</span></span>  <br/> |
|[<span data-ttu-id="5dd2b-186">LastModifiedTime</span><span class="sxs-lookup"><span data-stu-id="5dd2b-186">LastModifiedTime</span></span>](lastmodifiedtime.md) <br/> |<span data-ttu-id="5dd2b-187">Указывает время последнего изменения элемента.</span><span class="sxs-lookup"><span data-stu-id="5dd2b-187">Indicates when an item was last modified.</span></span>  <br/> |
|[<span data-ttu-id="5dd2b-188">Связанный</span><span class="sxs-lookup"><span data-stu-id="5dd2b-188">IsAssociated</span></span>](isassociated.md) <br/> |<span data-ttu-id="5dd2b-189">Указывает, связан ли элемент с папкой.</span><span class="sxs-lookup"><span data-stu-id="5dd2b-189">Indicates whether the item is associated with a folder.</span></span>  <br/> |
|[<span data-ttu-id="5dd2b-190">вебклиентреадформкуеристринг</span><span class="sxs-lookup"><span data-stu-id="5dd2b-190">WebClientReadFormQueryString</span></span>](webclientreadformquerystring.md) <br/> |<span data-ttu-id="5dd2b-191">Представляет URL-адрес для сцепления с конечной точкой Microsoft Office Outlook Web App для чтения элемента в Outlook Web App.</span><span class="sxs-lookup"><span data-stu-id="5dd2b-191">Represents a URL to concatenate to the Microsoft Office Outlook Web App endpoint to read an item in Outlook Web App.</span></span>  <br/> |
|[<span data-ttu-id="5dd2b-192">вебклиентедитформкуеристринг</span><span class="sxs-lookup"><span data-stu-id="5dd2b-192">WebClientEditFormQueryString</span></span>](webclienteditformquerystring.md) <br/> |<span data-ttu-id="5dd2b-193">Представляет URL-адрес для сцепления с конечной точкой Outlook Web App для изменения элемента в Outlook Web App.</span><span class="sxs-lookup"><span data-stu-id="5dd2b-193">Represents a URL to concatenate to the Outlook Web App endpoint to edit an item in Outlook Web App.</span></span>  <br/> |
|[<span data-ttu-id="5dd2b-194">ConversationId</span><span class="sxs-lookup"><span data-stu-id="5dd2b-194">ConversationId</span></span>](conversationid.md) <br/> |<span data-ttu-id="5dd2b-195">Содержит идентификатор элемента или беседы.</span><span class="sxs-lookup"><span data-stu-id="5dd2b-195">Contains the identifier of an item or conversation.</span></span>  <br/> |
|[<span data-ttu-id="5dd2b-196">UniqueBody</span><span class="sxs-lookup"><span data-stu-id="5dd2b-196">UniqueBody</span></span>](uniquebody.md) <br/> |<span data-ttu-id="5dd2b-197">Представляет фрагмент HTML или обычный текст, представляющий уникальный основной текст этой беседы.</span><span class="sxs-lookup"><span data-stu-id="5dd2b-197">Represents an HTML fragment or plain text which represents the unique body of this conversation.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="5dd2b-198">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="5dd2b-198">Parent elements</span></span>

|<span data-ttu-id="5dd2b-199">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="5dd2b-199">**Element**</span></span>|<span data-ttu-id="5dd2b-200">**Описание**</span><span class="sxs-lookup"><span data-stu-id="5dd2b-200">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5dd2b-201">аджацентмитингс</span><span class="sxs-lookup"><span data-stu-id="5dd2b-201">AdjacentMeetings</span></span>](adjacentmeetings.md) <br/> |<span data-ttu-id="5dd2b-202">Описывает все элементы календаря, смежные с временем собрания.</span><span class="sxs-lookup"><span data-stu-id="5dd2b-202">Describes all calendar items that are adjacent to a meeting time.</span></span>  <br/> |
|[<span data-ttu-id="5dd2b-203">аппендтоитемфиелд</span><span class="sxs-lookup"><span data-stu-id="5dd2b-203">AppendToItemField</span></span>](appendtoitemfield.md) <br/> |<span data-ttu-id="5dd2b-204">Определяет данные, добавляемые в одно свойство элемента/папки во время [операции UpdateItem](updateitem-operation.md).</span><span class="sxs-lookup"><span data-stu-id="5dd2b-204">Identifies data to append to a single property of an item/folder during an [UpdateItem operation](updateitem-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="5dd2b-205">конфликтингмитингс</span><span class="sxs-lookup"><span data-stu-id="5dd2b-205">ConflictingMeetings</span></span>](conflictingmeetings.md) <br/> |<span data-ttu-id="5dd2b-206">Определяет все элементы, которые конфликтуют с временем собрания.</span><span class="sxs-lookup"><span data-stu-id="5dd2b-206">Identifies all items that conflict with a meeting time.</span></span>  <br/> |
|[<span data-ttu-id="5dd2b-207">Create (Итемсинк)</span><span class="sxs-lookup"><span data-stu-id="5dd2b-207">Create (ItemSync)</span></span>](create-itemsync.md) <br/> |<span data-ttu-id="5dd2b-208">Определяет один элемент, который необходимо создать в локальном хранилище клиента.</span><span class="sxs-lookup"><span data-stu-id="5dd2b-208">Identifies a single item to create in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="5dd2b-209">ItemAttachment</span><span class="sxs-lookup"><span data-stu-id="5dd2b-209">ItemAttachment</span></span>](itemattachment.md) <br/> |<span data-ttu-id="5dd2b-210">Представляет элемент Exchange, присоединенный к другому элементу Exchange.</span><span class="sxs-lookup"><span data-stu-id="5dd2b-210">Represents an Exchange item that is attached to another Exchange item.</span></span>  <br/> |
|[<span data-ttu-id="5dd2b-211">Items</span><span class="sxs-lookup"><span data-stu-id="5dd2b-211">Items</span></span>](items.md) <br/> |<span data-ttu-id="5dd2b-212">Содержит массив элементов.</span><span class="sxs-lookup"><span data-stu-id="5dd2b-212">Contains an array of items.</span></span>  <br/> |
|[<span data-ttu-id="5dd2b-213">Элементы (Нонемптяррайофаллитемстипе)</span><span class="sxs-lookup"><span data-stu-id="5dd2b-213">Items (NonEmptyArrayOfAllItemsType)</span></span>](items-nonemptyarrayofallitemstype.md) <br/> |<span data-ttu-id="5dd2b-214">Содержит массив элементов для создания в папке, определяемой элементом [ParentFolderId (таржетфолдеридтипе)](parentfolderid-targetfolderidtype.md) .</span><span class="sxs-lookup"><span data-stu-id="5dd2b-214">Contains an array of items to create in the folder that is identified by the [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) element.</span></span>  <br/> |
|[<span data-ttu-id="5dd2b-215">сетитемфиелд</span><span class="sxs-lookup"><span data-stu-id="5dd2b-215">SetItemField</span></span>](setitemfield.md) <br/> |<span data-ttu-id="5dd2b-216">Представляет обновление одного свойства элемента в [операции UpdateItem](updateitem-operation.md).</span><span class="sxs-lookup"><span data-stu-id="5dd2b-216">Represents an update to a single property of an item in an [UpdateItem operation](updateitem-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="5dd2b-217">Обновление (Итемсинк)</span><span class="sxs-lookup"><span data-stu-id="5dd2b-217">Update (ItemSync)</span></span>](update-itemsync.md) <br/> |<span data-ttu-id="5dd2b-218">Определяет один элемент для обновления в локальном хранилище клиента.</span><span class="sxs-lookup"><span data-stu-id="5dd2b-218">Identifies a single item to update in the local client store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="5dd2b-219">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="5dd2b-219">Text value</span></span>

<span data-ttu-id="5dd2b-220">Нет.</span><span class="sxs-lookup"><span data-stu-id="5dd2b-220">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="5dd2b-221">Примечания</span><span class="sxs-lookup"><span data-stu-id="5dd2b-221">Remarks</span></span>

<span data-ttu-id="5dd2b-222">Важно отметить, что **ItemType** — это базовый тип для [Task](task.md), [календаритем](calendaritem.md), [Contact](contact.md), [дистрибутионлист](distributionlist.md)и [Message](message-ex15websvcsotherref.md).</span><span class="sxs-lookup"><span data-stu-id="5dd2b-222">It is important to note that **ItemType** is the base type for [Task](task.md), [CalendarItem](calendaritem.md), [Contact](contact.md), [DistributionList](distributionlist.md), and [Message](message-ex15websvcsotherref.md).</span></span>
  
<span data-ttu-id="5dd2b-223">Элементы [Message](message-ex15websvcsotherref.md) представляют сообщения электронной почты и все другие элементы, которые не являются строго типизированными схемой веб-служб Exchange (EWS).</span><span class="sxs-lookup"><span data-stu-id="5dd2b-223">[Message](message-ex15websvcsotherref.md) elements represent e-mail messages and all other items that are not strongly typed by the Exchange Web Services (EWS) schema.</span></span> <span data-ttu-id="5dd2b-224">Элементы, такие как IPM. Общий доступ и IPM. InfoPath возвращаются в виде элементов **Message** .</span><span class="sxs-lookup"><span data-stu-id="5dd2b-224">Items such as IPM.Sharing and IPM.InfoPath are returned as **Message** elements.</span></span> <span data-ttu-id="5dd2b-225">Microsoft Exchange Server 2010 не возвращает элемент базового **элемента** в ответах.</span><span class="sxs-lookup"><span data-stu-id="5dd2b-225">Microsoft Exchange Server 2010 does not return the base **Item** element in responses.</span></span> 
  
<span data-ttu-id="5dd2b-226">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="5dd2b-226">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5dd2b-227">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="5dd2b-227">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5dd2b-228">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="5dd2b-228">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="5dd2b-229">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="5dd2b-229">Schema Name</span></span>  <br/> |<span data-ttu-id="5dd2b-230">Схема Types</span><span class="sxs-lookup"><span data-stu-id="5dd2b-230">Types schema</span></span>  <br/> |
|<span data-ttu-id="5dd2b-231">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="5dd2b-231">Validation File</span></span>  <br/> |<span data-ttu-id="5dd2b-232">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="5dd2b-232">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="5dd2b-233">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="5dd2b-233">Can be Empty</span></span>  <br/> |<span data-ttu-id="5dd2b-234">False</span><span class="sxs-lookup"><span data-stu-id="5dd2b-234">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="5dd2b-235">См. также</span><span class="sxs-lookup"><span data-stu-id="5dd2b-235">See also</span></span>



- [<span data-ttu-id="5dd2b-236">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="5dd2b-236">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
  
[<span data-ttu-id="5dd2b-237">Справка по веб-служб Exchange для Exchange</span><span class="sxs-lookup"><span data-stu-id="5dd2b-237">EWS reference for Exchange</span></span>](ews-reference-for-exchange.md)

