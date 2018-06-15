---
title: UpdateItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UpdateItem
api_type:
- schema
ms.assetid: 34643d58-2743-45b0-a08d-bff6dc1da61d
description: Элемент UpdateItem определяет запрос на обновление элемента в почтовом ящике.
ms.openlocfilehash: 7b9b5f1dcffb95eb127572cb91f92d961c05a77e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/15/2018
ms.locfileid: "19840357"
---
# <a name="updateitem"></a><span data-ttu-id="d290b-103">UpdateItem</span><span class="sxs-lookup"><span data-stu-id="d290b-103">UpdateItem</span></span>

<span data-ttu-id="d290b-104">Элемент **UpdateItem** определяет запрос на обновление элемента в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="d290b-104">The **UpdateItem** element defines a request to update an item in a mailbox.</span></span> 
  
```XML
<UpdateItem ConflictResolution="" MessageDisposition="" SendMeetingInvitationsOrCancellations="" SuppressReadReceipts="">
   <SavedItemFolderId/>
   <ItemChanges/>
</UpdateItem>
```

 <span data-ttu-id="d290b-105">**UpdateItemType**</span><span class="sxs-lookup"><span data-stu-id="d290b-105">**UpdateItemType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d290b-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="d290b-106">Attributes and elements</span></span>

<span data-ttu-id="d290b-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="d290b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d290b-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="d290b-108">Attributes</span></span>

|<span data-ttu-id="d290b-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="d290b-109">**Attribute**</span></span>|<span data-ttu-id="d290b-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d290b-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="d290b-111">**ConflictResolution**</span><span class="sxs-lookup"><span data-stu-id="d290b-111">**ConflictResolution**</span></span> <br/> |<span data-ttu-id="d290b-112">Идентифицирует тип разрешения конфликтов попробовать во время обновления.</span><span class="sxs-lookup"><span data-stu-id="d290b-112">Identifies the type of conflict resolution to try during an update.</span></span> <span data-ttu-id="d290b-113">Значение по умолчанию — автоматическое разрешение.</span><span class="sxs-lookup"><span data-stu-id="d290b-113">The default value is AutoResolve.</span></span>  <br/> |
|<span data-ttu-id="d290b-114">**MessageDisposition**</span><span class="sxs-lookup"><span data-stu-id="d290b-114">**MessageDisposition**</span></span> <br/> |<span data-ttu-id="d290b-115">Описывает, как будут обрабатываться элемента после обновления.</span><span class="sxs-lookup"><span data-stu-id="d290b-115">Describes how the item will be handled after it is updated.</span></span> <span data-ttu-id="d290b-116">Атрибут **MessageDisposition** является обязательным для элементов сообщения, включая сообщения собрания, такие как отмен собрания, приглашений на собрания и ответы на приглашения.</span><span class="sxs-lookup"><span data-stu-id="d290b-116">The **MessageDisposition** attribute is required for message items, including meeting messages such as meeting cancellations, meeting requests, and meeting responses.</span></span>  <br/> |
|<span data-ttu-id="d290b-117">**SendMeetingInvitationsOrCancellations**</span><span class="sxs-lookup"><span data-stu-id="d290b-117">**SendMeetingInvitationsOrCancellations**</span></span> <br/> |<span data-ttu-id="d290b-118">Описывает, как собрание обновления передаются после обновления элемента календаря.</span><span class="sxs-lookup"><span data-stu-id="d290b-118">Describes how meeting updates are communicated after a calendar item is updated.</span></span> <span data-ttu-id="d290b-119">Этот атрибут является обязательным для элементов календаря и вхождения элемента календаря.</span><span class="sxs-lookup"><span data-stu-id="d290b-119">This attribute is required for calendar items and calendar item occurrences.</span></span>  <br/> |
|<span data-ttu-id="d290b-120">**SuppressReadReceipts**</span><span class="sxs-lookup"><span data-stu-id="d290b-120">**SuppressReadReceipts**</span></span> <br/> |<span data-ttu-id="d290b-121">Указывает, следует ли подавлять прочтении обновленного элемента.</span><span class="sxs-lookup"><span data-stu-id="d290b-121">Indicates whether read receipts for the updated item should be suppressed.</span></span> <span data-ttu-id="d290b-122">Текстовое значение **true,** указывает, что чтения, подавляются поступлений.</span><span class="sxs-lookup"><span data-stu-id="d290b-122">A text value of **true** indicates that read receipts should be suppressed.</span></span> <span data-ttu-id="d290b-123">Значение **false** указывает, что прочтении отправляются отправителю.</span><span class="sxs-lookup"><span data-stu-id="d290b-123">A value of **false** indicates that the read receipts will be sent to the sender.</span></span> <span data-ttu-id="d290b-124">Этот атрибут является необязательным.</span><span class="sxs-lookup"><span data-stu-id="d290b-124">This attribute is optional.</span></span>  <br/> <span data-ttu-id="d290b-125">Этот атрибут появился в Exchange Server 2013 с пакетом обновления 1.</span><span class="sxs-lookup"><span data-stu-id="d290b-125">This attribute was introduced in Exchange Server 2013 SP1.</span></span>  <br/> |
   
