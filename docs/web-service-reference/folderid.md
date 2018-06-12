---
title: FolderId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FolderId
api_type:
- schema
ms.assetid: 00d14e3e-4365-4f21-8f88-eaeea73b9bf7
description: Элемент FolderId содержит идентификатор и ключ изменения папки.
ms.openlocfilehash: 5764a164d5af183b8f313955ace5274dc6023a6a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762625"
---
# <a name="folderid"></a><span data-ttu-id="a7a01-103">FolderId</span><span class="sxs-lookup"><span data-stu-id="a7a01-103">FolderId</span></span>

<span data-ttu-id="a7a01-104">Элемент **FolderId** содержит идентификатор и ключ изменения папки.</span><span class="sxs-lookup"><span data-stu-id="a7a01-104">The **FolderId** element contains the identifier and change key of a folder.</span></span> 
  
```XML
<FolderId Id="" ChangeKey="" />
```

 <span data-ttu-id="a7a01-105">**FolderIdType**</span><span class="sxs-lookup"><span data-stu-id="a7a01-105">**FolderIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a7a01-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="a7a01-106">Attributes and elements</span></span>

<span data-ttu-id="a7a01-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="a7a01-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a7a01-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="a7a01-108">Attributes</span></span>

|<span data-ttu-id="a7a01-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="a7a01-109">**Attribute**</span></span>|<span data-ttu-id="a7a01-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="a7a01-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="a7a01-111">Id</span><span class="sxs-lookup"><span data-stu-id="a7a01-111">Id</span></span>  <br/> |<span data-ttu-id="a7a01-112">Содержит строку, которая определяет папке в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="a7a01-112">Contains a string that identifies a folder in the Exchange store.</span></span> <span data-ttu-id="a7a01-113">Этот атрибут является обязательным.</span><span class="sxs-lookup"><span data-stu-id="a7a01-113">This attribute is required.</span></span>  <br/> |
|<span data-ttu-id="a7a01-114">ChangeKey</span><span class="sxs-lookup"><span data-stu-id="a7a01-114">ChangeKey</span></span>  <br/> |<span data-ttu-id="a7a01-115">Содержит строку, которая определяет к папке, которая определена в атрибуте Id версии.</span><span class="sxs-lookup"><span data-stu-id="a7a01-115">Contains a string that identifies a version of a folder that is identified by the Id attribute.</span></span> <span data-ttu-id="a7a01-116">Этот атрибут является необязательным.</span><span class="sxs-lookup"><span data-stu-id="a7a01-116">This attribute is optional.</span></span> <span data-ttu-id="a7a01-117">Этот атрибут используется, чтобы убедиться в том, что используется правильный версии папки.</span><span class="sxs-lookup"><span data-stu-id="a7a01-117">Use this attribute to make sure that the correct version of a folder is used.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="a7a01-118">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="a7a01-118">Child elements</span></span>

<span data-ttu-id="a7a01-119">Нет.</span><span class="sxs-lookup"><span data-stu-id="a7a01-119">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="a7a01-120">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="a7a01-120">Parent elements</span></span>

