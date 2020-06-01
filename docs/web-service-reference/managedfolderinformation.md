---
title: манажедфолдеринформатион
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
description: Элемент Манажедфолдеринформатион содержит сведения о настраиваемой управляемой папке.
ms.openlocfilehash: ce15dcb15cccdce253494beefd2f4a2a7a0c0ad8
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44450951"
---
# <a name="managedfolderinformation"></a><span data-ttu-id="3ccca-103">манажедфолдеринформатион</span><span class="sxs-lookup"><span data-stu-id="3ccca-103">ManagedFolderInformation</span></span>

<span data-ttu-id="3ccca-104">Элемент **манажедфолдеринформатион** содержит сведения о настраиваемой управляемой папке.</span><span class="sxs-lookup"><span data-stu-id="3ccca-104">The **ManagedFolderInformation** element contains information about a managed custom folder.</span></span> 
  
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

 <span data-ttu-id="3ccca-105">**манажедфолдеринформатионтипе**</span><span class="sxs-lookup"><span data-stu-id="3ccca-105">**ManagedFolderInformationType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3ccca-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="3ccca-106">Attributes and elements</span></span>

<span data-ttu-id="3ccca-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="3ccca-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3ccca-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="3ccca-108">Attributes</span></span>

<span data-ttu-id="3ccca-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="3ccca-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3ccca-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="3ccca-110">Child elements</span></span>

|<span data-ttu-id="3ccca-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="3ccca-111">**Element**</span></span>|<span data-ttu-id="3ccca-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="3ccca-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3ccca-113">канделете</span><span class="sxs-lookup"><span data-stu-id="3ccca-113">CanDelete</span></span>](candelete.md) <br/> |<span data-ttu-id="3ccca-114">Указывает, может ли клиент удалить управляемую папку.</span><span class="sxs-lookup"><span data-stu-id="3ccca-114">Indicates whether a managed folder can be deleted by a customer.</span></span>  <br/> |
|[<span data-ttu-id="3ccca-115">канренамеормове</span><span class="sxs-lookup"><span data-stu-id="3ccca-115">CanRenameOrMove</span></span>](canrenameormove.md) <br/> |<span data-ttu-id="3ccca-116">Указывает, может ли пользователь переименование или перемещение данной управляемой папки.</span><span class="sxs-lookup"><span data-stu-id="3ccca-116">Indicates whether a given managed folder can be renamed or moved by the customer.</span></span>  <br/> |
|[<span data-ttu-id="3ccca-117">мустдисплайкоммент</span><span class="sxs-lookup"><span data-stu-id="3ccca-117">MustDisplayComment</span></span>](mustdisplaycomment.md) <br/> |<span data-ttu-id="3ccca-118">Указывает, должен ли отображаться комментарий к управляемой папке.</span><span class="sxs-lookup"><span data-stu-id="3ccca-118">Indicates whether the managed folder comment must be displayed.</span></span>  <br/> |
|[<span data-ttu-id="3ccca-119">хаскуота</span><span class="sxs-lookup"><span data-stu-id="3ccca-119">HasQuota</span></span>](hasquota.md) <br/> |<span data-ttu-id="3ccca-120">Указывает, есть ли у управляемой папки квота.</span><span class="sxs-lookup"><span data-stu-id="3ccca-120">Indicates whether the managed folder has a quota.</span></span>  <br/> |
|[<span data-ttu-id="3ccca-121">исманажедфолдерсрут</span><span class="sxs-lookup"><span data-stu-id="3ccca-121">IsManagedFoldersRoot</span></span>](ismanagedfoldersroot.md) <br/> |<span data-ttu-id="3ccca-122">Указывает, является ли управляемая папка корневой для всех управляемых папок.</span><span class="sxs-lookup"><span data-stu-id="3ccca-122">Indicates whether the managed folder is the root for all managed folders.</span></span>  <br/> |
|[<span data-ttu-id="3ccca-123">манажедфолдерид</span><span class="sxs-lookup"><span data-stu-id="3ccca-123">ManagedFolderId</span></span>](managedfolderid.md) <br/> |<span data-ttu-id="3ccca-124">Содержит идентификатор управляемой папки.</span><span class="sxs-lookup"><span data-stu-id="3ccca-124">Contains the folder ID of the managed folder.</span></span>  <br/> |
|[<span data-ttu-id="3ccca-125">Comment</span><span class="sxs-lookup"><span data-stu-id="3ccca-125">Comment</span></span>](comment.md) <br/> |<span data-ttu-id="3ccca-126">Содержит комментарий, связанный с управляемой папкой.</span><span class="sxs-lookup"><span data-stu-id="3ccca-126">Contains the comment that is associated with a managed folder.</span></span>  <br/> |
|[<span data-ttu-id="3ccca-127">StorageQuota</span><span class="sxs-lookup"><span data-stu-id="3ccca-127">StorageQuota</span></span>](storagequota.md) <br/> |<span data-ttu-id="3ccca-128">Описывает квоту хранилища для управляемой папки.</span><span class="sxs-lookup"><span data-stu-id="3ccca-128">Describes the storage quota for the managed folder.</span></span>  <br/> |
|[<span data-ttu-id="3ccca-129">FolderSize</span><span class="sxs-lookup"><span data-stu-id="3ccca-129">FolderSize</span></span>](foldersize.md) <br/> |<span data-ttu-id="3ccca-130">Описывает общий размер всего содержимого управляемой папки.</span><span class="sxs-lookup"><span data-stu-id="3ccca-130">Describes the total size of all the contents of a managed folder.</span></span>  <br/> |
|[<span data-ttu-id="3ccca-131">HomePage</span><span class="sxs-lookup"><span data-stu-id="3ccca-131">HomePage</span></span>](homepage.md) <br/> |<span data-ttu-id="3ccca-132">Задает URL-адрес, который будет домашней страницей по умолчанию для управляемой папки.</span><span class="sxs-lookup"><span data-stu-id="3ccca-132">Specifies the URL that will be the default home page for the managed folder.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="3ccca-133">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="3ccca-133">Parent elements</span></span>

