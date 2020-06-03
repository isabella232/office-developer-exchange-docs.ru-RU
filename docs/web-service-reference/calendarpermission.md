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
ms.openlocfilehash: c43f75e6cf5abc2dce9af6c04122ec9a589dcd58
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529478"
---
# <a name="calendarpermission"></a><span data-ttu-id="cf3a7-104">календарпермиссион</span><span class="sxs-lookup"><span data-stu-id="cf3a7-104">CalendarPermission</span></span>

<span data-ttu-id="cf3a7-105">Элемент **календарпермиссион** определяет доступ пользователя к папке календаря.</span><span class="sxs-lookup"><span data-stu-id="cf3a7-105">The **CalendarPermission** element defines the access that a user has to a Calendar folder.</span></span> <span data-ttu-id="cf3a7-106">Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="cf3a7-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
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

 <span data-ttu-id="cf3a7-107">**календарпермиссионтипе**</span><span class="sxs-lookup"><span data-stu-id="cf3a7-107">**CalendarPermissionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="cf3a7-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="cf3a7-108">Attributes and elements</span></span>

<span data-ttu-id="cf3a7-109">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="cf3a7-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="cf3a7-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="cf3a7-110">Attributes</span></span>

<span data-ttu-id="cf3a7-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="cf3a7-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="cf3a7-112">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="cf3a7-112">Child elements</span></span>

|<span data-ttu-id="cf3a7-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="cf3a7-113">**Element**</span></span>|<span data-ttu-id="cf3a7-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="cf3a7-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="cf3a7-115">календарпермиссионлевел</span><span class="sxs-lookup"><span data-stu-id="cf3a7-115">CalendarPermissionLevel</span></span>](calendarpermissionlevel.md) <br/> |<span data-ttu-id="cf3a7-116">Представляет уровень разрешений, который пользователь имеет в папке "Календарь".</span><span class="sxs-lookup"><span data-stu-id="cf3a7-116">Represents the permission level that a user has on a Calendar folder.</span></span> <span data-ttu-id="cf3a7-117">Этот элемент появился в Exchange 2007 с пакетом обновления 1.</span><span class="sxs-lookup"><span data-stu-id="cf3a7-117">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="cf3a7-118">канкреатеитемс</span><span class="sxs-lookup"><span data-stu-id="cf3a7-118">CanCreateItems</span></span>](cancreateitems.md) <br/> |<span data-ttu-id="cf3a7-119">Указывает, имеет ли пользователь разрешение на создание элементов в папке.</span><span class="sxs-lookup"><span data-stu-id="cf3a7-119">Indicates whether a user has permission to create items in a folder.</span></span> <span data-ttu-id="cf3a7-120">Этот элемент появился в Exchange 2007 с пакетом обновления 1.</span><span class="sxs-lookup"><span data-stu-id="cf3a7-120">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="cf3a7-121">канкреатесубфолдерс</span><span class="sxs-lookup"><span data-stu-id="cf3a7-121">CanCreateSubFolders</span></span>](cancreatesubfolders.md) <br/> |<span data-ttu-id="cf3a7-122">Указывает, имеет ли пользователь разрешение на создание вложенных папок в папке.</span><span class="sxs-lookup"><span data-stu-id="cf3a7-122">Indicates whether a user has permission to create subfolders in a folder.</span></span> <span data-ttu-id="cf3a7-123">Этот элемент появился в Exchange 2007 с пакетом обновления 1.</span><span class="sxs-lookup"><span data-stu-id="cf3a7-123">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="cf3a7-124">делетеитемс</span><span class="sxs-lookup"><span data-stu-id="cf3a7-124">DeleteItems</span></span>](deleteitems.md) <br/> |<span data-ttu-id="cf3a7-125">Указывает, имеет ли пользователь разрешение на удаление элементов в папке.</span><span class="sxs-lookup"><span data-stu-id="cf3a7-125">Indicates whether a user has permission to delete items in a folder.</span></span> <span data-ttu-id="cf3a7-126">Этот элемент появился в Exchange 2007 с пакетом обновления 1.</span><span class="sxs-lookup"><span data-stu-id="cf3a7-126">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="cf3a7-127">едититемс</span><span class="sxs-lookup"><span data-stu-id="cf3a7-127">EditItems</span></span>](edititems.md) <br/> |<span data-ttu-id="cf3a7-128">Указывает, имеет ли пользователь разрешение на изменение элементов в папке.</span><span class="sxs-lookup"><span data-stu-id="cf3a7-128">Indicates whether a user has permission to edit items in a folder.</span></span> <span data-ttu-id="cf3a7-129">Этот элемент появился в Exchange 2007 с пакетом обновления 1.</span><span class="sxs-lookup"><span data-stu-id="cf3a7-129">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="cf3a7-130">исфолдерконтакт</span><span class="sxs-lookup"><span data-stu-id="cf3a7-130">IsFolderContact</span></span>](isfoldercontact.md) <br/> |<span data-ttu-id="cf3a7-131">Указывает, является ли пользователь контактом для папки.</span><span class="sxs-lookup"><span data-stu-id="cf3a7-131">Indicates whether a user is a contact for a folder.</span></span> <span data-ttu-id="cf3a7-132">Этот элемент появился в Exchange 2007 с пакетом обновления 1.</span><span class="sxs-lookup"><span data-stu-id="cf3a7-132">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="cf3a7-133">исфолдеровнер</span><span class="sxs-lookup"><span data-stu-id="cf3a7-133">IsFolderOwner</span></span>](isfolderowner.md) <br/> |<span data-ttu-id="cf3a7-134">Указывает, является ли пользователь владельцем папки.</span><span class="sxs-lookup"><span data-stu-id="cf3a7-134">Indicates whether a user is the owner of a folder.</span></span> <span data-ttu-id="cf3a7-135">Этот элемент появился в Exchange 2007 с пакетом обновления 1.</span><span class="sxs-lookup"><span data-stu-id="cf3a7-135">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="cf3a7-136">исфолдервисибле</span><span class="sxs-lookup"><span data-stu-id="cf3a7-136">IsFolderVisible</span></span>](isfoldervisible.md) <br/> |<span data-ttu-id="cf3a7-137">Указывает, может ли пользователь просматривать папку.</span><span class="sxs-lookup"><span data-stu-id="cf3a7-137">Indicates whether a user can view a folder.</span></span> <span data-ttu-id="cf3a7-138">Этот элемент появился в Exchange 2007 с пакетом обновления 1.</span><span class="sxs-lookup"><span data-stu-id="cf3a7-138">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="cf3a7-139">ReadItems (Календарпермиссионтипе)</span><span class="sxs-lookup"><span data-stu-id="cf3a7-139">ReadItems (CalendarPermissionType)</span></span>](readitems-calendarpermissiontype.md) <br/> |<span data-ttu-id="cf3a7-140">Указывает, имеет ли пользователь разрешение на чтение элементов в папке "Календарь".</span><span class="sxs-lookup"><span data-stu-id="cf3a7-140">Indicates whether a user has permission to read items within a calendar folder.</span></span> <span data-ttu-id="cf3a7-141">Этот элемент появился в Exchange 2007 с пакетом обновления 1.</span><span class="sxs-lookup"><span data-stu-id="cf3a7-141">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="cf3a7-142">UserId</span><span class="sxs-lookup"><span data-stu-id="cf3a7-142">UserId</span></span>](userid.md) <br/> |<span data-ttu-id="cf3a7-143">Определяет делегата или пользователя с разрешениями на доступ к папке.</span><span class="sxs-lookup"><span data-stu-id="cf3a7-143">Identifies a delegate user or a user who has folder access permissions.</span></span> <span data-ttu-id="cf3a7-144">Этот элемент появился в Exchange 2007 с пакетом обновления 1.</span><span class="sxs-lookup"><span data-stu-id="cf3a7-144">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="cf3a7-145">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="cf3a7-145">Parent elements</span></span>

