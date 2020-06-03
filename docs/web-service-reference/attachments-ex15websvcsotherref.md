---
title: Вложения
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Attachments
api_type:
- schema
ms.assetid: b470e614-34bb-44f0-8790-7ddbdcbbd29d
description: Элемент вложениям содержит элементы или файлы, вложенные в элемент в хранилище Exchange.
ms.openlocfilehash: a9f79cd79f19e6226703c99c53c91efed600f495
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461536"
---
# <a name="attachments"></a><span data-ttu-id="735ad-103">Attachments</span><span class="sxs-lookup"><span data-stu-id="735ad-103">Attachments</span></span>

<span data-ttu-id="735ad-104">Элемент **вложениям** содержит элементы или файлы, вложенные в элемент в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="735ad-104">The **Attachments** element contains the items or files that are attached to an item in the Exchange store.</span></span> 
  
```xml
<Attachments>
   <ItemAttachment/>
   <FileAttachment/>
</Attachments>
```

 <span data-ttu-id="735ad-105">**Аррайофаттачментстипе** и **нонемптяррайофаттачментстипе**</span><span class="sxs-lookup"><span data-stu-id="735ad-105">**ArrayOfAttachmentsType** and **NonEmptyArrayOfAttachmentsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="735ad-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="735ad-106">Attributes and elements</span></span>

<span data-ttu-id="735ad-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="735ad-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="735ad-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="735ad-108">Attributes</span></span>

<span data-ttu-id="735ad-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="735ad-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="735ad-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="735ad-110">Child elements</span></span>

|<span data-ttu-id="735ad-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="735ad-111">**Element**</span></span>|<span data-ttu-id="735ad-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="735ad-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="735ad-113">ItemAttachment</span><span class="sxs-lookup"><span data-stu-id="735ad-113">ItemAttachment</span></span>](itemattachment.md) <br/> |<span data-ttu-id="735ad-114">Представляет элемент Exchange, присоединенный к другому элементу Exchange.</span><span class="sxs-lookup"><span data-stu-id="735ad-114">Represents an Exchange item that is attached to another Exchange item.</span></span>  <br/> |
|[<span data-ttu-id="735ad-115">FileAttachment</span><span class="sxs-lookup"><span data-stu-id="735ad-115">FileAttachment</span></span>](fileattachment.md) <br/> |<span data-ttu-id="735ad-116">Представляет файл, присоединенный к элементу в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="735ad-116">Represents a file that is attached to an item in the Exchange store.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="735ad-117">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="735ad-117">Parent elements</span></span>

