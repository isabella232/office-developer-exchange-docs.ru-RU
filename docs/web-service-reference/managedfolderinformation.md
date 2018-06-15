---
title: ManagedFolderInformation
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ManagedFolderInformation
api_type:
- schema
ms.assetid: dea980eb-8303-47fe-a380-20a8efc9ead6
description: Элемент ManagedFolderInformation содержит сведения о настраиваемой управляемой папки.
ms.openlocfilehash: ef46e2e0db440de2a8acae8316ce98d11bd6710e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19834341"
---
# <a name="managedfolderinformation"></a><span data-ttu-id="deabe-103">ManagedFolderInformation</span><span class="sxs-lookup"><span data-stu-id="deabe-103">ManagedFolderInformation</span></span>

<span data-ttu-id="deabe-104">Элемент **ManagedFolderInformation** содержит сведения о настраиваемой управляемой папки.</span><span class="sxs-lookup"><span data-stu-id="deabe-104">The **ManagedFolderInformation** element contains information about a managed custom folder.</span></span> 
  
```xml
<ManagedFolderInformation>
   <CanDelete/>
   <CanRenameOrMove/>
   <MustDisplayComment/>
   <HasQuota/>
   <IsManagedFoldersRoot/>
   <ManagedFolderId/>
   <Comment/>
   <StorageQuota/>
   <FolderSize/>
   <HomePage/>
</ManagedFolderInformation>
```

 <span data-ttu-id="deabe-105">**ManagedFolderInformationType**</span><span class="sxs-lookup"><span data-stu-id="deabe-105">**ManagedFolderInformationType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="deabe-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="deabe-106">Attributes and elements</span></span>

<span data-ttu-id="deabe-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="deabe-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="deabe-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="deabe-108">Attributes</span></span>

<span data-ttu-id="deabe-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="deabe-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="deabe-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="deabe-110">Child elements</span></span>

|<span data-ttu-id="deabe-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="deabe-111">**Element**</span></span>|<span data-ttu-id="deabe-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="deabe-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="deabe-113">CanDelete</span><span class="sxs-lookup"><span data-stu-id="deabe-113">CanDelete</span></span>](candelete.md) <br/> |<span data-ttu-id="deabe-114">Указывает, можно ли удалить управляемой папки клиентом.</span><span class="sxs-lookup"><span data-stu-id="deabe-114">Indicates whether a managed folder can be deleted by a customer.</span></span>  <br/> |
|[<span data-ttu-id="deabe-115">CanRenameOrMove</span><span class="sxs-lookup"><span data-stu-id="deabe-115">CanRenameOrMove</span></span>](canrenameormove.md) <br/> |<span data-ttu-id="deabe-116">Указывает, переименованы или перемещены клиентом указанной управляемой папки.</span><span class="sxs-lookup"><span data-stu-id="deabe-116">Indicates whether a given managed folder can be renamed or moved by the customer.</span></span>  <br/> |
|[<span data-ttu-id="deabe-117">MustDisplayComment</span><span class="sxs-lookup"><span data-stu-id="deabe-117">MustDisplayComment</span></span>](mustdisplaycomment.md) <br/> |<span data-ttu-id="deabe-118">Указывает, должно ли отображаться комментария управляемой папки.</span><span class="sxs-lookup"><span data-stu-id="deabe-118">Indicates whether the managed folder comment must be displayed.</span></span>  <br/> |
|[<span data-ttu-id="deabe-119">HasQuota</span><span class="sxs-lookup"><span data-stu-id="deabe-119">HasQuota</span></span>](hasquota.md) <br/> |<span data-ttu-id="deabe-120">Указывает, имеет ли управляемой папки квоту.</span><span class="sxs-lookup"><span data-stu-id="deabe-120">Indicates whether the managed folder has a quota.</span></span>  <br/> |
|[<span data-ttu-id="deabe-121">IsManagedFoldersRoot</span><span class="sxs-lookup"><span data-stu-id="deabe-121">IsManagedFoldersRoot</span></span>](ismanagedfoldersroot.md) <br/> |<span data-ttu-id="deabe-122">Указывает, является ли управляемых папок корневого каталога для всех управляемых папок.</span><span class="sxs-lookup"><span data-stu-id="deabe-122">Indicates whether the managed folder is the root for all managed folders.</span></span>  <br/> |
|[<span data-ttu-id="deabe-123">ManagedFolderId</span><span class="sxs-lookup"><span data-stu-id="deabe-123">ManagedFolderId</span></span>](managedfolderid.md) <br/> |<span data-ttu-id="deabe-124">Содержит идентификатор папки из управляемых папок.</span><span class="sxs-lookup"><span data-stu-id="deabe-124">Contains the folder ID of the managed folder.</span></span>  <br/> |
|[<span data-ttu-id="deabe-125">�����������</span><span class="sxs-lookup"><span data-stu-id="deabe-125">Comment</span></span>](comment.md) <br/> |<span data-ttu-id="deabe-126">Содержит комментарий, связанный с управляемой папки.</span><span class="sxs-lookup"><span data-stu-id="deabe-126">Contains the comment that is associated with a managed folder.</span></span>  <br/> |
|[<span data-ttu-id="deabe-127">StorageQuota</span><span class="sxs-lookup"><span data-stu-id="deabe-127">StorageQuota</span></span>](storagequota.md) <br/> |<span data-ttu-id="deabe-128">Описывает квоту хранилища для управляемых папок.</span><span class="sxs-lookup"><span data-stu-id="deabe-128">Describes the storage quota for the managed folder.</span></span>  <br/> |
|[<span data-ttu-id="deabe-129">FolderSize</span><span class="sxs-lookup"><span data-stu-id="deabe-129">FolderSize</span></span>](foldersize.md) <br/> |<span data-ttu-id="deabe-130">Описывает общий размер все содержимое управляемых папок.</span><span class="sxs-lookup"><span data-stu-id="deabe-130">Describes the total size of all the contents of a managed folder.</span></span>  <br/> |
|[<span data-ttu-id="deabe-131">Домашняя страница</span><span class="sxs-lookup"><span data-stu-id="deabe-131">HomePage</span></span>](homepage.md) <br/> |<span data-ttu-id="deabe-132">Задает URL-адрес, который будет по умолчанию домашнюю страницу для управляемых папок.</span><span class="sxs-lookup"><span data-stu-id="deabe-132">Specifies the URL that will be the default home page for the managed folder.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="deabe-133">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="deabe-133">Parent elements</span></span>

