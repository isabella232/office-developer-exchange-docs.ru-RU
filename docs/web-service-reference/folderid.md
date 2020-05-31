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
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762625"
---
# <a name="folderid"></a><span data-ttu-id="ec3bf-103">FolderId</span><span class="sxs-lookup"><span data-stu-id="ec3bf-103">FolderId</span></span>

<span data-ttu-id="ec3bf-104">Элемент **FolderId** содержит идентификатор и ключ изменения папки.</span><span class="sxs-lookup"><span data-stu-id="ec3bf-104">The **FolderId** element contains the identifier and change key of a folder.</span></span> 
  
```XML
<FolderId Id="" ChangeKey="" />
```

 <span data-ttu-id="ec3bf-105">**фолдеридтипе**</span><span class="sxs-lookup"><span data-stu-id="ec3bf-105">**FolderIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ec3bf-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="ec3bf-106">Attributes and elements</span></span>

<span data-ttu-id="ec3bf-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="ec3bf-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ec3bf-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="ec3bf-108">Attributes</span></span>

|<span data-ttu-id="ec3bf-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="ec3bf-109">**Attribute**</span></span>|<span data-ttu-id="ec3bf-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="ec3bf-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="ec3bf-111">Id</span><span class="sxs-lookup"><span data-stu-id="ec3bf-111">Id</span></span>  <br/> |<span data-ttu-id="ec3bf-112">Содержит строку, определяющую папку в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="ec3bf-112">Contains a string that identifies a folder in the Exchange store.</span></span> <span data-ttu-id="ec3bf-113">Этот атрибут является обязательным.</span><span class="sxs-lookup"><span data-stu-id="ec3bf-113">This attribute is required.</span></span>  <br/> |
|<span data-ttu-id="ec3bf-114">чанжекэй</span><span class="sxs-lookup"><span data-stu-id="ec3bf-114">ChangeKey</span></span>  <br/> |<span data-ttu-id="ec3bf-115">Содержит строку, определяющую версию папки, определяемую атрибутом ID.</span><span class="sxs-lookup"><span data-stu-id="ec3bf-115">Contains a string that identifies a version of a folder that is identified by the Id attribute.</span></span> <span data-ttu-id="ec3bf-116">Этот атрибут является необязательным.</span><span class="sxs-lookup"><span data-stu-id="ec3bf-116">This attribute is optional.</span></span> <span data-ttu-id="ec3bf-117">Используйте этот атрибут, чтобы убедиться, что используется правильная версия папки.</span><span class="sxs-lookup"><span data-stu-id="ec3bf-117">Use this attribute to make sure that the correct version of a folder is used.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="ec3bf-118">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="ec3bf-118">Child elements</span></span>

<span data-ttu-id="ec3bf-119">Нет.</span><span class="sxs-lookup"><span data-stu-id="ec3bf-119">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="ec3bf-120">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="ec3bf-120">Parent elements</span></span>