#### <a name="conflictresolution-attribute"></a><span data-ttu-id="d290b-126">Атрибут ConflictResolution</span><span class="sxs-lookup"><span data-stu-id="d290b-126">ConflictResolution Attribute</span></span>

|<span data-ttu-id="d290b-127">**Значение**</span><span class="sxs-lookup"><span data-stu-id="d290b-127">**Value**</span></span>|<span data-ttu-id="d290b-128">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d290b-128">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="d290b-129">NeverOverwrite</span><span class="sxs-lookup"><span data-stu-id="d290b-129">NeverOverwrite</span></span>  <br/> |<span data-ttu-id="d290b-130">Если происходит конфликт, происходит сбой операции обновления и возвращается сообщение об ошибке.</span><span class="sxs-lookup"><span data-stu-id="d290b-130">If there is a conflict, the update operation fails and an error is returned.</span></span>  <br/> |
|<span data-ttu-id="d290b-131">Автоматическое разрешение</span><span class="sxs-lookup"><span data-stu-id="d290b-131">AutoResolve</span></span>  <br/> |<span data-ttu-id="d290b-132">Операции обновления автоматически конфликты любой.</span><span class="sxs-lookup"><span data-stu-id="d290b-132">The update operation automatically resolves any conflict.</span></span>  <br/> |
|<span data-ttu-id="d290b-133">AlwaysOverwrite</span><span class="sxs-lookup"><span data-stu-id="d290b-133">AlwaysOverwrite</span></span>  <br/> |<span data-ttu-id="d290b-134">В случае конфликта операции обновления перезапишет данные.</span><span class="sxs-lookup"><span data-stu-id="d290b-134">If there is a conflict, the update operation will overwrite information.</span></span>  <br/> |
   
#### <a name="messagedisposition-attribute"></a><span data-ttu-id="d290b-135">Атрибут MessageDisposition</span><span class="sxs-lookup"><span data-stu-id="d290b-135">MessageDisposition Attribute</span></span>

|<span data-ttu-id="d290b-136">**Значение**</span><span class="sxs-lookup"><span data-stu-id="d290b-136">**Value**</span></span>|<span data-ttu-id="d290b-137">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d290b-137">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="d290b-138">SaveOnly</span><span class="sxs-lookup"><span data-stu-id="d290b-138">SaveOnly</span></span>  <br/> |<span data-ttu-id="d290b-139">Элемент обновлен и сохранения его текущей папки.</span><span class="sxs-lookup"><span data-stu-id="d290b-139">The item is updated and saved back to its current folder.</span></span>  <br/> |
|<span data-ttu-id="d290b-140">SendOnly</span><span class="sxs-lookup"><span data-stu-id="d290b-140">SendOnly</span></span>  <br/> |<span data-ttu-id="d290b-141">Элемент обновлен и отправляются, но копия не сохраняется.</span><span class="sxs-lookup"><span data-stu-id="d290b-141">The item is updated and sent but no copy is saved.</span></span>  <br/> |
|<span data-ttu-id="d290b-142">SendAndSaveCopy</span><span class="sxs-lookup"><span data-stu-id="d290b-142">SendAndSaveCopy</span></span>  <br/> |<span data-ttu-id="d290b-143">Элемент обновляется и копия сохраняется в папку, указанную в элементе [SavedItemFolderId](saveditemfolderid.md) .</span><span class="sxs-lookup"><span data-stu-id="d290b-143">The item is updated and a copy is saved in the folder identified by the [SavedItemFolderId](saveditemfolderid.md) element.</span></span>  <br/> |
   
#### <a name="sendmeetinginvitationsorcancellations-attribute"></a><span data-ttu-id="d290b-144">Атрибут SendMeetingInvitationsOrCancellations</span><span class="sxs-lookup"><span data-stu-id="d290b-144">SendMeetingInvitationsOrCancellations Attribute</span></span>

