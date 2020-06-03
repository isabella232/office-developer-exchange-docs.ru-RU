---
title: Задача
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Task
api_type:
- schema
ms.assetid: 7c84927e-db28-4c5d-b0b5-cbcc2b88d869
description: Элемент Task представляет задачу в хранилище Exchange.
ms.openlocfilehash: 669f90dfa74cd085091e9836a1d31ca53bbf165e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458945"
---
# <a name="task"></a><span data-ttu-id="25d47-103">Задача</span><span class="sxs-lookup"><span data-stu-id="25d47-103">Task</span></span>

<span data-ttu-id="25d47-104">Элемент **Task** представляет задачу в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="25d47-104">The **Task** element represents a task in the Exchange store.</span></span> 
  
```xml
<Task>
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
   <ActualWork/>
   <AssignedTime/>
   <BillingInformation/>
   <ChangeCount/>
   <Companies/>
   <CompleteDate/>
   <Contacts/>
   <DelegationState/>
   <Delegator/>
   <DueDate/>
   <IsAssignmentEditable/>
   <IsComplete/>
   <IsRecurring/>
   <IsTeamTask/>
   <Mileage/>
   <Owner/>
   <PercentComplete/>
   <Recurrence/>
   <StartDate/>
   <Status/>
   <StatusDescription/>
   <TotalWork/>
   <EffectiveRights/>
   <LastModifiedName/>
   <LastModifiedTime/>
   <IsAssociated/>
   <WebClientReadFormQueryString/>
   <WebClientEditFormQueryString/>
   <ConversationId/>
   <UniqueBody/>
</Task>
```

<span data-ttu-id="25d47-105">**тасктипе**</span><span class="sxs-lookup"><span data-stu-id="25d47-105">**TaskType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="25d47-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="25d47-106">Attributes and elements</span></span>

<span data-ttu-id="25d47-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="25d47-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="25d47-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="25d47-108">Attributes</span></span>

<span data-ttu-id="25d47-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="25d47-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="25d47-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="25d47-110">Child elements</span></span>