|<span data-ttu-id="ec3bf-121">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="ec3bf-121">**Element**</span></span>|<span data-ttu-id="ec3bf-122">**Описание**</span><span class="sxs-lookup"><span data-stu-id="ec3bf-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ec3bf-123">контекстфолдерид</span><span class="sxs-lookup"><span data-stu-id="ec3bf-123">ContextFolderId</span></span>](contextfolderid.md) <br/> |<span data-ttu-id="ec3bf-124">Указывает папку, предназначенную для действий, в которых используются папки.</span><span class="sxs-lookup"><span data-stu-id="ec3bf-124">Indicates the folder that is targeted for actions that use folders.</span></span>  <br/> |
|[<span data-ttu-id="ec3bf-125">копиедевент</span><span class="sxs-lookup"><span data-stu-id="ec3bf-125">CopiedEvent</span></span>](copiedevent.md) <br/> |<span data-ttu-id="ec3bf-126">Представляет событие, в котором копируется элемент или папка.</span><span class="sxs-lookup"><span data-stu-id="ec3bf-126">Represents an event in which an item or folder is copied.</span></span>  <br/> |
|[<span data-ttu-id="ec3bf-127">дестинатионфолдерид</span><span class="sxs-lookup"><span data-stu-id="ec3bf-127">DestinationFolderId</span></span>](destinationfolderid.md) <br/> |<span data-ttu-id="ec3bf-128">Указывает целевую папку для действий по копированию и перемещению.</span><span class="sxs-lookup"><span data-stu-id="ec3bf-128">Indicates the destination folder for copy and move actions.</span></span>  <br/> |
|[<span data-ttu-id="ec3bf-129">ParentFolderId (Таржетфолдеридтипе)</span><span class="sxs-lookup"><span data-stu-id="ec3bf-129">ParentFolderId (TargetFolderIdType)</span></span>](parentfolderid-targetfolderidtype.md) <br/> | <span data-ttu-id="ec3bf-130">Определяет папку, в которой создается новая папка или элемент.</span><span class="sxs-lookup"><span data-stu-id="ec3bf-130">Identifies the folder where a new folder or item is created.</span></span>  <br/><br/>  <span data-ttu-id="ec3bf-131">Ниже приведены выражения XPath для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="ec3bf-131">The following are the XPath expressions to this element:</span></span><br/>  <br/> `/CreateItem/ParentFolderId` <br/><br/>  `/CreateFolder/ParentFolderId` <br/> |
|[<span data-ttu-id="ec3bf-132">басефолдеридс</span><span class="sxs-lookup"><span data-stu-id="ec3bf-132">BaseFolderIds</span></span>](basefolderids.md) <br/> |<span data-ttu-id="ec3bf-133">Представляет коллекцию папок, которые будут mined для определения содержимого папки поиска.</span><span class="sxs-lookup"><span data-stu-id="ec3bf-133">Represents the collection of folders that will be mined to determine the contents of a search folder.</span></span>  <br/> |
|[<span data-ttu-id="ec3bf-134">Delete (Фолдерсинк)</span><span class="sxs-lookup"><span data-stu-id="ec3bf-134">Delete (FolderSync)</span></span>](delete-foldersync.md) <br/> |<span data-ttu-id="ec3bf-135">Определяет одну папку для удаления в локальном хранилище клиента.</span><span class="sxs-lookup"><span data-stu-id="ec3bf-135">Identifies a single folder to delete in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="ec3bf-136">Folder</span><span class="sxs-lookup"><span data-stu-id="ec3bf-136">Folder</span></span>](folder.md) <br/> |<span data-ttu-id="ec3bf-137">Представляет папку в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="ec3bf-137">Represents a folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="ec3bf-138">календарфолдер</span><span class="sxs-lookup"><span data-stu-id="ec3bf-138">CalendarFolder</span></span>](calendarfolder.md) <br/> |<span data-ttu-id="ec3bf-139">Представляет папку "Календарь" в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="ec3bf-139">Represents a calendar folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="ec3bf-140">FolderChange</span><span class="sxs-lookup"><span data-stu-id="ec3bf-140">FolderChange</span></span>](folderchange.md) <br/> |<span data-ttu-id="ec3bf-141">Представляет коллекцию изменений, выполняемых над одной папкой.</span><span class="sxs-lookup"><span data-stu-id="ec3bf-141">Represents a collection of changes to be performed on a single folder.</span></span>  <br/> <span data-ttu-id="ec3bf-142">Ниже приведено выражение XPath для этого элемента:`/UpdateFolder/FolderChanges/FolderChange`</span><span class="sxs-lookup"><span data-stu-id="ec3bf-142">The following is the XPath expression to this element:  `/UpdateFolder/FolderChanges/FolderChange`</span></span> <br/> |
|[<span data-ttu-id="ec3bf-143">контактсфолдер</span><span class="sxs-lookup"><span data-stu-id="ec3bf-143">ContactsFolder</span></span>](contactsfolder.md) <br/> |<span data-ttu-id="ec3bf-144">Представляет папку контактов в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="ec3bf-144">Represents a contact folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="ec3bf-145">SearchFolder</span><span class="sxs-lookup"><span data-stu-id="ec3bf-145">SearchFolder</span></span>](searchfolder.md) <br/> |<span data-ttu-id="ec3bf-146">Представляет папку поиска в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="ec3bf-146">Represents a search folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="ec3bf-147">тасксфолдер</span><span class="sxs-lookup"><span data-stu-id="ec3bf-147">TasksFolder</span></span>](tasksfolder.md) <br/> |<span data-ttu-id="ec3bf-148">Представляет папку задач в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="ec3bf-148">Represents a task folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="ec3bf-149">тофолдерид</span><span class="sxs-lookup"><span data-stu-id="ec3bf-149">ToFolderId</span></span>](tofolderid.md) <br/> | <span data-ttu-id="ec3bf-150">Представляет папку назначения для скопированного или перемещенного элемента или папки.</span><span class="sxs-lookup"><span data-stu-id="ec3bf-150">Represents the destination folder for a copied or moved item or folder.</span></span> <br/> <br/>  <span data-ttu-id="ec3bf-151">Ниже приведены выражения XPath для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="ec3bf-151">The following are the XPath expressions to this element:</span></span> <br/> <br/>  `/MoveFolder/ToFolderId` <br/> <br/> `/CopyFolder/ToFolderId` <br/> <br/> `/MoveItem/ToFolderId`<br/> <br/>  `/CopyItem/ToFolderId` <br/> |
|[<span data-ttu-id="ec3bf-152">саведитемфолдерид</span><span class="sxs-lookup"><span data-stu-id="ec3bf-152">SavedItemFolderId</span></span>](saveditemfolderid.md) <br/> | <span data-ttu-id="ec3bf-153">Определяет целевую папку для операций обновления, отправки и создания элементов в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="ec3bf-153">Identifies the target folder for operations that update, send, and create items in the Exchange store.</span></span>  <br/><br/>  <span data-ttu-id="ec3bf-154">Ниже приведены выражения XPath для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="ec3bf-154">The following are the XPath expressions to this element:</span></span> <br/> <br/>  `/CreateItem/SavedItemFolderId` <br/><br/>  `/UpdateItem/SavedItemFolderId` <br/><br/>  `/SendItem/SavedItemFolderId` <br/> |
|[<span data-ttu-id="ec3bf-155">синкфолдерид</span><span class="sxs-lookup"><span data-stu-id="ec3bf-155">SyncFolderId</span></span>](syncfolderid.md) <br/> |<span data-ttu-id="ec3bf-156">Представляет папку, содержащую синхронизируемые элементы.</span><span class="sxs-lookup"><span data-stu-id="ec3bf-156">Represents the folder that contains the items to synchronize.</span></span>  <br/> |
|[<span data-ttu-id="ec3bf-157">усерконфигуратионнаме</span><span class="sxs-lookup"><span data-stu-id="ec3bf-157">UserConfigurationName</span></span>](userconfigurationname.md) <br/> |<span data-ttu-id="ec3bf-158">Представляет имя объекта конфигурации пользователя.</span><span class="sxs-lookup"><span data-stu-id="ec3bf-158">Represents the name of a user configuration object.</span></span> <span data-ttu-id="ec3bf-159">Имя объекта конфигурации пользователя — это идентификатор объекта конфигурации пользователя.</span><span class="sxs-lookup"><span data-stu-id="ec3bf-159">The user configuration object name is the identifier for a user configuration object.</span></span>  <br/> |
|[<span data-ttu-id="ec3bf-160">CopyToFolder</span><span class="sxs-lookup"><span data-stu-id="ec3bf-160">CopyToFolder</span></span>](copytofolder.md) <br/> |<span data-ttu-id="ec3bf-161">Определяет идентификатор папки, в которую будут скопированы элементы электронной почты.</span><span class="sxs-lookup"><span data-stu-id="ec3bf-161">Identifies the ID of the folder that e-mail items will be copied to.</span></span>  <br/> |
|[<span data-ttu-id="ec3bf-162">MoveToFolder</span><span class="sxs-lookup"><span data-stu-id="ec3bf-162">MoveToFolder</span></span>](movetofolder.md) <br/> |<span data-ttu-id="ec3bf-163">Определяет идентификатор папки, в которую будут перемещены элементы электронной почты.</span><span class="sxs-lookup"><span data-stu-id="ec3bf-163">Identifies the ID of the folder that e-mail items will be moved to.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="ec3bf-164">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="ec3bf-164">Text value</span></span>

