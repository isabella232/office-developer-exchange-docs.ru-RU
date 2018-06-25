---
title: CalendarFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CalendarFolder
api_type:
- schema
ms.assetid: 48687a78-e757-4c04-9641-bf4302c6b565
description: Элемент CalendarFolder представляет папку, содержащую элементы календаря в первую очередь.
ms.openlocfilehash: 7dc90706eb45eb4617a68b9fdcf37669921af966
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761641"
---
# <a name="calendarfolder"></a><span data-ttu-id="2b7c3-103">CalendarFolder</span><span class="sxs-lookup"><span data-stu-id="2b7c3-103">CalendarFolder</span></span>

<span data-ttu-id="2b7c3-104">Элемент **CalendarFolder** представляет папку, содержащую элементы календаря в первую очередь.</span><span class="sxs-lookup"><span data-stu-id="2b7c3-104">The **CalendarFolder** element represents a folder that primarily contains calendar items.</span></span> 
  
```xml
<CalendarFolder>
   <FolderId/>
   <ParentFolderId/>
   <FolderClass/>
   <DisplayName/>
   <TotalCount/>
   <ChildFolderCount/>
   <ExtendedProperty/>
   <ManagedFolderInformation/>
   <EffectiveRights/>
   <SharingEffectiveRights/>
   <PermissionSet/>
</CalendarFolder>
```

 <span data-ttu-id="2b7c3-105">**CalendarFolderType**</span><span class="sxs-lookup"><span data-stu-id="2b7c3-105">**CalendarFolderType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2b7c3-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="2b7c3-106">Attributes and elements</span></span>

<span data-ttu-id="2b7c3-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="2b7c3-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2b7c3-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="2b7c3-108">Attributes</span></span>

<span data-ttu-id="2b7c3-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="2b7c3-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2b7c3-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="2b7c3-110">Child elements</span></span>

|<span data-ttu-id="2b7c3-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="2b7c3-111">**Element**</span></span>|<span data-ttu-id="2b7c3-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="2b7c3-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2b7c3-113">FolderId</span><span class="sxs-lookup"><span data-stu-id="2b7c3-113">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="2b7c3-114">Содержит идентификатор и ключ изменения папки.</span><span class="sxs-lookup"><span data-stu-id="2b7c3-114">Contains the identifier and change key of a folder.</span></span>  <br/> |
|[<span data-ttu-id="2b7c3-115">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="2b7c3-115">ParentFolderId</span></span>](parentfolderid.md) <br/> |<span data-ttu-id="2b7c3-116">Представляет идентификатор родительской папки, содержащей папку.</span><span class="sxs-lookup"><span data-stu-id="2b7c3-116">Represents the identifier of the parent folder that contains the folder.</span></span>  <br/> |
|[<span data-ttu-id="2b7c3-117">FolderClass</span><span class="sxs-lookup"><span data-stu-id="2b7c3-117">FolderClass</span></span>](folderclass.md) <br/> |<span data-ttu-id="2b7c3-118">Представляет класс папки для данной папки.</span><span class="sxs-lookup"><span data-stu-id="2b7c3-118">Represents the folder class for a given folder.</span></span>  <br/> |
|[<span data-ttu-id="2b7c3-119">Отображаемое имя (строка)</span><span class="sxs-lookup"><span data-stu-id="2b7c3-119">DisplayName (string)</span></span>](displayname-string.md) <br/> |<span data-ttu-id="2b7c3-120">Содержит отображаемое имя папки.</span><span class="sxs-lookup"><span data-stu-id="2b7c3-120">Contains the display name of a folder.</span></span>  <br/> |
|[<span data-ttu-id="2b7c3-121">TotalCount</span><span class="sxs-lookup"><span data-stu-id="2b7c3-121">TotalCount</span></span>](totalcount.md) <br/> |<span data-ttu-id="2b7c3-122">Представляет общее число элементов в указанной папке.</span><span class="sxs-lookup"><span data-stu-id="2b7c3-122">Represents the total count of items within a given folder.</span></span>  <br/> |
|[<span data-ttu-id="2b7c3-123">ChildFolderCount</span><span class="sxs-lookup"><span data-stu-id="2b7c3-123">ChildFolderCount</span></span>](childfoldercount.md) <br/> |<span data-ttu-id="2b7c3-124">Представляет число дочерних папок, содержащихся в папке.</span><span class="sxs-lookup"><span data-stu-id="2b7c3-124">Represents the number of child folders that are contained within a folder.</span></span> <span data-ttu-id="2b7c3-125">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2b7c3-125">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="2b7c3-126">ExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="2b7c3-126">ExtendedProperty</span></span>](extendedproperty.md) <br/> |<span data-ttu-id="2b7c3-127">Определяет расширенные свойства папки.</span><span class="sxs-lookup"><span data-stu-id="2b7c3-127">Identifies extended properties on folders.</span></span>  <br/> |
|[<span data-ttu-id="2b7c3-128">ManagedFolderInformation</span><span class="sxs-lookup"><span data-stu-id="2b7c3-128">ManagedFolderInformation</span></span>](managedfolderinformation.md) <br/> |<span data-ttu-id="2b7c3-129">Содержит сведения об управляемых папок.</span><span class="sxs-lookup"><span data-stu-id="2b7c3-129">Contains information about a managed folder.</span></span>  <br/> |
|[<span data-ttu-id="2b7c3-130">EffectiveRights</span><span class="sxs-lookup"><span data-stu-id="2b7c3-130">EffectiveRights</span></span>](effectiverights.md) <br/> |<span data-ttu-id="2b7c3-131">Содержит права клиента на основании параметров разрешений для элемента или папки.</span><span class="sxs-lookup"><span data-stu-id="2b7c3-131">Contains the client's rights based on the permission settings for the item or folder.</span></span> <span data-ttu-id="2b7c3-132">Этот элемент доступен только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2b7c3-132">This element is read-only.</span></span>  <br/> |
|[<span data-ttu-id="2b7c3-133">SharingEffectiveRights (CalendarPermissionReadAccessType)</span><span class="sxs-lookup"><span data-stu-id="2b7c3-133">SharingEffectiveRights (CalendarPermissionReadAccessType)</span></span>](sharingeffectiverights-calendarpermissionreadaccesstype.md) <br/> |<span data-ttu-id="2b7c3-134">Указывает разрешения, которые пользователь имеет для данных календаря общий.</span><span class="sxs-lookup"><span data-stu-id="2b7c3-134">Indicates the permissions that the user has for the calendar data that is being shared.</span></span>  <br/> |
|[<span data-ttu-id="2b7c3-135">PermissionSet (CalendarPermissionSetType)</span><span class="sxs-lookup"><span data-stu-id="2b7c3-135">PermissionSet (CalendarPermissionSetType)</span></span>](permissionset-calendarpermissionsettype.md) <br/> |<span data-ttu-id="2b7c3-136">Содержит все настроенные разрешения для папки «Календарь».</span><span class="sxs-lookup"><span data-stu-id="2b7c3-136">Contains all the configured permissions for a calendar folder.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="2b7c3-137">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="2b7c3-137">Parent elements</span></span>

