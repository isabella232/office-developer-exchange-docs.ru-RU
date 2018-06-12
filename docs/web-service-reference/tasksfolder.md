---
title: TasksFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- TasksFolder
api_type:
- schema
ms.assetid: 5a9a4612-8064-4986-b467-c44f268c64df
description: Элемент TasksFolder представляет папку задачи, содержащихся в почтовом ящике.
ms.openlocfilehash: b2151c68519a6ff15fbc74b48fc93a7e06af9e76
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19840138"
---
# <a name="tasksfolder"></a><span data-ttu-id="2e8c4-103">TasksFolder</span><span class="sxs-lookup"><span data-stu-id="2e8c4-103">TasksFolder</span></span>

<span data-ttu-id="2e8c4-104">Элемент **TasksFolder** представляет папку задачи, содержащихся в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="2e8c4-104">The **TasksFolder** element represents a Tasks folder that is contained in a mailbox.</span></span> 
  
```xml
<TasksFolder>
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
</TasksFolder>
```

<span data-ttu-id="2e8c4-105">**TasksFolderType**</span><span class="sxs-lookup"><span data-stu-id="2e8c4-105">**TasksFolderType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="2e8c4-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="2e8c4-106">Attributes and elements</span></span>

<span data-ttu-id="2e8c4-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="2e8c4-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2e8c4-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="2e8c4-108">Attributes</span></span>

<span data-ttu-id="2e8c4-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="2e8c4-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2e8c4-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="2e8c4-110">Child elements</span></span>

|<span data-ttu-id="2e8c4-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="2e8c4-111">**Element**</span></span>|<span data-ttu-id="2e8c4-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="2e8c4-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2e8c4-113">FolderId</span><span class="sxs-lookup"><span data-stu-id="2e8c4-113">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="2e8c4-114">Содержит идентификатор и ключ изменения папки задач.</span><span class="sxs-lookup"><span data-stu-id="2e8c4-114">Contains the identifier and change key of a Tasks folder.</span></span>  <br/> |
|[<span data-ttu-id="2e8c4-115">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="2e8c4-115">ParentFolderId</span></span>](parentfolderid.md) <br/> |<span data-ttu-id="2e8c4-116">Представляет идентификатор родительской папки, содержащей папки задач.</span><span class="sxs-lookup"><span data-stu-id="2e8c4-116">Represents the identifier of the parent folder that contains the Tasks folder.</span></span>  <br/> |
|[<span data-ttu-id="2e8c4-117">FolderClass</span><span class="sxs-lookup"><span data-stu-id="2e8c4-117">FolderClass</span></span>](folderclass.md) <br/> |<span data-ttu-id="2e8c4-118">Представляет класс папки для папки задач.</span><span class="sxs-lookup"><span data-stu-id="2e8c4-118">Represents the folder class for a Tasks folder.</span></span>  <br/> |
|[<span data-ttu-id="2e8c4-119">Отображаемое имя (строка)</span><span class="sxs-lookup"><span data-stu-id="2e8c4-119">DisplayName (string)</span></span>](displayname-string.md) <br/> |<span data-ttu-id="2e8c4-120">Содержит отображаемое имя папки задач.</span><span class="sxs-lookup"><span data-stu-id="2e8c4-120">Contains the display name of a Tasks folder.</span></span>  <br/> |
|[<span data-ttu-id="2e8c4-121">TotalCount</span><span class="sxs-lookup"><span data-stu-id="2e8c4-121">TotalCount</span></span>](totalcount.md) <br/> |<span data-ttu-id="2e8c4-122">Представляет общее число элементов в папке задачи.</span><span class="sxs-lookup"><span data-stu-id="2e8c4-122">Represents the total count of items within a Tasks folder.</span></span>  <br/> |
|[<span data-ttu-id="2e8c4-123">ChildFolderCount</span><span class="sxs-lookup"><span data-stu-id="2e8c4-123">ChildFolderCount</span></span>](childfoldercount.md) <br/> |<span data-ttu-id="2e8c4-124">Представляет число дочерних папок, содержащихся в папке задачи.</span><span class="sxs-lookup"><span data-stu-id="2e8c4-124">Represents the number of child folders that are contained within a Tasks folder.</span></span> <span data-ttu-id="2e8c4-125">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2e8c4-125">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="2e8c4-126">ExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="2e8c4-126">ExtendedProperty</span></span>](extendedproperty.md) <br/> |<span data-ttu-id="2e8c4-127">Определяет расширенные свойства папки задач.</span><span class="sxs-lookup"><span data-stu-id="2e8c4-127">Identifies extended properties on a Tasks folder.</span></span>  <br/> |
|[<span data-ttu-id="2e8c4-128">ManagedFolderInformation</span><span class="sxs-lookup"><span data-stu-id="2e8c4-128">ManagedFolderInformation</span></span>](managedfolderinformation.md) <br/> |<span data-ttu-id="2e8c4-129">Содержит сведения об управляемых папок.</span><span class="sxs-lookup"><span data-stu-id="2e8c4-129">Contains information about a managed folder.</span></span>  <br/> |
|[<span data-ttu-id="2e8c4-130">UnreadCount</span><span class="sxs-lookup"><span data-stu-id="2e8c4-130">UnreadCount</span></span>](unreadcount.md) <br/> |<span data-ttu-id="2e8c4-131">Представляет количество непрочитанных элементов в папке задач.</span><span class="sxs-lookup"><span data-stu-id="2e8c4-131">Represents the count of unread items within a Tasks folder.</span></span>  <br/> |
|[<span data-ttu-id="2e8c4-132">PermissionSet (PermissionSetType)</span><span class="sxs-lookup"><span data-stu-id="2e8c4-132">PermissionSet (PermissionSetType)</span></span>](permissionset-permissionsettype.md) <br/> |<span data-ttu-id="2e8c4-133">Содержит все настроенные разрешения для папки.</span><span class="sxs-lookup"><span data-stu-id="2e8c4-133">Contains all the configured permissions for a folder.</span></span> <span data-ttu-id="2e8c4-134">Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="2e8c4-134">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span>  <br/> |
|[<span data-ttu-id="2e8c4-135">EffectiveRights</span><span class="sxs-lookup"><span data-stu-id="2e8c4-135">EffectiveRights</span></span>](effectiverights.md) <br/> |<span data-ttu-id="2e8c4-136">Содержит права клиента на основании параметров разрешений для элемента или папки.</span><span class="sxs-lookup"><span data-stu-id="2e8c4-136">Contains the client's rights based on the permission settings for the item or folder.</span></span> <span data-ttu-id="2e8c4-137">Этот элемент доступен только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2e8c4-137">This element is read-only.</span></span> <span data-ttu-id="2e8c4-138">Этот элемент был представлен в Microsoft Exchange 2007 с пакетом обновления 1.</span><span class="sxs-lookup"><span data-stu-id="2e8c4-138">This element was introduced in Microsoft Exchange 2007 SP1.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="2e8c4-139">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="2e8c4-139">Parent elements</span></span>