|<span data-ttu-id="25d47-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="25d47-111">**Element**</span></span>|<span data-ttu-id="25d47-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="25d47-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="25d47-113">Сохранитьmimecontent</span><span class="sxs-lookup"><span data-stu-id="25d47-113">MimeContent</span></span>](mimecontent.md) <br/> |<span data-ttu-id="25d47-114">Содержит собственный многоцелевой поток расширений почты в Интернете (MIME) объекта, представленного в формате base64Binary.</span><span class="sxs-lookup"><span data-stu-id="25d47-114">Contains the native Multipurpose Internet Mail Extensions (MIME) stream of an object that is represented in base64Binary format.</span></span>  <br/> |
|[<span data-ttu-id="25d47-115">Идентификатор</span><span class="sxs-lookup"><span data-stu-id="25d47-115">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="25d47-116">Содержит уникальный идентификатор и ключ изменения элемента в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="25d47-116">Contains the unique identifier and change key of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="25d47-117">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="25d47-117">ParentFolderId</span></span>](parentfolderid.md) <br/> |<span data-ttu-id="25d47-118">Представляет идентификатор родительской папки, содержащей элемент или папку.</span><span class="sxs-lookup"><span data-stu-id="25d47-118">Represents the identifier of the parent folder that contains the item or folder.</span></span>  <br/> |
|[<span data-ttu-id="25d47-119">ItemClass</span><span class="sxs-lookup"><span data-stu-id="25d47-119">ItemClass</span></span>](itemclass.md) <br/> |<span data-ttu-id="25d47-120">Представляет класс сообщения для элемента.</span><span class="sxs-lookup"><span data-stu-id="25d47-120">Represents the message class of an item.</span></span>  <br/> |
|[<span data-ttu-id="25d47-121">Тема</span><span class="sxs-lookup"><span data-stu-id="25d47-121">Subject</span></span>](subject.md) <br/> |<span data-ttu-id="25d47-122">Представляет тему для элементов хранилища Exchange и объектов ответа.</span><span class="sxs-lookup"><span data-stu-id="25d47-122">Represents the subject for Exchange store items and response objects.</span></span>  <br/> |
|[<span data-ttu-id="25d47-123">Sensitivity</span><span class="sxs-lookup"><span data-stu-id="25d47-123">Sensitivity</span></span>](sensitivity.md) <br/> |<span data-ttu-id="25d47-124">Содержит статус чувствительности элемента.</span><span class="sxs-lookup"><span data-stu-id="25d47-124">Contains the status for an item's sensitivity.</span></span>  <br/> |
|[<span data-ttu-id="25d47-125">Body</span><span class="sxs-lookup"><span data-stu-id="25d47-125">Body</span></span>](body.md) <br/> |<span data-ttu-id="25d47-126">Представляет реальное содержимое основного текста сообщения.</span><span class="sxs-lookup"><span data-stu-id="25d47-126">Represents the actual body content of a message.</span></span>  <br/> |
|[<span data-ttu-id="25d47-127">Вложения</span><span class="sxs-lookup"><span data-stu-id="25d47-127">Attachments</span></span>](attachments-ex15websvcsotherref.md) <br/> |<span data-ttu-id="25d47-128">Содержит элементы или файлы, вложенные в элемент в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="25d47-128">Contains the items or files that are attached to an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="25d47-129">DateTimeReceived</span><span class="sxs-lookup"><span data-stu-id="25d47-129">DateTimeReceived</span></span>](datetimereceived.md) <br/> |<span data-ttu-id="25d47-130">Представляет дату и время получения элемента в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="25d47-130">Represents the date and time that an item in a mailbox was received.</span></span>  <br/> |
|[<span data-ttu-id="25d47-131">Размер</span><span class="sxs-lookup"><span data-stu-id="25d47-131">Size</span></span>](size.md) <br/> |<span data-ttu-id="25d47-132">Представляет размер элемента (в байтах).</span><span class="sxs-lookup"><span data-stu-id="25d47-132">Represents the size, in bytes, of an item.</span></span> <span data-ttu-id="25d47-133">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="25d47-133">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="25d47-134">Категории</span><span class="sxs-lookup"><span data-stu-id="25d47-134">Categories</span></span>](categories-ex15websvcsotherref.md) <br/> |<span data-ttu-id="25d47-135">Представляет коллекцию строк, определяющих, к каким категориям принадлежит элемент в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="25d47-135">Represents a collection of strings that identify to which categories an item in the mailbox belongs.</span></span>  <br/> |
|[<span data-ttu-id="25d47-136">Importance</span><span class="sxs-lookup"><span data-stu-id="25d47-136">Importance</span></span>](importance.md) <br/> |<span data-ttu-id="25d47-137">Описывает важность элемента.</span><span class="sxs-lookup"><span data-stu-id="25d47-137">Describes the importance of an item.</span></span>  <br/> |
|[<span data-ttu-id="25d47-138">инреплито</span><span class="sxs-lookup"><span data-stu-id="25d47-138">InReplyTo</span></span>](inreplyto.md) <br/> |<span data-ttu-id="25d47-139">Представляет идентификатор элемента, который является ответом на этот элемент.</span><span class="sxs-lookup"><span data-stu-id="25d47-139">Represents the identifier of the item to which this item is a reply.</span></span>  <br/> |
|[<span data-ttu-id="25d47-140">Отправлено</span><span class="sxs-lookup"><span data-stu-id="25d47-140">IsSubmitted</span></span>](issubmitted.md) <br/> |<span data-ttu-id="25d47-141">Указывает, был ли элемент отправлен в папку "Исходящие" по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="25d47-141">Indicates whether an item has been submitted to the Outbox default folder.</span></span>  <br/> |
|[<span data-ttu-id="25d47-142">Черновик</span><span class="sxs-lookup"><span data-stu-id="25d47-142">IsDraft</span></span>](isdraft.md) <br/> |<span data-ttu-id="25d47-143">Указывает, был ли элемент еще не отправлен.</span><span class="sxs-lookup"><span data-stu-id="25d47-143">Represents whether an item has not yet been sent.</span></span>  <br/> |
|[<span data-ttu-id="25d47-144">исфромме</span><span class="sxs-lookup"><span data-stu-id="25d47-144">IsFromMe</span></span>](isfromme.md) <br/> |<span data-ttu-id="25d47-145">Указывает, отправляет ли пользователь элемент.</span><span class="sxs-lookup"><span data-stu-id="25d47-145">Indicates whether a user sent an item to him or herself.</span></span>  <br/> |
|[<span data-ttu-id="25d47-146">исресенд</span><span class="sxs-lookup"><span data-stu-id="25d47-146">IsResend</span></span>](isresend.md) <br/> |<span data-ttu-id="25d47-147">Указывает, был ли ранее отправлен элемент.</span><span class="sxs-lookup"><span data-stu-id="25d47-147">Indicates whether the item had previously been sent.</span></span>  <br/> |
|[<span data-ttu-id="25d47-148">исунмодифиед</span><span class="sxs-lookup"><span data-stu-id="25d47-148">IsUnmodified</span></span>](isunmodified.md) <br/> |<span data-ttu-id="25d47-149">Указывает, был ли изменен элемент.</span><span class="sxs-lookup"><span data-stu-id="25d47-149">Indicates whether the item has been modified.</span></span>  <br/> |
|[<span data-ttu-id="25d47-150">InternetMessageHeaders</span><span class="sxs-lookup"><span data-stu-id="25d47-150">InternetMessageHeaders</span></span>](internetmessageheaders.md) <br/> |<span data-ttu-id="25d47-151">Представляет коллекцию всех заголовков сообщений Интернета, которые находятся в элементе почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="25d47-151">Represents the collection of all Internet message headers that are contained in an item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="25d47-152">датетимесент</span><span class="sxs-lookup"><span data-stu-id="25d47-152">DateTimeSent</span></span>](datetimesent.md) <br/> |<span data-ttu-id="25d47-153">Представляет дату и время отправки элемента в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="25d47-153">Represents the date and time that an item in a mailbox was sent.</span></span>  <br/> |
|[<span data-ttu-id="25d47-154">DateTimeCreated</span><span class="sxs-lookup"><span data-stu-id="25d47-154">DateTimeCreated</span></span>](datetimecreated.md) <br/> |<span data-ttu-id="25d47-155">Представляет дату и время создания определенного элемента в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="25d47-155">Represents the date and time that a given item in the mailbox was created.</span></span>  <br/> |
|[<span data-ttu-id="25d47-156">респонсеобжектс</span><span class="sxs-lookup"><span data-stu-id="25d47-156">ResponseObjects</span></span>](responseobjects.md) <br/> |<span data-ttu-id="25d47-157">Содержит коллекцию всех объектов ответа, связанных с элементом в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="25d47-157">Contains a collection of all the response objects that are associated with an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="25d47-158">реминдердуеби</span><span class="sxs-lookup"><span data-stu-id="25d47-158">ReminderDueBy</span></span>](reminderdueby.md) <br/> |<span data-ttu-id="25d47-159">Представляет дату и время возникновения события.</span><span class="sxs-lookup"><span data-stu-id="25d47-159">Represents the date and time when the event occurs.</span></span> <span data-ttu-id="25d47-160">Он используется элементом [реминдерминутесбефорестарт](reminderminutesbeforestart.md) для определения времени отображения напоминания.</span><span class="sxs-lookup"><span data-stu-id="25d47-160">This is used by the [ReminderMinutesBeforeStart](reminderminutesbeforestart.md) element to determine when the reminder is displayed.</span></span>  <br/> |
|[<span data-ttu-id="25d47-161">реминдериссет</span><span class="sxs-lookup"><span data-stu-id="25d47-161">ReminderIsSet</span></span>](reminderisset.md) <br/> |<span data-ttu-id="25d47-162">Указывает, задано ли напоминание для элемента в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="25d47-162">Indicates whether a reminder has been set for an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="25d47-163">ReminderMinutesBeforeStart</span><span class="sxs-lookup"><span data-stu-id="25d47-163">ReminderMinutesBeforeStart</span></span>](reminderminutesbeforestart.md) <br/> |<span data-ttu-id="25d47-164">Представляет количество минут до события при отображении напоминания.</span><span class="sxs-lookup"><span data-stu-id="25d47-164">Represents the number of minutes before an event when a reminder is displayed.</span></span>  <br/> |
|[<span data-ttu-id="25d47-165">дисплайкк</span><span class="sxs-lookup"><span data-stu-id="25d47-165">DisplayCc</span></span>](displaycc.md) <br/> |<span data-ttu-id="25d47-166">Представляет отображаемую строку, используемую для содержимого поля "копия".</span><span class="sxs-lookup"><span data-stu-id="25d47-166">Represents the display string that is used for the contents of the Cc box.</span></span> <span data-ttu-id="25d47-167">Это объединенная строка всех отображаемых имен получателей копии.</span><span class="sxs-lookup"><span data-stu-id="25d47-167">This is the concatenated string of all Cc recipient display names.</span></span>  <br/> |
|[<span data-ttu-id="25d47-168">дисплайто</span><span class="sxs-lookup"><span data-stu-id="25d47-168">DisplayTo</span></span>](displayto.md) <br/> |<span data-ttu-id="25d47-169">Представляет отображаемую строку, используемую для содержимого поля "Кому".</span><span class="sxs-lookup"><span data-stu-id="25d47-169">Represents the display string that is used for the contents of the To box.</span></span> <span data-ttu-id="25d47-170">Это объединенная строка для отображаемых имен получателей.</span><span class="sxs-lookup"><span data-stu-id="25d47-170">This is the concatenated string of all To recipient display names.</span></span>  <br/> |
|[<span data-ttu-id="25d47-171">HasAttachments</span><span class="sxs-lookup"><span data-stu-id="25d47-171">HasAttachments</span></span>](hasattachments.md) <br/> |<span data-ttu-id="25d47-172">Представляет свойство, для которого задано значение **true** , если элемент имеет по крайней мере одно видимое вложение.</span><span class="sxs-lookup"><span data-stu-id="25d47-172">Represents a property that is set to **true** if an item has at least one visible attachment.</span></span> <span data-ttu-id="25d47-173">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="25d47-173">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="25d47-174">ExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="25d47-174">ExtendedProperty</span></span>](extendedproperty.md) <br/> |<span data-ttu-id="25d47-175">Определяет расширенные свойства для папок и элементов.</span><span class="sxs-lookup"><span data-stu-id="25d47-175">Identifies extended properties on folders and items.</span></span>  <br/> |
|[<span data-ttu-id="25d47-176">Culture</span><span class="sxs-lookup"><span data-stu-id="25d47-176">Culture</span></span>](culture.md) <br/> |<span data-ttu-id="25d47-177">Представляет язык и региональные параметры для определенного элемента в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="25d47-177">Represents the culture for a given item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="25d47-178">ActualWork</span><span class="sxs-lookup"><span data-stu-id="25d47-178">ActualWork</span></span>](actualwork.md) <br/> |<span data-ttu-id="25d47-179">Представляет фактическое количество времени, затраченное на выполнение задачи.</span><span class="sxs-lookup"><span data-stu-id="25d47-179">Represents the actual amount of time that is spent on a task.</span></span>  <br/> |
|[<span data-ttu-id="25d47-180">ассигнедтиме</span><span class="sxs-lookup"><span data-stu-id="25d47-180">AssignedTime</span></span>](assignedtime.md) <br/> |<span data-ttu-id="25d47-181">Представляет время, когда задача назначена контакту.</span><span class="sxs-lookup"><span data-stu-id="25d47-181">Represents the time when a task is assigned to a contact.</span></span>  <br/> |
|[<span data-ttu-id="25d47-182">BillingInformation</span><span class="sxs-lookup"><span data-stu-id="25d47-182">BillingInformation</span></span>](billinginformation.md) <br/> |<span data-ttu-id="25d47-183">Содержит сведения о выставлении счетов для задачи.</span><span class="sxs-lookup"><span data-stu-id="25d47-183">Holds billing information for a task.</span></span>  <br/> |
|[<span data-ttu-id="25d47-184">чанжекаунт</span><span class="sxs-lookup"><span data-stu-id="25d47-184">ChangeCount</span></span>](changecount.md) <br/> |<span data-ttu-id="25d47-185">Указывает версию задачи.</span><span class="sxs-lookup"><span data-stu-id="25d47-185">Specifies the version of the task.</span></span>  <br/> |
|[<span data-ttu-id="25d47-186">Companies</span><span class="sxs-lookup"><span data-stu-id="25d47-186">Companies</span></span>](companies.md) <br/> |<span data-ttu-id="25d47-187">Представляет коллекцию компаний, связанных с контактом или задачей.</span><span class="sxs-lookup"><span data-stu-id="25d47-187">Represents the collection of companies that are associated with a contact or task.</span></span>  <br/> |
|[<span data-ttu-id="25d47-188">комплетедате</span><span class="sxs-lookup"><span data-stu-id="25d47-188">CompleteDate</span></span>](completedate.md) <br/> |<span data-ttu-id="25d47-189">Представляет дату завершения задачи.</span><span class="sxs-lookup"><span data-stu-id="25d47-189">Represents the date on which a task is completed.</span></span>  <br/> |
|[<span data-ttu-id="25d47-190">Контакты</span><span class="sxs-lookup"><span data-stu-id="25d47-190">Contacts</span></span>](contacts-ex15websvcsotherref.md) <br/> |<span data-ttu-id="25d47-191">Содержит список контактов, связанных с задачей.</span><span class="sxs-lookup"><span data-stu-id="25d47-191">Contains a list of contacts that are associated with a task.</span></span>  <br/> |
|[<span data-ttu-id="25d47-192">DelegationState</span><span class="sxs-lookup"><span data-stu-id="25d47-192">DelegationState</span></span>](delegationstate.md) <br/> |<span data-ttu-id="25d47-193">Представляет состояние делегированной задачи.</span><span class="sxs-lookup"><span data-stu-id="25d47-193">Represents the status of a delegated task.</span></span>  <br/> |
|[<span data-ttu-id="25d47-194">Delegator</span><span class="sxs-lookup"><span data-stu-id="25d47-194">Delegator</span></span>](delegator.md) <br/> |<span data-ttu-id="25d47-195">Содержит имя представителя, которому назначена задача.</span><span class="sxs-lookup"><span data-stu-id="25d47-195">Contains the name of the delegator who assigned the task.</span></span>  <br/> |
|[<span data-ttu-id="25d47-196">DueDate</span><span class="sxs-lookup"><span data-stu-id="25d47-196">DueDate</span></span>](duedate.md) <br/> |<span data-ttu-id="25d47-197">Представляет дату выполнения элемента задачи.</span><span class="sxs-lookup"><span data-stu-id="25d47-197">Represents the date when a task item is due.</span></span>  <br/> |
|[<span data-ttu-id="25d47-198">исассигнментедитабле</span><span class="sxs-lookup"><span data-stu-id="25d47-198">IsAssignmentEditable</span></span>](isassignmenteditable.md) <br/> |<span data-ttu-id="25d47-199">Указывает, является ли задача редактируемой.</span><span class="sxs-lookup"><span data-stu-id="25d47-199">Indicates whether the task is editable or not.</span></span>  <br/> |
|[<span data-ttu-id="25d47-200">Выполнение</span><span class="sxs-lookup"><span data-stu-id="25d47-200">IsComplete</span></span>](iscomplete.md) <br/> |<span data-ttu-id="25d47-201">Указывает, завершена ли задача.</span><span class="sxs-lookup"><span data-stu-id="25d47-201">Indicates whether the task has been completed or not.</span></span>  <br/> |
|[<span data-ttu-id="25d47-202">IsRecurring</span><span class="sxs-lookup"><span data-stu-id="25d47-202">IsRecurring</span></span>](isrecurring.md) <br/> |<span data-ttu-id="25d47-203">Указывает, является ли задача частью повторяющегося элемента.</span><span class="sxs-lookup"><span data-stu-id="25d47-203">Indicates whether a task is part of a recurring item.</span></span> <span data-ttu-id="25d47-204">Этот элемент доступен только для чтения.</span><span class="sxs-lookup"><span data-stu-id="25d47-204">This element is read-only.</span></span>  <br/> |
|[<span data-ttu-id="25d47-205">истеамтаск</span><span class="sxs-lookup"><span data-stu-id="25d47-205">IsTeamTask</span></span>](isteamtask.md) <br/> |<span data-ttu-id="25d47-206">Указывает, принадлежит ли задача группе или нет.</span><span class="sxs-lookup"><span data-stu-id="25d47-206">Indicates whether the task is owned by a team or not.</span></span>  <br/> |
|[<span data-ttu-id="25d47-207">Mileage</span><span class="sxs-lookup"><span data-stu-id="25d47-207">Mileage</span></span>](mileage.md) <br/> |<span data-ttu-id="25d47-208">Представляет расстояние для элемента задачи.</span><span class="sxs-lookup"><span data-stu-id="25d47-208">Represents mileage for a task item.</span></span>  <br/> |
|[<span data-ttu-id="25d47-209">Owner</span><span class="sxs-lookup"><span data-stu-id="25d47-209">Owner</span></span>](owner.md) <br/> |<span data-ttu-id="25d47-210">Представляет владельца задачи.</span><span class="sxs-lookup"><span data-stu-id="25d47-210">Represents the owner of a task.</span></span>  <br/> |
|[<span data-ttu-id="25d47-211">PercentComplete</span><span class="sxs-lookup"><span data-stu-id="25d47-211">PercentComplete</span></span>](percentcomplete.md) <br/> |<span data-ttu-id="25d47-212">Описывает состояние выполнения задачи.</span><span class="sxs-lookup"><span data-stu-id="25d47-212">Describes the completion status of a task.</span></span>  <br/> |
|[<span data-ttu-id="25d47-213">Повторение (Таскрекурренцетипе)</span><span class="sxs-lookup"><span data-stu-id="25d47-213">Recurrence (TaskRecurrenceType)</span></span>](recurrence-taskrecurrencetype.md) <br/> |<span data-ttu-id="25d47-214">Содержит сведения о повторении для повторяющихся задач.</span><span class="sxs-lookup"><span data-stu-id="25d47-214">Contains recurrence information for recurring tasks.</span></span>  <br/> |
|[<span data-ttu-id="25d47-215">StartDate</span><span class="sxs-lookup"><span data-stu-id="25d47-215">StartDate</span></span>](startdate.md) <br/> |<span data-ttu-id="25d47-216">Представляет дату начала элемента задачи.</span><span class="sxs-lookup"><span data-stu-id="25d47-216">Represents the start date of a task item.</span></span>  <br/> |
|[<span data-ttu-id="25d47-217">Status</span><span class="sxs-lookup"><span data-stu-id="25d47-217">Status</span></span>](status.md) <br/> |<span data-ttu-id="25d47-218">Представляет состояние элемента задачи.</span><span class="sxs-lookup"><span data-stu-id="25d47-218">Represents the status of a task item.</span></span>  <br/> |
|[<span data-ttu-id="25d47-219">статусдескриптион</span><span class="sxs-lookup"><span data-stu-id="25d47-219">StatusDescription</span></span>](statusdescription.md) <br/> |<span data-ttu-id="25d47-220">Содержит описание состояния задачи.</span><span class="sxs-lookup"><span data-stu-id="25d47-220">Contains an explanation of the task status.</span></span>  <br/> |
|[<span data-ttu-id="25d47-221">TotalWork</span><span class="sxs-lookup"><span data-stu-id="25d47-221">TotalWork</span></span>](totalwork.md) <br/> |<span data-ttu-id="25d47-222">Содержит описание объема работы, связанного с элементом.</span><span class="sxs-lookup"><span data-stu-id="25d47-222">Contains a description of how much work is associated with an item.</span></span>  <br/> |
|[<span data-ttu-id="25d47-223">еффективеригхтс</span><span class="sxs-lookup"><span data-stu-id="25d47-223">EffectiveRights</span></span>](effectiverights.md) <br/> |<span data-ttu-id="25d47-224">Содержит права клиента на основе параметров разрешений для элемента или папки.</span><span class="sxs-lookup"><span data-stu-id="25d47-224">Contains the rights of the client based on the permission settings for the item or folder.</span></span> <span data-ttu-id="25d47-225">Этот элемент доступен только для чтения.</span><span class="sxs-lookup"><span data-stu-id="25d47-225">This element is read-only.</span></span>  <br/> |
|[<span data-ttu-id="25d47-226">ластмодифиеднаме</span><span class="sxs-lookup"><span data-stu-id="25d47-226">LastModifiedName</span></span>](lastmodifiedname.md) <br/> |<span data-ttu-id="25d47-227">Содержит отображаемое имя последнего пользователя для изменения элемента.</span><span class="sxs-lookup"><span data-stu-id="25d47-227">Contains the display name of the last user to modify an item.</span></span>  <br/> |
|[<span data-ttu-id="25d47-228">LastModifiedTime</span><span class="sxs-lookup"><span data-stu-id="25d47-228">LastModifiedTime</span></span>](lastmodifiedtime.md) <br/> |<span data-ttu-id="25d47-229">Указывает время последнего изменения элемента.</span><span class="sxs-lookup"><span data-stu-id="25d47-229">Indicates when an item was last modified.</span></span>  <br/> |
|[<span data-ttu-id="25d47-230">Связанный</span><span class="sxs-lookup"><span data-stu-id="25d47-230">IsAssociated</span></span>](isassociated.md) <br/> |<span data-ttu-id="25d47-231">Указывает, связан ли элемент с папкой.</span><span class="sxs-lookup"><span data-stu-id="25d47-231">Indicates whether the item is associated with a folder.</span></span>  <br/> |
|[<span data-ttu-id="25d47-232">вебклиентреадформкуеристринг</span><span class="sxs-lookup"><span data-stu-id="25d47-232">WebClientReadFormQueryString</span></span>](webclientreadformquerystring.md) <br/> |<span data-ttu-id="25d47-233">Представляет URL-адрес для сцепления с конечной точкой Microsoft Office Outlook Web App для чтения элемента в Outlook Web App.</span><span class="sxs-lookup"><span data-stu-id="25d47-233">Represents a URL to concatenate to the Microsoft Office Outlook Web App endpoint to read an item in Outlook Web App.</span></span>  <br/> |
|[<span data-ttu-id="25d47-234">вебклиентедитформкуеристринг</span><span class="sxs-lookup"><span data-stu-id="25d47-234">WebClientEditFormQueryString</span></span>](webclienteditformquerystring.md) <br/> |<span data-ttu-id="25d47-235">Представляет URL-адрес для сцепления с конечной точкой Outlook Web App для изменения элемента в Outlook Web App.</span><span class="sxs-lookup"><span data-stu-id="25d47-235">Represents a URL to concatenate to the Outlook Web App endpoint to edit an item in Outlook Web App.</span></span>  <br/> |
|[<span data-ttu-id="25d47-236">ConversationId</span><span class="sxs-lookup"><span data-stu-id="25d47-236">ConversationId</span></span>](conversationid.md) <br/> |<span data-ttu-id="25d47-237">Содержит идентификатор элемента или беседы.</span><span class="sxs-lookup"><span data-stu-id="25d47-237">Contains the identifier of an item or conversation.</span></span>  <br/> |
|[<span data-ttu-id="25d47-238">UniqueBody</span><span class="sxs-lookup"><span data-stu-id="25d47-238">UniqueBody</span></span>](uniquebody.md) <br/> |<span data-ttu-id="25d47-239">Представляет фрагмент HTML или обычный текст, представляющий уникальный основной текст этой беседы.</span><span class="sxs-lookup"><span data-stu-id="25d47-239">Represents an HTML fragment or plain text which represents the unique body of this conversation.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="25d47-240">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="25d47-240">Parent elements</span></span>

