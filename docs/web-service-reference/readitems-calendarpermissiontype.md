---
title: ReadItems (Календарпермиссионтипе)
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
description: Элемент ReadItems указывает, имеет ли пользователь разрешение на чтение элементов в папке "Календарь". Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).
ms.openlocfilehash: e040b643016781f9f890050f189191356f8d4f0b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44468301"
---
# <a name="readitems-calendarpermissiontype"></a><span data-ttu-id="82951-104">ReadItems (Календарпермиссионтипе)</span><span class="sxs-lookup"><span data-stu-id="82951-104">ReadItems (CalendarPermissionType)</span></span>

<span data-ttu-id="82951-105">Элемент **ReadItems** указывает, имеет ли пользователь разрешение на чтение элементов в папке "Календарь".</span><span class="sxs-lookup"><span data-stu-id="82951-105">The **ReadItems** element indicates whether a user has permission to read items within a Calendar folder.</span></span> <span data-ttu-id="82951-106">Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="82951-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<ReadItems>None or TimeOnly or TimeAndSubjectAndLocation or FullDetails</ReadItems>
```

 <span data-ttu-id="82951-107">**календарпермиссионреадакцесстипе**</span><span class="sxs-lookup"><span data-stu-id="82951-107">**CalendarPermissionReadAccessType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="82951-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="82951-108">Attributes and elements</span></span>

<span data-ttu-id="82951-109">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="82951-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="82951-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="82951-110">Attributes</span></span>

<span data-ttu-id="82951-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="82951-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="82951-112">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="82951-112">Child elements</span></span>

<span data-ttu-id="82951-113">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="82951-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="82951-114">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="82951-114">Parent elements</span></span>

|<span data-ttu-id="82951-115">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="82951-115">**Element**</span></span>|<span data-ttu-id="82951-116">**Описание**</span><span class="sxs-lookup"><span data-stu-id="82951-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="82951-117">календарпермиссион</span><span class="sxs-lookup"><span data-stu-id="82951-117">CalendarPermission</span></span>](calendarpermission.md) <br/> |<span data-ttu-id="82951-p103">Определяет доступ пользователя к папке календаря. Этот элемент появился в Exchange 2007 с пакетом обновления 1.</span><span class="sxs-lookup"><span data-stu-id="82951-p103">Defines the access that a user has to a Calendar folder. This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="82951-120">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="82951-120">Text value</span></span>

<span data-ttu-id="82951-121">В следующей таблице приведены возможные значения для элемента **ReadItems** .</span><span class="sxs-lookup"><span data-stu-id="82951-121">The following table lists the possible values for the **ReadItems** element.</span></span> 
  
<span data-ttu-id="82951-122">**Текстовые значения элементов ReadItems**</span><span class="sxs-lookup"><span data-stu-id="82951-122">**ReadItems element text values**</span></span>

|<span data-ttu-id="82951-123">**Значение**</span><span class="sxs-lookup"><span data-stu-id="82951-123">**Value**</span></span>|<span data-ttu-id="82951-124">**Описание**</span><span class="sxs-lookup"><span data-stu-id="82951-124">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="82951-125">Нет</span><span class="sxs-lookup"><span data-stu-id="82951-125">None</span></span>  <br/> |<span data-ttu-id="82951-126">Указывает, что у пользователя нет разрешения на просмотр элементов в календаре.</span><span class="sxs-lookup"><span data-stu-id="82951-126">Indicates that the user does not have permission to view items in the calendar.</span></span>  <br/> |
|<span data-ttu-id="82951-127">тимеонли</span><span class="sxs-lookup"><span data-stu-id="82951-127">TimeOnly</span></span>  <br/> |<span data-ttu-id="82951-128">Указывает, что у пользователя есть разрешение на просмотр сведений о занятости в календаре.</span><span class="sxs-lookup"><span data-stu-id="82951-128">Indicates that the user has permission to view only free/busy time in the calendar.</span></span>  <br/> |
|<span data-ttu-id="82951-129">тимеандсубжектандлокатион</span><span class="sxs-lookup"><span data-stu-id="82951-129">TimeAndSubjectAndLocation</span></span>  <br/> |<span data-ttu-id="82951-130">Указывает, что пользователь имеет разрешение на просмотр сведений о занятости в календаре и теме и местоположении встреч.</span><span class="sxs-lookup"><span data-stu-id="82951-130">Indicates that the user has permission to view free/busy time in the calendar and the subject and location of appointments.</span></span>  <br/> |
|<span data-ttu-id="82951-131">фуллдетаилс</span><span class="sxs-lookup"><span data-stu-id="82951-131">FullDetails</span></span>  <br/> |<span data-ttu-id="82951-132">Указывает, что у пользователя есть разрешение на просмотр всех элементов календаря, в том числе сведения о занятости, теме, местоположении и сведения о встречах.</span><span class="sxs-lookup"><span data-stu-id="82951-132">Indicates that the user has permission to view all items in the calendar, including free/busy time and subject, location, and details of appointments.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="82951-133">Примечания</span><span class="sxs-lookup"><span data-stu-id="82951-133">Remarks</span></span>

<span data-ttu-id="82951-134">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="82951-134">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="82951-135">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="82951-135">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="82951-136">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="82951-136">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="82951-137">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="82951-137">Schema Name</span></span>  <br/> |<span data-ttu-id="82951-138">Схема Types</span><span class="sxs-lookup"><span data-stu-id="82951-138">Types schema</span></span>  <br/> |
|<span data-ttu-id="82951-139">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="82951-139">Validation File</span></span>  <br/> |<span data-ttu-id="82951-140">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="82951-140">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="82951-141">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="82951-141">Can be Empty</span></span>  <br/> |<span data-ttu-id="82951-142">False</span><span class="sxs-lookup"><span data-stu-id="82951-142">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="82951-143">См. также</span><span class="sxs-lookup"><span data-stu-id="82951-143">See also</span></span>



- [<span data-ttu-id="82951-144">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="82951-144">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="82951-145">Setting Folder-Level Permissions</span><span class="sxs-lookup"><span data-stu-id="82951-145">Setting Folder-Level Permissions</span></span>](https://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

