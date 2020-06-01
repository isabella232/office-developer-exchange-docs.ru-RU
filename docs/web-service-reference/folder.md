---
title: Folder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Folder
api_type:
- schema
ms.assetid: 812948d8-c7db-45ce-bb3a-77233a53a974
description: Элемент Folder определяет папку для создания, получения, поиска, синхронизации или обновления.
ms.openlocfilehash: 156813b3f7ecc6a2e1437f473ae1daa76b138e6e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457251"
---
# <a name="folder"></a><span data-ttu-id="ad7a7-103">Folder</span><span class="sxs-lookup"><span data-stu-id="ad7a7-103">Folder</span></span>

<span data-ttu-id="ad7a7-104">Элемент **Folder** определяет папку для создания, получения, поиска, синхронизации или обновления.</span><span class="sxs-lookup"><span data-stu-id="ad7a7-104">The **Folder** element defines a folder to create, get, find, synchronize, or update.</span></span> 
  
```xml
<Folder>
   <FolderId/>
   <ParentFolderId/>
   <FolderClass/>
   <DisplayName/>
   <TotalCount/>
   <ChildFolderCount/>
   <ExtendedProperty/>
   <ManagedFolderInformation/>
   <UnreadCount/>
   <PermissionSet/>
   <EffectiveRights/>
</Folder>
```

 <span data-ttu-id="ad7a7-105">**фолдертипе**</span><span class="sxs-lookup"><span data-stu-id="ad7a7-105">**FolderType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ad7a7-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="ad7a7-106">Attributes and elements</span></span>

<span data-ttu-id="ad7a7-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="ad7a7-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ad7a7-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="ad7a7-108">Attributes</span></span>

<span data-ttu-id="ad7a7-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="ad7a7-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ad7a7-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="ad7a7-110">Child elements</span></span>

|<span data-ttu-id="ad7a7-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="ad7a7-111">**Element**</span></span>|<span data-ttu-id="ad7a7-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="ad7a7-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ad7a7-113">FolderId</span><span class="sxs-lookup"><span data-stu-id="ad7a7-113">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="ad7a7-114">Содержит идентификатор и ключ изменения папки.</span><span class="sxs-lookup"><span data-stu-id="ad7a7-114">Contains the identifier and change key of a folder.</span></span>  <br/> |
|[<span data-ttu-id="ad7a7-115">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="ad7a7-115">ParentFolderId</span></span>](parentfolderid.md) <br/> |<span data-ttu-id="ad7a7-116">Представляет идентификатор родительской папки, содержащей папку.</span><span class="sxs-lookup"><span data-stu-id="ad7a7-116">Represents the identifier of the parent folder that contains the folder.</span></span>  <br/> |
|[<span data-ttu-id="ad7a7-117">фолдеркласс</span><span class="sxs-lookup"><span data-stu-id="ad7a7-117">FolderClass</span></span>](folderclass.md) <br/> |<span data-ttu-id="ad7a7-118">Представляет класс папки для данной папки.</span><span class="sxs-lookup"><span data-stu-id="ad7a7-118">Represents the folder class for a given folder.</span></span>  <br/> |
|[<span data-ttu-id="ad7a7-119">DisplayName (строка)</span><span class="sxs-lookup"><span data-stu-id="ad7a7-119">DisplayName (string)</span></span>](displayname-string.md) <br/> |<span data-ttu-id="ad7a7-120">Содержит отображаемое имя папки.</span><span class="sxs-lookup"><span data-stu-id="ad7a7-120">Contains the display name of a folder.</span></span>  <br/> |
|[<span data-ttu-id="ad7a7-121">тоталкаунт</span><span class="sxs-lookup"><span data-stu-id="ad7a7-121">TotalCount</span></span>](totalcount.md) <br/> |<span data-ttu-id="ad7a7-122">Представляет общее количество элементов в заданной папке.</span><span class="sxs-lookup"><span data-stu-id="ad7a7-122">Represents the total count of items within a given folder.</span></span>  <br/> |
|[<span data-ttu-id="ad7a7-123">чилдфолдеркаунт</span><span class="sxs-lookup"><span data-stu-id="ad7a7-123">ChildFolderCount</span></span>](childfoldercount.md) <br/> |<span data-ttu-id="ad7a7-124">Представляет количество дочерних папок, содержащихся в папке.</span><span class="sxs-lookup"><span data-stu-id="ad7a7-124">Represents the number of child folders that are contained within a folder.</span></span> <span data-ttu-id="ad7a7-125">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ad7a7-125">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="ad7a7-126">ExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="ad7a7-126">ExtendedProperty</span></span>](extendedproperty.md) <br/> |<span data-ttu-id="ad7a7-127">Определяет расширенные свойства для папок.</span><span class="sxs-lookup"><span data-stu-id="ad7a7-127">Identifies extended properties on folders.</span></span>  <br/> |
|[<span data-ttu-id="ad7a7-128">манажедфолдеринформатион</span><span class="sxs-lookup"><span data-stu-id="ad7a7-128">ManagedFolderInformation</span></span>](managedfolderinformation.md) <br/> |<span data-ttu-id="ad7a7-129">Содержит сведения об управляемой папке.</span><span class="sxs-lookup"><span data-stu-id="ad7a7-129">Contains information about a managed folder.</span></span>  <br/> |
|[<span data-ttu-id="ad7a7-130">унреадкаунт</span><span class="sxs-lookup"><span data-stu-id="ad7a7-130">UnreadCount</span></span>](unreadcount.md) <br/> |<span data-ttu-id="ad7a7-131">Представляет количество непрочитанных элементов в заданной папке.</span><span class="sxs-lookup"><span data-stu-id="ad7a7-131">Represents the count of unread items within a given folder.</span></span>  <br/> |
|[<span data-ttu-id="ad7a7-132">PermissionSet (Пермиссионсеттипе)</span><span class="sxs-lookup"><span data-stu-id="ad7a7-132">PermissionSet (PermissionSetType)</span></span>](permissionset-permissionsettype.md) <br/> |<span data-ttu-id="ad7a7-133">Содержит все настроенные разрешения для папки.</span><span class="sxs-lookup"><span data-stu-id="ad7a7-133">Contains all the configured permissions for a folder.</span></span> <span data-ttu-id="ad7a7-134">Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="ad7a7-134">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span>  <br/> |
|[<span data-ttu-id="ad7a7-135">еффективеригхтс</span><span class="sxs-lookup"><span data-stu-id="ad7a7-135">EffectiveRights</span></span>](effectiverights.md) <br/> |<span data-ttu-id="ad7a7-136">Содержит права клиента на основе параметров разрешений для элемента или папки.</span><span class="sxs-lookup"><span data-stu-id="ad7a7-136">Contains the client's rights based on the permission settings for the item or folder.</span></span> <span data-ttu-id="ad7a7-137">Этот элемент доступен только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ad7a7-137">This element is read-only.</span></span> <span data-ttu-id="ad7a7-138">Этот элемент появился в Exchange 2007 с пакетом обновления 1.</span><span class="sxs-lookup"><span data-stu-id="ad7a7-138">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="ad7a7-139">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="ad7a7-139">Parent elements</span></span>