|<span data-ttu-id="25d47-241">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="25d47-241">**Element**</span></span>|<span data-ttu-id="25d47-242">**Описание**</span><span class="sxs-lookup"><span data-stu-id="25d47-242">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="25d47-243">аджацентмитингс</span><span class="sxs-lookup"><span data-stu-id="25d47-243">AdjacentMeetings</span></span>](adjacentmeetings.md) <br/> |<span data-ttu-id="25d47-244">Описывает все элементы календаря, смежные с временем собрания.</span><span class="sxs-lookup"><span data-stu-id="25d47-244">Describes all calendar items that are adjacent to a meeting time.</span></span>  <br/> |
|[<span data-ttu-id="25d47-245">аппендтоитемфиелд</span><span class="sxs-lookup"><span data-stu-id="25d47-245">AppendToItemField</span></span>](appendtoitemfield.md) <br/> |<span data-ttu-id="25d47-246">Определяет данные, добавляемые в одно свойство элемента/папки во время [операции UpdateItem](updateitem-operation.md).</span><span class="sxs-lookup"><span data-stu-id="25d47-246">Identifies data to append to a single property of an item/folder during an [UpdateItem operation](updateitem-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="25d47-247">конфликтингмитингс</span><span class="sxs-lookup"><span data-stu-id="25d47-247">ConflictingMeetings</span></span>](conflictingmeetings.md) <br/> |<span data-ttu-id="25d47-248">Определяет все элементы, которые конфликтуют с временем собрания.</span><span class="sxs-lookup"><span data-stu-id="25d47-248">Identifies all items that conflict with a meeting time.</span></span>  <br/> |
|[<span data-ttu-id="25d47-249">Create (Итемсинк)</span><span class="sxs-lookup"><span data-stu-id="25d47-249">Create (ItemSync)</span></span>](create-itemsync.md) <br/> |<span data-ttu-id="25d47-250">Определяет один элемент, который необходимо создать в локальном хранилище клиента.</span><span class="sxs-lookup"><span data-stu-id="25d47-250">Identifies a single item to create in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="25d47-251">ItemAttachment</span><span class="sxs-lookup"><span data-stu-id="25d47-251">ItemAttachment</span></span>](itemattachment.md) <br/> |<span data-ttu-id="25d47-252">Представляет элемент Exchange, присоединенный к другому элементу Exchange.</span><span class="sxs-lookup"><span data-stu-id="25d47-252">Represents an Exchange item that is attached to another Exchange item.</span></span>  <br/> |
|[<span data-ttu-id="25d47-253">Items</span><span class="sxs-lookup"><span data-stu-id="25d47-253">Items</span></span>](items.md) <br/> |<span data-ttu-id="25d47-254">Содержит массив элементов.</span><span class="sxs-lookup"><span data-stu-id="25d47-254">Contains an array of items.</span></span>  <br/> |
|[<span data-ttu-id="25d47-255">сетитемфиелд</span><span class="sxs-lookup"><span data-stu-id="25d47-255">SetItemField</span></span>](setitemfield.md) <br/> |<span data-ttu-id="25d47-256">Представляет обновление одного свойства элемента в [операции UpdateItem](updateitem-operation.md).</span><span class="sxs-lookup"><span data-stu-id="25d47-256">Represents an update to a single property of an item in an [UpdateItem operation](updateitem-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="25d47-257">Обновление (Итемсинк)</span><span class="sxs-lookup"><span data-stu-id="25d47-257">Update (ItemSync)</span></span>](update-itemsync.md) <br/> |<span data-ttu-id="25d47-258">Определяет один элемент для обновления в локальном хранилище клиента.</span><span class="sxs-lookup"><span data-stu-id="25d47-258">Identifies a single item to update in the local client store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="25d47-259">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="25d47-259">Text value</span></span>

