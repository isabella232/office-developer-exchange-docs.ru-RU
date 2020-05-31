---
title: календарфолдер
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
description: Элемент Календарфолдер представляет папку, в которой в основном содержатся элементы календаря.
ms.openlocfilehash: 7dc90706eb45eb4617a68b9fdcf37669921af966
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761641"
---
# <a name="calendarfolder"></a><span data-ttu-id="425dc-103">календарфолдер</span><span class="sxs-lookup"><span data-stu-id="425dc-103">CalendarFolder</span></span>

<span data-ttu-id="425dc-104">Элемент **календарфолдер** представляет папку, в которой в основном содержатся элементы календаря.</span><span class="sxs-lookup"><span data-stu-id="425dc-104">The **CalendarFolder** element represents a folder that primarily contains calendar items.</span></span> 
  
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

 <span data-ttu-id="425dc-105">**календарфолдертипе**</span><span class="sxs-lookup"><span data-stu-id="425dc-105">**CalendarFolderType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="425dc-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="425dc-106">Attributes and elements</span></span>

<span data-ttu-id="425dc-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="425dc-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="425dc-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="425dc-108">Attributes</span></span>

<span data-ttu-id="425dc-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="425dc-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="425dc-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="425dc-110">Child elements</span></span>

|<span data-ttu-id="425dc-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="425dc-111">**Element**</span></span>|<span data-ttu-id="425dc-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="425dc-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="425dc-113">FolderId</span><span class="sxs-lookup"><span data-stu-id="425dc-113">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="425dc-114">Содержит идентификатор и ключ изменения папки.</span><span class="sxs-lookup"><span data-stu-id="425dc-114">Contains the identifier and change key of a folder.</span></span>  <br/> |
|[<span data-ttu-id="425dc-115">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="425dc-115">ParentFolderId</span></span>](parentfolderid.md) <br/> |<span data-ttu-id="425dc-116">Представляет идентификатор родительской папки, содержащей папку.</span><span class="sxs-lookup"><span data-stu-id="425dc-116">Represents the identifier of the parent folder that contains the folder.</span></span>  <br/> |
|[<span data-ttu-id="425dc-117">фолдеркласс</span><span class="sxs-lookup"><span data-stu-id="425dc-117">FolderClass</span></span>](folderclass.md) <br/> |<span data-ttu-id="425dc-118">Представляет класс папки для данной папки.</span><span class="sxs-lookup"><span data-stu-id="425dc-118">Represents the folder class for a given folder.</span></span>  <br/> |
|[<span data-ttu-id="425dc-119">DisplayName (строка)</span><span class="sxs-lookup"><span data-stu-id="425dc-119">DisplayName (string)</span></span>](displayname-string.md) <br/> |<span data-ttu-id="425dc-120">Содержит отображаемое имя папки.</span><span class="sxs-lookup"><span data-stu-id="425dc-120">Contains the display name of a folder.</span></span>  <br/> |
|[<span data-ttu-id="425dc-121">тоталкаунт</span><span class="sxs-lookup"><span data-stu-id="425dc-121">TotalCount</span></span>](totalcount.md) <br/> |<span data-ttu-id="425dc-122">Представляет общее количество элементов в заданной папке.</span><span class="sxs-lookup"><span data-stu-id="425dc-122">Represents the total count of items within a given folder.</span></span>  <br/> |
|[<span data-ttu-id="425dc-123">чилдфолдеркаунт</span><span class="sxs-lookup"><span data-stu-id="425dc-123">ChildFolderCount</span></span>](childfoldercount.md) <br/> |<span data-ttu-id="425dc-124">Представляет количество дочерних папок, содержащихся в папке.</span><span class="sxs-lookup"><span data-stu-id="425dc-124">Represents the number of child folders that are contained within a folder.</span></span> <span data-ttu-id="425dc-125">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="425dc-125">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="425dc-126">ExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="425dc-126">ExtendedProperty</span></span>](extendedproperty.md) <br/> |<span data-ttu-id="425dc-127">Определяет расширенные свойства для папок.</span><span class="sxs-lookup"><span data-stu-id="425dc-127">Identifies extended properties on folders.</span></span>  <br/> |
|[<span data-ttu-id="425dc-128">манажедфолдеринформатион</span><span class="sxs-lookup"><span data-stu-id="425dc-128">ManagedFolderInformation</span></span>](managedfolderinformation.md) <br/> |<span data-ttu-id="425dc-129">Содержит сведения об управляемой папке.</span><span class="sxs-lookup"><span data-stu-id="425dc-129">Contains information about a managed folder.</span></span>  <br/> |
|[<span data-ttu-id="425dc-130">еффективеригхтс</span><span class="sxs-lookup"><span data-stu-id="425dc-130">EffectiveRights</span></span>](effectiverights.md) <br/> |<span data-ttu-id="425dc-131">Содержит права клиента на основе параметров разрешений для элемента или папки.</span><span class="sxs-lookup"><span data-stu-id="425dc-131">Contains the client's rights based on the permission settings for the item or folder.</span></span> <span data-ttu-id="425dc-132">Этот элемент доступен только для чтения.</span><span class="sxs-lookup"><span data-stu-id="425dc-132">This element is read-only.</span></span>  <br/> |
|[<span data-ttu-id="425dc-133">Шаринжеффективеригхтс (Календарпермиссионреадакцесстипе)</span><span class="sxs-lookup"><span data-stu-id="425dc-133">SharingEffectiveRights (CalendarPermissionReadAccessType)</span></span>](sharingeffectiverights-calendarpermissionreadaccesstype.md) <br/> |<span data-ttu-id="425dc-134">Указывает разрешения, которые есть у пользователя для данных календаря, к которым предоставлен общий доступ.</span><span class="sxs-lookup"><span data-stu-id="425dc-134">Indicates the permissions that the user has for the calendar data that is being shared.</span></span>  <br/> |
|[<span data-ttu-id="425dc-135">PermissionSet (Календарпермиссионсеттипе)</span><span class="sxs-lookup"><span data-stu-id="425dc-135">PermissionSet (CalendarPermissionSetType)</span></span>](permissionset-calendarpermissionsettype.md) <br/> |<span data-ttu-id="425dc-136">Содержит все настроенные разрешения для папки "Календарь".</span><span class="sxs-lookup"><span data-stu-id="425dc-136">Contains all the configured permissions for a calendar folder.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="425dc-137">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="425dc-137">Parent elements</span></span>