<span data-ttu-id="ec3bf-165">Нет.</span><span class="sxs-lookup"><span data-stu-id="ec3bf-165">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="ec3bf-166">Примечания</span><span class="sxs-lookup"><span data-stu-id="ec3bf-166">Remarks</span></span>

<span data-ttu-id="ec3bf-167">Все элементы **FolderId** имеют тип **фолдеридтипе** .</span><span class="sxs-lookup"><span data-stu-id="ec3bf-167">All **FolderId** elements are of the **FolderIdType** type.</span></span> <span data-ttu-id="ec3bf-168">Элемент **FolderId** является обязательным для каждого случая, за исключением элементов, тип которых расширяет **басефолдертипе** или где элемент **FolderId** является частью выбора.</span><span class="sxs-lookup"><span data-stu-id="ec3bf-168">The **FolderId** element is required in every case except in elements whose type extends the **BaseFolderType** or where the **FolderId** element is a part of a choice.</span></span> <span data-ttu-id="ec3bf-169">Просмотрите схему, чтобы получить дополнительные сведения.</span><span class="sxs-lookup"><span data-stu-id="ec3bf-169">Review the schema for more information.</span></span> 
  
<span data-ttu-id="ec3bf-170">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="ec3bf-170">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ec3bf-171">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="ec3bf-171">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ec3bf-172">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="ec3bf-172">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="ec3bf-173">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="ec3bf-173">Schema Name</span></span>  <br/> |<span data-ttu-id="ec3bf-174">Схема Types</span><span class="sxs-lookup"><span data-stu-id="ec3bf-174">Types schema</span></span>  <br/> |
|<span data-ttu-id="ec3bf-175">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="ec3bf-175">Validation File</span></span>  <br/> |<span data-ttu-id="ec3bf-176">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="ec3bf-176">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="ec3bf-177">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="ec3bf-177">Can be Empty</span></span>  <br/> |<span data-ttu-id="ec3bf-178">False</span><span class="sxs-lookup"><span data-stu-id="ec3bf-178">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ec3bf-179">См. также</span><span class="sxs-lookup"><span data-stu-id="ec3bf-179">See also</span></span>

- [<span data-ttu-id="ec3bf-180">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="ec3bf-180">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="ec3bf-181">Создание папок (веб-службы Exchange)</span><span class="sxs-lookup"><span data-stu-id="ec3bf-181">Creating Folders (Exchange Web Services)</span></span>](http://msdn.microsoft.com/library/3b15b0ec-8691-45ed-9a24-a91ff732d6cf%28Office.15%29.aspx)

