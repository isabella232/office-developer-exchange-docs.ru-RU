---
title: суппрессреадрецеипт
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
description: Элемент Суппрессреадрецеипт используется для подавления уведомлений о прочтении.
ms.openlocfilehash: b6b4fe5db26195882a7def5cac8266a942def996
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44455956"
---
# <a name="suppressreadreceipt"></a><span data-ttu-id="54b4c-103">суппрессреадрецеипт</span><span class="sxs-lookup"><span data-stu-id="54b4c-103">SuppressReadReceipt</span></span>

<span data-ttu-id="54b4c-104">Элемент **суппрессреадрецеипт** используется для подавления уведомлений о прочтении.</span><span class="sxs-lookup"><span data-stu-id="54b4c-104">The **SuppressReadReceipt** element is used to suppress read receipts.</span></span> 
  
```xml
<SuppressReadReceipt>
   <ReferenceItemId/>
</SuppressReadReceipt>
```

 <span data-ttu-id="54b4c-105">**суппрессреадрецеипттипе**</span><span class="sxs-lookup"><span data-stu-id="54b4c-105">**SuppressReadReceiptType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="54b4c-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="54b4c-106">Attributes and elements</span></span>

<span data-ttu-id="54b4c-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="54b4c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="54b4c-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="54b4c-108">Attributes</span></span>

<span data-ttu-id="54b4c-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="54b4c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="54b4c-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="54b4c-110">Child elements</span></span>

|<span data-ttu-id="54b4c-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="54b4c-111">**Element**</span></span>|<span data-ttu-id="54b4c-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="54b4c-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="54b4c-113">референцеитемид</span><span class="sxs-lookup"><span data-stu-id="54b4c-113">ReferenceItemId</span></span>](referenceitemid.md) <br/> |<span data-ttu-id="54b4c-114">Определяет элемент, на который ссылается объект Response.</span><span class="sxs-lookup"><span data-stu-id="54b4c-114">Identifies the item to which the response object refers.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="54b4c-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="54b4c-115">Parent elements</span></span>

|<span data-ttu-id="54b4c-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="54b4c-116">**Element**</span></span>|<span data-ttu-id="54b4c-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="54b4c-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="54b4c-118">аджацентмитингс</span><span class="sxs-lookup"><span data-stu-id="54b4c-118">AdjacentMeetings</span></span>](adjacentmeetings.md) <br/> | <span data-ttu-id="54b4c-119">Описывает все элементы, смежные с временем собрания.</span><span class="sxs-lookup"><span data-stu-id="54b4c-119">Describes all items that are adjacent to a meeting time.</span></span>  <br/><br/>  <span data-ttu-id="54b4c-120">Ниже приведены некоторые выражения XPath для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="54b4c-120">The following are some of the XPath expressions to this element:</span></span><br/>  <br/>  `/CalendarItem/AdjacentMeetings` <br/>  `/MeetingRequest/AdjacentMeetings` <br/>  `/SetItemField/CalendarItem/AdjacentMeetings` <br/>  `/AppendToItemField/CalendarItem/AdjacentMeetings` <br/>  `/AcceptItem/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings` <br/>  `/DeclineItem/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings` <br/>  `/TentativelyAcceptItem/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings` <br/>  `/UpdateItem/ItemChanges/ItemChange/Updates/SetItemField/CalendarItem/AdjacentMeetings` <br/>  `/UpdateItem/ItemChanges/ItemChange/Updates/AppendToItemField/CalendarItem/AdjacentMeetings` <br/>  `/CreateAttachmentResponseMessage/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings` <br/>  `/GetAttachmentResponseMessage/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings` <br/> |
|[<span data-ttu-id="54b4c-121">конфликтингмитингс</span><span class="sxs-lookup"><span data-stu-id="54b4c-121">ConflictingMeetings</span></span>](conflictingmeetings.md) <br/> | <span data-ttu-id="54b4c-122">Описывает все элементы, которые конфликтуют с временем собрания.</span><span class="sxs-lookup"><span data-stu-id="54b4c-122">Describes all items that conflict with a meeting time.</span></span> <br/> <br/>  <span data-ttu-id="54b4c-123">Ниже приведены некоторые выражения XPath для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="54b4c-123">The following are some of the XPath expressions to this element:</span></span> <br/> <br/>  `/CalendarItem/ConflictingMeetings` <br/>  `/MeetingRequest/ConflictingMeetings` <br/>  `/SetItemField/CalendarItem/ConflictingMeetings` <br/>  `/AppendToItemField/CalendarItem/ConflictingMeetings` <br/>  `/AcceptItem/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings` <br/>  `/DeclineItem/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings` <br/>  `/TentativelyAcceptItem/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings` <br/>  `/UpdateItem/ItemChanges/ItemChange/Updates/SetItemField/CalendarItem/ConflictingMeetings` <br/>  `/UpdateItem/ItemChanges/ItemChange/Updates/AppendToItemField/CalendarItem/ConflictingMeetings` <br/>  `/CreateAttachmentResponseMessage/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings` <br/>  `/GetAttachmentResponseMessage/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings` <br/> |
|[<span data-ttu-id="54b4c-124">респонсеобжектс</span><span class="sxs-lookup"><span data-stu-id="54b4c-124">ResponseObjects</span></span>](responseobjects.md) <br/> |<span data-ttu-id="54b4c-125">Содержит коллекцию всех объектов ответа, связанных с элементом в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="54b4c-125">Contains a collection of all the response objects that are associated with an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="54b4c-126">Элементы (Нонемптяррайофаллитемстипе)</span><span class="sxs-lookup"><span data-stu-id="54b4c-126">Items (NonEmptyArrayOfAllItemsType)</span></span>](items-nonemptyarrayofallitemstype.md) <br/> |<span data-ttu-id="54b4c-127">Содержит массив элементов для создания в папке, определяемой элементом [ParentFolderId (таржетфолдеридтипе)](parentfolderid-targetfolderidtype.md) .</span><span class="sxs-lookup"><span data-stu-id="54b4c-127">Contains an array of items to create in the folder that is identified by the [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) element.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="54b4c-128">Примечания</span><span class="sxs-lookup"><span data-stu-id="54b4c-128">Remarks</span></span>

<span data-ttu-id="54b4c-129">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="54b4c-129">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="54b4c-130">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="54b4c-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="54b4c-131">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="54b4c-131">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="54b4c-132">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="54b4c-132">Schema Name</span></span>  <br/> |<span data-ttu-id="54b4c-133">Схема Types</span><span class="sxs-lookup"><span data-stu-id="54b4c-133">Types schema</span></span>  <br/> |
|<span data-ttu-id="54b4c-134">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="54b4c-134">Validation File</span></span>  <br/> |<span data-ttu-id="54b4c-135">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="54b4c-135">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="54b4c-136">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="54b4c-136">Can be Empty</span></span>  <br/> |<span data-ttu-id="54b4c-137">False</span><span class="sxs-lookup"><span data-stu-id="54b4c-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="54b4c-138">См. также</span><span class="sxs-lookup"><span data-stu-id="54b4c-138">See also</span></span>

- [<span data-ttu-id="54b4c-139">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="54b4c-139">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

