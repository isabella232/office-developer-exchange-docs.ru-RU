---
title: SharingEffectiveRights (CalendarPermissionReadAccessType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SharingEffectiveRights
api_type:
- schema
ms.assetid: b519f642-a9ef-4300-92e6-ed8202855fde
description: Элемент SharingEffectiveRights указывает разрешения, которые пользователь имеет для данных календаря общий.
ms.openlocfilehash: e7d2aa061650c33d27de042ae8a6348f9a7d3430
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835480"
---
# <a name="sharingeffectiverights-calendarpermissionreadaccesstype"></a><span data-ttu-id="352c9-103">SharingEffectiveRights (CalendarPermissionReadAccessType)</span><span class="sxs-lookup"><span data-stu-id="352c9-103">SharingEffectiveRights (CalendarPermissionReadAccessType)</span></span>

<span data-ttu-id="352c9-104">Элемент **SharingEffectiveRights** указывает разрешения, которые пользователь имеет для данных календаря общий.</span><span class="sxs-lookup"><span data-stu-id="352c9-104">The **SharingEffectiveRights** element indicates the permissions that the user has for the calendar data that is being shared.</span></span> 
  
```XML
<SharingEffectiveRights>None | TimeOnly | TimeAndSubjectAndLocation | FullDetails</SharingEffectiveRights>
```

 <span data-ttu-id="352c9-105">**CalendarPermissionReadAccessType**</span><span class="sxs-lookup"><span data-stu-id="352c9-105">**CalendarPermissionReadAccessType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="352c9-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="352c9-106">Attributes and elements</span></span>

<span data-ttu-id="352c9-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="352c9-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="352c9-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="352c9-108">Attributes</span></span>

<span data-ttu-id="352c9-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="352c9-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="352c9-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="352c9-110">Child elements</span></span>

<span data-ttu-id="352c9-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="352c9-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="352c9-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="352c9-112">Parent elements</span></span>

|<span data-ttu-id="352c9-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="352c9-113">**Element**</span></span>|<span data-ttu-id="352c9-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="352c9-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="352c9-115">CalendarFolder</span><span class="sxs-lookup"><span data-stu-id="352c9-115">CalendarFolder</span></span>](calendarfolder.md) <br/> |<span data-ttu-id="352c9-116">Представляет папку, содержащую элементы календаря в первую очередь.</span><span class="sxs-lookup"><span data-stu-id="352c9-116">Represents a folder that primarily contains calendar items.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="352c9-117">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="352c9-117">Text value</span></span>

<span data-ttu-id="352c9-118">В следующей таблице приведены возможные значения для элемента **SharingEffectiveRights** .</span><span class="sxs-lookup"><span data-stu-id="352c9-118">The following table lists the possible values for the **SharingEffectiveRights** element.</span></span> 
  
|<span data-ttu-id="352c9-119">**Значение**</span><span class="sxs-lookup"><span data-stu-id="352c9-119">**Value**</span></span>|<span data-ttu-id="352c9-120">**Описание**</span><span class="sxs-lookup"><span data-stu-id="352c9-120">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="352c9-121">Нет</span><span class="sxs-lookup"><span data-stu-id="352c9-121">None</span></span>  <br/> |<span data-ttu-id="352c9-122">Указывает, что пользователь не имеет разрешения на просмотр элементов в календаре.</span><span class="sxs-lookup"><span data-stu-id="352c9-122">Indicates that the user does not have permission to view items in the calendar.</span></span>  <br/> |
|<span data-ttu-id="352c9-123">TimeOnly</span><span class="sxs-lookup"><span data-stu-id="352c9-123">TimeOnly</span></span>  <br/> |<span data-ttu-id="352c9-124">Указывает, что пользователь имеет разрешения на просмотр только занятости в календаре.</span><span class="sxs-lookup"><span data-stu-id="352c9-124">Indicates that the user has permission to view only free/busy time in the calendar.</span></span>  <br/> |
|<span data-ttu-id="352c9-125">TimeAndSubjectAndLocation</span><span class="sxs-lookup"><span data-stu-id="352c9-125">TimeAndSubjectAndLocation</span></span>  <br/> |<span data-ttu-id="352c9-126">Указывает, что пользователь имеет разрешения на просмотр сведений о доступности времени в календаре и тему и место встречи.</span><span class="sxs-lookup"><span data-stu-id="352c9-126">Indicates that the user has permission to view free/busy time in the calendar and the subject and location of appointments.</span></span>  <br/> |
|<span data-ttu-id="352c9-127">FullDetails</span><span class="sxs-lookup"><span data-stu-id="352c9-127">FullDetails</span></span>  <br/> |<span data-ttu-id="352c9-128">Указывает, что пользователь имеет разрешения на просмотр всех элементов в календаре, включая занятости и тему, местоположение и сведения о встречах.</span><span class="sxs-lookup"><span data-stu-id="352c9-128">Indicates that the user has permission to view all items in the calendar, including free/busy time and subject, location, and details of appointments.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="352c9-129">Замечания</span><span class="sxs-lookup"><span data-stu-id="352c9-129">Remarks</span></span>

<span data-ttu-id="352c9-130">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="352c9-130">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="352c9-131">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="352c9-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="352c9-132">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="352c9-132">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="352c9-133">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="352c9-133">Schema Name</span></span>  <br/> |<span data-ttu-id="352c9-134">Схема Types</span><span class="sxs-lookup"><span data-stu-id="352c9-134">Types schema</span></span>  <br/> |
|<span data-ttu-id="352c9-135">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="352c9-135">Validation File</span></span>  <br/> |<span data-ttu-id="352c9-136">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="352c9-136">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="352c9-137">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="352c9-137">Can be Empty</span></span>  <br/> |<span data-ttu-id="352c9-138">False</span><span class="sxs-lookup"><span data-stu-id="352c9-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="352c9-139">См. также</span><span class="sxs-lookup"><span data-stu-id="352c9-139">See also</span></span>



- [<span data-ttu-id="352c9-140">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="352c9-140">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