|<span data-ttu-id="735ad-118">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="735ad-118">**Element**</span></span>|<span data-ttu-id="735ad-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="735ad-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="735ad-120">CreateAttachment</span><span class="sxs-lookup"><span data-stu-id="735ad-120">CreateAttachment</span></span>](createattachment.md) <br/> |<span data-ttu-id="735ad-121">Определяет запрос на создание вложения для элемента в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="735ad-121">Defines a request to create an attachment to an item in the Exchange store.</span></span><br/><br/> <span data-ttu-id="735ad-122">Ниже приведено выражение XPath для этого элемента:`/CreateAttachment`</span><span class="sxs-lookup"><span data-stu-id="735ad-122">The following is the XPath expression to this element:  `/CreateAttachment`</span></span> <br/> |
|[<span data-ttu-id="735ad-123">акцептитем</span><span class="sxs-lookup"><span data-stu-id="735ad-123">AcceptItem</span></span>](acceptitem.md) <br/> | <span data-ttu-id="735ad-124">Представляет ответ на принять приглашение на собрание.</span><span class="sxs-lookup"><span data-stu-id="735ad-124">Represents an Accept reply to a meeting request.</span></span><br/><br/><span data-ttu-id="735ad-125">Ниже приведены некоторые выражения XPath для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="735ad-125">The following are some of the XPath expressions to this element:</span></span><ul><li>`/CreateItem/Items`</li><li>`/MeetingRequest/ConflictingMeetings` </li><li>`/SetItemField/CalendarItem/ConflictingMeetings`</li><li>`/AppendToItemField/CalendarItem/ConflictingMeetings`</li><li>`/AcceptItem/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings`</li><li>`/DeclineItem/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings`</li><li>`/UpdateItem/ItemChanges/ItemChange/Updates/AppendToItemField/CalendarItem/AdjacentMeetings`</li><li>`/CreateAttachmentResponseMessage/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings`</li><li>`/GetAttachmentResponseMessage/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings`</li></ul> |
|[<span data-ttu-id="735ad-126">деклинеитем</span><span class="sxs-lookup"><span data-stu-id="735ad-126">DeclineItem</span></span>](declineitem.md) <br/> |<span data-ttu-id="735ad-127">Представляет отклонить ответ на приглашения на собрание.</span><span class="sxs-lookup"><span data-stu-id="735ad-127">Represents a Decline reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="735ad-128">тентативелякцептитем</span><span class="sxs-lookup"><span data-stu-id="735ad-128">TentativelyAcceptItem</span></span>](tentativelyacceptitem.md) <br/> |<span data-ttu-id="735ad-129">Представляет под вопросом ответ на приглашения на собрание.</span><span class="sxs-lookup"><span data-stu-id="735ad-129">Represents a Tentative reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="735ad-130">RemoveItem</span><span class="sxs-lookup"><span data-stu-id="735ad-130">RemoveItem</span></span>](removeitem.md) <br/> |<span data-ttu-id="735ad-131">Удаляет элемент из хранилища Exchange.</span><span class="sxs-lookup"><span data-stu-id="735ad-131">Removes an item from the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="735ad-132">Ресурс</span><span class="sxs-lookup"><span data-stu-id="735ad-132">Item</span></span>](item.md) <br/> |<span data-ttu-id="735ad-133">Представляет общий элемент Exchange.</span><span class="sxs-lookup"><span data-stu-id="735ad-133">Represents a generic Exchange item.</span></span>  <br/> |
|[<span data-ttu-id="735ad-134">митингмессаже</span><span class="sxs-lookup"><span data-stu-id="735ad-134">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="735ad-135">Представляет собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="735ad-135">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="735ad-136">Свойство meetingrequest</span><span class="sxs-lookup"><span data-stu-id="735ad-136">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="735ad-137">Представляет приглашение на собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="735ad-137">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="735ad-138">митингреспонсе</span><span class="sxs-lookup"><span data-stu-id="735ad-138">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="735ad-139">Представляет ответ на приглашение на собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="735ad-139">Represents a meeting response in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="735ad-140">митингканцеллатион</span><span class="sxs-lookup"><span data-stu-id="735ad-140">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="735ad-141">Представляет отмену собрания в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="735ad-141">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="735ad-142">Message</span><span class="sxs-lookup"><span data-stu-id="735ad-142">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="735ad-143">Представляет сообщение электронной почты Exchange.</span><span class="sxs-lookup"><span data-stu-id="735ad-143">Represents an Exchange e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="735ad-144">Задача</span><span class="sxs-lookup"><span data-stu-id="735ad-144">Task</span></span>](task.md) <br/> |<span data-ttu-id="735ad-145">Представляет задачу в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="735ad-145">Represents a task in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="735ad-146">календаритем</span><span class="sxs-lookup"><span data-stu-id="735ad-146">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="735ad-147">Представляет элемент календаря Exchange.</span><span class="sxs-lookup"><span data-stu-id="735ad-147">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="735ad-148">Контакт</span><span class="sxs-lookup"><span data-stu-id="735ad-148">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="735ad-149">Представляет элемент контакта Exchange.</span><span class="sxs-lookup"><span data-stu-id="735ad-149">Represents an Exchange contact item.</span></span>  <br/> |
|[<span data-ttu-id="735ad-150">дистрибутионлист</span><span class="sxs-lookup"><span data-stu-id="735ad-150">DistributionList</span></span>](distributionlist.md) <br/> |<span data-ttu-id="735ad-151">Представляет список рассылки.</span><span class="sxs-lookup"><span data-stu-id="735ad-151">Represents a distribution list.</span></span>  <br/> |
|[<span data-ttu-id="735ad-152">креатеаттачментреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="735ad-152">CreateAttachmentResponseMessage</span></span>](createattachmentresponsemessage.md) <br/> |<span data-ttu-id="735ad-153">Содержит состояние и результат одного запроса CreateAttachment.</span><span class="sxs-lookup"><span data-stu-id="735ad-153">Contains the status and result of a single CreateAttachment request.</span></span>  <br/> |
|[<span data-ttu-id="735ad-154">жетаттачментреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="735ad-154">GetAttachmentResponseMessage</span></span>](getattachmentresponsemessage.md) <br/> |<span data-ttu-id="735ad-155">Содержит состояние и результат запроса GetAttachment.</span><span class="sxs-lookup"><span data-stu-id="735ad-155">Contains the status and result of a GetAttachment request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="735ad-156">Примечания</span><span class="sxs-lookup"><span data-stu-id="735ad-156">Remarks</span></span>

<span data-ttu-id="735ad-157">Элементы **вложения** имеют одни и те же дочерние элементы, но основаны на разных типах: **аррайофаттачментстипе** и **нонемптяррайофаттачментстипе**.</span><span class="sxs-lookup"><span data-stu-id="735ad-157">The **Attachments** elements have the same child elements but are based on different types: **ArrayOfAttachmentsType** and **NonEmptyArrayOfAttachmentsType**.</span></span> <span data-ttu-id="735ad-158">Типы определяют, является ли дочерний элемент обязательным.</span><span class="sxs-lookup"><span data-stu-id="735ad-158">The types define whether a child element is required.</span></span> <span data-ttu-id="735ad-159">**Аррайофаттачментстипе** используется только в ответном сообщении.</span><span class="sxs-lookup"><span data-stu-id="735ad-159">The **ArrayOfAttachmentsType** is only used in the response message.</span></span> <span data-ttu-id="735ad-160">Кроме того, обратите внимание, что эти элементы встречаются как в пространстве имен messages, так и в пространстве имен Types.</span><span class="sxs-lookup"><span data-stu-id="735ad-160">It is also important to note that these elements occur in both the messages and types namespaces.</span></span> 
  
<span data-ttu-id="735ad-161">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="735ad-161">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="735ad-162">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="735ad-162">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="735ad-163">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="735ad-163">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="735ad-164">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="735ad-164">Schema Name</span></span>  <br/> |<span data-ttu-id="735ad-165">Схема Types</span><span class="sxs-lookup"><span data-stu-id="735ad-165">Types schema</span></span>  <br/> |
|<span data-ttu-id="735ad-166">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="735ad-166">Validation File</span></span>  <br/> |<span data-ttu-id="735ad-167">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="735ad-167">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="735ad-168">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="735ad-168">Can be Empty</span></span>  <br/> |<span data-ttu-id="735ad-169">False</span><span class="sxs-lookup"><span data-stu-id="735ad-169">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="735ad-170">См. также</span><span class="sxs-lookup"><span data-stu-id="735ad-170">See also</span></span>

- [<span data-ttu-id="735ad-171">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="735ad-171">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

