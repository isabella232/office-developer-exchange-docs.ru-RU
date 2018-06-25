---
title: RemoveItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RemoveItem
api_type:
- schema
ms.assetid: 766878e3-9007-454f-8501-45139bc5c0e2
description: Элемент RemoveItem представляет объект ответа, который используется для удаления элемента собрания при получении сообщения MeetingCancellation.
ms.openlocfilehash: 6897363eba602e6a135ad255822197f9296dd44a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835108"
---
# <a name="removeitem"></a><span data-ttu-id="7ba28-103">RemoveItem</span><span class="sxs-lookup"><span data-stu-id="7ba28-103">RemoveItem</span></span>

<span data-ttu-id="7ba28-104">Элемент **RemoveItem** представляет объект ответа, который используется для удаления элемента собрания при получении сообщения MeetingCancellation.</span><span class="sxs-lookup"><span data-stu-id="7ba28-104">The **RemoveItem** element represents a response object that is used to remove a meeting item when a MeetingCancellation message is received.</span></span> 
  
```xml
<RemoveItem ObjectName="">
   <ReferenceItemId/>
</RemoveItem>
```

 <span data-ttu-id="7ba28-105">**RemoveItemType**</span><span class="sxs-lookup"><span data-stu-id="7ba28-105">**RemoveItemType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7ba28-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="7ba28-106">Attributes and elements</span></span>

<span data-ttu-id="7ba28-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="7ba28-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7ba28-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="7ba28-108">Attributes</span></span>

|<span data-ttu-id="7ba28-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="7ba28-109">**Attribute**</span></span>|<span data-ttu-id="7ba28-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="7ba28-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="7ba28-111">**Имя объекта**</span><span class="sxs-lookup"><span data-stu-id="7ba28-111">**ObjectName**</span></span> <br/> |<span data-ttu-id="7ba28-112">Представляет имя объекта класса RemoveItem ответ в виде строки на английском языке.</span><span class="sxs-lookup"><span data-stu-id="7ba28-112">Represents the name of the RemoveItem reply object class as an English string.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="7ba28-113">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="7ba28-113">Child elements</span></span>

|<span data-ttu-id="7ba28-114">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="7ba28-114">**Element**</span></span>|<span data-ttu-id="7ba28-115">**Описание**</span><span class="sxs-lookup"><span data-stu-id="7ba28-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7ba28-116">ReferenceItemId</span><span class="sxs-lookup"><span data-stu-id="7ba28-116">ReferenceItemId</span></span>](referenceitemid.md) <br/> |<span data-ttu-id="7ba28-117">Определяет элемент, к которому относится объект ответа RemoveItem.</span><span class="sxs-lookup"><span data-stu-id="7ba28-117">Identifies the item to which the RemoveItem response object refers.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="7ba28-118">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="7ba28-118">Parent elements</span></span>

|<span data-ttu-id="7ba28-119">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="7ba28-119">**Element**</span></span>|<span data-ttu-id="7ba28-120">**Описание**</span><span class="sxs-lookup"><span data-stu-id="7ba28-120">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7ba28-121">Элементы (NonEmptyArrayOfAllItemsType)</span><span class="sxs-lookup"><span data-stu-id="7ba28-121">Items (NonEmptyArrayOfAllItemsType)</span></span>](items-nonemptyarrayofallitemstype.md) <br/> |<span data-ttu-id="7ba28-122">Содержит массив элементов для создания в папке, указанной с помощью элемента [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) .</span><span class="sxs-lookup"><span data-stu-id="7ba28-122">Contains an array of items to create in the folder that is identified by the [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) element.</span></span>  <br/> |
|[<span data-ttu-id="7ba28-123">ResponseObjects</span><span class="sxs-lookup"><span data-stu-id="7ba28-123">ResponseObjects</span></span>](responseobjects.md) <br/> |<span data-ttu-id="7ba28-124">Содержит коллекцию всех объектов ответа, которые связаны с элемента в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="7ba28-124">Contains a collection of all the response objects that are associated with an item in the Exchange store.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="7ba28-125">Замечания</span><span class="sxs-lookup"><span data-stu-id="7ba28-125">Remarks</span></span>

 <span data-ttu-id="7ba28-126">**RemoveItem** действителен только в [MeetingCancellation](meetingcancellation.md).</span><span class="sxs-lookup"><span data-stu-id="7ba28-126">**RemoveItem** is valid only for a [MeetingCancellation](meetingcancellation.md).</span></span> <span data-ttu-id="7ba28-127">В противном случае возникает ошибка.</span><span class="sxs-lookup"><span data-stu-id="7ba28-127">Otherwise, an error is thrown.</span></span>
  
> [!NOTE]
> <span data-ttu-id="7ba28-128">[ItemClass](itemclass.md) для отмены собрания — IPM. Schedule.Meeting.Canceled.</span><span class="sxs-lookup"><span data-stu-id="7ba28-128">The [ItemClass](itemclass.md) for a meeting cancellation is IPM.Schedule.Meeting.Canceled.</span></span> 
  
<span data-ttu-id="7ba28-129">Чтобы удалить [MeetingRequest](meetingrequest.md) и связанного [элемента календаря, имеющего](calendaritem.md), используйте объект ответа [DeclineItem](declineitem.md) вместо **RemoveItem**.</span><span class="sxs-lookup"><span data-stu-id="7ba28-129">To remove a [MeetingRequest](meetingrequest.md) and the associated [CalendarItem](calendaritem.md), use the [DeclineItem](declineitem.md) response object instead of **RemoveItem**.</span></span>
  
 <span data-ttu-id="7ba28-130">**RemoveItem** не поддерживается для делегированный доступ.</span><span class="sxs-lookup"><span data-stu-id="7ba28-130">**RemoveItem** is not supported for delegate access.</span></span> 
  
<span data-ttu-id="7ba28-131">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="7ba28-131">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7ba28-132">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="7ba28-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7ba28-133">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="7ba28-133">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="7ba28-134">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="7ba28-134">Schema Name</span></span>  <br/> |<span data-ttu-id="7ba28-135">Схема Types</span><span class="sxs-lookup"><span data-stu-id="7ba28-135">Types schema</span></span>  <br/> |
|<span data-ttu-id="7ba28-136">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="7ba28-136">Validation File</span></span>  <br/> |<span data-ttu-id="7ba28-137">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="7ba28-137">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="7ba28-138">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="7ba28-138">Can be Empty</span></span>  <br/> |<span data-ttu-id="7ba28-139">False</span><span class="sxs-lookup"><span data-stu-id="7ba28-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7ba28-140">См. также</span><span class="sxs-lookup"><span data-stu-id="7ba28-140">See also</span></span>



- [<span data-ttu-id="7ba28-141">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="7ba28-141">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

