---
title: SearchFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SearchFolder
api_type:
- schema
ms.assetid: 1a7d408b-2e98-4391-8834-085ed6d5757c
description: Элемент SearchFolder представляет папки поиска, которая содержится в почтовом ящике.
ms.openlocfilehash: d842c54dab7950c68e26804b676834c2d95debad
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835302"
---
# <a name="searchfolder"></a><span data-ttu-id="8c205-103">SearchFolder</span><span class="sxs-lookup"><span data-stu-id="8c205-103">SearchFolder</span></span>

<span data-ttu-id="8c205-104">Элемент **SearchFolder** представляет папки поиска, которая содержится в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="8c205-104">The **SearchFolder** element represents a search folder that is contained in a mailbox.</span></span> 
  
```xml
<SearchFolder>
   <FolderId/>
   <ParentFolderId/>
   <FolderClass/>
   <DisplayName/>
   <TotalCount/>
   <ChildFolderCount/>
   <ExtendedProperty/>
   <ManagedFolderInformation/>
   <UnreadCount/>
   <SearchParameters/>
   <PermissionSet/>
      <EffectiveRights/>
</SearchFolder>
```

 <span data-ttu-id="8c205-105">**SearchFolderType**</span><span class="sxs-lookup"><span data-stu-id="8c205-105">**SearchFolderType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="8c205-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="8c205-106">Attributes and elements</span></span>

<span data-ttu-id="8c205-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="8c205-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8c205-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="8c205-108">Attributes</span></span>

<span data-ttu-id="8c205-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="8c205-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8c205-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="8c205-110">Child elements</span></span>

|<span data-ttu-id="8c205-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="8c205-111">**Element**</span></span>|<span data-ttu-id="8c205-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="8c205-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8c205-113">FolderId</span><span class="sxs-lookup"><span data-stu-id="8c205-113">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="8c205-114">Содержит идентификатор и ключ изменения папки.</span><span class="sxs-lookup"><span data-stu-id="8c205-114">Contains the identifier and change key of a folder.</span></span>  <br/> |
|[<span data-ttu-id="8c205-115">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="8c205-115">ParentFolderId</span></span>](parentfolderid.md) <br/> |<span data-ttu-id="8c205-116">Представляет идентификатор родительской папки, содержащей папку.</span><span class="sxs-lookup"><span data-stu-id="8c205-116">Represents the identifier of the parent folder that contains the folder.</span></span>  <br/> |
|[<span data-ttu-id="8c205-117">FolderClass</span><span class="sxs-lookup"><span data-stu-id="8c205-117">FolderClass</span></span>](folderclass.md) <br/> |<span data-ttu-id="8c205-118">Представляет класс папки для данной папки.</span><span class="sxs-lookup"><span data-stu-id="8c205-118">Represents the folder class for a given folder.</span></span>  <br/> |
|[<span data-ttu-id="8c205-119">Отображаемое имя (строка)</span><span class="sxs-lookup"><span data-stu-id="8c205-119">DisplayName (string)</span></span>](displayname-string.md) <br/> |<span data-ttu-id="8c205-120">Содержит отображаемое имя папки.</span><span class="sxs-lookup"><span data-stu-id="8c205-120">Contains the display name of a folder.</span></span>  <br/> |
|[<span data-ttu-id="8c205-121">TotalCount</span><span class="sxs-lookup"><span data-stu-id="8c205-121">TotalCount</span></span>](totalcount.md) <br/> |<span data-ttu-id="8c205-122">Представляет общее число элементов в указанной папке.</span><span class="sxs-lookup"><span data-stu-id="8c205-122">Represents the total count of items within a given folder.</span></span>  <br/> |
|[<span data-ttu-id="8c205-123">ChildFolderCount</span><span class="sxs-lookup"><span data-stu-id="8c205-123">ChildFolderCount</span></span>](childfoldercount.md) <br/> |<span data-ttu-id="8c205-124">Представляет число дочерних папок, содержащихся в папке.</span><span class="sxs-lookup"><span data-stu-id="8c205-124">Represents the number of child folders contained within a folder.</span></span> <span data-ttu-id="8c205-125">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8c205-125">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="8c205-126">ExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="8c205-126">ExtendedProperty</span></span>](extendedproperty.md) <br/> |<span data-ttu-id="8c205-127">Определяет расширенные свойства папки.</span><span class="sxs-lookup"><span data-stu-id="8c205-127">Identifies extended properties on folders.</span></span>  <br/> |
|[<span data-ttu-id="8c205-128">ManagedFolderInformation</span><span class="sxs-lookup"><span data-stu-id="8c205-128">ManagedFolderInformation</span></span>](managedfolderinformation.md) <br/> |<span data-ttu-id="8c205-129">Содержит сведения об управляемых папок.</span><span class="sxs-lookup"><span data-stu-id="8c205-129">Contains information about a managed folder.</span></span>  <br/> |
|[<span data-ttu-id="8c205-130">UnreadCount</span><span class="sxs-lookup"><span data-stu-id="8c205-130">UnreadCount</span></span>](unreadcount.md) <br/> |<span data-ttu-id="8c205-131">Представляет количество непрочитанных элементов в указанной папке.</span><span class="sxs-lookup"><span data-stu-id="8c205-131">Represents the count of unread items within a given folder.</span></span>  <br/> |
|[<span data-ttu-id="8c205-132">SearchParameters</span><span class="sxs-lookup"><span data-stu-id="8c205-132">SearchParameters</span></span>](searchparameters.md) <br/> |<span data-ttu-id="8c205-133">Содержит параметры, определяющие папки поиска.</span><span class="sxs-lookup"><span data-stu-id="8c205-133">Contains the parameters that define a search folder.</span></span>  <br/> |
|[<span data-ttu-id="8c205-134">PermissionSet (PermissionSetType)</span><span class="sxs-lookup"><span data-stu-id="8c205-134">PermissionSet (PermissionSetType)</span></span>](permissionset-permissionsettype.md) <br/> |<span data-ttu-id="8c205-135">Содержит все настроенные разрешения для папки.</span><span class="sxs-lookup"><span data-stu-id="8c205-135">Contains all the configured permissions for a folder.</span></span> <span data-ttu-id="8c205-136">Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="8c205-136">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span>  <br/> |
|[<span data-ttu-id="8c205-137">EffectiveRights</span><span class="sxs-lookup"><span data-stu-id="8c205-137">EffectiveRights</span></span>](effectiverights.md) <br/> |<span data-ttu-id="8c205-138">Содержит права клиента на основании параметров разрешений для элемента или папки.</span><span class="sxs-lookup"><span data-stu-id="8c205-138">Contains the client's rights based on the permission settings for the item or folder.</span></span> <span data-ttu-id="8c205-139">Этот элемент доступен только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8c205-139">This element is read-only.</span></span> <span data-ttu-id="8c205-140">Этот элемент появился в Exchange 2007 с пакетом обновления 1.</span><span class="sxs-lookup"><span data-stu-id="8c205-140">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="8c205-141">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="8c205-141">Parent elements</span></span>