<span data-ttu-id="25d47-260">Нет.</span><span class="sxs-lookup"><span data-stu-id="25d47-260">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="25d47-261">Примечания</span><span class="sxs-lookup"><span data-stu-id="25d47-261">Remarks</span></span>

<span data-ttu-id="25d47-262">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="25d47-262">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="25d47-263">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="25d47-263">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="25d47-264">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="25d47-264">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="25d47-265">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="25d47-265">Schema name</span></span>  <br/> |<span data-ttu-id="25d47-266">Схема Types</span><span class="sxs-lookup"><span data-stu-id="25d47-266">Types schema</span></span>  <br/> |
|<span data-ttu-id="25d47-267">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="25d47-267">Validation file</span></span>  <br/> |<span data-ttu-id="25d47-268">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="25d47-268">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="25d47-269">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="25d47-269">Can be empty</span></span>  <br/> |<span data-ttu-id="25d47-270">False</span><span class="sxs-lookup"><span data-stu-id="25d47-270">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="25d47-271">См. также</span><span class="sxs-lookup"><span data-stu-id="25d47-271">See also</span></span>

- [<span data-ttu-id="25d47-272">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="25d47-272">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="25d47-273">Создание задач</span><span class="sxs-lookup"><span data-stu-id="25d47-273">Creating Tasks</span></span>](https://msdn.microsoft.com/library/0ef97334-e8a0-4f67-a23a-dd9e2bbad49f%28Office.15%29.aspx)
- [<span data-ttu-id="25d47-274">Удаление задач</span><span class="sxs-lookup"><span data-stu-id="25d47-274">Deleting Tasks</span></span>](https://msdn.microsoft.com/library/a3d7e25f-8a35-4901-b1d9-d31f418ab340%28Office.15%29.aspx)

