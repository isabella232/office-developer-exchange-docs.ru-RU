---
title: ReadItems (CalendarPermissionType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ReadItems
api_type:
- schema
ms.assetid: bec01982-26a1-4373-b1e6-2e0c838d83c4
description: Элемент ReadItems указывает, является ли пользователь имеет разрешение на чтение элементов внутри папки календаря. Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).
ms.openlocfilehash: 532b90c47cca7117a89d59e7012436268be9ebb0
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19834964"
---
# <a name="readitems-calendarpermissiontype"></a><span data-ttu-id="9cc7d-104">ReadItems (CalendarPermissionType)</span><span class="sxs-lookup"><span data-stu-id="9cc7d-104">ReadItems (CalendarPermissionType)</span></span>

<span data-ttu-id="9cc7d-105">Элемент **ReadItems** указывает, является ли пользователь имеет разрешение на чтение элементов внутри папки календаря.</span><span class="sxs-lookup"><span data-stu-id="9cc7d-105">The **ReadItems** element indicates whether a user has permission to read items within a Calendar folder.</span></span> <span data-ttu-id="9cc7d-106">Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="9cc7d-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<ReadItems>None or TimeOnly or TimeAndSubjectAndLocation or FullDetails</ReadItems>
```

 <span data-ttu-id="9cc7d-107">**CalendarPermissionReadAccessType**</span><span class="sxs-lookup"><span data-stu-id="9cc7d-107">**CalendarPermissionReadAccessType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9cc7d-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="9cc7d-108">Attributes and elements</span></span>

<span data-ttu-id="9cc7d-109">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="9cc7d-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9cc7d-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="9cc7d-110">Attributes</span></span>

<span data-ttu-id="9cc7d-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="9cc7d-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9cc7d-112">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="9cc7d-112">Child elements</span></span>

<span data-ttu-id="9cc7d-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="9cc7d-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="9cc7d-114">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="9cc7d-114">Parent elements</span></span>

|<span data-ttu-id="9cc7d-115">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="9cc7d-115">**Element**</span></span>|<span data-ttu-id="9cc7d-116">**Описание**</span><span class="sxs-lookup"><span data-stu-id="9cc7d-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9cc7d-117">CalendarPermission</span><span class="sxs-lookup"><span data-stu-id="9cc7d-117">CalendarPermission</span></span>](calendarpermission.md) <br/> |<span data-ttu-id="9cc7d-p103">Определяет доступ пользователя к папке календаря. Этот элемент появился в Exchange 2007 с пакетом обновления 1.</span><span class="sxs-lookup"><span data-stu-id="9cc7d-p103">Defines the access that a user has to a Calendar folder. This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="9cc7d-120">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="9cc7d-120">Text value</span></span>

<span data-ttu-id="9cc7d-121">В следующей таблице приведены возможные значения для элемента **ReadItems** .</span><span class="sxs-lookup"><span data-stu-id="9cc7d-121">The following table lists the possible values for the **ReadItems** element.</span></span> 
  
<span data-ttu-id="9cc7d-122">**ReadItems элемент текстовые значения**</span><span class="sxs-lookup"><span data-stu-id="9cc7d-122">**ReadItems element text values**</span></span>

|<span data-ttu-id="9cc7d-123">**Значение**</span><span class="sxs-lookup"><span data-stu-id="9cc7d-123">**Value**</span></span>|<span data-ttu-id="9cc7d-124">**Описание**</span><span class="sxs-lookup"><span data-stu-id="9cc7d-124">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="9cc7d-125">Нет</span><span class="sxs-lookup"><span data-stu-id="9cc7d-125">None</span></span>  <br/> |<span data-ttu-id="9cc7d-126">Указывает, что пользователь не имеет разрешения на просмотр элементов в календаре.</span><span class="sxs-lookup"><span data-stu-id="9cc7d-126">Indicates that the user does not have permission to view items in the calendar.</span></span>  <br/> |
|<span data-ttu-id="9cc7d-127">TimeOnly</span><span class="sxs-lookup"><span data-stu-id="9cc7d-127">TimeOnly</span></span>  <br/> |<span data-ttu-id="9cc7d-128">Указывает, что пользователь имеет разрешения на просмотр только занятости в календаре.</span><span class="sxs-lookup"><span data-stu-id="9cc7d-128">Indicates that the user has permission to view only free/busy time in the calendar.</span></span>  <br/> |
|<span data-ttu-id="9cc7d-129">TimeAndSubjectAndLocation</span><span class="sxs-lookup"><span data-stu-id="9cc7d-129">TimeAndSubjectAndLocation</span></span>  <br/> |<span data-ttu-id="9cc7d-130">Указывает, что пользователь имеет разрешения на просмотр сведений о доступности времени в календаре и тему и место встречи.</span><span class="sxs-lookup"><span data-stu-id="9cc7d-130">Indicates that the user has permission to view free/busy time in the calendar and the subject and location of appointments.</span></span>  <br/> |
|<span data-ttu-id="9cc7d-131">FullDetails</span><span class="sxs-lookup"><span data-stu-id="9cc7d-131">FullDetails</span></span>  <br/> |<span data-ttu-id="9cc7d-132">Указывает, что пользователь имеет разрешения на просмотр всех элементов в календаре, включая занятости и тему, местоположение и сведения о встречах.</span><span class="sxs-lookup"><span data-stu-id="9cc7d-132">Indicates that the user has permission to view all items in the calendar, including free/busy time and subject, location, and details of appointments.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="9cc7d-133">Замечания</span><span class="sxs-lookup"><span data-stu-id="9cc7d-133">Remarks</span></span>

<span data-ttu-id="9cc7d-134">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="9cc7d-134">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9cc7d-135">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="9cc7d-135">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9cc7d-136">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="9cc7d-136">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="9cc7d-137">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="9cc7d-137">Schema Name</span></span>  <br/> |<span data-ttu-id="9cc7d-138">Схема Types</span><span class="sxs-lookup"><span data-stu-id="9cc7d-138">Types schema</span></span>  <br/> |
|<span data-ttu-id="9cc7d-139">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="9cc7d-139">Validation File</span></span>  <br/> |<span data-ttu-id="9cc7d-140">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="9cc7d-140">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="9cc7d-141">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="9cc7d-141">Can be Empty</span></span>  <br/> |<span data-ttu-id="9cc7d-142">False</span><span class="sxs-lookup"><span data-stu-id="9cc7d-142">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9cc7d-143">См. также</span><span class="sxs-lookup"><span data-stu-id="9cc7d-143">See also</span></span>



- [<span data-ttu-id="9cc7d-144">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="9cc7d-144">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="9cc7d-145">Setting Folder-Level Permissions</span><span class="sxs-lookup"><span data-stu-id="9cc7d-145">Setting Folder-Level Permissions</span></span>](http://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

