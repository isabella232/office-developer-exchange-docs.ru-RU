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
description: Элемент RemoveItem представляет объект Response, который используется для удаления элемента собрания при получении сообщения Митингканцеллатион.
ms.openlocfilehash: c0cd5c1f9894287ee78c2f7a65b8f4d3b943414e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44467692"
---
# <a name="removeitem"></a><span data-ttu-id="0d827-103">RemoveItem</span><span class="sxs-lookup"><span data-stu-id="0d827-103">RemoveItem</span></span>

<span data-ttu-id="0d827-104">Элемент **RemoveItem** представляет объект Response, который используется для удаления элемента собрания при получении сообщения митингканцеллатион.</span><span class="sxs-lookup"><span data-stu-id="0d827-104">The **RemoveItem** element represents a response object that is used to remove a meeting item when a MeetingCancellation message is received.</span></span> 
  
```xml
<RemoveItem ObjectName="">
   <ReferenceItemId/>
</RemoveItem>
```

 <span data-ttu-id="0d827-105">**ремовеитемтипе**</span><span class="sxs-lookup"><span data-stu-id="0d827-105">**RemoveItemType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0d827-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="0d827-106">Attributes and elements</span></span>

<span data-ttu-id="0d827-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="0d827-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0d827-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="0d827-108">Attributes</span></span>

|<span data-ttu-id="0d827-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="0d827-109">**Attribute**</span></span>|<span data-ttu-id="0d827-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="0d827-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="0d827-111">**ObjectName**</span><span class="sxs-lookup"><span data-stu-id="0d827-111">**ObjectName**</span></span> <br/> |<span data-ttu-id="0d827-112">Представляет имя класса объекта ответа RemoveItem в виде строки на английском языке.</span><span class="sxs-lookup"><span data-stu-id="0d827-112">Represents the name of the RemoveItem reply object class as an English string.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="0d827-113">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="0d827-113">Child elements</span></span>

|<span data-ttu-id="0d827-114">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="0d827-114">**Element**</span></span>|<span data-ttu-id="0d827-115">**Описание**</span><span class="sxs-lookup"><span data-stu-id="0d827-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0d827-116">референцеитемид</span><span class="sxs-lookup"><span data-stu-id="0d827-116">ReferenceItemId</span></span>](referenceitemid.md) <br/> |<span data-ttu-id="0d827-117">Определяет элемент, на который ссылается объект ответа RemoveItem.</span><span class="sxs-lookup"><span data-stu-id="0d827-117">Identifies the item to which the RemoveItem response object refers.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="0d827-118">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="0d827-118">Parent elements</span></span>

|<span data-ttu-id="0d827-119">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="0d827-119">**Element**</span></span>|<span data-ttu-id="0d827-120">**Описание**</span><span class="sxs-lookup"><span data-stu-id="0d827-120">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0d827-121">Элементы (Нонемптяррайофаллитемстипе)</span><span class="sxs-lookup"><span data-stu-id="0d827-121">Items (NonEmptyArrayOfAllItemsType)</span></span>](items-nonemptyarrayofallitemstype.md) <br/> |<span data-ttu-id="0d827-122">Содержит массив элементов для создания в папке, определяемой элементом [ParentFolderId (таржетфолдеридтипе)](parentfolderid-targetfolderidtype.md) .</span><span class="sxs-lookup"><span data-stu-id="0d827-122">Contains an array of items to create in the folder that is identified by the [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) element.</span></span>  <br/> |
|[<span data-ttu-id="0d827-123">респонсеобжектс</span><span class="sxs-lookup"><span data-stu-id="0d827-123">ResponseObjects</span></span>](responseobjects.md) <br/> |<span data-ttu-id="0d827-124">Содержит коллекцию всех объектов ответа, связанных с элементом в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="0d827-124">Contains a collection of all the response objects that are associated with an item in the Exchange store.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="0d827-125">Примечания</span><span class="sxs-lookup"><span data-stu-id="0d827-125">Remarks</span></span>

 <span data-ttu-id="0d827-126">**RemoveItem** является допустимым только для [митингканцеллатион](meetingcancellation.md).</span><span class="sxs-lookup"><span data-stu-id="0d827-126">**RemoveItem** is valid only for a [MeetingCancellation](meetingcancellation.md).</span></span> <span data-ttu-id="0d827-127">В противном случае возникает ошибка.</span><span class="sxs-lookup"><span data-stu-id="0d827-127">Otherwise, an error is thrown.</span></span>
  
> [!NOTE]
> <span data-ttu-id="0d827-128">[ItemClass](itemclass.md) для отмены собрания — IPM. Schedule. Meeting. Canceled.</span><span class="sxs-lookup"><span data-stu-id="0d827-128">The [ItemClass](itemclass.md) for a meeting cancellation is IPM.Schedule.Meeting.Canceled.</span></span> 
  
<span data-ttu-id="0d827-129">Чтобы удалить объект [свойство meetingrequest](meetingrequest.md) и связанный с ним [Календаритем](calendaritem.md), вместо **RemoveItem**используйте объект отклика [деклинеитем](declineitem.md) .</span><span class="sxs-lookup"><span data-stu-id="0d827-129">To remove a [MeetingRequest](meetingrequest.md) and the associated [CalendarItem](calendaritem.md), use the [DeclineItem](declineitem.md) response object instead of **RemoveItem**.</span></span>
  
 <span data-ttu-id="0d827-130">**RemoveItem** не поддерживается для делегированного доступа.</span><span class="sxs-lookup"><span data-stu-id="0d827-130">**RemoveItem** is not supported for delegate access.</span></span> 
  
<span data-ttu-id="0d827-131">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="0d827-131">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0d827-132">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="0d827-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0d827-133">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="0d827-133">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="0d827-134">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="0d827-134">Schema Name</span></span>  <br/> |<span data-ttu-id="0d827-135">Схема Types</span><span class="sxs-lookup"><span data-stu-id="0d827-135">Types schema</span></span>  <br/> |
|<span data-ttu-id="0d827-136">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="0d827-136">Validation File</span></span>  <br/> |<span data-ttu-id="0d827-137">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="0d827-137">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="0d827-138">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="0d827-138">Can be Empty</span></span>  <br/> |<span data-ttu-id="0d827-139">False</span><span class="sxs-lookup"><span data-stu-id="0d827-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0d827-140">См. также</span><span class="sxs-lookup"><span data-stu-id="0d827-140">See also</span></span>



- [<span data-ttu-id="0d827-141">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="0d827-141">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

