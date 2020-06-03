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
ms.openlocfilehash: 3bad638aa21019472df8f487f1e065d2e725e750
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465753"
---
# <a name="parentfolderid"></a><span data-ttu-id="65199-103">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="65199-103">ParentFolderId</span></span>

<span data-ttu-id="65199-104">Элемент **ParentFolderId** представляет идентификатор родительской папки, содержащей элемент или папку.</span><span class="sxs-lookup"><span data-stu-id="65199-104">The **ParentFolderId** element represents the identifier of the parent folder that contains the item or folder.</span></span> 
  
```XML
<ParentFolderId Id="" ChangeKey=""/>
```

<span data-ttu-id="65199-105">**фолдеридтипе**</span><span class="sxs-lookup"><span data-stu-id="65199-105">**FolderIdType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="65199-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="65199-106">Attributes and elements</span></span>

<span data-ttu-id="65199-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="65199-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="65199-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="65199-108">Attributes</span></span>

|<span data-ttu-id="65199-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="65199-109">**Attribute**</span></span>|<span data-ttu-id="65199-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="65199-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="65199-111">**Id**</span><span class="sxs-lookup"><span data-stu-id="65199-111">**Id**</span></span> <br/> |<span data-ttu-id="65199-112">Содержит строку, определяющую папку в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="65199-112">Contains a string that identifies a folder in the Exchange store.</span></span> <span data-ttu-id="65199-113">Этот атрибут является обязательным.</span><span class="sxs-lookup"><span data-stu-id="65199-113">This attribute is required.</span></span>  <br/> |
|<span data-ttu-id="65199-114">**чанжекэй**</span><span class="sxs-lookup"><span data-stu-id="65199-114">**ChangeKey**</span></span> <br/> |<span data-ttu-id="65199-115">Содержит строку, определяющую версию папки, определяемую атрибутом **ID** .</span><span class="sxs-lookup"><span data-stu-id="65199-115">Contains a string that identifies a version of a folder that is identified by the **Id** attribute.</span></span> <span data-ttu-id="65199-116">Этот атрибут является необязательным.</span><span class="sxs-lookup"><span data-stu-id="65199-116">This attribute is optional.</span></span> <span data-ttu-id="65199-117">Используйте этот атрибут, чтобы убедиться, что используется правильная версия папки.</span><span class="sxs-lookup"><span data-stu-id="65199-117">Use this attribute to make sure that the correct version of a folder is used.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="65199-118">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="65199-118">Child elements</span></span>

<span data-ttu-id="65199-119">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="65199-119">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="65199-120">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="65199-120">Parent elements</span></span>

