---
title: тасксфолдер
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
description: Элемент Тасксфолдер представляет папку Tasks, содержащуюся в почтовом ящике.
ms.openlocfilehash: 522fe485482bd8159927f9925b7a5582ba2e1c22
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465340"
---
# <a name="tasksfolder"></a><span data-ttu-id="27151-103">тасксфолдер</span><span class="sxs-lookup"><span data-stu-id="27151-103">TasksFolder</span></span>

<span data-ttu-id="27151-104">Элемент **тасксфолдер** представляет папку Tasks, содержащуюся в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="27151-104">The **TasksFolder** element represents a Tasks folder that is contained in a mailbox.</span></span> 
  
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

<span data-ttu-id="27151-105">**тасксфолдертипе**</span><span class="sxs-lookup"><span data-stu-id="27151-105">**TasksFolderType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="27151-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="27151-106">Attributes and elements</span></span>

<span data-ttu-id="27151-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="27151-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="27151-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="27151-108">Attributes</span></span>

<span data-ttu-id="27151-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="27151-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="27151-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="27151-110">Child elements</span></span>

|<span data-ttu-id="27151-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="27151-111">**Element**</span></span>|<span data-ttu-id="27151-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="27151-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="27151-113">FolderId</span><span class="sxs-lookup"><span data-stu-id="27151-113">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="27151-114">Содержит идентификатор и ключ изменения папки Tasks.</span><span class="sxs-lookup"><span data-stu-id="27151-114">Contains the identifier and change key of a Tasks folder.</span></span>  <br/> |
|[<span data-ttu-id="27151-115">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="27151-115">ParentFolderId</span></span>](parentfolderid.md) <br/> |<span data-ttu-id="27151-116">Представляет идентификатор родительской папки, содержащей папку Tasks.</span><span class="sxs-lookup"><span data-stu-id="27151-116">Represents the identifier of the parent folder that contains the Tasks folder.</span></span>  <br/> |
|[<span data-ttu-id="27151-117">фолдеркласс</span><span class="sxs-lookup"><span data-stu-id="27151-117">FolderClass</span></span>](folderclass.md) <br/> |<span data-ttu-id="27151-118">Представляет класс Folder для папки Tasks.</span><span class="sxs-lookup"><span data-stu-id="27151-118">Represents the folder class for a Tasks folder.</span></span>  <br/> |
|[<span data-ttu-id="27151-119">DisplayName (строка)</span><span class="sxs-lookup"><span data-stu-id="27151-119">DisplayName (string)</span></span>](displayname-string.md) <br/> |<span data-ttu-id="27151-120">Содержит отображаемое имя папки задач.</span><span class="sxs-lookup"><span data-stu-id="27151-120">Contains the display name of a Tasks folder.</span></span>  <br/> |
|[<span data-ttu-id="27151-121">тоталкаунт</span><span class="sxs-lookup"><span data-stu-id="27151-121">TotalCount</span></span>](totalcount.md) <br/> |<span data-ttu-id="27151-122">Представляет общее количество элементов в папке "задачи".</span><span class="sxs-lookup"><span data-stu-id="27151-122">Represents the total count of items within a Tasks folder.</span></span>  <br/> |
|[<span data-ttu-id="27151-123">чилдфолдеркаунт</span><span class="sxs-lookup"><span data-stu-id="27151-123">ChildFolderCount</span></span>](childfoldercount.md) <br/> |<span data-ttu-id="27151-124">Представляет количество дочерних папок, содержащихся в папке Tasks.</span><span class="sxs-lookup"><span data-stu-id="27151-124">Represents the number of child folders that are contained within a Tasks folder.</span></span> <span data-ttu-id="27151-125">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="27151-125">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="27151-126">ExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="27151-126">ExtendedProperty</span></span>](extendedproperty.md) <br/> |<span data-ttu-id="27151-127">Определяет расширенные свойства для папки Tasks.</span><span class="sxs-lookup"><span data-stu-id="27151-127">Identifies extended properties on a Tasks folder.</span></span>  <br/> |
|[<span data-ttu-id="27151-128">манажедфолдеринформатион</span><span class="sxs-lookup"><span data-stu-id="27151-128">ManagedFolderInformation</span></span>](managedfolderinformation.md) <br/> |<span data-ttu-id="27151-129">Содержит сведения об управляемой папке.</span><span class="sxs-lookup"><span data-stu-id="27151-129">Contains information about a managed folder.</span></span>  <br/> |
|[<span data-ttu-id="27151-130">унреадкаунт</span><span class="sxs-lookup"><span data-stu-id="27151-130">UnreadCount</span></span>](unreadcount.md) <br/> |<span data-ttu-id="27151-131">Представляет количество непрочитанных элементов в папке "задачи".</span><span class="sxs-lookup"><span data-stu-id="27151-131">Represents the count of unread items within a Tasks folder.</span></span>  <br/> |
|[<span data-ttu-id="27151-132">PermissionSet (Пермиссионсеттипе)</span><span class="sxs-lookup"><span data-stu-id="27151-132">PermissionSet (PermissionSetType)</span></span>](permissionset-permissionsettype.md) <br/> |<span data-ttu-id="27151-133">Содержит все настроенные разрешения для папки.</span><span class="sxs-lookup"><span data-stu-id="27151-133">Contains all the configured permissions for a folder.</span></span> <span data-ttu-id="27151-134">Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="27151-134">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span>  <br/> |
|[<span data-ttu-id="27151-135">еффективеригхтс</span><span class="sxs-lookup"><span data-stu-id="27151-135">EffectiveRights</span></span>](effectiverights.md) <br/> |<span data-ttu-id="27151-136">Содержит права клиента на основе параметров разрешений для элемента или папки.</span><span class="sxs-lookup"><span data-stu-id="27151-136">Contains the client's rights based on the permission settings for the item or folder.</span></span> <span data-ttu-id="27151-137">Этот элемент доступен только для чтения.</span><span class="sxs-lookup"><span data-stu-id="27151-137">This element is read-only.</span></span> <span data-ttu-id="27151-138">Этот элемент появился в Microsoft Exchange 2007 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="27151-138">This element was introduced in Microsoft Exchange 2007 SP1.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="27151-139">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="27151-139">Parent elements</span></span>