|<span data-ttu-id="2b7c3-138">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="2b7c3-138">**Element**</span></span>|<span data-ttu-id="2b7c3-139">**Описание**</span><span class="sxs-lookup"><span data-stu-id="2b7c3-139">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2b7c3-140">AppendToFolderField</span><span class="sxs-lookup"><span data-stu-id="2b7c3-140">AppendToFolderField</span></span>](appendtofolderfield.md) <br/> |<span data-ttu-id="2b7c3-141">Указывает данные для добавления к папке свойство во время [операции UpdateFolder](updatefolder-operation.md).</span><span class="sxs-lookup"><span data-stu-id="2b7c3-141">Specifies data to append to a folder property during an [UpdateFolder operation](updatefolder-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="2b7c3-142">Создание (FolderSync)</span><span class="sxs-lookup"><span data-stu-id="2b7c3-142">Create (FolderSync)</span></span>](create-foldersync.md) <br/> |<span data-ttu-id="2b7c3-143">Определяет одну папку для создания в локальном хранилище клиента.</span><span class="sxs-lookup"><span data-stu-id="2b7c3-143">Identifies a single folder to create in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="2b7c3-144">SetFolderField</span><span class="sxs-lookup"><span data-stu-id="2b7c3-144">SetFolderField</span></span>](setfolderfield.md) <br/> |<span data-ttu-id="2b7c3-145">Представляет обновление для одного свойства папки в рамках одной [операции UpdateFolder](updatefolder-operation.md).</span><span class="sxs-lookup"><span data-stu-id="2b7c3-145">Represents an update to a single property on a folder in an [UpdateFolder operation](updatefolder-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="2b7c3-146">Обновление (FolderSync)</span><span class="sxs-lookup"><span data-stu-id="2b7c3-146">Update (FolderSync)</span></span>](update-foldersync.md) <br/> |<span data-ttu-id="2b7c3-147">Определяет одну папку для обновления в локальном хранилище клиента.</span><span class="sxs-lookup"><span data-stu-id="2b7c3-147">Identifies a single folder to update in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="2b7c3-148">Папки</span><span class="sxs-lookup"><span data-stu-id="2b7c3-148">Folders</span></span>](folders-ex15websvcsotherref.md) <br/> |<span data-ttu-id="2b7c3-149">Содержит набор папок, используемых в операциях папки.</span><span class="sxs-lookup"><span data-stu-id="2b7c3-149">Contains an array of folders that are used in folder operations.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="2b7c3-150">Замечания</span><span class="sxs-lookup"><span data-stu-id="2b7c3-150">Remarks</span></span>

<span data-ttu-id="2b7c3-151">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="2b7c3-151">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2b7c3-152">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="2b7c3-152">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2b7c3-153">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="2b7c3-153">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="2b7c3-154">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="2b7c3-154">Schema Name</span></span>  <br/> |<span data-ttu-id="2b7c3-155">Схема Types</span><span class="sxs-lookup"><span data-stu-id="2b7c3-155">Types schema</span></span>  <br/> |
|<span data-ttu-id="2b7c3-156">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="2b7c3-156">Validation File</span></span>  <br/> |<span data-ttu-id="2b7c3-157">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="2b7c3-157">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="2b7c3-158">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="2b7c3-158">Can be Empty</span></span>  <br/> |<span data-ttu-id="2b7c3-159">False</span><span class="sxs-lookup"><span data-stu-id="2b7c3-159">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="2b7c3-160">См. также</span><span class="sxs-lookup"><span data-stu-id="2b7c3-160">See also</span></span>



- [<span data-ttu-id="2b7c3-161">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="2b7c3-161">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