|<span data-ttu-id="65199-121">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="65199-121">**Element**</span></span>|<span data-ttu-id="65199-122">**Описание**</span><span class="sxs-lookup"><span data-stu-id="65199-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="65199-123">календарфолдер</span><span class="sxs-lookup"><span data-stu-id="65199-123">CalendarFolder</span></span>](calendarfolder.md) <br/> |<span data-ttu-id="65199-124">Представляет папку "Календарь" в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="65199-124">Represents a calendar folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="65199-125">календаритем</span><span class="sxs-lookup"><span data-stu-id="65199-125">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="65199-126">Представляет элемент календаря в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="65199-126">Represents a calendar item in a mailbox.</span></span>  <br/> |
|<span data-ttu-id="65199-127">[контакт](contact.md);</span><span class="sxs-lookup"><span data-stu-id="65199-127">[Contact](contact.md)</span></span> <br/> |<span data-ttu-id="65199-128">Представляет элемент контакта в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="65199-128">Represents a contact item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="65199-129">контактсфолдер</span><span class="sxs-lookup"><span data-stu-id="65199-129">ContactsFolder</span></span>](contactsfolder.md) <br/> |<span data-ttu-id="65199-130">Представляет папку "Контакты" в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="65199-130">Represents a contacts folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="65199-131">копиедевент</span><span class="sxs-lookup"><span data-stu-id="65199-131">CopiedEvent</span></span>](copiedevent.md) <br/> |<span data-ttu-id="65199-132">Представляет событие, в котором копируется элемент или папка.</span><span class="sxs-lookup"><span data-stu-id="65199-132">Represents an event in which an item or folder is copied.</span></span>  <br/> |
|[<span data-ttu-id="65199-133">креатедевент</span><span class="sxs-lookup"><span data-stu-id="65199-133">CreatedEvent</span></span>](createdevent.md) <br/> |<span data-ttu-id="65199-134">Представляет событие, в котором создается элемент или папка.</span><span class="sxs-lookup"><span data-stu-id="65199-134">Represents an event in which an item or folder is created.</span></span>  <br/> |
|[<span data-ttu-id="65199-135">делетедевент</span><span class="sxs-lookup"><span data-stu-id="65199-135">DeletedEvent</span></span>](deletedevent.md) <br/> |<span data-ttu-id="65199-136">Представляет событие, в котором удаляется элемент или папка.</span><span class="sxs-lookup"><span data-stu-id="65199-136">Represents an event in which an item or folder is deleted.</span></span>  <br/> |
|[<span data-ttu-id="65199-137">дистрибутионлист</span><span class="sxs-lookup"><span data-stu-id="65199-137">DistributionList</span></span>](distributionlist.md) <br/> |<span data-ttu-id="65199-138">Представляет частный список рассылки в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="65199-138">Represents a private distribution list in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="65199-139">Folder</span><span class="sxs-lookup"><span data-stu-id="65199-139">Folder</span></span>](folder.md) <br/> |<span data-ttu-id="65199-140">Представляет папку в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="65199-140">Represents a folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="65199-141">Ресурс</span><span class="sxs-lookup"><span data-stu-id="65199-141">Item</span></span>](item.md) <br/> |<span data-ttu-id="65199-142">Представляет общий элемент Exchange.</span><span class="sxs-lookup"><span data-stu-id="65199-142">Represents a generic Exchange item.</span></span>  <br/> |
|[<span data-ttu-id="65199-143">Элемент (Уплоадитемтипе)</span><span class="sxs-lookup"><span data-stu-id="65199-143">Item (UploadItemType)</span></span>](item-uploaditemtype.md) <br/> |<span data-ttu-id="65199-144">Представляет отдельный элемент для отправки в почтовый ящик.</span><span class="sxs-lookup"><span data-stu-id="65199-144">Represents a single item to upload into a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="65199-145">митингканцеллатион</span><span class="sxs-lookup"><span data-stu-id="65199-145">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="65199-146">Представляет отмену собрания в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="65199-146">Represents a meeting cancellation in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="65199-147">митингмессаже</span><span class="sxs-lookup"><span data-stu-id="65199-147">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="65199-148">Представляет сообщение о собрании в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="65199-148">Represents a meeting message in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="65199-149">Свойство meetingrequest</span><span class="sxs-lookup"><span data-stu-id="65199-149">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="65199-150">Представляет приглашение на собрание в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="65199-150">Represents a meeting request in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="65199-151">митингреспонсе</span><span class="sxs-lookup"><span data-stu-id="65199-151">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="65199-152">Представляет ответ на приглашение на собрание в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="65199-152">Represents a meeting response in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="65199-153">Сообщение</span><span class="sxs-lookup"><span data-stu-id="65199-153">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="65199-154">Представляет сообщение электронной почты в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="65199-154">Represents an e-mail message in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="65199-155">модифиедевент</span><span class="sxs-lookup"><span data-stu-id="65199-155">ModifiedEvent</span></span>](modifiedevent.md) <br/> |<span data-ttu-id="65199-156">Представляет событие, в котором изменяется элемент или папка.</span><span class="sxs-lookup"><span data-stu-id="65199-156">Represents an event in which an item or folder is modified.</span></span>  <br/> |
|[<span data-ttu-id="65199-157">моведевент</span><span class="sxs-lookup"><span data-stu-id="65199-157">MovedEvent</span></span>](movedevent.md) <br/> |<span data-ttu-id="65199-158">Представляет событие, в котором элемент или папка перемещаются из одной родительской папки в другую.</span><span class="sxs-lookup"><span data-stu-id="65199-158">Represents an event in which an item or folder is moved from one parent folder to another parent folder.</span></span>  <br/> |
|[<span data-ttu-id="65199-159">невмаилевент</span><span class="sxs-lookup"><span data-stu-id="65199-159">NewMailEvent</span></span>](newmailevent.md) <br/> |<span data-ttu-id="65199-160">Представляет событие, которое вызывается новым почтовым элементом в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="65199-160">Represents an event that is triggered by a new mail item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="65199-161">акцептитем</span><span class="sxs-lookup"><span data-stu-id="65199-161">AcceptItem</span></span>](acceptitem.md) <br/> |<span data-ttu-id="65199-162">Представляет ответ на принять приглашение на собрание.</span><span class="sxs-lookup"><span data-stu-id="65199-162">Represents an Accept reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="65199-163">тентативелякцептитем</span><span class="sxs-lookup"><span data-stu-id="65199-163">TentativelyAcceptItem</span></span>](tentativelyacceptitem.md) <br/> |<span data-ttu-id="65199-164">Представляет под вопросом ответ на приглашения на собрание.</span><span class="sxs-lookup"><span data-stu-id="65199-164">Represents a Tentative reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="65199-165">деклинеитем</span><span class="sxs-lookup"><span data-stu-id="65199-165">DeclineItem</span></span>](declineitem.md) <br/> |<span data-ttu-id="65199-166">Представляет отклонить ответ на приглашения на собрание.</span><span class="sxs-lookup"><span data-stu-id="65199-166">Represents a Decline reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="65199-167">RemoveItem</span><span class="sxs-lookup"><span data-stu-id="65199-167">RemoveItem</span></span>](removeitem.md) <br/> |<span data-ttu-id="65199-168">Удаляет элемент из хранилища Exchange.</span><span class="sxs-lookup"><span data-stu-id="65199-168">Removes an item from the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="65199-169">Task</span><span class="sxs-lookup"><span data-stu-id="65199-169">Task</span></span>](task.md) <br/> |<span data-ttu-id="65199-170">Представляет элемент задачи в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="65199-170">Represents a task item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="65199-171">реплитоитем</span><span class="sxs-lookup"><span data-stu-id="65199-171">ReplyToItem</span></span>](replytoitem.md) <br/> |<span data-ttu-id="65199-172">Содержит ответ создателем элемента в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="65199-172">Contains a reply to the creator of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="65199-173">репляллтоитем</span><span class="sxs-lookup"><span data-stu-id="65199-173">ReplyAllToItem</span></span>](replyalltoitem.md) <br/> |<span data-ttu-id="65199-174">Содержит ответить всем получателям определенного элемента в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="65199-174">Contains a reply to all identified recipients of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="65199-175">форвардитем</span><span class="sxs-lookup"><span data-stu-id="65199-175">ForwardItem</span></span>](forwarditem.md) <br/> |<span data-ttu-id="65199-176">Содержит элемент хранилища Exchange переадресация получателям.</span><span class="sxs-lookup"><span data-stu-id="65199-176">Contains an Exchange store item to forward to recipients.</span></span>  <br/> |
|[<span data-ttu-id="65199-177">канцелкалендаритем</span><span class="sxs-lookup"><span data-stu-id="65199-177">CancelCalendarItem</span></span>](cancelcalendaritem.md) <br/> |<span data-ttu-id="65199-178">Представляет объект ответа, которая используется для отмены собрания.</span><span class="sxs-lookup"><span data-stu-id="65199-178">Represents the response object that is used to cancel a meeting.</span></span>  <br/> |
|[<span data-ttu-id="65199-179">тасксфолдер</span><span class="sxs-lookup"><span data-stu-id="65199-179">TasksFolder</span></span>](tasksfolder.md) <br/> |<span data-ttu-id="65199-180">Представляет папку задач в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="65199-180">Represents a task folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="65199-181">SearchFolder</span><span class="sxs-lookup"><span data-stu-id="65199-181">SearchFolder</span></span>](searchfolder.md) <br/> |<span data-ttu-id="65199-182">Представляет папку поиска в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="65199-182">Represents a search folder in a mailbox.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="65199-183">Примечания</span><span class="sxs-lookup"><span data-stu-id="65199-183">Remarks</span></span>

<span data-ttu-id="65199-184">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="65199-184">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="65199-185">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="65199-185">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="65199-186">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="65199-186">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="65199-187">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="65199-187">Schema Name</span></span>  <br/> |<span data-ttu-id="65199-188">Схема Types</span><span class="sxs-lookup"><span data-stu-id="65199-188">Types schema</span></span>  <br/> |
|<span data-ttu-id="65199-189">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="65199-189">Validation File</span></span>  <br/> |<span data-ttu-id="65199-190">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="65199-190">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="65199-191">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="65199-191">Can be Empty</span></span>  <br/> |<span data-ttu-id="65199-192">False</span><span class="sxs-lookup"><span data-stu-id="65199-192">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="65199-193">См. также</span><span class="sxs-lookup"><span data-stu-id="65199-193">See also</span></span>

- [<span data-ttu-id="65199-194">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="65199-194">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