|<span data-ttu-id="27151-140">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="27151-140">**Element**</span></span>|<span data-ttu-id="27151-141">**Описание**</span><span class="sxs-lookup"><span data-stu-id="27151-141">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="27151-142">аппендтофолдерфиелд</span><span class="sxs-lookup"><span data-stu-id="27151-142">AppendToFolderField</span></span>](appendtofolderfield.md) <br/> |<span data-ttu-id="27151-143">Задает данные, добавляемые к свойству folder во время [операции операцию UpdateFolder](updatefolder-operation.md).</span><span class="sxs-lookup"><span data-stu-id="27151-143">Specifies data to append to a folder property during an [UpdateFolder operation](updatefolder-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="27151-144">Create (Фолдерсинк)</span><span class="sxs-lookup"><span data-stu-id="27151-144">Create (FolderSync)</span></span>](create-foldersync.md) <br/> |<span data-ttu-id="27151-145">Определяет одну папку для создания в локальном хранилище клиента.</span><span class="sxs-lookup"><span data-stu-id="27151-145">Identifies a single folder to create in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="27151-146">сетфолдерфиелд</span><span class="sxs-lookup"><span data-stu-id="27151-146">SetFolderField</span></span>](setfolderfield.md) <br/> |<span data-ttu-id="27151-147">Представляет обновление одного свойства папки в [операции операцию UpdateFolder](updatefolder-operation.md).</span><span class="sxs-lookup"><span data-stu-id="27151-147">Represents an update to a single property on a folder in an [UpdateFolder operation](updatefolder-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="27151-148">Обновление (Фолдерсинк)</span><span class="sxs-lookup"><span data-stu-id="27151-148">Update (FolderSync)</span></span>](update-foldersync.md) <br/> |<span data-ttu-id="27151-149">Определяет одну папку для обновления в локальном хранилище клиента.</span><span class="sxs-lookup"><span data-stu-id="27151-149">Identifies a single folder to update in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="27151-150">Folders</span><span class="sxs-lookup"><span data-stu-id="27151-150">Folders</span></span>](folders-ex15websvcsotherref.md) <br/> |<span data-ttu-id="27151-151">Содержит массив папок, используемых в операциях с папками.</span><span class="sxs-lookup"><span data-stu-id="27151-151">Contains an array of folders that are used in folder operations.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="27151-152">Примечания</span><span class="sxs-lookup"><span data-stu-id="27151-152">Remarks</span></span>

<span data-ttu-id="27151-153">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="27151-153">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="27151-154">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="27151-154">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="27151-155">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="27151-155">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="27151-156">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="27151-156">Schema Name</span></span>  <br/> |<span data-ttu-id="27151-157">Схема Types</span><span class="sxs-lookup"><span data-stu-id="27151-157">Types schema</span></span>  <br/> |
|<span data-ttu-id="27151-158">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="27151-158">Validation File</span></span>  <br/> |<span data-ttu-id="27151-159">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="27151-159">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="27151-160">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="27151-160">Can be Empty</span></span>  <br/> |<span data-ttu-id="27151-161">False</span><span class="sxs-lookup"><span data-stu-id="27151-161">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="27151-162">См. также</span><span class="sxs-lookup"><span data-stu-id="27151-162">See also</span></span>

- [<span data-ttu-id="27151-163">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="27151-163">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