|<span data-ttu-id="a7a01-121">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="a7a01-121">**Element**</span></span>|<span data-ttu-id="a7a01-122">**Описание**</span><span class="sxs-lookup"><span data-stu-id="a7a01-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a7a01-123">ContextFolderId</span><span class="sxs-lookup"><span data-stu-id="a7a01-123">ContextFolderId</span></span>](contextfolderid.md) <br/> |<span data-ttu-id="a7a01-124">Указывает папку, предназначенное для действий, использующих папок.</span><span class="sxs-lookup"><span data-stu-id="a7a01-124">Indicates the folder that is targeted for actions that use folders.</span></span>  <br/> |
|[<span data-ttu-id="a7a01-125">CopiedEvent</span><span class="sxs-lookup"><span data-stu-id="a7a01-125">CopiedEvent</span></span>](copiedevent.md) <br/> |<span data-ttu-id="a7a01-126">Представляет событие, в котором копирование элемента или папки.</span><span class="sxs-lookup"><span data-stu-id="a7a01-126">Represents an event in which an item or folder is copied.</span></span>  <br/> |
|[<span data-ttu-id="a7a01-127">DestinationFolderId</span><span class="sxs-lookup"><span data-stu-id="a7a01-127">DestinationFolderId</span></span>](destinationfolderid.md) <br/> |<span data-ttu-id="a7a01-128">Определяет папку назначения для копирования и перемещения действия.</span><span class="sxs-lookup"><span data-stu-id="a7a01-128">Indicates the destination folder for copy and move actions.</span></span>  <br/> |
|[<span data-ttu-id="a7a01-129">ParentFolderId (TargetFolderIdType)</span><span class="sxs-lookup"><span data-stu-id="a7a01-129">ParentFolderId (TargetFolderIdType)</span></span>](parentfolderid-targetfolderidtype.md) <br/> | <span data-ttu-id="a7a01-130">Определяет папку, где создается на новую папку или элемент.</span><span class="sxs-lookup"><span data-stu-id="a7a01-130">Identifies the folder where a new folder or item is created.</span></span>  <br/><br/>  <span data-ttu-id="a7a01-131">Ниже приведены выражения XPath для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="a7a01-131">The following are the XPath expressions to this element:</span></span><br/>  <br/> `/CreateItem/ParentFolderId` <br/><br/>  `/CreateFolder/ParentFolderId` <br/> |
|[<span data-ttu-id="a7a01-132">BaseFolderIds</span><span class="sxs-lookup"><span data-stu-id="a7a01-132">BaseFolderIds</span></span>](basefolderids.md) <br/> |<span data-ttu-id="a7a01-133">Представляет коллекцию папок, которые будут получены для определения содержимого папки поиска.</span><span class="sxs-lookup"><span data-stu-id="a7a01-133">Represents the collection of folders that will be mined to determine the contents of a search folder.</span></span>  <br/> |
|[<span data-ttu-id="a7a01-134">Удаление (FolderSync)</span><span class="sxs-lookup"><span data-stu-id="a7a01-134">Delete (FolderSync)</span></span>](delete-foldersync.md) <br/> |<span data-ttu-id="a7a01-135">Определяет одну папку для удаления в локальном хранилище клиента.</span><span class="sxs-lookup"><span data-stu-id="a7a01-135">Identifies a single folder to delete in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="a7a01-136">Folder</span><span class="sxs-lookup"><span data-stu-id="a7a01-136">Folder</span></span>](folder.md) <br/> |<span data-ttu-id="a7a01-137">Представляет папку в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="a7a01-137">Represents a folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="a7a01-138">CalendarFolder</span><span class="sxs-lookup"><span data-stu-id="a7a01-138">CalendarFolder</span></span>](calendarfolder.md) <br/> |<span data-ttu-id="a7a01-139">Представляет папку Календарь в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="a7a01-139">Represents a calendar folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="a7a01-140">FolderChange</span><span class="sxs-lookup"><span data-stu-id="a7a01-140">FolderChange</span></span>](folderchange.md) <br/> |<span data-ttu-id="a7a01-141">Представляет коллекцию изменений выполняется на одной папке.</span><span class="sxs-lookup"><span data-stu-id="a7a01-141">Represents a collection of changes to be performed on a single folder.</span></span>  <br/> <span data-ttu-id="a7a01-142">Ниже приведен выражение XPath для этого элемента.`/UpdateFolder/FolderChanges/FolderChange`</span><span class="sxs-lookup"><span data-stu-id="a7a01-142">The following is the XPath expression to this element:  `/UpdateFolder/FolderChanges/FolderChange`</span></span> <br/> |
|[<span data-ttu-id="a7a01-143">ContactsFolder</span><span class="sxs-lookup"><span data-stu-id="a7a01-143">ContactsFolder</span></span>](contactsfolder.md) <br/> |<span data-ttu-id="a7a01-144">Представляет папке контактов в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="a7a01-144">Represents a contact folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="a7a01-145">SearchFolder</span><span class="sxs-lookup"><span data-stu-id="a7a01-145">SearchFolder</span></span>](searchfolder.md) <br/> |<span data-ttu-id="a7a01-146">Представляет папку поиска в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="a7a01-146">Represents a search folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="a7a01-147">TasksFolder</span><span class="sxs-lookup"><span data-stu-id="a7a01-147">TasksFolder</span></span>](tasksfolder.md) <br/> |<span data-ttu-id="a7a01-148">Представляет папку задач в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="a7a01-148">Represents a task folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="a7a01-149">ToFolderId</span><span class="sxs-lookup"><span data-stu-id="a7a01-149">ToFolderId</span></span>](tofolderid.md) <br/> | <span data-ttu-id="a7a01-150">Представляет конечной папки для копируемые или перемещения элемента или папки.</span><span class="sxs-lookup"><span data-stu-id="a7a01-150">Represents the destination folder for a copied or moved item or folder.</span></span> <br/> <br/>  <span data-ttu-id="a7a01-151">Ниже приведены выражения XPath для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="a7a01-151">The following are the XPath expressions to this element:</span></span> <br/> <br/>  `/MoveFolder/ToFolderId` <br/> <br/> `/CopyFolder/ToFolderId` <br/> <br/> `/MoveItem/ToFolderId`<br/> <br/>  `/CopyItem/ToFolderId` <br/> |
|[<span data-ttu-id="a7a01-152">SavedItemFolderId</span><span class="sxs-lookup"><span data-stu-id="a7a01-152">SavedItemFolderId</span></span>](saveditemfolderid.md) <br/> | <span data-ttu-id="a7a01-153">Определяет папку назначения для операций, обновление, отправка и создания элементов в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="a7a01-153">Identifies the target folder for operations that update, send, and create items in the Exchange store.</span></span>  <br/><br/>  <span data-ttu-id="a7a01-154">Ниже приведены выражения XPath для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="a7a01-154">The following are the XPath expressions to this element:</span></span> <br/> <br/>  `/CreateItem/SavedItemFolderId` <br/><br/>  `/UpdateItem/SavedItemFolderId` <br/><br/>  `/SendItem/SavedItemFolderId` <br/> |
|[<span data-ttu-id="a7a01-155">SyncFolderId</span><span class="sxs-lookup"><span data-stu-id="a7a01-155">SyncFolderId</span></span>](syncfolderid.md) <br/> |<span data-ttu-id="a7a01-156">Представляет папку, содержащую элементы для синхронизации.</span><span class="sxs-lookup"><span data-stu-id="a7a01-156">Represents the folder that contains the items to synchronize.</span></span>  <br/> |
|[<span data-ttu-id="a7a01-157">UserConfigurationName</span><span class="sxs-lookup"><span data-stu-id="a7a01-157">UserConfigurationName</span></span>](userconfigurationname.md) <br/> |<span data-ttu-id="a7a01-158">Представляет имя объекта конфигурации пользователя.</span><span class="sxs-lookup"><span data-stu-id="a7a01-158">Represents the name of a user configuration object.</span></span> <span data-ttu-id="a7a01-159">Имя объекта конфигурации пользователя — это идентификатор объекта конфигурации пользователя.</span><span class="sxs-lookup"><span data-stu-id="a7a01-159">The user configuration object name is the identifier for a user configuration object.</span></span>  <br/> |
|[<span data-ttu-id="a7a01-160">CopyToFolder</span><span class="sxs-lookup"><span data-stu-id="a7a01-160">CopyToFolder</span></span>](copytofolder.md) <br/> |<span data-ttu-id="a7a01-161">Определение идентификатора к папке, где будет скопировано элементов электронной почты.</span><span class="sxs-lookup"><span data-stu-id="a7a01-161">Identifies the ID of the folder that e-mail items will be copied to.</span></span>  <br/> |
|[<span data-ttu-id="a7a01-162">MoveToFolder</span><span class="sxs-lookup"><span data-stu-id="a7a01-162">MoveToFolder</span></span>](movetofolder.md) <br/> |<span data-ttu-id="a7a01-163">Определение идентификатора к папке, где планируется переместить сообщения электронной почты.</span><span class="sxs-lookup"><span data-stu-id="a7a01-163">Identifies the ID of the folder that e-mail items will be moved to.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="a7a01-164">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="a7a01-164">Text value</span></span>

