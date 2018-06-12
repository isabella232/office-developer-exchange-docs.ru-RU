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
description: Элемент задачи представляет задачу в хранилище Exchange.
ms.openlocfilehash: 2c61fca6ac85290e34f1365b0cb9e841e1fe279f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19840143"
---
# <a name="task"></a><span data-ttu-id="f5fa5-103">Задача</span><span class="sxs-lookup"><span data-stu-id="f5fa5-103">Task</span></span>

<span data-ttu-id="f5fa5-104">Элемент **задачи** представляет задачу в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="f5fa5-104">The **Task** element represents a task in the Exchange store.</span></span> 
  
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

<span data-ttu-id="f5fa5-105">**Тип задачи**</span><span class="sxs-lookup"><span data-stu-id="f5fa5-105">**TaskType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="f5fa5-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="f5fa5-106">Attributes and elements</span></span>

<span data-ttu-id="f5fa5-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="f5fa5-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f5fa5-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="f5fa5-108">Attributes</span></span>

<span data-ttu-id="f5fa5-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="f5fa5-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f5fa5-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="f5fa5-110">Child elements</span></span>

|<span data-ttu-id="f5fa5-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="f5fa5-111">**Element**</span></span>|<span data-ttu-id="f5fa5-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="f5fa5-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f5fa5-113">MimeContent</span><span class="sxs-lookup"><span data-stu-id="f5fa5-113">MimeContent</span></span>](mimecontent.md) <br/> |<span data-ttu-id="f5fa5-114">Содержит собственный поток Multipurpose Internet Mail Extensions (MIME), представленного в формате base64Binary объекта.</span><span class="sxs-lookup"><span data-stu-id="f5fa5-114">Contains the native Multipurpose Internet Mail Extensions (MIME) stream of an object that is represented in base64Binary format.</span></span>  <br/> |
|[<span data-ttu-id="f5fa5-115">Идентификатор элемента</span><span class="sxs-lookup"><span data-stu-id="f5fa5-115">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="f5fa5-116">Содержит уникальный идентификатор и меняет ключ элемента в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="f5fa5-116">Contains the unique identifier and change key of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="f5fa5-117">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="f5fa5-117">ParentFolderId</span></span>](parentfolderid.md) <br/> |<span data-ttu-id="f5fa5-118">Представляет идентификатор родительской папки, содержащей элемент или папку.</span><span class="sxs-lookup"><span data-stu-id="f5fa5-118">Represents the identifier of the parent folder that contains the item or folder.</span></span>  <br/> |
|[<span data-ttu-id="f5fa5-119">ItemClass</span><span class="sxs-lookup"><span data-stu-id="f5fa5-119">ItemClass</span></span>](itemclass.md) <br/> |<span data-ttu-id="f5fa5-120">Представляет класс сообщения элемента.</span><span class="sxs-lookup"><span data-stu-id="f5fa5-120">Represents the message class of an item.</span></span>  <br/> |
|[<span data-ttu-id="f5fa5-121">Subject</span><span class="sxs-lookup"><span data-stu-id="f5fa5-121">Subject</span></span>](subject.md) <br/> |<span data-ttu-id="f5fa5-122">Представляет тему для элементов хранилища Exchange и объекты ответа.</span><span class="sxs-lookup"><span data-stu-id="f5fa5-122">Represents the subject for Exchange store items and response objects.</span></span>  <br/> |
|[<span data-ttu-id="f5fa5-123">Уровень конфиденциальности сообщения</span><span class="sxs-lookup"><span data-stu-id="f5fa5-123">Sensitivity</span></span>](sensitivity.md) <br/> |<span data-ttu-id="f5fa5-124">Содержит сведения о состоянии уровень конфиденциальности сообщения элемента.</span><span class="sxs-lookup"><span data-stu-id="f5fa5-124">Contains the status for an item's sensitivity.</span></span>  <br/> |
|[<span data-ttu-id="f5fa5-125">Body</span><span class="sxs-lookup"><span data-stu-id="f5fa5-125">Body</span></span>](body.md) <br/> |<span data-ttu-id="f5fa5-126">Представляет фактическое содержимое основного текста сообщения.</span><span class="sxs-lookup"><span data-stu-id="f5fa5-126">Represents the actual body content of a message.</span></span>  <br/> |
|[<span data-ttu-id="f5fa5-127">Вложения</span><span class="sxs-lookup"><span data-stu-id="f5fa5-127">Attachments</span></span>](attachments-ex15websvcsotherref.md) <br/> |<span data-ttu-id="f5fa5-128">Содержит элементы или файлы, подключенные к элементу в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="f5fa5-128">Contains the items or files that are attached to an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="f5fa5-129">DateTimeReceived</span><span class="sxs-lookup"><span data-stu-id="f5fa5-129">DateTimeReceived</span></span>](datetimereceived.md) <br/> |<span data-ttu-id="f5fa5-130">Представляет дату и время получения элемента в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="f5fa5-130">Represents the date and time that an item in a mailbox was received.</span></span>  <br/> |
|[<span data-ttu-id="f5fa5-131">Размер</span><span class="sxs-lookup"><span data-stu-id="f5fa5-131">Size</span></span>](size.md) <br/> |<span data-ttu-id="f5fa5-132">Представляет размер в байтах, элемента.</span><span class="sxs-lookup"><span data-stu-id="f5fa5-132">Represents the size, in bytes, of an item.</span></span> <span data-ttu-id="f5fa5-133">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f5fa5-133">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="f5fa5-134">Категории</span><span class="sxs-lookup"><span data-stu-id="f5fa5-134">Categories</span></span>](categories-ex15websvcsotherref.md) <br/> |<span data-ttu-id="f5fa5-135">Представляет набор строк, чтобы указать, к какой категории относится элемент в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="f5fa5-135">Represents a collection of strings that identify to which categories an item in the mailbox belongs.</span></span>  <br/> |
|[<span data-ttu-id="f5fa5-136">Важность</span><span class="sxs-lookup"><span data-stu-id="f5fa5-136">Importance</span></span>](importance.md) <br/> |<span data-ttu-id="f5fa5-137">Описывает важность элемента.</span><span class="sxs-lookup"><span data-stu-id="f5fa5-137">Describes the importance of an item.</span></span>  <br/> |
|[<span data-ttu-id="f5fa5-138">InReplyTo</span><span class="sxs-lookup"><span data-stu-id="f5fa5-138">InReplyTo</span></span>](inreplyto.md) <br/> |<span data-ttu-id="f5fa5-139">Представляет идентификатор элемента, к которому этот элемент является ее в ответ.</span><span class="sxs-lookup"><span data-stu-id="f5fa5-139">Represents the identifier of the item to which this item is a reply.</span></span>  <br/> |
|[<span data-ttu-id="f5fa5-140">IsSubmitted</span><span class="sxs-lookup"><span data-stu-id="f5fa5-140">IsSubmitted</span></span>](issubmitted.md) <br/> |<span data-ttu-id="f5fa5-141">Указывает, является ли элемент был отправлен исходящие папке по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="f5fa5-141">Indicates whether an item has been submitted to the Outbox default folder.</span></span>  <br/> |
|[<span data-ttu-id="f5fa5-142">IsDraft</span><span class="sxs-lookup"><span data-stu-id="f5fa5-142">IsDraft</span></span>](isdraft.md) <br/> |<span data-ttu-id="f5fa5-143">Представляет ли элемент еще не были отправлены.</span><span class="sxs-lookup"><span data-stu-id="f5fa5-143">Represents whether an item has not yet been sent.</span></span>  <br/> |
|[<span data-ttu-id="f5fa5-144">IsFromMe</span><span class="sxs-lookup"><span data-stu-id="f5fa5-144">IsFromMe</span></span>](isfromme.md) <br/> |<span data-ttu-id="f5fa5-145">Указывает, отправил ли пользователь элемента для его сами себя.</span><span class="sxs-lookup"><span data-stu-id="f5fa5-145">Indicates whether a user sent an item to him or herself.</span></span>  <br/> |
|[<span data-ttu-id="f5fa5-146">IsResend</span><span class="sxs-lookup"><span data-stu-id="f5fa5-146">IsResend</span></span>](isresend.md) <br/> |<span data-ttu-id="f5fa5-147">Указывает, является ли элемент ранее еще был отправлен.</span><span class="sxs-lookup"><span data-stu-id="f5fa5-147">Indicates whether the item had previously been sent.</span></span>  <br/> |
|[<span data-ttu-id="f5fa5-148">IsUnmodified</span><span class="sxs-lookup"><span data-stu-id="f5fa5-148">IsUnmodified</span></span>](isunmodified.md) <br/> |<span data-ttu-id="f5fa5-149">Указывает, были ли изменены элемента.</span><span class="sxs-lookup"><span data-stu-id="f5fa5-149">Indicates whether the item has been modified.</span></span>  <br/> |
|[<span data-ttu-id="f5fa5-150">InternetMessageHeaders</span><span class="sxs-lookup"><span data-stu-id="f5fa5-150">InternetMessageHeaders</span></span>](internetmessageheaders.md) <br/> |<span data-ttu-id="f5fa5-151">Представляет коллекцию всех заголовков сообщений Интернета, содержащихся в элемента в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="f5fa5-151">Represents the collection of all Internet message headers that are contained in an item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="f5fa5-152">DateTimeSent</span><span class="sxs-lookup"><span data-stu-id="f5fa5-152">DateTimeSent</span></span>](datetimesent.md) <br/> |<span data-ttu-id="f5fa5-153">Представляет дату и время отправки элемента в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="f5fa5-153">Represents the date and time that an item in a mailbox was sent.</span></span>  <br/> |
|[<span data-ttu-id="f5fa5-154">DateTimeCreated</span><span class="sxs-lookup"><span data-stu-id="f5fa5-154">DateTimeCreated</span></span>](datetimecreated.md) <br/> |<span data-ttu-id="f5fa5-155">Представляет дату и время создания данного элемента в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="f5fa5-155">Represents the date and time that a given item in the mailbox was created.</span></span>  <br/> |
|[<span data-ttu-id="f5fa5-156">ResponseObjects</span><span class="sxs-lookup"><span data-stu-id="f5fa5-156">ResponseObjects</span></span>](responseobjects.md) <br/> |<span data-ttu-id="f5fa5-157">Содержит коллекцию всех объектов ответа, которые связаны с элемента в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="f5fa5-157">Contains a collection of all the response objects that are associated with an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="f5fa5-158">ReminderDueBy</span><span class="sxs-lookup"><span data-stu-id="f5fa5-158">ReminderDueBy</span></span>](reminderdueby.md) <br/> |<span data-ttu-id="f5fa5-159">Представляет дату и время, когда происходит событие.</span><span class="sxs-lookup"><span data-stu-id="f5fa5-159">Represents the date and time when the event occurs.</span></span> <span data-ttu-id="f5fa5-160">Используется в элементе [ReminderMinutesBeforeStart](reminderminutesbeforestart.md) определить, когда отображается оповещение.</span><span class="sxs-lookup"><span data-stu-id="f5fa5-160">This is used by the [ReminderMinutesBeforeStart](reminderminutesbeforestart.md) element to determine when the reminder is displayed.</span></span>  <br/> |
|[<span data-ttu-id="f5fa5-161">ReminderIsSet</span><span class="sxs-lookup"><span data-stu-id="f5fa5-161">ReminderIsSet</span></span>](reminderisset.md) <br/> |<span data-ttu-id="f5fa5-162">Указывает, установлен ли напоминания для элемента в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="f5fa5-162">Indicates whether a reminder has been set for an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="f5fa5-163">ReminderMinutesBeforeStart</span><span class="sxs-lookup"><span data-stu-id="f5fa5-163">ReminderMinutesBeforeStart</span></span>](reminderminutesbeforestart.md) <br/> |<span data-ttu-id="f5fa5-164">Представляет число минут и только потом событие, когда отображается напоминание.</span><span class="sxs-lookup"><span data-stu-id="f5fa5-164">Represents the number of minutes before an event when a reminder is displayed.</span></span>  <br/> |
|[<span data-ttu-id="f5fa5-165">DisplayCc</span><span class="sxs-lookup"><span data-stu-id="f5fa5-165">DisplayCc</span></span>](displaycc.md) <br/> |<span data-ttu-id="f5fa5-166">Строка отображения, который используется для содержимого в поле "Копия".</span><span class="sxs-lookup"><span data-stu-id="f5fa5-166">Represents the display string that is used for the contents of the Cc box.</span></span> <span data-ttu-id="f5fa5-167">Это составное строка всех получателей отображаемые имена «копия».</span><span class="sxs-lookup"><span data-stu-id="f5fa5-167">This is the concatenated string of all Cc recipient display names.</span></span>  <br/> |
|[<span data-ttu-id="f5fa5-168">DisplayTo</span><span class="sxs-lookup"><span data-stu-id="f5fa5-168">DisplayTo</span></span>](displayto.md) <br/> |<span data-ttu-id="f5fa5-169">Строка отображения, который используется для содержимого в поле «Кому».</span><span class="sxs-lookup"><span data-stu-id="f5fa5-169">Represents the display string that is used for the contents of the To box.</span></span> <span data-ttu-id="f5fa5-170">Это составное строка всех для получателей отображаемые имена.</span><span class="sxs-lookup"><span data-stu-id="f5fa5-170">This is the concatenated string of all To recipient display names.</span></span>  <br/> |
|[<span data-ttu-id="f5fa5-171">HasAttachments</span><span class="sxs-lookup"><span data-stu-id="f5fa5-171">HasAttachments</span></span>](hasattachments.md) <br/> |<span data-ttu-id="f5fa5-172">Представляет свойство, которое задано значение **true,** Если у элемента есть по крайней мере один видимым вложения.</span><span class="sxs-lookup"><span data-stu-id="f5fa5-172">Represents a property that is set to **true** if an item has at least one visible attachment.</span></span> <span data-ttu-id="f5fa5-173">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f5fa5-173">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="f5fa5-174">ExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="f5fa5-174">ExtendedProperty</span></span>](extendedproperty.md) <br/> |<span data-ttu-id="f5fa5-175">Определяет расширенные свойства для папок и элементов.</span><span class="sxs-lookup"><span data-stu-id="f5fa5-175">Identifies extended properties on folders and items.</span></span>  <br/> |
|[<span data-ttu-id="f5fa5-176">Язык и региональные параметры</span><span class="sxs-lookup"><span data-stu-id="f5fa5-176">Culture</span></span>](culture.md) <br/> |<span data-ttu-id="f5fa5-177">Представляет язык и региональные параметры для заданного элемента в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="f5fa5-177">Represents the culture for a given item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="f5fa5-178">ActualWork</span><span class="sxs-lookup"><span data-stu-id="f5fa5-178">ActualWork</span></span>](actualwork.md) <br/> |<span data-ttu-id="f5fa5-179">Представляет фактическое время, затраченное на задачи.</span><span class="sxs-lookup"><span data-stu-id="f5fa5-179">Represents the actual amount of time that is spent on a task.</span></span>  <br/> |
|[<span data-ttu-id="f5fa5-180">AssignedTime</span><span class="sxs-lookup"><span data-stu-id="f5fa5-180">AssignedTime</span></span>](assignedtime.md) <br/> |<span data-ttu-id="f5fa5-181">Представляет время, когда задача назначена контакта.</span><span class="sxs-lookup"><span data-stu-id="f5fa5-181">Represents the time when a task is assigned to a contact.</span></span>  <br/> |
|[<span data-ttu-id="f5fa5-182">BillingInformation</span><span class="sxs-lookup"><span data-stu-id="f5fa5-182">BillingInformation</span></span>](billinginformation.md) <br/> |<span data-ttu-id="f5fa5-183">Содержит сведения о задаче по выставлению счетов.</span><span class="sxs-lookup"><span data-stu-id="f5fa5-183">Holds billing information for a task.</span></span>  <br/> |
|[<span data-ttu-id="f5fa5-184">ChangeCount</span><span class="sxs-lookup"><span data-stu-id="f5fa5-184">ChangeCount</span></span>](changecount.md) <br/> |<span data-ttu-id="f5fa5-185">Указывает версию задачи.</span><span class="sxs-lookup"><span data-stu-id="f5fa5-185">Specifies the version of the task.</span></span>  <br/> |
|[<span data-ttu-id="f5fa5-186">Компании</span><span class="sxs-lookup"><span data-stu-id="f5fa5-186">Companies</span></span>](companies.md) <br/> |<span data-ttu-id="f5fa5-187">Представляет коллекцию компании, связанные с контактом или задач.</span><span class="sxs-lookup"><span data-stu-id="f5fa5-187">Represents the collection of companies that are associated with a contact or task.</span></span>  <br/> |
|[<span data-ttu-id="f5fa5-188">CompleteDate</span><span class="sxs-lookup"><span data-stu-id="f5fa5-188">CompleteDate</span></span>](completedate.md) <br/> |<span data-ttu-id="f5fa5-189">Представляет дату, на котором выполняются.</span><span class="sxs-lookup"><span data-stu-id="f5fa5-189">Represents the date on which a task is completed.</span></span>  <br/> |
|[<span data-ttu-id="f5fa5-190">Контакты</span><span class="sxs-lookup"><span data-stu-id="f5fa5-190">Contacts</span></span>](contacts-ex15websvcsotherref.md) <br/> |<span data-ttu-id="f5fa5-191">Содержит список контактов, связанных с задачей.</span><span class="sxs-lookup"><span data-stu-id="f5fa5-191">Contains a list of contacts that are associated with a task.</span></span>  <br/> |
|[<span data-ttu-id="f5fa5-192">DelegationState</span><span class="sxs-lookup"><span data-stu-id="f5fa5-192">DelegationState</span></span>](delegationstate.md) <br/> |<span data-ttu-id="f5fa5-193">Представляет состояние делегированные задачи.</span><span class="sxs-lookup"><span data-stu-id="f5fa5-193">Represents the status of a delegated task.</span></span>  <br/> |
|[<span data-ttu-id="f5fa5-194">Представитель</span><span class="sxs-lookup"><span data-stu-id="f5fa5-194">Delegator</span></span>](delegator.md) <br/> |<span data-ttu-id="f5fa5-195">Содержит имя сотрудника, назначена задача.</span><span class="sxs-lookup"><span data-stu-id="f5fa5-195">Contains the name of the delegator who assigned the task.</span></span>  <br/> |
|[<span data-ttu-id="f5fa5-196">DueDate</span><span class="sxs-lookup"><span data-stu-id="f5fa5-196">DueDate</span></span>](duedate.md) <br/> |<span data-ttu-id="f5fa5-197">Представляет дату, когда срок выполнения элемента задачи.</span><span class="sxs-lookup"><span data-stu-id="f5fa5-197">Represents the date when a task item is due.</span></span>  <br/> |
|[<span data-ttu-id="f5fa5-198">IsAssignmentEditable</span><span class="sxs-lookup"><span data-stu-id="f5fa5-198">IsAssignmentEditable</span></span>](isassignmenteditable.md) <br/> |<span data-ttu-id="f5fa5-199">Указывает, является ли задача редактирования.</span><span class="sxs-lookup"><span data-stu-id="f5fa5-199">Indicates whether the task is editable or not.</span></span>  <br/> |
|[<span data-ttu-id="f5fa5-200">IsComplete</span><span class="sxs-lookup"><span data-stu-id="f5fa5-200">IsComplete</span></span>](iscomplete.md) <br/> |<span data-ttu-id="f5fa5-201">Указывает, была выполнена ли задача или нет.</span><span class="sxs-lookup"><span data-stu-id="f5fa5-201">Indicates whether the task has been completed or not.</span></span>  <br/> |
|[<span data-ttu-id="f5fa5-202">IsRecurring</span><span class="sxs-lookup"><span data-stu-id="f5fa5-202">IsRecurring</span></span>](isrecurring.md) <br/> |<span data-ttu-id="f5fa5-203">Указывает, является ли задача частью повторяющегося элемента.</span><span class="sxs-lookup"><span data-stu-id="f5fa5-203">Indicates whether a task is part of a recurring item.</span></span> <span data-ttu-id="f5fa5-204">Этот элемент доступен только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f5fa5-204">This element is read-only.</span></span>  <br/> |
|[<span data-ttu-id="f5fa5-205">IsTeamTask</span><span class="sxs-lookup"><span data-stu-id="f5fa5-205">IsTeamTask</span></span>](isteamtask.md) <br/> |<span data-ttu-id="f5fa5-206">Указывает, принадлежит ли задача группой.</span><span class="sxs-lookup"><span data-stu-id="f5fa5-206">Indicates whether the task is owned by a team or not.</span></span>  <br/> |
|[<span data-ttu-id="f5fa5-207">Расстояние</span><span class="sxs-lookup"><span data-stu-id="f5fa5-207">Mileage</span></span>](mileage.md) <br/> |<span data-ttu-id="f5fa5-208">Представляет расстояние для элемента задачи.</span><span class="sxs-lookup"><span data-stu-id="f5fa5-208">Represents mileage for a task item.</span></span>  <br/> |
|[<span data-ttu-id="f5fa5-209">Владелец</span><span class="sxs-lookup"><span data-stu-id="f5fa5-209">Owner</span></span>](owner.md) <br/> |<span data-ttu-id="f5fa5-210">Представляет владельца задачи.</span><span class="sxs-lookup"><span data-stu-id="f5fa5-210">Represents the owner of a task.</span></span>  <br/> |
|[<span data-ttu-id="f5fa5-211">PercentComplete</span><span class="sxs-lookup"><span data-stu-id="f5fa5-211">PercentComplete</span></span>](percentcomplete.md) <br/> |<span data-ttu-id="f5fa5-212">Описание состояния завершения задания.</span><span class="sxs-lookup"><span data-stu-id="f5fa5-212">Describes the completion status of a task.</span></span>  <br/> |
|[<span data-ttu-id="f5fa5-213">Повторение (TaskRecurrenceType)</span><span class="sxs-lookup"><span data-stu-id="f5fa5-213">Recurrence (TaskRecurrenceType)</span></span>](recurrence-taskrecurrencetype.md) <br/> |<span data-ttu-id="f5fa5-214">Содержит данные о повторении для повторяющихся задач.</span><span class="sxs-lookup"><span data-stu-id="f5fa5-214">Contains recurrence information for recurring tasks.</span></span>  <br/> |
|[<span data-ttu-id="f5fa5-215">Дата начала</span><span class="sxs-lookup"><span data-stu-id="f5fa5-215">StartDate</span></span>](startdate.md) <br/> |<span data-ttu-id="f5fa5-216">Представляет дату начала элемента задачи.</span><span class="sxs-lookup"><span data-stu-id="f5fa5-216">Represents the start date of a task item.</span></span>  <br/> |
|[<span data-ttu-id="f5fa5-217">Состояние</span><span class="sxs-lookup"><span data-stu-id="f5fa5-217">Status</span></span>](status.md) <br/> |<span data-ttu-id="f5fa5-218">Представляет состояние элемента задачи.</span><span class="sxs-lookup"><span data-stu-id="f5fa5-218">Represents the status of a task item.</span></span>  <br/> |
|[<span data-ttu-id="f5fa5-219">StatusDescription</span><span class="sxs-lookup"><span data-stu-id="f5fa5-219">StatusDescription</span></span>](statusdescription.md) <br/> |<span data-ttu-id="f5fa5-220">Содержит описание состояния задачи.</span><span class="sxs-lookup"><span data-stu-id="f5fa5-220">Contains an explanation of the task status.</span></span>  <br/> |
|[<span data-ttu-id="f5fa5-221">TotalWork</span><span class="sxs-lookup"><span data-stu-id="f5fa5-221">TotalWork</span></span>](totalwork.md) <br/> |<span data-ttu-id="f5fa5-222">Содержит описание объем работы связан с элементом.</span><span class="sxs-lookup"><span data-stu-id="f5fa5-222">Contains a description of how much work is associated with an item.</span></span>  <br/> |
|[<span data-ttu-id="f5fa5-223">EffectiveRights</span><span class="sxs-lookup"><span data-stu-id="f5fa5-223">EffectiveRights</span></span>](effectiverights.md) <br/> |<span data-ttu-id="f5fa5-224">Содержит правами клиент, построенный на параметры разрешений для элемента или папки.</span><span class="sxs-lookup"><span data-stu-id="f5fa5-224">Contains the rights of the client based on the permission settings for the item or folder.</span></span> <span data-ttu-id="f5fa5-225">Этот элемент доступен только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f5fa5-225">This element is read-only.</span></span>  <br/> |
|[<span data-ttu-id="f5fa5-226">LastModifiedName</span><span class="sxs-lookup"><span data-stu-id="f5fa5-226">LastModifiedName</span></span>](lastmodifiedname.md) <br/> |<span data-ttu-id="f5fa5-227">Содержит отображаемое имя последнего пользователя, чтобы изменить элемент.</span><span class="sxs-lookup"><span data-stu-id="f5fa5-227">Contains the display name of the last user to modify an item.</span></span>  <br/> |
|[<span data-ttu-id="f5fa5-228">LastModifiedTime</span><span class="sxs-lookup"><span data-stu-id="f5fa5-228">LastModifiedTime</span></span>](lastmodifiedtime.md) <br/> |<span data-ttu-id="f5fa5-229">Указывает время последнего изменения элемента.</span><span class="sxs-lookup"><span data-stu-id="f5fa5-229">Indicates when an item was last modified.</span></span>  <br/> |
|[<span data-ttu-id="f5fa5-230">IsAssociated</span><span class="sxs-lookup"><span data-stu-id="f5fa5-230">IsAssociated</span></span>](isassociated.md) <br/> |<span data-ttu-id="f5fa5-231">Указывает, является ли элемент связан с папкой.</span><span class="sxs-lookup"><span data-stu-id="f5fa5-231">Indicates whether the item is associated with a folder.</span></span>  <br/> |
|[<span data-ttu-id="f5fa5-232">WebClientReadFormQueryString</span><span class="sxs-lookup"><span data-stu-id="f5fa5-232">WebClientReadFormQueryString</span></span>](webclientreadformquerystring.md) <br/> |<span data-ttu-id="f5fa5-233">Представляет URL-адрес для присоединения к конечной точке Microsoft Office Outlook Web App для чтения элемента в Outlook Web App.</span><span class="sxs-lookup"><span data-stu-id="f5fa5-233">Represents a URL to concatenate to the Microsoft Office Outlook Web App endpoint to read an item in Outlook Web App.</span></span>  <br/> |
|[<span data-ttu-id="f5fa5-234">WebClientEditFormQueryString</span><span class="sxs-lookup"><span data-stu-id="f5fa5-234">WebClientEditFormQueryString</span></span>](webclienteditformquerystring.md) <br/> |<span data-ttu-id="f5fa5-235">Представляет URL-адрес для объединения в конечную точку Outlook Web App для редактирования элемента в Outlook Web App.</span><span class="sxs-lookup"><span data-stu-id="f5fa5-235">Represents a URL to concatenate to the Outlook Web App endpoint to edit an item in Outlook Web App.</span></span>  <br/> |
|[<span data-ttu-id="f5fa5-236">ConversationId</span><span class="sxs-lookup"><span data-stu-id="f5fa5-236">ConversationId</span></span>](conversationid.md) <br/> |<span data-ttu-id="f5fa5-237">Содержит идентификатор элемента или беседы.</span><span class="sxs-lookup"><span data-stu-id="f5fa5-237">Contains the identifier of an item or conversation.</span></span>  <br/> |
|[<span data-ttu-id="f5fa5-238">UniqueBody</span><span class="sxs-lookup"><span data-stu-id="f5fa5-238">UniqueBody</span></span>](uniquebody.md) <br/> |<span data-ttu-id="f5fa5-239">Представляет фрагмент HTML или обычный текст, который представляет уникальное body эту беседу.</span><span class="sxs-lookup"><span data-stu-id="f5fa5-239">Represents an HTML fragment or plain text which represents the unique body of this conversation.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f5fa5-240">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="f5fa5-240">Parent elements</span></span>

