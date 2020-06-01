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
ms.openlocfilehash: 43821db58457ffce22be918a7ba6427f57230010
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44466572"
---
# <a name="updateitem"></a><span data-ttu-id="0d81c-103">UpdateItem</span><span class="sxs-lookup"><span data-stu-id="0d81c-103">UpdateItem</span></span>

<span data-ttu-id="0d81c-104">Элемент **UpdateItem** определяет запрос на обновление элемента в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="0d81c-104">The **UpdateItem** element defines a request to update an item in a mailbox.</span></span> 
  
```XML
<UpdateItem ConflictResolution="" MessageDisposition="" SendMeetingInvitationsOrCancellations="" SuppressReadReceipts="">
   <SavedItemFolderId/>
   <ItemChanges/>
</UpdateItem>
```

 <span data-ttu-id="0d81c-105">**упдатеитемтипе**</span><span class="sxs-lookup"><span data-stu-id="0d81c-105">**UpdateItemType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0d81c-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="0d81c-106">Attributes and elements</span></span>

<span data-ttu-id="0d81c-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="0d81c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0d81c-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="0d81c-108">Attributes</span></span>

|<span data-ttu-id="0d81c-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="0d81c-109">**Attribute**</span></span>|<span data-ttu-id="0d81c-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="0d81c-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="0d81c-111">**ConflictResolution**</span><span class="sxs-lookup"><span data-stu-id="0d81c-111">**ConflictResolution**</span></span> <br/> |<span data-ttu-id="0d81c-112">Определяет тип разрешения конфликтов, которое необходимо попробовать во время обновления.</span><span class="sxs-lookup"><span data-stu-id="0d81c-112">Identifies the type of conflict resolution to try during an update.</span></span> <span data-ttu-id="0d81c-113">Значение по умолчанию — "Авторазрешение".</span><span class="sxs-lookup"><span data-stu-id="0d81c-113">The default value is AutoResolve.</span></span>  <br/> |
|<span data-ttu-id="0d81c-114">**мессажедиспоситион**</span><span class="sxs-lookup"><span data-stu-id="0d81c-114">**MessageDisposition**</span></span> <br/> |<span data-ttu-id="0d81c-115">Описывает, как будет обрабатываться элемент после его обновления.</span><span class="sxs-lookup"><span data-stu-id="0d81c-115">Describes how the item will be handled after it is updated.</span></span> <span data-ttu-id="0d81c-116">Атрибут **мессажедиспоситион** необходим для элементов сообщения, включая сообщения о собраниях, такие как отмена собраний, приглашения на собрания и ответы на собрания.</span><span class="sxs-lookup"><span data-stu-id="0d81c-116">The **MessageDisposition** attribute is required for message items, including meeting messages such as meeting cancellations, meeting requests, and meeting responses.</span></span>  <br/> |
|<span data-ttu-id="0d81c-117">**сендмитингинвитатионсорканцеллатионс**</span><span class="sxs-lookup"><span data-stu-id="0d81c-117">**SendMeetingInvitationsOrCancellations**</span></span> <br/> |<span data-ttu-id="0d81c-118">Описывает способ общения обновлений собраний после обновления элемента календаря.</span><span class="sxs-lookup"><span data-stu-id="0d81c-118">Describes how meeting updates are communicated after a calendar item is updated.</span></span> <span data-ttu-id="0d81c-119">Этот атрибут необходим для элементов календаря и вхождений элементов календаря.</span><span class="sxs-lookup"><span data-stu-id="0d81c-119">This attribute is required for calendar items and calendar item occurrences.</span></span>  <br/> |
|<span data-ttu-id="0d81c-120">**суппрессреадрецеиптс**</span><span class="sxs-lookup"><span data-stu-id="0d81c-120">**SuppressReadReceipts**</span></span> <br/> |<span data-ttu-id="0d81c-121">Указывает, следует ли подавлять уведомления о прочтении обновленного элемента.</span><span class="sxs-lookup"><span data-stu-id="0d81c-121">Indicates whether read receipts for the updated item should be suppressed.</span></span> <span data-ttu-id="0d81c-122">Текстовое значение **true** указывает, что уведомления о прочтении должны подавляться.</span><span class="sxs-lookup"><span data-stu-id="0d81c-122">A text value of **true** indicates that read receipts should be suppressed.</span></span> <span data-ttu-id="0d81c-123">Значение **false** указывает, что уведомления о прочтении будут отправляться отправителю.</span><span class="sxs-lookup"><span data-stu-id="0d81c-123">A value of **false** indicates that the read receipts will be sent to the sender.</span></span> <span data-ttu-id="0d81c-124">Этот атрибут является необязательным.</span><span class="sxs-lookup"><span data-stu-id="0d81c-124">This attribute is optional.</span></span>  <br/> <span data-ttu-id="0d81c-125">Этот атрибут появился в Exchange Server 2013 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="0d81c-125">This attribute was introduced in Exchange Server 2013 SP1.</span></span>  <br/> |
   
