---
title: CalendarPermissions
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CalendarPermissions
api_type:
- schema
ms.assetid: 9b659d83-45fb-42a2-b052-5bc4dbe3854d
description: Элемент CalendarPermissions содержит массив календаря разрешений на папку. Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).
ms.openlocfilehash: 3dee635e4449cbb3717f5d2fab8838f3e43102a4
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761653"
---
# <a name="calendarpermissions"></a><span data-ttu-id="3563f-104">CalendarPermissions</span><span class="sxs-lookup"><span data-stu-id="3563f-104">CalendarPermissions</span></span>

<span data-ttu-id="3563f-105">Элемент **CalendarPermissions** содержит массив календаря разрешений на папку.</span><span class="sxs-lookup"><span data-stu-id="3563f-105">The **CalendarPermissions** element contains an array of calendar permissions for a folder.</span></span> <span data-ttu-id="3563f-106">Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="3563f-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<CalendarPermissions>
   <PermissionSet/>
</CalendarPermissions>
```

 <span data-ttu-id="3563f-107">**ArrayOfCalendarPermissionsType**</span><span class="sxs-lookup"><span data-stu-id="3563f-107">**ArrayOfCalendarPermissionsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3563f-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="3563f-108">Attributes and elements</span></span>

<span data-ttu-id="3563f-109">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="3563f-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3563f-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="3563f-110">Attributes</span></span>

<span data-ttu-id="3563f-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="3563f-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3563f-112">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="3563f-112">Child elements</span></span>

|<span data-ttu-id="3563f-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="3563f-113">**Element**</span></span>|<span data-ttu-id="3563f-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="3563f-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3563f-115">CalendarPermission</span><span class="sxs-lookup"><span data-stu-id="3563f-115">CalendarPermission</span></span>](calendarpermission.md) <br/> |<span data-ttu-id="3563f-116">Определяет делегат пользователь имеет доступ к папке календаря.</span><span class="sxs-lookup"><span data-stu-id="3563f-116">Defines the access that a delegate user has to a calendar folder.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="3563f-117">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="3563f-117">Parent elements</span></span>

|<span data-ttu-id="3563f-118">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="3563f-118">**Element**</span></span>|<span data-ttu-id="3563f-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="3563f-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3563f-120">PermissionSet (CalendarPermissionSetType)</span><span class="sxs-lookup"><span data-stu-id="3563f-120">PermissionSet (CalendarPermissionSetType)</span></span>](permissionset-calendarpermissionsettype.md) <br/> |<span data-ttu-id="3563f-121">Содержит все настроенные разрешения для папки «Календарь».</span><span class="sxs-lookup"><span data-stu-id="3563f-121">Contains all the configured permissions for a calendar folder.</span></span> <span data-ttu-id="3563f-122">Этот элемент появился в Exchange 2007 с пакетом обновления 1.</span><span class="sxs-lookup"><span data-stu-id="3563f-122">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="3563f-123">Замечания</span><span class="sxs-lookup"><span data-stu-id="3563f-123">Remarks</span></span>

<span data-ttu-id="3563f-124">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="3563f-124">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3563f-125">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="3563f-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3563f-126">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="3563f-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="3563f-127">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="3563f-127">Schema Name</span></span>  <br/> |<span data-ttu-id="3563f-128">Схема Types</span><span class="sxs-lookup"><span data-stu-id="3563f-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="3563f-129">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="3563f-129">Validation File</span></span>  <br/> |<span data-ttu-id="3563f-130">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="3563f-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="3563f-131">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="3563f-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="3563f-132">False</span><span class="sxs-lookup"><span data-stu-id="3563f-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3563f-133">См. также</span><span class="sxs-lookup"><span data-stu-id="3563f-133">See also</span></span>



- [<span data-ttu-id="3563f-134">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="3563f-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="3563f-135">Setting Folder-Level Permissions</span><span class="sxs-lookup"><span data-stu-id="3563f-135">Setting Folder-Level Permissions</span></span>](http://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

