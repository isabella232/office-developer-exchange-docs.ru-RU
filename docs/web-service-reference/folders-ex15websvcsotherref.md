---
title: Папки
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Folders
api_type:
- schema
ms.assetid: 8e71cb44-1df6-444a-add7-0c1363863f65
description: Элемент папки содержит массив папки, которые используются в операциях папки.
ms.openlocfilehash: 34372f2480825c7a9977eeae8e730c201307f36b
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/28/2018
ms.locfileid: "21353590"
---
# <a name="folders"></a><span data-ttu-id="6f1d7-103">Папки</span><span class="sxs-lookup"><span data-stu-id="6f1d7-103">Folders</span></span>

<span data-ttu-id="6f1d7-104">Элемент **папки** содержит массив папки, которые используются в операциях папки.</span><span class="sxs-lookup"><span data-stu-id="6f1d7-104">The **Folders** element contains an array of folders that are used in folder operations.</span></span> 
  
```xml
<Folders>
   <Folder/>
</Folders>
```

```xml
<Folders>
   <ContactsFolder/> 
</Folders>
```

```xml
<Folders>
   <TasksFolder/>
</Folders>
```

```xml
<Folders>
   <CalendarFolder/>
</Folders>
```

```xml
<Folders>
   <SearchFolder/> 
</Folders>
```

<span data-ttu-id="6f1d7-105">**ArrayOfFoldersType** или **NonEmptyArrayOfFoldersType**</span><span class="sxs-lookup"><span data-stu-id="6f1d7-105">**ArrayOfFoldersType** or **NonEmptyArrayOfFoldersType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="6f1d7-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="6f1d7-106">Attributes and elements</span></span>

<span data-ttu-id="6f1d7-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="6f1d7-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6f1d7-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="6f1d7-108">Attributes</span></span>

<span data-ttu-id="6f1d7-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="6f1d7-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6f1d7-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="6f1d7-110">Child elements</span></span>

|<span data-ttu-id="6f1d7-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="6f1d7-111">**Element**</span></span>|<span data-ttu-id="6f1d7-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="6f1d7-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6f1d7-113">Folder</span><span class="sxs-lookup"><span data-stu-id="6f1d7-113">Folder</span></span>](folder.md) <br/> |<span data-ttu-id="6f1d7-114">Определяет папку для создания, получение, найти, синхронизировать или обновить.</span><span class="sxs-lookup"><span data-stu-id="6f1d7-114">Identifies a folder to create, get, find, synchronize, or update.</span></span>  <br/> |
|[<span data-ttu-id="6f1d7-115">CalendarFolder</span><span class="sxs-lookup"><span data-stu-id="6f1d7-115">CalendarFolder</span></span>](calendarfolder.md) <br/> |<span data-ttu-id="6f1d7-116">Представляет папку, содержащую элементы календаря в первую очередь.</span><span class="sxs-lookup"><span data-stu-id="6f1d7-116">Represents a folder that primarily contains calendar items.</span></span>  <br/> |
|[<span data-ttu-id="6f1d7-117">ContactsFolder</span><span class="sxs-lookup"><span data-stu-id="6f1d7-117">ContactsFolder</span></span>](contactsfolder.md) <br/> |<span data-ttu-id="6f1d7-118">Представляет папку контактов в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="6f1d7-118">Represents a Contacts folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="6f1d7-119">SearchFolder</span><span class="sxs-lookup"><span data-stu-id="6f1d7-119">SearchFolder</span></span>](searchfolder.md) <br/> |<span data-ttu-id="6f1d7-120">Представляет папку поиска, содержащихся в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="6f1d7-120">Represents a Search folder contained in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="6f1d7-121">TasksFolder</span><span class="sxs-lookup"><span data-stu-id="6f1d7-121">TasksFolder</span></span>](tasksfolder.md) <br/> |<span data-ttu-id="6f1d7-122">Представляет папку задачи в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="6f1d7-122">Represents a Tasks folder in a mailbox.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="6f1d7-123">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="6f1d7-123">Parent elements</span></span>