|<span data-ttu-id="deabe-134">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="deabe-134">**Element**</span></span>|<span data-ttu-id="deabe-135">**Описание**</span><span class="sxs-lookup"><span data-stu-id="deabe-135">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="deabe-136">Folder</span><span class="sxs-lookup"><span data-stu-id="deabe-136">Folder</span></span>](folder.md) <br/> |<span data-ttu-id="deabe-137">Представляет папку в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="deabe-137">Represents a folder in the Exchange store.</span></span> <span data-ttu-id="deabe-138">Управляемые настраиваемые папки можно только вложенные папки в папку с именем **Управляемых папок**.</span><span class="sxs-lookup"><span data-stu-id="deabe-138">Managed custom folders can only be subfolders of the folder named **Managed Folders**.</span></span>  <br/> |
|[<span data-ttu-id="deabe-139">CalendarFolder</span><span class="sxs-lookup"><span data-stu-id="deabe-139">CalendarFolder</span></span>](calendarfolder.md) <br/> |<span data-ttu-id="deabe-140">Не применимо.</span><span class="sxs-lookup"><span data-stu-id="deabe-140">Not applicable.</span></span>  <br/> |
|[<span data-ttu-id="deabe-141">ContactsFolder</span><span class="sxs-lookup"><span data-stu-id="deabe-141">ContactsFolder</span></span>](contactsfolder.md) <br/> |<span data-ttu-id="deabe-142">Не применимо.</span><span class="sxs-lookup"><span data-stu-id="deabe-142">Not applicable.</span></span>  <br/> |
|[<span data-ttu-id="deabe-143">SearchFolder</span><span class="sxs-lookup"><span data-stu-id="deabe-143">SearchFolder</span></span>](searchfolder.md) <br/> |<span data-ttu-id="deabe-144">Не применимо.</span><span class="sxs-lookup"><span data-stu-id="deabe-144">Not applicable.</span></span>  <br/> |
|[<span data-ttu-id="deabe-145">TasksFolder</span><span class="sxs-lookup"><span data-stu-id="deabe-145">TasksFolder</span></span>](tasksfolder.md) <br/> |<span data-ttu-id="deabe-146">Неприменимо.</span><span class="sxs-lookup"><span data-stu-id="deabe-146">Not applicable.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="deabe-147">Заметки</span><span class="sxs-lookup"><span data-stu-id="deabe-147">Remarks</span></span>

<span data-ttu-id="deabe-148">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="deabe-148">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="deabe-149">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="deabe-149">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="deabe-150">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="deabe-150">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="deabe-151">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="deabe-151">Schema name</span></span>  <br/> |<span data-ttu-id="deabe-152">Схема Types</span><span class="sxs-lookup"><span data-stu-id="deabe-152">Types schema</span></span>  <br/> |
|<span data-ttu-id="deabe-153">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="deabe-153">Validation file</span></span>  <br/> |<span data-ttu-id="deabe-154">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="deabe-154">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="deabe-155">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="deabe-155">Can be empty</span></span>  <br/> |<span data-ttu-id="deabe-156">False</span><span class="sxs-lookup"><span data-stu-id="deabe-156">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="deabe-157">См. также</span><span class="sxs-lookup"><span data-stu-id="deabe-157">See also</span></span>



[<span data-ttu-id="deabe-158">Операция CreateManagedFolder</span><span class="sxs-lookup"><span data-stu-id="deabe-158">CreateManagedFolder operation</span></span>](createmanagedfolder-operation.md)


- [<span data-ttu-id="deabe-159">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="deabe-159">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="deabe-160">Добавление управляемых папок</span><span class="sxs-lookup"><span data-stu-id="deabe-160">Adding Managed Folders</span></span>](http://msdn.microsoft.com/library/846658c6-7043-40fb-8439-19f97c2a967f%28Office.15%29.aspx)