#### <a name="conflictresolution-attribute"></a><span data-ttu-id="0d81c-126">Атрибут Конфликтресолутион</span><span class="sxs-lookup"><span data-stu-id="0d81c-126">ConflictResolution Attribute</span></span>

|<span data-ttu-id="0d81c-127">**Значение**</span><span class="sxs-lookup"><span data-stu-id="0d81c-127">**Value**</span></span>|<span data-ttu-id="0d81c-128">**Описание**</span><span class="sxs-lookup"><span data-stu-id="0d81c-128">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="0d81c-129">невероверврите</span><span class="sxs-lookup"><span data-stu-id="0d81c-129">NeverOverwrite</span></span>  <br/> |<span data-ttu-id="0d81c-130">При возникновении конфликта операция обновления завершается с ошибкой, и возвращается ошибка.</span><span class="sxs-lookup"><span data-stu-id="0d81c-130">If there is a conflict, the update operation fails and an error is returned.</span></span>  <br/> |
|<span data-ttu-id="0d81c-131">Авторазрешение</span><span class="sxs-lookup"><span data-stu-id="0d81c-131">AutoResolve</span></span>  <br/> |<span data-ttu-id="0d81c-132">При выполнении операции обновления автоматически разрешается любой конфликт.</span><span class="sxs-lookup"><span data-stu-id="0d81c-132">The update operation automatically resolves any conflict.</span></span>  <br/> |
|<span data-ttu-id="0d81c-133">алвайсоверврите</span><span class="sxs-lookup"><span data-stu-id="0d81c-133">AlwaysOverwrite</span></span>  <br/> |<span data-ttu-id="0d81c-134">При возникновении конфликта операция обновления перезапишет сведения.</span><span class="sxs-lookup"><span data-stu-id="0d81c-134">If there is a conflict, the update operation will overwrite information.</span></span>  <br/> |
   
#### <a name="messagedisposition-attribute"></a><span data-ttu-id="0d81c-135">Атрибут Мессажедиспоситион</span><span class="sxs-lookup"><span data-stu-id="0d81c-135">MessageDisposition Attribute</span></span>

|<span data-ttu-id="0d81c-136">**Значение**</span><span class="sxs-lookup"><span data-stu-id="0d81c-136">**Value**</span></span>|<span data-ttu-id="0d81c-137">**Описание**</span><span class="sxs-lookup"><span data-stu-id="0d81c-137">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="0d81c-138">савеонли</span><span class="sxs-lookup"><span data-stu-id="0d81c-138">SaveOnly</span></span>  <br/> |<span data-ttu-id="0d81c-139">Элемент обновляется и сохраняется в текущей папке.</span><span class="sxs-lookup"><span data-stu-id="0d81c-139">The item is updated and saved back to its current folder.</span></span>  <br/> |
|<span data-ttu-id="0d81c-140">сендонли</span><span class="sxs-lookup"><span data-stu-id="0d81c-140">SendOnly</span></span>  <br/> |<span data-ttu-id="0d81c-141">Элемент обновляется и отправляется, но копия не сохраняется.</span><span class="sxs-lookup"><span data-stu-id="0d81c-141">The item is updated and sent but no copy is saved.</span></span>  <br/> |
|<span data-ttu-id="0d81c-142">SendAndSaveCopy</span><span class="sxs-lookup"><span data-stu-id="0d81c-142">SendAndSaveCopy</span></span>  <br/> |<span data-ttu-id="0d81c-143">Элемент обновляется, а копия сохраняется в папке, указанной с помощью элемента [саведитемфолдерид](saveditemfolderid.md) .</span><span class="sxs-lookup"><span data-stu-id="0d81c-143">The item is updated and a copy is saved in the folder identified by the [SavedItemFolderId](saveditemfolderid.md) element.</span></span>  <br/> |
   
#### <a name="sendmeetinginvitationsorcancellations-attribute"></a><span data-ttu-id="0d81c-144">Атрибут Сендмитингинвитатионсорканцеллатионс</span><span class="sxs-lookup"><span data-stu-id="0d81c-144">SendMeetingInvitationsOrCancellations Attribute</span></span>

