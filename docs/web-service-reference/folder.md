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
description: Элемент Folder определяет папку для создания, получение, найти, синхронизировать или обновить.
ms.openlocfilehash: ecfea52d2105599372a22b78778ac0d0d066bc60
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762622"
---
# <a name="folder"></a><span data-ttu-id="72f4a-103">Folder</span><span class="sxs-lookup"><span data-stu-id="72f4a-103">Folder</span></span>

<span data-ttu-id="72f4a-104">Элемент **Folder** определяет папку для создания, получение, найти, синхронизировать или обновить.</span><span class="sxs-lookup"><span data-stu-id="72f4a-104">The **Folder** element defines a folder to create, get, find, synchronize, or update.</span></span> 
  
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

 <span data-ttu-id="72f4a-105">**FolderType**</span><span class="sxs-lookup"><span data-stu-id="72f4a-105">**FolderType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="72f4a-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="72f4a-106">Attributes and elements</span></span>

<span data-ttu-id="72f4a-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="72f4a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="72f4a-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="72f4a-108">Attributes</span></span>

<span data-ttu-id="72f4a-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="72f4a-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="72f4a-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="72f4a-110">Child elements</span></span>

|<span data-ttu-id="72f4a-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="72f4a-111">**Element**</span></span>|<span data-ttu-id="72f4a-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="72f4a-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="72f4a-113">FolderId</span><span class="sxs-lookup"><span data-stu-id="72f4a-113">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="72f4a-114">Содержит идентификатор и ключ изменения папки.</span><span class="sxs-lookup"><span data-stu-id="72f4a-114">Contains the identifier and change key of a folder.</span></span>  <br/> |
|[<span data-ttu-id="72f4a-115">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="72f4a-115">ParentFolderId</span></span>](parentfolderid.md) <br/> |<span data-ttu-id="72f4a-116">Представляет идентификатор родительской папки, содержащей папку.</span><span class="sxs-lookup"><span data-stu-id="72f4a-116">Represents the identifier of the parent folder that contains the folder.</span></span>  <br/> |
|[<span data-ttu-id="72f4a-117">FolderClass</span><span class="sxs-lookup"><span data-stu-id="72f4a-117">FolderClass</span></span>](folderclass.md) <br/> |<span data-ttu-id="72f4a-118">Представляет класс папки для данной папки.</span><span class="sxs-lookup"><span data-stu-id="72f4a-118">Represents the folder class for a given folder.</span></span>  <br/> |
|[<span data-ttu-id="72f4a-119">Отображаемое имя (строка)</span><span class="sxs-lookup"><span data-stu-id="72f4a-119">DisplayName (string)</span></span>](displayname-string.md) <br/> |<span data-ttu-id="72f4a-120">Содержит отображаемое имя папки.</span><span class="sxs-lookup"><span data-stu-id="72f4a-120">Contains the display name of a folder.</span></span>  <br/> |
|[<span data-ttu-id="72f4a-121">TotalCount</span><span class="sxs-lookup"><span data-stu-id="72f4a-121">TotalCount</span></span>](totalcount.md) <br/> |<span data-ttu-id="72f4a-122">Представляет общее число элементов в указанной папке.</span><span class="sxs-lookup"><span data-stu-id="72f4a-122">Represents the total count of items within a given folder.</span></span>  <br/> |
|[<span data-ttu-id="72f4a-123">ChildFolderCount</span><span class="sxs-lookup"><span data-stu-id="72f4a-123">ChildFolderCount</span></span>](childfoldercount.md) <br/> |<span data-ttu-id="72f4a-124">Представляет число дочерних папок, содержащихся в папке.</span><span class="sxs-lookup"><span data-stu-id="72f4a-124">Represents the number of child folders that are contained within a folder.</span></span> <span data-ttu-id="72f4a-125">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="72f4a-125">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="72f4a-126">ExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="72f4a-126">ExtendedProperty</span></span>](extendedproperty.md) <br/> |<span data-ttu-id="72f4a-127">Определяет расширенные свойства папки.</span><span class="sxs-lookup"><span data-stu-id="72f4a-127">Identifies extended properties on folders.</span></span>  <br/> |
|[<span data-ttu-id="72f4a-128">ManagedFolderInformation</span><span class="sxs-lookup"><span data-stu-id="72f4a-128">ManagedFolderInformation</span></span>](managedfolderinformation.md) <br/> |<span data-ttu-id="72f4a-129">Содержит сведения об управляемых папок.</span><span class="sxs-lookup"><span data-stu-id="72f4a-129">Contains information about a managed folder.</span></span>  <br/> |
|[<span data-ttu-id="72f4a-130">UnreadCount</span><span class="sxs-lookup"><span data-stu-id="72f4a-130">UnreadCount</span></span>](unreadcount.md) <br/> |<span data-ttu-id="72f4a-131">Представляет количество непрочитанных элементов в указанной папке.</span><span class="sxs-lookup"><span data-stu-id="72f4a-131">Represents the count of unread items within a given folder.</span></span>  <br/> |
|[<span data-ttu-id="72f4a-132">PermissionSet (PermissionSetType)</span><span class="sxs-lookup"><span data-stu-id="72f4a-132">PermissionSet (PermissionSetType)</span></span>](permissionset-permissionsettype.md) <br/> |<span data-ttu-id="72f4a-133">Содержит все настроенные разрешения для папки.</span><span class="sxs-lookup"><span data-stu-id="72f4a-133">Contains all the configured permissions for a folder.</span></span> <span data-ttu-id="72f4a-134">Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="72f4a-134">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span>  <br/> |
|[<span data-ttu-id="72f4a-135">EffectiveRights</span><span class="sxs-lookup"><span data-stu-id="72f4a-135">EffectiveRights</span></span>](effectiverights.md) <br/> |<span data-ttu-id="72f4a-136">Содержит права клиента на основании параметров разрешений для элемента или папки.</span><span class="sxs-lookup"><span data-stu-id="72f4a-136">Contains the client's rights based on the permission settings for the item or folder.</span></span> <span data-ttu-id="72f4a-137">Этот элемент доступен только для чтения.</span><span class="sxs-lookup"><span data-stu-id="72f4a-137">This element is read-only.</span></span> <span data-ttu-id="72f4a-138">Этот элемент появился в Exchange 2007 с пакетом обновления 1.</span><span class="sxs-lookup"><span data-stu-id="72f4a-138">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="72f4a-139">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="72f4a-139">Parent elements</span></span>

