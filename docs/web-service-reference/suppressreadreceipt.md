---
title: SuppressReadReceipt
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SuppressReadReceipt
api_type:
- schema
ms.assetid: fc09bcc2-c003-4322-8315-d929bd0a9e2e
description: Элемент SuppressReadReceipt используется для отмены вывода прочтении.
ms.openlocfilehash: de2eef68abd25c8208530ba5e98ab3278c8702d1
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19840116"
---
# <a name="suppressreadreceipt"></a><span data-ttu-id="08292-103">SuppressReadReceipt</span><span class="sxs-lookup"><span data-stu-id="08292-103">SuppressReadReceipt</span></span>

<span data-ttu-id="08292-104">Элемент **SuppressReadReceipt** используется для отмены вывода прочтении.</span><span class="sxs-lookup"><span data-stu-id="08292-104">The **SuppressReadReceipt** element is used to suppress read receipts.</span></span> 
  
```xml
<SuppressReadReceipt>
   <ReferenceItemId/>
</SuppressReadReceipt>
```

 <span data-ttu-id="08292-105">**SuppressReadReceiptType**</span><span class="sxs-lookup"><span data-stu-id="08292-105">**SuppressReadReceiptType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="08292-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="08292-106">Attributes and elements</span></span>

<span data-ttu-id="08292-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="08292-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="08292-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="08292-108">Attributes</span></span>

<span data-ttu-id="08292-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="08292-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="08292-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="08292-110">Child elements</span></span>

|<span data-ttu-id="08292-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="08292-111">**Element**</span></span>|<span data-ttu-id="08292-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="08292-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="08292-113">ReferenceItemId</span><span class="sxs-lookup"><span data-stu-id="08292-113">ReferenceItemId</span></span>](referenceitemid.md) <br/> |<span data-ttu-id="08292-114">Определяет элемент, к которому относится объект ответа.</span><span class="sxs-lookup"><span data-stu-id="08292-114">Identifies the item to which the response object refers.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="08292-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="08292-115">Parent elements</span></span>

|<span data-ttu-id="08292-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="08292-116">**Element**</span></span>|<span data-ttu-id="08292-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="08292-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="08292-118">AdjacentMeetings</span><span class="sxs-lookup"><span data-stu-id="08292-118">AdjacentMeetings</span></span>](adjacentmeetings.md) <br/> | <span data-ttu-id="08292-119">Описание всех элементов, расположенных во время собрания.</span><span class="sxs-lookup"><span data-stu-id="08292-119">Describes all items that are adjacent to a meeting time.</span></span>  <br/><br/>  <span data-ttu-id="08292-120">Ниже приведены некоторые из выражения XPath для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="08292-120">The following are some of the XPath expressions to this element:</span></span><br/>  <br/>  `/CalendarItem/AdjacentMeetings` <br/>  `/MeetingRequest/AdjacentMeetings` <br/>  `/SetItemField/CalendarItem/AdjacentMeetings` <br/>  `/AppendToItemField/CalendarItem/AdjacentMeetings` <br/>  `/AcceptItem/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings` <br/>  `/DeclineItem/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings` <br/>  `/TentativelyAcceptItem/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings` <br/>  `/UpdateItem/ItemChanges/ItemChange/Updates/SetItemField/CalendarItem/AdjacentMeetings` <br/>  `/UpdateItem/ItemChanges/ItemChange/Updates/AppendToItemField/CalendarItem/AdjacentMeetings` <br/>  `/CreateAttachmentResponseMessage/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings` <br/>  `/GetAttachmentResponseMessage/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings` <br/> |
|[<span data-ttu-id="08292-121">ConflictingMeetings</span><span class="sxs-lookup"><span data-stu-id="08292-121">ConflictingMeetings</span></span>](conflictingmeetings.md) <br/> | <span data-ttu-id="08292-122">Описание всех элементов, конфликтующие с время собрания.</span><span class="sxs-lookup"><span data-stu-id="08292-122">Describes all items that conflict with a meeting time.</span></span> <br/> <br/>  <span data-ttu-id="08292-123">Ниже приведены некоторые из выражения XPath для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="08292-123">The following are some of the XPath expressions to this element:</span></span> <br/> <br/>  `/CalendarItem/ConflictingMeetings` <br/>  `/MeetingRequest/ConflictingMeetings` <br/>  `/SetItemField/CalendarItem/ConflictingMeetings` <br/>  `/AppendToItemField/CalendarItem/ConflictingMeetings` <br/>  `/AcceptItem/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings` <br/>  `/DeclineItem/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings` <br/>  `/TentativelyAcceptItem/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings` <br/>  `/UpdateItem/ItemChanges/ItemChange/Updates/SetItemField/CalendarItem/ConflictingMeetings` <br/>  `/UpdateItem/ItemChanges/ItemChange/Updates/AppendToItemField/CalendarItem/ConflictingMeetings` <br/>  `/CreateAttachmentResponseMessage/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings` <br/>  `/GetAttachmentResponseMessage/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings` <br/> |
|[<span data-ttu-id="08292-124">ResponseObjects</span><span class="sxs-lookup"><span data-stu-id="08292-124">ResponseObjects</span></span>](responseobjects.md) <br/> |<span data-ttu-id="08292-125">Содержит коллекцию всех объектов ответа, которые связаны с элемента в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="08292-125">Contains a collection of all the response objects that are associated with an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="08292-126">Элементы (NonEmptyArrayOfAllItemsType)</span><span class="sxs-lookup"><span data-stu-id="08292-126">Items (NonEmptyArrayOfAllItemsType)</span></span>](items-nonemptyarrayofallitemstype.md) <br/> |<span data-ttu-id="08292-127">Содержит массив элементов для создания в папке, указанной с помощью элемента [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) .</span><span class="sxs-lookup"><span data-stu-id="08292-127">Contains an array of items to create in the folder that is identified by the [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) element.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="08292-128">Замечания</span><span class="sxs-lookup"><span data-stu-id="08292-128">Remarks</span></span>

<span data-ttu-id="08292-129">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="08292-129">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="08292-130">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="08292-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="08292-131">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="08292-131">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="08292-132">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="08292-132">Schema Name</span></span>  <br/> |<span data-ttu-id="08292-133">Схема Types</span><span class="sxs-lookup"><span data-stu-id="08292-133">Types schema</span></span>  <br/> |
|<span data-ttu-id="08292-134">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="08292-134">Validation File</span></span>  <br/> |<span data-ttu-id="08292-135">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="08292-135">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="08292-136">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="08292-136">Can be Empty</span></span>  <br/> |<span data-ttu-id="08292-137">False</span><span class="sxs-lookup"><span data-stu-id="08292-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="08292-138">См. также</span><span class="sxs-lookup"><span data-stu-id="08292-138">See also</span></span>

- [<span data-ttu-id="08292-139">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="08292-139">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

