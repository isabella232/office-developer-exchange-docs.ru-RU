---
title: ParentFolderId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ParentFolderId
api_type:
- schema
ms.assetid: 258f4b1f-367e-4c7d-9c29-eb775a2398c7
description: Элемент ParentFolderId представляет идентификатор родительской папки, содержащей элемент или папку.
ms.openlocfilehash: 3f60e8adb62fbf464a58af4169fbcd83910877cc
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19834687"
---
# <a name="parentfolderid"></a><span data-ttu-id="e068c-103">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="e068c-103">ParentFolderId</span></span>

<span data-ttu-id="e068c-104">Элемент **ParentFolderId** представляет идентификатор родительской папки, содержащей элемент или папку.</span><span class="sxs-lookup"><span data-stu-id="e068c-104">The **ParentFolderId** element represents the identifier of the parent folder that contains the item or folder.</span></span> 
  
```XML
<ParentFolderId Id="" ChangeKey=""/>
```

<span data-ttu-id="e068c-105">**FolderIdType**</span><span class="sxs-lookup"><span data-stu-id="e068c-105">**FolderIdType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="e068c-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="e068c-106">Attributes and elements</span></span>

<span data-ttu-id="e068c-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="e068c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e068c-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="e068c-108">Attributes</span></span>

|<span data-ttu-id="e068c-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="e068c-109">**Attribute**</span></span>|<span data-ttu-id="e068c-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="e068c-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="e068c-111">
  **Id**</span><span class="sxs-lookup"><span data-stu-id="e068c-111">**Id**</span></span> <br/> |<span data-ttu-id="e068c-112">Содержит строку, которая определяет папке в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="e068c-112">Contains a string that identifies a folder in the Exchange store.</span></span> <span data-ttu-id="e068c-113">Этот атрибут является обязательным.</span><span class="sxs-lookup"><span data-stu-id="e068c-113">This attribute is required.</span></span>  <br/> |
|<span data-ttu-id="e068c-114">**ChangeKey**</span><span class="sxs-lookup"><span data-stu-id="e068c-114">**ChangeKey**</span></span> <br/> |<span data-ttu-id="e068c-115">Содержит строку, которая определяет к папке, которая определена в атрибуте **Id** версии.</span><span class="sxs-lookup"><span data-stu-id="e068c-115">Contains a string that identifies a version of a folder that is identified by the **Id** attribute.</span></span> <span data-ttu-id="e068c-116">Этот атрибут является необязательным.</span><span class="sxs-lookup"><span data-stu-id="e068c-116">This attribute is optional.</span></span> <span data-ttu-id="e068c-117">Этот атрибут используется, чтобы убедиться в том, что используется правильный версии папки.</span><span class="sxs-lookup"><span data-stu-id="e068c-117">Use this attribute to make sure that the correct version of a folder is used.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="e068c-118">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="e068c-118">Child elements</span></span>

<span data-ttu-id="e068c-119">Нет.</span><span class="sxs-lookup"><span data-stu-id="e068c-119">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="e068c-120">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="e068c-120">Parent elements</span></span>

