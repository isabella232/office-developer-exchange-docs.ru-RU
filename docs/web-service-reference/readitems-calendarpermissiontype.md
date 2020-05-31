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
ms.openlocfilehash: 532b90c47cca7117a89d59e7012436268be9ebb0
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834964"
---
# <a name="readitems-calendarpermissiontype"></a><span data-ttu-id="2c0b7-104">ReadItems (Календарпермиссионтипе)</span><span class="sxs-lookup"><span data-stu-id="2c0b7-104">ReadItems (CalendarPermissionType)</span></span>

<span data-ttu-id="2c0b7-105">Элемент **ReadItems** указывает, имеет ли пользователь разрешение на чтение элементов в папке "Календарь".</span><span class="sxs-lookup"><span data-stu-id="2c0b7-105">The **ReadItems** element indicates whether a user has permission to read items within a Calendar folder.</span></span> <span data-ttu-id="2c0b7-106">Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="2c0b7-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<ReadItems>None or TimeOnly or TimeAndSubjectAndLocation or FullDetails</ReadItems>
```

 <span data-ttu-id="2c0b7-107">**календарпермиссионреадакцесстипе**</span><span class="sxs-lookup"><span data-stu-id="2c0b7-107">**CalendarPermissionReadAccessType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2c0b7-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="2c0b7-108">Attributes and elements</span></span>

<span data-ttu-id="2c0b7-109">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="2c0b7-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2c0b7-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="2c0b7-110">Attributes</span></span>

<span data-ttu-id="2c0b7-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="2c0b7-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2c0b7-112">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="2c0b7-112">Child elements</span></span>

<span data-ttu-id="2c0b7-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="2c0b7-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="2c0b7-114">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="2c0b7-114">Parent elements</span></span>

|<span data-ttu-id="2c0b7-115">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="2c0b7-115">**Element**</span></span>|<span data-ttu-id="2c0b7-116">**Описание**</span><span class="sxs-lookup"><span data-stu-id="2c0b7-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2c0b7-117">календарпермиссион</span><span class="sxs-lookup"><span data-stu-id="2c0b7-117">CalendarPermission</span></span>](calendarpermission.md) <br/> |<span data-ttu-id="2c0b7-p103">Определяет доступ пользователя к папке календаря. Этот элемент появился в Exchange 2007 с пакетом обновления 1.</span><span class="sxs-lookup"><span data-stu-id="2c0b7-p103">Defines the access that a user has to a Calendar folder. This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="2c0b7-120">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="2c0b7-120">Text value</span></span>

<span data-ttu-id="2c0b7-121">В следующей таблице приведены возможные значения для элемента **ReadItems** .</span><span class="sxs-lookup"><span data-stu-id="2c0b7-121">The following table lists the possible values for the **ReadItems** element.</span></span> 
  
<span data-ttu-id="2c0b7-122">**Текстовые значения элементов ReadItems**</span><span class="sxs-lookup"><span data-stu-id="2c0b7-122">**ReadItems element text values**</span></span>

|<span data-ttu-id="2c0b7-123">**Значение**</span><span class="sxs-lookup"><span data-stu-id="2c0b7-123">**Value**</span></span>|<span data-ttu-id="2c0b7-124">**Описание**</span><span class="sxs-lookup"><span data-stu-id="2c0b7-124">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="2c0b7-125">Нет</span><span class="sxs-lookup"><span data-stu-id="2c0b7-125">None</span></span>  <br/> |<span data-ttu-id="2c0b7-126">Указывает, что у пользователя нет разрешения на просмотр элементов в календаре.</span><span class="sxs-lookup"><span data-stu-id="2c0b7-126">Indicates that the user does not have permission to view items in the calendar.</span></span>  <br/> |
|<span data-ttu-id="2c0b7-127">тимеонли</span><span class="sxs-lookup"><span data-stu-id="2c0b7-127">TimeOnly</span></span>  <br/> |<span data-ttu-id="2c0b7-128">Указывает, что у пользователя есть разрешение на просмотр сведений о занятости в календаре.</span><span class="sxs-lookup"><span data-stu-id="2c0b7-128">Indicates that the user has permission to view only free/busy time in the calendar.</span></span>  <br/> |
|<span data-ttu-id="2c0b7-129">тимеандсубжектандлокатион</span><span class="sxs-lookup"><span data-stu-id="2c0b7-129">TimeAndSubjectAndLocation</span></span>  <br/> |<span data-ttu-id="2c0b7-130">Указывает, что пользователь имеет разрешение на просмотр сведений о занятости в календаре и теме и местоположении встреч.</span><span class="sxs-lookup"><span data-stu-id="2c0b7-130">Indicates that the user has permission to view free/busy time in the calendar and the subject and location of appointments.</span></span>  <br/> |
|<span data-ttu-id="2c0b7-131">фуллдетаилс</span><span class="sxs-lookup"><span data-stu-id="2c0b7-131">FullDetails</span></span>  <br/> |<span data-ttu-id="2c0b7-132">Указывает, что у пользователя есть разрешение на просмотр всех элементов календаря, в том числе сведения о занятости, теме, местоположении и сведения о встречах.</span><span class="sxs-lookup"><span data-stu-id="2c0b7-132">Indicates that the user has permission to view all items in the calendar, including free/busy time and subject, location, and details of appointments.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="2c0b7-133">Примечания</span><span class="sxs-lookup"><span data-stu-id="2c0b7-133">Remarks</span></span>

<span data-ttu-id="2c0b7-134">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="2c0b7-134">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2c0b7-135">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="2c0b7-135">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2c0b7-136">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="2c0b7-136">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="2c0b7-137">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="2c0b7-137">Schema Name</span></span>  <br/> |<span data-ttu-id="2c0b7-138">Схема Types</span><span class="sxs-lookup"><span data-stu-id="2c0b7-138">Types schema</span></span>  <br/> |
|<span data-ttu-id="2c0b7-139">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="2c0b7-139">Validation File</span></span>  <br/> |<span data-ttu-id="2c0b7-140">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="2c0b7-140">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="2c0b7-141">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="2c0b7-141">Can be Empty</span></span>  <br/> |<span data-ttu-id="2c0b7-142">False</span><span class="sxs-lookup"><span data-stu-id="2c0b7-142">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="2c0b7-143">См. также</span><span class="sxs-lookup"><span data-stu-id="2c0b7-143">See also</span></span>



- [<span data-ttu-id="2c0b7-144">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="2c0b7-144">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="2c0b7-145">Setting Folder-Level Permissions</span><span class="sxs-lookup"><span data-stu-id="2c0b7-145">Setting Folder-Level Permissions</span></span>](http://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