|<span data-ttu-id="0d81c-145">**Значение**</span><span class="sxs-lookup"><span data-stu-id="0d81c-145">**Value**</span></span>|<span data-ttu-id="0d81c-146">**Описание**</span><span class="sxs-lookup"><span data-stu-id="0d81c-146">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="0d81c-147">сендтононе</span><span class="sxs-lookup"><span data-stu-id="0d81c-147">SendToNone</span></span>  <br/> |<span data-ttu-id="0d81c-148">Элемент календаря обновляется, но обновления не отправляются участникам.</span><span class="sxs-lookup"><span data-stu-id="0d81c-148">The calendar item is updated but updates are not sent to attendees.</span></span>  <br/> |
|<span data-ttu-id="0d81c-149">сендонлитоалл</span><span class="sxs-lookup"><span data-stu-id="0d81c-149">SendOnlyToAll</span></span>  <br/> |<span data-ttu-id="0d81c-150">Элемент календаря обновляется, а обновление собрания отправляется всем участникам, но не сохраняется в папке "Отправленные".</span><span class="sxs-lookup"><span data-stu-id="0d81c-150">The calendar item is updated and the meeting update is sent to all attendees but is not saved in the Sent Items folder.</span></span>  <br/> |
|<span data-ttu-id="0d81c-151">сендонлиточанжед</span><span class="sxs-lookup"><span data-stu-id="0d81c-151">SendOnlyToChanged</span></span>  <br/> |<span data-ttu-id="0d81c-152">Элемент календаря обновляется, а обновление собрания отправляется только участникам, на которые влияет изменение собрания.</span><span class="sxs-lookup"><span data-stu-id="0d81c-152">The calendar item is updated and the meeting update is sent only to attendees that are affected by the change in the meeting.</span></span>  <br/> |
|<span data-ttu-id="0d81c-153">сендтоалландсавекопи</span><span class="sxs-lookup"><span data-stu-id="0d81c-153">SendToAllAndSaveCopy</span></span>  <br/> |<span data-ttu-id="0d81c-154">Элемент календаря обновляется, обновление собрания отправляется всем участникам, а копия сохраняется в папке "Отправленные".</span><span class="sxs-lookup"><span data-stu-id="0d81c-154">The calendar item is updated, the meeting update is sent to all attendees, and a copy is saved in the Sent Items folder.</span></span>  <br/> |
|<span data-ttu-id="0d81c-155">сендточанжедандсавекопи</span><span class="sxs-lookup"><span data-stu-id="0d81c-155">SendToChangedAndSaveCopy</span></span>  <br/> |<span data-ttu-id="0d81c-156">Элемент календаря обновляется, но обновление собрания отправляется всем участникам, на которые влияет изменение собрания, а копия сохраняется в папке "Отправленные".</span><span class="sxs-lookup"><span data-stu-id="0d81c-156">The calendar item is updated, the meeting update is sent to all attendees that are affected by the change in the meeting, and a copy is saved in the Sent Items folder.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="0d81c-157">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="0d81c-157">Child elements</span></span>

|<span data-ttu-id="0d81c-158">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="0d81c-158">**Element**</span></span>|<span data-ttu-id="0d81c-159">**Описание**</span><span class="sxs-lookup"><span data-stu-id="0d81c-159">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0d81c-160">саведитемфолдерид</span><span class="sxs-lookup"><span data-stu-id="0d81c-160">SavedItemFolderId</span></span>](saveditemfolderid.md) <br/> |<span data-ttu-id="0d81c-161">Определяет целевую папку для операций обновления, отправки и создания элементов в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="0d81c-161">Identifies the target folder for operations that update, send, and create items in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="0d81c-162">итемчанжес</span><span class="sxs-lookup"><span data-stu-id="0d81c-162">ItemChanges</span></span>](itemchanges.md) <br/> |<span data-ttu-id="0d81c-163">Содержит массив элементов [итемчанже](itemchange.md) , определяющих элементы и обновления, которые необходимо применить к элементам.</span><span class="sxs-lookup"><span data-stu-id="0d81c-163">Contains an array of [ItemChange](itemchange.md) elements that identify items and the updates to apply to the items.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="0d81c-164">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="0d81c-164">Parent elements</span></span>

<span data-ttu-id="0d81c-165">Нет.</span><span class="sxs-lookup"><span data-stu-id="0d81c-165">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="0d81c-166">Примечания</span><span class="sxs-lookup"><span data-stu-id="0d81c-166">Remarks</span></span>

<span data-ttu-id="0d81c-167">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="0d81c-167">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0d81c-168">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="0d81c-168">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0d81c-169">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="0d81c-169">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="0d81c-170">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="0d81c-170">Schema Name</span></span>  <br/> |<span data-ttu-id="0d81c-171">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="0d81c-171">Messages schema</span></span>  <br/> |
|<span data-ttu-id="0d81c-172">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="0d81c-172">Validation File</span></span>  <br/> |<span data-ttu-id="0d81c-173">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="0d81c-173">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="0d81c-174">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="0d81c-174">Can be Empty</span></span>  <br/> |<span data-ttu-id="0d81c-175">False</span><span class="sxs-lookup"><span data-stu-id="0d81c-175">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0d81c-176">См. также</span><span class="sxs-lookup"><span data-stu-id="0d81c-176">See also</span></span>



[<span data-ttu-id="0d81c-177">Операция UpdateItem</span><span class="sxs-lookup"><span data-stu-id="0d81c-177">UpdateItem operation</span></span>](updateitem-operation.md)