|<span data-ttu-id="3ccca-134">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="3ccca-134">**Element**</span></span>|<span data-ttu-id="3ccca-135">**Описание**</span><span class="sxs-lookup"><span data-stu-id="3ccca-135">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3ccca-136">Folder</span><span class="sxs-lookup"><span data-stu-id="3ccca-136">Folder</span></span>](folder.md) <br/> |<span data-ttu-id="3ccca-137">Представляет папку в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="3ccca-137">Represents a folder in the Exchange store.</span></span> <span data-ttu-id="3ccca-138">Управляемые папки могут быть только вложенными папками с именем " **управляемые папки**".</span><span class="sxs-lookup"><span data-stu-id="3ccca-138">Managed custom folders can only be subfolders of the folder named **Managed Folders**.</span></span>  <br/> |
|[<span data-ttu-id="3ccca-139">календарфолдер</span><span class="sxs-lookup"><span data-stu-id="3ccca-139">CalendarFolder</span></span>](calendarfolder.md) <br/> |<span data-ttu-id="3ccca-140">Неприменимо.</span><span class="sxs-lookup"><span data-stu-id="3ccca-140">Not applicable.</span></span>  <br/> |
|[<span data-ttu-id="3ccca-141">контактсфолдер</span><span class="sxs-lookup"><span data-stu-id="3ccca-141">ContactsFolder</span></span>](contactsfolder.md) <br/> |<span data-ttu-id="3ccca-142">Неприменимо.</span><span class="sxs-lookup"><span data-stu-id="3ccca-142">Not applicable.</span></span>  <br/> |
|[<span data-ttu-id="3ccca-143">SearchFolder</span><span class="sxs-lookup"><span data-stu-id="3ccca-143">SearchFolder</span></span>](searchfolder.md) <br/> |<span data-ttu-id="3ccca-144">Неприменимо.</span><span class="sxs-lookup"><span data-stu-id="3ccca-144">Not applicable.</span></span>  <br/> |
|[<span data-ttu-id="3ccca-145">тасксфолдер</span><span class="sxs-lookup"><span data-stu-id="3ccca-145">TasksFolder</span></span>](tasksfolder.md) <br/> |<span data-ttu-id="3ccca-146">Неприменимо.</span><span class="sxs-lookup"><span data-stu-id="3ccca-146">Not applicable.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="3ccca-147">Заметки</span><span class="sxs-lookup"><span data-stu-id="3ccca-147">Remarks</span></span>

<span data-ttu-id="3ccca-148">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="3ccca-148">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3ccca-149">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="3ccca-149">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3ccca-150">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="3ccca-150">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="3ccca-151">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="3ccca-151">Schema name</span></span>  <br/> |<span data-ttu-id="3ccca-152">Схема Types</span><span class="sxs-lookup"><span data-stu-id="3ccca-152">Types schema</span></span>  <br/> |
|<span data-ttu-id="3ccca-153">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="3ccca-153">Validation file</span></span>  <br/> |<span data-ttu-id="3ccca-154">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="3ccca-154">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="3ccca-155">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="3ccca-155">Can be empty</span></span>  <br/> |<span data-ttu-id="3ccca-156">False</span><span class="sxs-lookup"><span data-stu-id="3ccca-156">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3ccca-157">См. также</span><span class="sxs-lookup"><span data-stu-id="3ccca-157">See also</span></span>



[<span data-ttu-id="3ccca-158">Операция CreateManagedFolder</span><span class="sxs-lookup"><span data-stu-id="3ccca-158">CreateManagedFolder operation</span></span>](createmanagedfolder-operation.md)


- [<span data-ttu-id="3ccca-159">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="3ccca-159">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="3ccca-160">Добавление управляемых папок</span><span class="sxs-lookup"><span data-stu-id="3ccca-160">Adding Managed Folders</span></span>](https://msdn.microsoft.com/library/846658c6-7043-40fb-8439-19f97c2a967f%28Office.15%29.aspx)