|<span data-ttu-id="72f4a-140">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="72f4a-140">**Element**</span></span>|<span data-ttu-id="72f4a-141">**Описание**</span><span class="sxs-lookup"><span data-stu-id="72f4a-141">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="72f4a-142">AppendToFolderField</span><span class="sxs-lookup"><span data-stu-id="72f4a-142">AppendToFolderField</span></span>](appendtofolderfield.md) <br/> |<span data-ttu-id="72f4a-143">Указывает данные для добавления к папке свойство во время [операции UpdateFolder](updatefolder-operation.md).</span><span class="sxs-lookup"><span data-stu-id="72f4a-143">Specifies data to append to a folder property during an [UpdateFolder operation](updatefolder-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="72f4a-144">Создание (FolderSync)</span><span class="sxs-lookup"><span data-stu-id="72f4a-144">Create (FolderSync)</span></span>](create-foldersync.md) <br/> |<span data-ttu-id="72f4a-145">Определяет одну папку для создания в локальном хранилище клиента.</span><span class="sxs-lookup"><span data-stu-id="72f4a-145">Identifies a single folder to create in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="72f4a-146">SetFolderField</span><span class="sxs-lookup"><span data-stu-id="72f4a-146">SetFolderField</span></span>](setfolderfield.md) <br/> |<span data-ttu-id="72f4a-147">Представляет обновление для одного свойства папки в рамках одной [операции UpdateFolder](updatefolder-operation.md).</span><span class="sxs-lookup"><span data-stu-id="72f4a-147">Represents an update to a single property on a folder in an [UpdateFolder operation](updatefolder-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="72f4a-148">Обновление (FolderSync)</span><span class="sxs-lookup"><span data-stu-id="72f4a-148">Update (FolderSync)</span></span>](update-foldersync.md) <br/> |<span data-ttu-id="72f4a-149">Определяет одну папку для обновления в локальном хранилище клиента.</span><span class="sxs-lookup"><span data-stu-id="72f4a-149">Identifies a single folder to update in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="72f4a-150">Папки</span><span class="sxs-lookup"><span data-stu-id="72f4a-150">Folders</span></span>](folders-ex15websvcsotherref.md) <br/> |<span data-ttu-id="72f4a-151">Содержит набор папок, используемых в операциях папки.</span><span class="sxs-lookup"><span data-stu-id="72f4a-151">Contains an array of folders that are used in folder operations.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="72f4a-152">Замечания</span><span class="sxs-lookup"><span data-stu-id="72f4a-152">Remarks</span></span>

<span data-ttu-id="72f4a-153">Схема, описывающая этот элемент находится в виртуальном каталоге EWS компьютера, на котором работает с установленной ролью сервера клиентского доступа Exchange 2007.</span><span class="sxs-lookup"><span data-stu-id="72f4a-153">The schema that describes this element is located in the EWS virtual directory of the computer that is running Exchange 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="72f4a-154">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="72f4a-154">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="72f4a-155">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="72f4a-155">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="72f4a-156">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="72f4a-156">Schema Name</span></span>  <br/> |<span data-ttu-id="72f4a-157">Схема Types</span><span class="sxs-lookup"><span data-stu-id="72f4a-157">Types schema</span></span>  <br/> |
|<span data-ttu-id="72f4a-158">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="72f4a-158">Validation File</span></span>  <br/> |<span data-ttu-id="72f4a-159">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="72f4a-159">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="72f4a-160">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="72f4a-160">Can be Empty</span></span>  <br/> |<span data-ttu-id="72f4a-161">False</span><span class="sxs-lookup"><span data-stu-id="72f4a-161">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="72f4a-162">См. также</span><span class="sxs-lookup"><span data-stu-id="72f4a-162">See also</span></span>



[<span data-ttu-id="72f4a-163">Операция SyncFolderItems</span><span class="sxs-lookup"><span data-stu-id="72f4a-163">SyncFolderItems operation</span></span>](syncfolderitems-operation.md)


- [<span data-ttu-id="72f4a-164">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="72f4a-164">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