|<span data-ttu-id="6f1d7-124">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="6f1d7-124">**Element**</span></span>|<span data-ttu-id="6f1d7-125">**Описание**</span><span class="sxs-lookup"><span data-stu-id="6f1d7-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6f1d7-126">CopyFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="6f1d7-126">CopyFolderResponseMessage</span></span>](copyfolderresponsemessage.md) <br/> |<span data-ttu-id="6f1d7-127">Содержит состояние и результат одного запроса [CopyFolder операции](copyfolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="6f1d7-127">Contains the status and result of a single [CopyFolder operation](copyfolder-operation.md) request.</span></span>  <br/> |
|[<span data-ttu-id="6f1d7-128">CreateFolder</span><span class="sxs-lookup"><span data-stu-id="6f1d7-128">CreateFolder</span></span>](createfolder.md) <br/> |<span data-ttu-id="6f1d7-129">Определяет запрос на создание папки в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="6f1d7-129">Defines a request to create a folder in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="6f1d7-130">CreateFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="6f1d7-130">CreateFolderResponseMessage</span></span>](createfolderresponsemessage.md) <br/> |<span data-ttu-id="6f1d7-131">Содержит состояние и результат одного запроса [CreateFolder операции](createfolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="6f1d7-131">Contains the status and result of a single [CreateFolder operation](createfolder-operation.md) request.</span></span>  <br/> |
|[<span data-ttu-id="6f1d7-132">CreateManagedFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="6f1d7-132">CreateManagedFolderResponseMessage</span></span>](createmanagedfolderresponsemessage.md) <br/> |<span data-ttu-id="6f1d7-133">Содержит состояние и результат одного запроса [CreateManagedFolder операции](createmanagedfolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="6f1d7-133">Contains the status and result of a single [CreateManagedFolder operation](createmanagedfolder-operation.md) request.</span></span>  <br/> |
|[<span data-ttu-id="6f1d7-134">GetFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="6f1d7-134">GetFolderResponseMessage</span></span>](getfolderresponsemessage.md) <br/> |<span data-ttu-id="6f1d7-135">Содержит состояние и результат [операции GetFolder](getfolder-operation.md) запроса.</span><span class="sxs-lookup"><span data-stu-id="6f1d7-135">Contains the status and result of a [GetFolder operation](getfolder-operation.md) request.</span></span>  <br/> |
|[<span data-ttu-id="6f1d7-136">MoveFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="6f1d7-136">MoveFolderResponseMessage</span></span>](movefolderresponsemessage.md) <br/> |<span data-ttu-id="6f1d7-137">Содержит состояние и результат [операции MoveFolder](movefolder-operation.md) запроса.</span><span class="sxs-lookup"><span data-stu-id="6f1d7-137">Contains the status and result of a [MoveFolder operation](movefolder-operation.md) request.</span></span>  <br/> |
|[<span data-ttu-id="6f1d7-138">ParentFolderId (TargetFolderIdType)</span><span class="sxs-lookup"><span data-stu-id="6f1d7-138">ParentFolderId (TargetFolderIdType)</span></span>](parentfolderid-targetfolderidtype.md) <br/> |<span data-ttu-id="6f1d7-139">Указывает папку, где будет создана новая папка.</span><span class="sxs-lookup"><span data-stu-id="6f1d7-139">Identifies the folder where a new folder is created.</span></span>  <br/> |
|[<span data-ttu-id="6f1d7-140">RootFolder (FindFolderResponseMessage)</span><span class="sxs-lookup"><span data-stu-id="6f1d7-140">RootFolder (FindFolderResponseMessage)</span></span>](rootfolder-findfolderresponsemessage.md) <br/> |<span data-ttu-id="6f1d7-141">Содержит результаты поиска в одной корневой папке во время [операции FindFolder](findfolder-operation.md).</span><span class="sxs-lookup"><span data-stu-id="6f1d7-141">Contains the results from searching a single root folder during a [FindFolder operation](findfolder-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="6f1d7-142">UpdateFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="6f1d7-142">UpdateFolderResponseMessage</span></span>](updatefolderresponsemessage.md) <br/> |<span data-ttu-id="6f1d7-143">Содержит состояние и результат одного запроса [UpdateFolder операции](updatefolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="6f1d7-143">Contains the status and result of a single [UpdateFolder operation](updatefolder-operation.md) request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="6f1d7-144">Замечания</span><span class="sxs-lookup"><span data-stu-id="6f1d7-144">Remarks</span></span>

<span data-ttu-id="6f1d7-145">Этот элемент является обязательным дочерним элементом элемента [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) .</span><span class="sxs-lookup"><span data-stu-id="6f1d7-145">This element is a required child element of the [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) element.</span></span> 
  
<span data-ttu-id="6f1d7-146">Схема, описывающая этот элемент находится в виртуальном каталоге EWS компьютера, на котором выполняется Microsoft Exchange Server 2010 с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="6f1d7-146">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6f1d7-147">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="6f1d7-147">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6f1d7-148">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="6f1d7-148">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="6f1d7-149">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="6f1d7-149">Schema Name</span></span>  <br/> |<span data-ttu-id="6f1d7-150">Схема Types</span><span class="sxs-lookup"><span data-stu-id="6f1d7-150">Types schema</span></span>  <br/> |
|<span data-ttu-id="6f1d7-151">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="6f1d7-151">Validation File</span></span>  <br/> |<span data-ttu-id="6f1d7-152">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="6f1d7-152">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="6f1d7-153">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="6f1d7-153">Can be Empty</span></span>  <br/> |<span data-ttu-id="6f1d7-154">False</span><span class="sxs-lookup"><span data-stu-id="6f1d7-154">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6f1d7-155">См. также</span><span class="sxs-lookup"><span data-stu-id="6f1d7-155">See also</span></span>

- [<span data-ttu-id="6f1d7-156">ParentFolderId (TargetFolderIdType)</span><span class="sxs-lookup"><span data-stu-id="6f1d7-156">ParentFolderId (TargetFolderIdType)</span></span>](parentfolderid-targetfolderidtype.md)