|<span data-ttu-id="8c205-142">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="8c205-142">**Element**</span></span>|<span data-ttu-id="8c205-143">**Описание**</span><span class="sxs-lookup"><span data-stu-id="8c205-143">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8c205-144">AppendToFolderField</span><span class="sxs-lookup"><span data-stu-id="8c205-144">AppendToFolderField</span></span>](appendtofolderfield.md) <br/> |<span data-ttu-id="8c205-145">Указывает данные для добавления к папке свойство во время [операции UpdateFolder](updatefolder-operation.md).</span><span class="sxs-lookup"><span data-stu-id="8c205-145">Specifies data to append to a folder property during an [UpdateFolder operation](updatefolder-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="8c205-146">Создание (FolderSync)</span><span class="sxs-lookup"><span data-stu-id="8c205-146">Create (FolderSync)</span></span>](create-foldersync.md) <br/> |<span data-ttu-id="8c205-147">Определяет одну папку для создания в локальном хранилище клиента.</span><span class="sxs-lookup"><span data-stu-id="8c205-147">Identifies a single folder to create in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="8c205-148">SetFolderField</span><span class="sxs-lookup"><span data-stu-id="8c205-148">SetFolderField</span></span>](setfolderfield.md) <br/> |<span data-ttu-id="8c205-149">Представляет обновление для одного свойства папки в рамках одной [операции UpdateFolder](updatefolder-operation.md).</span><span class="sxs-lookup"><span data-stu-id="8c205-149">Represents an update to a single property on a folder in an [UpdateFolder operation](updatefolder-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="8c205-150">Обновление (FolderSync)</span><span class="sxs-lookup"><span data-stu-id="8c205-150">Update (FolderSync)</span></span>](update-foldersync.md) <br/> |<span data-ttu-id="8c205-151">Определяет одну папку для обновления в локальном хранилище клиента.</span><span class="sxs-lookup"><span data-stu-id="8c205-151">Identifies a single folder to update in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="8c205-152">Папки</span><span class="sxs-lookup"><span data-stu-id="8c205-152">Folders</span></span>](folders-ex15websvcsotherref.md) <br/> |<span data-ttu-id="8c205-153">Содержит набор папок, используемых в папке операции.</span><span class="sxs-lookup"><span data-stu-id="8c205-153">Contains an array of folders used in folder operations.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="8c205-154">Замечания</span><span class="sxs-lookup"><span data-stu-id="8c205-154">Remarks</span></span>

 <span data-ttu-id="8c205-155">**SearchFolder** используется для папок поиска регулярных и MicrosoftOfficeOutlook и Outlook Web Access отображается папки поиска.</span><span class="sxs-lookup"><span data-stu-id="8c205-155">**SearchFolder** is used for both regular search folders and MicrosoftOfficeOutlook and Outlook Web Access visible search folders.</span></span> <span data-ttu-id="8c205-156">Для папки поиска должна быть видна для Outlook и Outlook Web Access необходимо создать папку в папке различающееся SearchFolders.</span><span class="sxs-lookup"><span data-stu-id="8c205-156">For a search folder to be visible to Outlook and Outlook Web Access, the folder must be created under the SearchFolders distinguished folder.</span></span> 
  
<span data-ttu-id="8c205-157">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="8c205-157">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="8c205-158">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="8c205-158">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8c205-159">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="8c205-159">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="8c205-160">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="8c205-160">Schema Name</span></span>  <br/> |<span data-ttu-id="8c205-161">Схема Types</span><span class="sxs-lookup"><span data-stu-id="8c205-161">Types schema</span></span>  <br/> |
|<span data-ttu-id="8c205-162">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="8c205-162">Validation File</span></span>  <br/> |<span data-ttu-id="8c205-163">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="8c205-163">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="8c205-164">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="8c205-164">Can be Empty</span></span>  <br/> |<span data-ttu-id="8c205-165">False</span><span class="sxs-lookup"><span data-stu-id="8c205-165">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="8c205-166">См. также</span><span class="sxs-lookup"><span data-stu-id="8c205-166">See also</span></span>



- [<span data-ttu-id="8c205-167">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="8c205-167">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