|<span data-ttu-id="cf3a7-146">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="cf3a7-146">**Element**</span></span>|<span data-ttu-id="cf3a7-147">**Описание**</span><span class="sxs-lookup"><span data-stu-id="cf3a7-147">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="cf3a7-148">календарпермиссионс</span><span class="sxs-lookup"><span data-stu-id="cf3a7-148">CalendarPermissions</span></span>](calendarpermissions.md) <br/> |<span data-ttu-id="cf3a7-149">Содержит массив разрешений календаря для папки.</span><span class="sxs-lookup"><span data-stu-id="cf3a7-149">Contains an array of calendar permissions for a folder.</span></span> <span data-ttu-id="cf3a7-150">Этот элемент появился в Exchange 2007 с пакетом обновления 1.</span><span class="sxs-lookup"><span data-stu-id="cf3a7-150">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="cf3a7-151">Примечания</span><span class="sxs-lookup"><span data-stu-id="cf3a7-151">Remarks</span></span>

<span data-ttu-id="cf3a7-152">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="cf3a7-152">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="cf3a7-153">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="cf3a7-153">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="cf3a7-154">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="cf3a7-154">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="cf3a7-155">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="cf3a7-155">Schema Name</span></span>  <br/> |<span data-ttu-id="cf3a7-156">Схема Types</span><span class="sxs-lookup"><span data-stu-id="cf3a7-156">Types schema</span></span>  <br/> |
|<span data-ttu-id="cf3a7-157">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="cf3a7-157">Validation File</span></span>  <br/> |<span data-ttu-id="cf3a7-158">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="cf3a7-158">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="cf3a7-159">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="cf3a7-159">Can be Empty</span></span>  <br/> |<span data-ttu-id="cf3a7-160">False</span><span class="sxs-lookup"><span data-stu-id="cf3a7-160">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="cf3a7-161">См. также</span><span class="sxs-lookup"><span data-stu-id="cf3a7-161">See also</span></span>



- [<span data-ttu-id="cf3a7-162">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="cf3a7-162">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="cf3a7-163">Setting Folder-Level Permissions</span><span class="sxs-lookup"><span data-stu-id="cf3a7-163">Setting Folder-Level Permissions</span></span>](https://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