|<span data-ttu-id="425dc-138">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="425dc-138">**Element**</span></span>|<span data-ttu-id="425dc-139">**Описание**</span><span class="sxs-lookup"><span data-stu-id="425dc-139">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="425dc-140">аппендтофолдерфиелд</span><span class="sxs-lookup"><span data-stu-id="425dc-140">AppendToFolderField</span></span>](appendtofolderfield.md) <br/> |<span data-ttu-id="425dc-141">Задает данные, добавляемые к свойству folder во время [операции операцию UpdateFolder](updatefolder-operation.md).</span><span class="sxs-lookup"><span data-stu-id="425dc-141">Specifies data to append to a folder property during an [UpdateFolder operation](updatefolder-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="425dc-142">Create (Фолдерсинк)</span><span class="sxs-lookup"><span data-stu-id="425dc-142">Create (FolderSync)</span></span>](create-foldersync.md) <br/> |<span data-ttu-id="425dc-143">Определяет одну папку для создания в локальном хранилище клиента.</span><span class="sxs-lookup"><span data-stu-id="425dc-143">Identifies a single folder to create in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="425dc-144">сетфолдерфиелд</span><span class="sxs-lookup"><span data-stu-id="425dc-144">SetFolderField</span></span>](setfolderfield.md) <br/> |<span data-ttu-id="425dc-145">Представляет обновление одного свойства папки в [операции операцию UpdateFolder](updatefolder-operation.md).</span><span class="sxs-lookup"><span data-stu-id="425dc-145">Represents an update to a single property on a folder in an [UpdateFolder operation](updatefolder-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="425dc-146">Обновление (Фолдерсинк)</span><span class="sxs-lookup"><span data-stu-id="425dc-146">Update (FolderSync)</span></span>](update-foldersync.md) <br/> |<span data-ttu-id="425dc-147">Определяет одну папку для обновления в локальном хранилище клиента.</span><span class="sxs-lookup"><span data-stu-id="425dc-147">Identifies a single folder to update in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="425dc-148">Folders</span><span class="sxs-lookup"><span data-stu-id="425dc-148">Folders</span></span>](folders-ex15websvcsotherref.md) <br/> |<span data-ttu-id="425dc-149">Содержит массив папок, используемых в операциях с папками.</span><span class="sxs-lookup"><span data-stu-id="425dc-149">Contains an array of folders that are used in folder operations.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="425dc-150">Примечания</span><span class="sxs-lookup"><span data-stu-id="425dc-150">Remarks</span></span>

<span data-ttu-id="425dc-151">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="425dc-151">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="425dc-152">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="425dc-152">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="425dc-153">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="425dc-153">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="425dc-154">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="425dc-154">Schema Name</span></span>  <br/> |<span data-ttu-id="425dc-155">Схема Types</span><span class="sxs-lookup"><span data-stu-id="425dc-155">Types schema</span></span>  <br/> |
|<span data-ttu-id="425dc-156">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="425dc-156">Validation File</span></span>  <br/> |<span data-ttu-id="425dc-157">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="425dc-157">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="425dc-158">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="425dc-158">Can be Empty</span></span>  <br/> |<span data-ttu-id="425dc-159">False</span><span class="sxs-lookup"><span data-stu-id="425dc-159">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="425dc-160">См. также</span><span class="sxs-lookup"><span data-stu-id="425dc-160">See also</span></span>



- [<span data-ttu-id="425dc-161">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="425dc-161">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

