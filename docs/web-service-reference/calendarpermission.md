---
title: календарпермиссион
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CalendarPermission
api_type:
- schema
ms.assetid: 3aafb221-a04b-41f6-804e-eda810f1ba28
description: Элемент Календарпермиссион определяет доступ пользователя к папке календаря. Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).
ms.openlocfilehash: 7f6ceb6895add3fdd82cdd595463b3a80db822e5
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761649"
---
# <a name="calendarpermission"></a><span data-ttu-id="6f2e8-104">календарпермиссион</span><span class="sxs-lookup"><span data-stu-id="6f2e8-104">CalendarPermission</span></span>

<span data-ttu-id="6f2e8-105">Элемент **календарпермиссион** определяет доступ пользователя к папке календаря.</span><span class="sxs-lookup"><span data-stu-id="6f2e8-105">The **CalendarPermission** element defines the access that a user has to a Calendar folder.</span></span> <span data-ttu-id="6f2e8-106">Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="6f2e8-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<Permission>
   <CalendarPermissionLevel/>
   <CanCreateItems/>
   <CanCreateSubfolders/>
   <IsFolderOwner/>
   <IsFolderVisible/>
   <IsFolderContact/>
   <EditItems/>
   <DeleteItems/>
   <ReadItems/>
   <UserId/>