|<span data-ttu-id="ad7a7-140">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="ad7a7-140">**Element**</span></span>|<span data-ttu-id="ad7a7-141">**Описание**</span><span class="sxs-lookup"><span data-stu-id="ad7a7-141">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ad7a7-142">аппендтофолдерфиелд</span><span class="sxs-lookup"><span data-stu-id="ad7a7-142">AppendToFolderField</span></span>](appendtofolderfield.md) <br/> |<span data-ttu-id="ad7a7-143">Задает данные, добавляемые к свойству folder во время [операции операцию UpdateFolder](updatefolder-operation.md).</span><span class="sxs-lookup"><span data-stu-id="ad7a7-143">Specifies data to append to a folder property during an [UpdateFolder operation](updatefolder-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="ad7a7-144">Create (Фолдерсинк)</span><span class="sxs-lookup"><span data-stu-id="ad7a7-144">Create (FolderSync)</span></span>](create-foldersync.md) <br/> |<span data-ttu-id="ad7a7-145">Определяет одну папку для создания в локальном хранилище клиента.</span><span class="sxs-lookup"><span data-stu-id="ad7a7-145">Identifies a single folder to create in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="ad7a7-146">сетфолдерфиелд</span><span class="sxs-lookup"><span data-stu-id="ad7a7-146">SetFolderField</span></span>](setfolderfield.md) <br/> |<span data-ttu-id="ad7a7-147">Представляет обновление одного свойства папки в [операции операцию UpdateFolder](updatefolder-operation.md).</span><span class="sxs-lookup"><span data-stu-id="ad7a7-147">Represents an update to a single property on a folder in an [UpdateFolder operation](updatefolder-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="ad7a7-148">Обновление (Фолдерсинк)</span><span class="sxs-lookup"><span data-stu-id="ad7a7-148">Update (FolderSync)</span></span>](update-foldersync.md) <br/> |<span data-ttu-id="ad7a7-149">Определяет одну папку для обновления в локальном хранилище клиента.</span><span class="sxs-lookup"><span data-stu-id="ad7a7-149">Identifies a single folder to update in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="ad7a7-150">Folders</span><span class="sxs-lookup"><span data-stu-id="ad7a7-150">Folders</span></span>](folders-ex15websvcsotherref.md) <br/> |<span data-ttu-id="ad7a7-151">Содержит массив папок, используемых в операциях с папками.</span><span class="sxs-lookup"><span data-stu-id="ad7a7-151">Contains an array of folders that are used in folder operations.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="ad7a7-152">Примечания</span><span class="sxs-lookup"><span data-stu-id="ad7a7-152">Remarks</span></span>

<span data-ttu-id="ad7a7-153">Схема, описывающая этот элемент, находится в виртуальном каталоге EWS компьютера, на котором работает Exchange 2007, на котором установлена роль сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="ad7a7-153">The schema that describes this element is located in the EWS virtual directory of the computer that is running Exchange 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ad7a7-154">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="ad7a7-154">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ad7a7-155">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="ad7a7-155">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="ad7a7-156">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="ad7a7-156">Schema Name</span></span>  <br/> |<span data-ttu-id="ad7a7-157">Схема Types</span><span class="sxs-lookup"><span data-stu-id="ad7a7-157">Types schema</span></span>  <br/> |
|<span data-ttu-id="ad7a7-158">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="ad7a7-158">Validation File</span></span>  <br/> |<span data-ttu-id="ad7a7-159">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="ad7a7-159">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="ad7a7-160">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="ad7a7-160">Can be Empty</span></span>  <br/> |<span data-ttu-id="ad7a7-161">False</span><span class="sxs-lookup"><span data-stu-id="ad7a7-161">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ad7a7-162">См. также</span><span class="sxs-lookup"><span data-stu-id="ad7a7-162">See also</span></span>



[<span data-ttu-id="ad7a7-163">Операция SyncFolderItems</span><span class="sxs-lookup"><span data-stu-id="ad7a7-163">SyncFolderItems operation</span></span>](syncfolderitems-operation.md)


- [<span data-ttu-id="ad7a7-164">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="ad7a7-164">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