|<span data-ttu-id="e068c-121">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="e068c-121">**Element**</span></span>|<span data-ttu-id="e068c-122">**Описание**</span><span class="sxs-lookup"><span data-stu-id="e068c-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e068c-123">CalendarFolder</span><span class="sxs-lookup"><span data-stu-id="e068c-123">CalendarFolder</span></span>](calendarfolder.md) <br/> |<span data-ttu-id="e068c-124">Представляет папку Календарь в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="e068c-124">Represents a calendar folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="e068c-125">Элемента календаря, имеющего</span><span class="sxs-lookup"><span data-stu-id="e068c-125">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="e068c-126">Представляет элемент календаря в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="e068c-126">Represents a calendar item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="e068c-127">Контакт</span><span class="sxs-lookup"><span data-stu-id="e068c-127">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="e068c-128">Представляет контакт в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="e068c-128">Represents a contact item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="e068c-129">ContactsFolder</span><span class="sxs-lookup"><span data-stu-id="e068c-129">ContactsFolder</span></span>](contactsfolder.md) <br/> |<span data-ttu-id="e068c-130">Представляет папку контактов в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="e068c-130">Represents a contacts folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="e068c-131">CopiedEvent</span><span class="sxs-lookup"><span data-stu-id="e068c-131">CopiedEvent</span></span>](copiedevent.md) <br/> |<span data-ttu-id="e068c-132">Представляет событие, в котором копирование элемента или папки.</span><span class="sxs-lookup"><span data-stu-id="e068c-132">Represents an event in which an item or folder is copied.</span></span>  <br/> |
|[<span data-ttu-id="e068c-133">CreatedEvent</span><span class="sxs-lookup"><span data-stu-id="e068c-133">CreatedEvent</span></span>](createdevent.md) <br/> |<span data-ttu-id="e068c-134">Представляет событие, в котором создается элемента или папки.</span><span class="sxs-lookup"><span data-stu-id="e068c-134">Represents an event in which an item or folder is created.</span></span>  <br/> |
|[<span data-ttu-id="e068c-135">DeletedEvent</span><span class="sxs-lookup"><span data-stu-id="e068c-135">DeletedEvent</span></span>](deletedevent.md) <br/> |<span data-ttu-id="e068c-136">Представляет событие, в котором удаляется элемент или папку.</span><span class="sxs-lookup"><span data-stu-id="e068c-136">Represents an event in which an item or folder is deleted.</span></span>  <br/> |
|[<span data-ttu-id="e068c-137">DistributionList</span><span class="sxs-lookup"><span data-stu-id="e068c-137">DistributionList</span></span>](distributionlist.md) <br/> |<span data-ttu-id="e068c-138">Представляет список рассылки закрытый в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="e068c-138">Represents a private distribution list in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="e068c-139">Folder</span><span class="sxs-lookup"><span data-stu-id="e068c-139">Folder</span></span>](folder.md) <br/> |<span data-ttu-id="e068c-140">Представляет папку в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="e068c-140">Represents a folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="e068c-141">Элемент</span><span class="sxs-lookup"><span data-stu-id="e068c-141">Item</span></span>](item.md) <br/> |<span data-ttu-id="e068c-142">Представляет универсальный элемент Exchange.</span><span class="sxs-lookup"><span data-stu-id="e068c-142">Represents a generic Exchange item.</span></span>  <br/> |
|[<span data-ttu-id="e068c-143">Элемент (UploadItemType)</span><span class="sxs-lookup"><span data-stu-id="e068c-143">Item (UploadItemType)</span></span>](item-uploaditemtype.md) <br/> |<span data-ttu-id="e068c-144">Представляет один элемент для передачи в почтовый ящик.</span><span class="sxs-lookup"><span data-stu-id="e068c-144">Represents a single item to upload into a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="e068c-145">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="e068c-145">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="e068c-146">Представляет отмены собрания в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="e068c-146">Represents a meeting cancellation in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="e068c-147">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="e068c-147">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="e068c-148">Представляет сообщение собрания в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="e068c-148">Represents a meeting message in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="e068c-149">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="e068c-149">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="e068c-150">Представляет приглашения на собрание в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="e068c-150">Represents a meeting request in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="e068c-151">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="e068c-151">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="e068c-152">Представляет ответ на приглашение в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="e068c-152">Represents a meeting response in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="e068c-153">Message</span><span class="sxs-lookup"><span data-stu-id="e068c-153">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="e068c-154">Представляет сообщение электронной почты в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="e068c-154">Represents an e-mail message in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="e068c-155">ModifiedEvent</span><span class="sxs-lookup"><span data-stu-id="e068c-155">ModifiedEvent</span></span>](modifiedevent.md) <br/> |<span data-ttu-id="e068c-156">Представляет событие, в котором изменения элемента или папки.</span><span class="sxs-lookup"><span data-stu-id="e068c-156">Represents an event in which an item or folder is modified.</span></span>  <br/> |
|[<span data-ttu-id="e068c-157">MovedEvent</span><span class="sxs-lookup"><span data-stu-id="e068c-157">MovedEvent</span></span>](movedevent.md) <br/> |<span data-ttu-id="e068c-158">Представляет событие, в котором элемент или папка перемещаются из одной родительской папки в другую.</span><span class="sxs-lookup"><span data-stu-id="e068c-158">Represents an event in which an item or folder is moved from one parent folder to another parent folder.</span></span>  <br/> |
|[<span data-ttu-id="e068c-159">NewMailEvent</span><span class="sxs-lookup"><span data-stu-id="e068c-159">NewMailEvent</span></span>](newmailevent.md) <br/> |<span data-ttu-id="e068c-160">Представляет событие, которое инициируется нового элемента почты в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="e068c-160">Represents an event that is triggered by a new mail item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="e068c-161">AcceptItem</span><span class="sxs-lookup"><span data-stu-id="e068c-161">AcceptItem</span></span>](acceptitem.md) <br/> |<span data-ttu-id="e068c-162">Представляет ответ на принять приглашение на собрание.</span><span class="sxs-lookup"><span data-stu-id="e068c-162">Represents an Accept reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="e068c-163">TentativelyAcceptItem</span><span class="sxs-lookup"><span data-stu-id="e068c-163">TentativelyAcceptItem</span></span>](tentativelyacceptitem.md) <br/> |<span data-ttu-id="e068c-164">Представляет под вопросом ответ на приглашения на собрание.</span><span class="sxs-lookup"><span data-stu-id="e068c-164">Represents a Tentative reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="e068c-165">DeclineItem</span><span class="sxs-lookup"><span data-stu-id="e068c-165">DeclineItem</span></span>](declineitem.md) <br/> |<span data-ttu-id="e068c-166">Представляет отклонить ответ на приглашения на собрание.</span><span class="sxs-lookup"><span data-stu-id="e068c-166">Represents a Decline reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="e068c-167">RemoveItem</span><span class="sxs-lookup"><span data-stu-id="e068c-167">RemoveItem</span></span>](removeitem.md) <br/> |<span data-ttu-id="e068c-168">Удаляет элемент из хранилища Exchange.</span><span class="sxs-lookup"><span data-stu-id="e068c-168">Removes an item from the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="e068c-169">Задача</span><span class="sxs-lookup"><span data-stu-id="e068c-169">Task</span></span>](task.md) <br/> |<span data-ttu-id="e068c-170">Представляет элемент задачи в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="e068c-170">Represents a task item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="e068c-171">ReplyToItem</span><span class="sxs-lookup"><span data-stu-id="e068c-171">ReplyToItem</span></span>](replytoitem.md) <br/> |<span data-ttu-id="e068c-172">Содержит ответ создателем элемента в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="e068c-172">Contains a reply to the creator of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="e068c-173">ReplyAllToItem</span><span class="sxs-lookup"><span data-stu-id="e068c-173">ReplyAllToItem</span></span>](replyalltoitem.md) <br/> |<span data-ttu-id="e068c-174">Содержит ответить всем получателям определенного элемента в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="e068c-174">Contains a reply to all identified recipients of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="e068c-175">ForwardItem</span><span class="sxs-lookup"><span data-stu-id="e068c-175">ForwardItem</span></span>](forwarditem.md) <br/> |<span data-ttu-id="e068c-176">Содержит элемент хранилища Exchange переадресация получателям.</span><span class="sxs-lookup"><span data-stu-id="e068c-176">Contains an Exchange store item to forward to recipients.</span></span>  <br/> |
|[<span data-ttu-id="e068c-177">CancelCalendarItem</span><span class="sxs-lookup"><span data-stu-id="e068c-177">CancelCalendarItem</span></span>](cancelcalendaritem.md) <br/> |<span data-ttu-id="e068c-178">Представляет объект ответа, которая используется для отмены собрания.</span><span class="sxs-lookup"><span data-stu-id="e068c-178">Represents the response object that is used to cancel a meeting.</span></span>  <br/> |
|[<span data-ttu-id="e068c-179">TasksFolder</span><span class="sxs-lookup"><span data-stu-id="e068c-179">TasksFolder</span></span>](tasksfolder.md) <br/> |<span data-ttu-id="e068c-180">Представляет папку задач в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="e068c-180">Represents a task folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="e068c-181">SearchFolder</span><span class="sxs-lookup"><span data-stu-id="e068c-181">SearchFolder</span></span>](searchfolder.md) <br/> |<span data-ttu-id="e068c-182">Представляет папку поиска в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="e068c-182">Represents a search folder in a mailbox.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="e068c-183">Замечания</span><span class="sxs-lookup"><span data-stu-id="e068c-183">Remarks</span></span>

<span data-ttu-id="e068c-184">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="e068c-184">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e068c-185">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="e068c-185">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e068c-186">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="e068c-186">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="e068c-187">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="e068c-187">Schema Name</span></span>  <br/> |<span data-ttu-id="e068c-188">Схема Types</span><span class="sxs-lookup"><span data-stu-id="e068c-188">Types schema</span></span>  <br/> |
|<span data-ttu-id="e068c-189">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="e068c-189">Validation File</span></span>  <br/> |<span data-ttu-id="e068c-190">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="e068c-190">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="e068c-191">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="e068c-191">Can be Empty</span></span>  <br/> |<span data-ttu-id="e068c-192">False</span><span class="sxs-lookup"><span data-stu-id="e068c-192">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e068c-193">См. также</span><span class="sxs-lookup"><span data-stu-id="e068c-193">See also</span></span>

- [<span data-ttu-id="e068c-194">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="e068c-194">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