</Permission>
```

 <span data-ttu-id="6f2e8-107">**календарпермиссионтипе**</span><span class="sxs-lookup"><span data-stu-id="6f2e8-107">**CalendarPermissionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6f2e8-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="6f2e8-108">Attributes and elements</span></span>

<span data-ttu-id="6f2e8-109">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="6f2e8-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6f2e8-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="6f2e8-110">Attributes</span></span>

<span data-ttu-id="6f2e8-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="6f2e8-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6f2e8-112">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="6f2e8-112">Child elements</span></span>

|<span data-ttu-id="6f2e8-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="6f2e8-113">**Element**</span></span>|<span data-ttu-id="6f2e8-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="6f2e8-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6f2e8-115">календарпермиссионлевел</span><span class="sxs-lookup"><span data-stu-id="6f2e8-115">CalendarPermissionLevel</span></span>](calendarpermissionlevel.md) <br/> |<span data-ttu-id="6f2e8-116">Представляет уровень разрешений, который пользователь имеет в папке "Календарь".</span><span class="sxs-lookup"><span data-stu-id="6f2e8-116">Represents the permission level that a user has on a Calendar folder.</span></span> <span data-ttu-id="6f2e8-117">Этот элемент появился в Exchange 2007 с пакетом обновления 1.</span><span class="sxs-lookup"><span data-stu-id="6f2e8-117">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="6f2e8-118">канкреатеитемс</span><span class="sxs-lookup"><span data-stu-id="6f2e8-118">CanCreateItems</span></span>](cancreateitems.md) <br/> |<span data-ttu-id="6f2e8-119">Указывает, имеет ли пользователь разрешение на создание элементов в папке.</span><span class="sxs-lookup"><span data-stu-id="6f2e8-119">Indicates whether a user has permission to create items in a folder.</span></span> <span data-ttu-id="6f2e8-120">Этот элемент появился в Exchange 2007 с пакетом обновления 1.</span><span class="sxs-lookup"><span data-stu-id="6f2e8-120">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="6f2e8-121">канкреатесубфолдерс</span><span class="sxs-lookup"><span data-stu-id="6f2e8-121">CanCreateSubFolders</span></span>](cancreatesubfolders.md) <br/> |<span data-ttu-id="6f2e8-122">Указывает, имеет ли пользователь разрешение на создание вложенных папок в папке.</span><span class="sxs-lookup"><span data-stu-id="6f2e8-122">Indicates whether a user has permission to create subfolders in a folder.</span></span> <span data-ttu-id="6f2e8-123">Этот элемент появился в Exchange 2007 с пакетом обновления 1.</span><span class="sxs-lookup"><span data-stu-id="6f2e8-123">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="6f2e8-124">делетеитемс</span><span class="sxs-lookup"><span data-stu-id="6f2e8-124">DeleteItems</span></span>](deleteitems.md) <br/> |<span data-ttu-id="6f2e8-125">Указывает, имеет ли пользователь разрешение на удаление элементов в папке.</span><span class="sxs-lookup"><span data-stu-id="6f2e8-125">Indicates whether a user has permission to delete items in a folder.</span></span> <span data-ttu-id="6f2e8-126">Этот элемент появился в Exchange 2007 с пакетом обновления 1.</span><span class="sxs-lookup"><span data-stu-id="6f2e8-126">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="6f2e8-127">едититемс</span><span class="sxs-lookup"><span data-stu-id="6f2e8-127">EditItems</span></span>](edititems.md) <br/> |<span data-ttu-id="6f2e8-128">Указывает, имеет ли пользователь разрешение на изменение элементов в папке.</span><span class="sxs-lookup"><span data-stu-id="6f2e8-128">Indicates whether a user has permission to edit items in a folder.</span></span> <span data-ttu-id="6f2e8-129">Этот элемент появился в Exchange 2007 с пакетом обновления 1.</span><span class="sxs-lookup"><span data-stu-id="6f2e8-129">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="6f2e8-130">исфолдерконтакт</span><span class="sxs-lookup"><span data-stu-id="6f2e8-130">IsFolderContact</span></span>](isfoldercontact.md) <br/> |<span data-ttu-id="6f2e8-131">Указывает, является ли пользователь контактом для папки.</span><span class="sxs-lookup"><span data-stu-id="6f2e8-131">Indicates whether a user is a contact for a folder.</span></span> <span data-ttu-id="6f2e8-132">Этот элемент появился в Exchange 2007 с пакетом обновления 1.</span><span class="sxs-lookup"><span data-stu-id="6f2e8-132">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="6f2e8-133">исфолдеровнер</span><span class="sxs-lookup"><span data-stu-id="6f2e8-133">IsFolderOwner</span></span>](isfolderowner.md) <br/> |<span data-ttu-id="6f2e8-134">Указывает, является ли пользователь владельцем папки.</span><span class="sxs-lookup"><span data-stu-id="6f2e8-134">Indicates whether a user is the owner of a folder.</span></span> <span data-ttu-id="6f2e8-135">Этот элемент появился в Exchange 2007 с пакетом обновления 1.</span><span class="sxs-lookup"><span data-stu-id="6f2e8-135">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="6f2e8-136">исфолдервисибле</span><span class="sxs-lookup"><span data-stu-id="6f2e8-136">IsFolderVisible</span></span>](isfoldervisible.md) <br/> |<span data-ttu-id="6f2e8-137">Указывает, может ли пользователь просматривать папку.</span><span class="sxs-lookup"><span data-stu-id="6f2e8-137">Indicates whether a user can view a folder.</span></span> <span data-ttu-id="6f2e8-138">Этот элемент появился в Exchange 2007 с пакетом обновления 1.</span><span class="sxs-lookup"><span data-stu-id="6f2e8-138">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="6f2e8-139">ReadItems (Календарпермиссионтипе)</span><span class="sxs-lookup"><span data-stu-id="6f2e8-139">ReadItems (CalendarPermissionType)</span></span>](readitems-calendarpermissiontype.md) <br/> |<span data-ttu-id="6f2e8-140">Указывает, имеет ли пользователь разрешение на чтение элементов в папке "Календарь".</span><span class="sxs-lookup"><span data-stu-id="6f2e8-140">Indicates whether a user has permission to read items within a calendar folder.</span></span> <span data-ttu-id="6f2e8-141">Этот элемент появился в Exchange 2007 с пакетом обновления 1.</span><span class="sxs-lookup"><span data-stu-id="6f2e8-141">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="6f2e8-142">UserId</span><span class="sxs-lookup"><span data-stu-id="6f2e8-142">UserId</span></span>](userid.md) <br/> |<span data-ttu-id="6f2e8-143">Определяет делегата или пользователя с разрешениями на доступ к папке.</span><span class="sxs-lookup"><span data-stu-id="6f2e8-143">Identifies a delegate user or a user who has folder access permissions.</span></span> <span data-ttu-id="6f2e8-144">Этот элемент появился в Exchange 2007 с пакетом обновления 1.</span><span class="sxs-lookup"><span data-stu-id="6f2e8-144">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="6f2e8-145">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="6f2e8-145">Parent elements</span></span>

|<span data-ttu-id="6f2e8-146">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="6f2e8-146">**Element**</span></span>|<span data-ttu-id="6f2e8-147">**Описание**</span><span class="sxs-lookup"><span data-stu-id="6f2e8-147">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6f2e8-148">календарпермиссионс</span><span class="sxs-lookup"><span data-stu-id="6f2e8-148">CalendarPermissions</span></span>](calendarpermissions.md) <br/> |<span data-ttu-id="6f2e8-149">Содержит массив разрешений календаря для папки.</span><span class="sxs-lookup"><span data-stu-id="6f2e8-149">Contains an array of calendar permissions for a folder.</span></span> <span data-ttu-id="6f2e8-150">Этот элемент появился в Exchange 2007 с пакетом обновления 1.</span><span class="sxs-lookup"><span data-stu-id="6f2e8-150">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="6f2e8-151">Примечания</span><span class="sxs-lookup"><span data-stu-id="6f2e8-151">Remarks</span></span>

<span data-ttu-id="6f2e8-152">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="6f2e8-152">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6f2e8-153">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="6f2e8-153">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6f2e8-154">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="6f2e8-154">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="6f2e8-155">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="6f2e8-155">Schema Name</span></span>  <br/> |<span data-ttu-id="6f2e8-156">Схема Types</span><span class="sxs-lookup"><span data-stu-id="6f2e8-156">Types schema</span></span>  <br/> |
|<span data-ttu-id="6f2e8-157">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="6f2e8-157">Validation File</span></span>  <br/> |<span data-ttu-id="6f2e8-158">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="6f2e8-158">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="6f2e8-159">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="6f2e8-159">Can be Empty</span></span>  <br/> |<span data-ttu-id="6f2e8-160">False</span><span class="sxs-lookup"><span data-stu-id="6f2e8-160">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6f2e8-161">См. также</span><span class="sxs-lookup"><span data-stu-id="6f2e8-161">See also</span></span>



- [<span data-ttu-id="6f2e8-162">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="6f2e8-162">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="6f2e8-163">Setting Folder-Level Permissions</span><span class="sxs-lookup"><span data-stu-id="6f2e8-163">Setting Folder-Level Permissions</span></span>](http://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