<span data-ttu-id="a7a01-165">Нет.</span><span class="sxs-lookup"><span data-stu-id="a7a01-165">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="a7a01-166">Замечания</span><span class="sxs-lookup"><span data-stu-id="a7a01-166">Remarks</span></span>

<span data-ttu-id="a7a01-167">Все элементы **FolderId** , типа **FolderIdType** .</span><span class="sxs-lookup"><span data-stu-id="a7a01-167">All **FolderId** elements are of the **FolderIdType** type.</span></span> <span data-ttu-id="a7a01-168">Элемент **FolderId** является обязательным во всех случаях, за исключением в элементах, тип которого расширяет **BaseFolderType** или где **FolderId** элемент является частью выбор.</span><span class="sxs-lookup"><span data-stu-id="a7a01-168">The **FolderId** element is required in every case except in elements whose type extends the **BaseFolderType** or where the **FolderId** element is a part of a choice.</span></span> <span data-ttu-id="a7a01-169">Просмотрите схемы для получения дополнительных сведений.</span><span class="sxs-lookup"><span data-stu-id="a7a01-169">Review the schema for more information.</span></span> 
  
<span data-ttu-id="a7a01-170">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="a7a01-170">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a7a01-171">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="a7a01-171">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a7a01-172">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="a7a01-172">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="a7a01-173">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="a7a01-173">Schema Name</span></span>  <br/> |<span data-ttu-id="a7a01-174">Схема Types</span><span class="sxs-lookup"><span data-stu-id="a7a01-174">Types schema</span></span>  <br/> |
|<span data-ttu-id="a7a01-175">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="a7a01-175">Validation File</span></span>  <br/> |<span data-ttu-id="a7a01-176">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="a7a01-176">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="a7a01-177">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="a7a01-177">Can be Empty</span></span>  <br/> |<span data-ttu-id="a7a01-178">False</span><span class="sxs-lookup"><span data-stu-id="a7a01-178">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a7a01-179">См. также</span><span class="sxs-lookup"><span data-stu-id="a7a01-179">See also</span></span>

- [<span data-ttu-id="a7a01-180">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="a7a01-180">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="a7a01-181">Создание папки (веб-служб Exchange)</span><span class="sxs-lookup"><span data-stu-id="a7a01-181">Creating Folders (Exchange Web Services)</span></span>](http://msdn.microsoft.com/library/3b15b0ec-8691-45ed-9a24-a91ff732d6cf%28Office.15%29.aspx)