|<span data-ttu-id="2e8c4-140">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="2e8c4-140">**Element**</span></span>|<span data-ttu-id="2e8c4-141">**Описание**</span><span class="sxs-lookup"><span data-stu-id="2e8c4-141">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2e8c4-142">AppendToFolderField</span><span class="sxs-lookup"><span data-stu-id="2e8c4-142">AppendToFolderField</span></span>](appendtofolderfield.md) <br/> |<span data-ttu-id="2e8c4-143">Указывает данные для добавления к папке свойство во время [операции UpdateFolder](updatefolder-operation.md).</span><span class="sxs-lookup"><span data-stu-id="2e8c4-143">Specifies data to append to a folder property during an [UpdateFolder operation](updatefolder-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="2e8c4-144">Создание (FolderSync)</span><span class="sxs-lookup"><span data-stu-id="2e8c4-144">Create (FolderSync)</span></span>](create-foldersync.md) <br/> |<span data-ttu-id="2e8c4-145">Определяет одну папку для создания в локальном хранилище клиента.</span><span class="sxs-lookup"><span data-stu-id="2e8c4-145">Identifies a single folder to create in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="2e8c4-146">SetFolderField</span><span class="sxs-lookup"><span data-stu-id="2e8c4-146">SetFolderField</span></span>](setfolderfield.md) <br/> |<span data-ttu-id="2e8c4-147">Представляет обновление для одного свойства папки в рамках одной [операции UpdateFolder](updatefolder-operation.md).</span><span class="sxs-lookup"><span data-stu-id="2e8c4-147">Represents an update to a single property on a folder in an [UpdateFolder operation](updatefolder-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="2e8c4-148">Обновление (FolderSync)</span><span class="sxs-lookup"><span data-stu-id="2e8c4-148">Update (FolderSync)</span></span>](update-foldersync.md) <br/> |<span data-ttu-id="2e8c4-149">Определяет одну папку для обновления в локальном хранилище клиента.</span><span class="sxs-lookup"><span data-stu-id="2e8c4-149">Identifies a single folder to update in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="2e8c4-150">Папки</span><span class="sxs-lookup"><span data-stu-id="2e8c4-150">Folders</span></span>](folders-ex15websvcsotherref.md) <br/> |<span data-ttu-id="2e8c4-151">Содержит набор папок, используемых в операциях папки.</span><span class="sxs-lookup"><span data-stu-id="2e8c4-151">Contains an array of folders that are used in folder operations.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="2e8c4-152">Замечания</span><span class="sxs-lookup"><span data-stu-id="2e8c4-152">Remarks</span></span>

<span data-ttu-id="2e8c4-153">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="2e8c4-153">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2e8c4-154">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="2e8c4-154">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2e8c4-155">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="2e8c4-155">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="2e8c4-156">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="2e8c4-156">Schema Name</span></span>  <br/> |<span data-ttu-id="2e8c4-157">Схема Types</span><span class="sxs-lookup"><span data-stu-id="2e8c4-157">Types schema</span></span>  <br/> |
|<span data-ttu-id="2e8c4-158">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="2e8c4-158">Validation File</span></span>  <br/> |<span data-ttu-id="2e8c4-159">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="2e8c4-159">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="2e8c4-160">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="2e8c4-160">Can be Empty</span></span>  <br/> |<span data-ttu-id="2e8c4-161">False</span><span class="sxs-lookup"><span data-stu-id="2e8c4-161">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="2e8c4-162">См. также</span><span class="sxs-lookup"><span data-stu-id="2e8c4-162">See also</span></span>

- [<span data-ttu-id="2e8c4-163">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="2e8c4-163">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