|<span data-ttu-id="f5fa5-241">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="f5fa5-241">**Element**</span></span>|<span data-ttu-id="f5fa5-242">**Описание**</span><span class="sxs-lookup"><span data-stu-id="f5fa5-242">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f5fa5-243">AdjacentMeetings</span><span class="sxs-lookup"><span data-stu-id="f5fa5-243">AdjacentMeetings</span></span>](adjacentmeetings.md) <br/> |<span data-ttu-id="f5fa5-244">Описание всех элементов календаря, расположенных на время собрания.</span><span class="sxs-lookup"><span data-stu-id="f5fa5-244">Describes all calendar items that are adjacent to a meeting time.</span></span>  <br/> |
|[<span data-ttu-id="f5fa5-245">AppendToItemField</span><span class="sxs-lookup"><span data-stu-id="f5fa5-245">AppendToItemField</span></span>](appendtoitemfield.md) <br/> |<span data-ttu-id="f5fa5-246">Указывает данные для добавления к отдельное свойство item/папки во время [операции UpdateItem](updateitem-operation.md).</span><span class="sxs-lookup"><span data-stu-id="f5fa5-246">Identifies data to append to a single property of an item/folder during an [UpdateItem operation](updateitem-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="f5fa5-247">ConflictingMeetings</span><span class="sxs-lookup"><span data-stu-id="f5fa5-247">ConflictingMeetings</span></span>](conflictingmeetings.md) <br/> |<span data-ttu-id="f5fa5-248">Определяет все элементы, конфликтующие с время собрания.</span><span class="sxs-lookup"><span data-stu-id="f5fa5-248">Identifies all items that conflict with a meeting time.</span></span>  <br/> |
|[<span data-ttu-id="f5fa5-249">Создание (ItemSync)</span><span class="sxs-lookup"><span data-stu-id="f5fa5-249">Create (ItemSync)</span></span>](create-itemsync.md) <br/> |<span data-ttu-id="f5fa5-250">Определяет один элемент для создания в локальном хранилище клиента.</span><span class="sxs-lookup"><span data-stu-id="f5fa5-250">Identifies a single item to create in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="f5fa5-251">ItemAttachment</span><span class="sxs-lookup"><span data-stu-id="f5fa5-251">ItemAttachment</span></span>](itemattachment.md) <br/> |<span data-ttu-id="f5fa5-252">Представляет собой элемент Exchange, подключенный к другой элемент Exchange.</span><span class="sxs-lookup"><span data-stu-id="f5fa5-252">Represents an Exchange item that is attached to another Exchange item.</span></span>  <br/> |
|[<span data-ttu-id="f5fa5-253">Элементы</span><span class="sxs-lookup"><span data-stu-id="f5fa5-253">Items</span></span>](items.md) <br/> |<span data-ttu-id="f5fa5-254">Содержит массив элементов.</span><span class="sxs-lookup"><span data-stu-id="f5fa5-254">Contains an array of items.</span></span>  <br/> |
|[<span data-ttu-id="f5fa5-255">SetItemField</span><span class="sxs-lookup"><span data-stu-id="f5fa5-255">SetItemField</span></span>](setitemfield.md) <br/> |<span data-ttu-id="f5fa5-256">Представляет отдельное свойство элемента в [UpdateItem операции](updateitem-operation.md)обновления.</span><span class="sxs-lookup"><span data-stu-id="f5fa5-256">Represents an update to a single property of an item in an [UpdateItem operation](updateitem-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="f5fa5-257">Обновление (ItemSync)</span><span class="sxs-lookup"><span data-stu-id="f5fa5-257">Update (ItemSync)</span></span>](update-itemsync.md) <br/> |<span data-ttu-id="f5fa5-258">Определяет один элемент для обновления в локальном хранилище клиента.</span><span class="sxs-lookup"><span data-stu-id="f5fa5-258">Identifies a single item to update in the local client store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="f5fa5-259">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="f5fa5-259">Text value</span></span>