|<span data-ttu-id="d290b-145">**Значение**</span><span class="sxs-lookup"><span data-stu-id="d290b-145">**Value**</span></span>|<span data-ttu-id="d290b-146">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d290b-146">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="d290b-147">SendToNone</span><span class="sxs-lookup"><span data-stu-id="d290b-147">SendToNone</span></span>  <br/> |<span data-ttu-id="d290b-148">Обновление элемента календаря, но обновления не отправляются участникам.</span><span class="sxs-lookup"><span data-stu-id="d290b-148">The calendar item is updated but updates are not sent to attendees.</span></span>  <br/> |
|<span data-ttu-id="d290b-149">SendOnlyToAll</span><span class="sxs-lookup"><span data-stu-id="d290b-149">SendOnlyToAll</span></span>  <br/> |<span data-ttu-id="d290b-150">Обновлены элемента календаря и обновление собрания отправляется всех участников, но не сохраняются в папке «Отправленные».</span><span class="sxs-lookup"><span data-stu-id="d290b-150">The calendar item is updated and the meeting update is sent to all attendees but is not saved in the Sent Items folder.</span></span>  <br/> |
|<span data-ttu-id="d290b-151">SendOnlyToChanged</span><span class="sxs-lookup"><span data-stu-id="d290b-151">SendOnlyToChanged</span></span>  <br/> |<span data-ttu-id="d290b-152">Обновлены элемента календаря и обновление собрания отправляется только участникам, которые повлияет переход на собрании.</span><span class="sxs-lookup"><span data-stu-id="d290b-152">The calendar item is updated and the meeting update is sent only to attendees that are affected by the change in the meeting.</span></span>  <br/> |
|<span data-ttu-id="d290b-153">SendToAllAndSaveCopy</span><span class="sxs-lookup"><span data-stu-id="d290b-153">SendToAllAndSaveCopy</span></span>  <br/> |<span data-ttu-id="d290b-154">Обновления элемента календаря, сообщения о встрече всем участникам и копия сохраняется в папке «Отправленные».</span><span class="sxs-lookup"><span data-stu-id="d290b-154">The calendar item is updated, the meeting update is sent to all attendees, and a copy is saved in the Sent Items folder.</span></span>  <br/> |
|<span data-ttu-id="d290b-155">SendToChangedAndSaveCopy</span><span class="sxs-lookup"><span data-stu-id="d290b-155">SendToChangedAndSaveCopy</span></span>  <br/> |<span data-ttu-id="d290b-156">Обновлено элемента календаря, сообщения о встрече для всех участников, которые повлияет переход на собрании и копия сохраняется в папке «Отправленные».</span><span class="sxs-lookup"><span data-stu-id="d290b-156">The calendar item is updated, the meeting update is sent to all attendees that are affected by the change in the meeting, and a copy is saved in the Sent Items folder.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="d290b-157">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="d290b-157">Child elements</span></span>

|<span data-ttu-id="d290b-158">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="d290b-158">**Element**</span></span>|<span data-ttu-id="d290b-159">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d290b-159">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d290b-160">SavedItemFolderId</span><span class="sxs-lookup"><span data-stu-id="d290b-160">SavedItemFolderId</span></span>](saveditemfolderid.md) <br/> |<span data-ttu-id="d290b-161">Определяет папку назначения для операций, обновление, отправка и создания элементов в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="d290b-161">Identifies the target folder for operations that update, send, and create items in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="d290b-162">ItemChanges</span><span class="sxs-lookup"><span data-stu-id="d290b-162">ItemChanges</span></span>](itemchanges.md) <br/> |<span data-ttu-id="d290b-163">Содержит массив элементов [ItemChange](itemchange.md) , чтобы указать элементы и обновления, чтобы применить к элементам.</span><span class="sxs-lookup"><span data-stu-id="d290b-163">Contains an array of [ItemChange](itemchange.md) elements that identify items and the updates to apply to the items.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d290b-164">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="d290b-164">Parent elements</span></span>

<span data-ttu-id="d290b-165">Нет.</span><span class="sxs-lookup"><span data-stu-id="d290b-165">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="d290b-166">Замечания</span><span class="sxs-lookup"><span data-stu-id="d290b-166">Remarks</span></span>

<span data-ttu-id="d290b-167">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="d290b-167">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d290b-168">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="d290b-168">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d290b-169">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="d290b-169">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="d290b-170">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="d290b-170">Schema Name</span></span>  <br/> |<span data-ttu-id="d290b-171">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="d290b-171">Messages schema</span></span>  <br/> |
|<span data-ttu-id="d290b-172">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="d290b-172">Validation File</span></span>  <br/> |<span data-ttu-id="d290b-173">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="d290b-173">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="d290b-174">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="d290b-174">Can be Empty</span></span>  <br/> |<span data-ttu-id="d290b-175">False</span><span class="sxs-lookup"><span data-stu-id="d290b-175">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d290b-176">См. также</span><span class="sxs-lookup"><span data-stu-id="d290b-176">See also</span></span>



[<span data-ttu-id="d290b-177">UpdateItem Operation</span><span class="sxs-lookup"><span data-stu-id="d290b-177">UpdateItem operation</span></span>](updateitem-operation.md)