<span data-ttu-id="f5fa5-260">Нет.</span><span class="sxs-lookup"><span data-stu-id="f5fa5-260">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="f5fa5-261">Замечания</span><span class="sxs-lookup"><span data-stu-id="f5fa5-261">Remarks</span></span>

<span data-ttu-id="f5fa5-262">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="f5fa5-262">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f5fa5-263">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="f5fa5-263">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f5fa5-264">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="f5fa5-264">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="f5fa5-265">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="f5fa5-265">Schema name</span></span>  <br/> |<span data-ttu-id="f5fa5-266">Схема Types</span><span class="sxs-lookup"><span data-stu-id="f5fa5-266">Types schema</span></span>  <br/> |
|<span data-ttu-id="f5fa5-267">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="f5fa5-267">Validation file</span></span>  <br/> |<span data-ttu-id="f5fa5-268">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="f5fa5-268">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="f5fa5-269">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="f5fa5-269">Can be empty</span></span>  <br/> |<span data-ttu-id="f5fa5-270">False</span><span class="sxs-lookup"><span data-stu-id="f5fa5-270">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f5fa5-271">См. также</span><span class="sxs-lookup"><span data-stu-id="f5fa5-271">See also</span></span>

- [<span data-ttu-id="f5fa5-272">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="f5fa5-272">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="f5fa5-273">Создание задач</span><span class="sxs-lookup"><span data-stu-id="f5fa5-273">Creating Tasks</span></span>](http://msdn.microsoft.com/library/0ef97334-e8a0-4f67-a23a-dd9e2bbad49f%28Office.15%29.aspx)
- [<span data-ttu-id="f5fa5-274">Удаление задачи</span><span class="sxs-lookup"><span data-stu-id="f5fa5-274">Deleting Tasks</span></span>](http://msdn.microsoft.com/library/a3d7e25f-8a35-4901-b1d9-d31f418ab340%28Office.15%29.aspx)

