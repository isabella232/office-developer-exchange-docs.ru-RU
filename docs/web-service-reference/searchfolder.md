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
description: Элемент SearchFolder представляет папку поиска, содержащуюся в почтовом ящике.
ms.openlocfilehash: e1d5893e00f3b199451622061785e2566c6f32e5
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44464009"
---
# <a name="searchfolder"></a><span data-ttu-id="1b919-103">SearchFolder</span><span class="sxs-lookup"><span data-stu-id="1b919-103">SearchFolder</span></span>

<span data-ttu-id="1b919-104">Элемент **SearchFolder** представляет папку поиска, содержащуюся в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="1b919-104">The **SearchFolder** element represents a search folder that is contained in a mailbox.</span></span> 
  
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

 <span data-ttu-id="1b919-105">**сеарчфолдертипе**</span><span class="sxs-lookup"><span data-stu-id="1b919-105">**SearchFolderType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1b919-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="1b919-106">Attributes and elements</span></span>

<span data-ttu-id="1b919-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="1b919-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1b919-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="1b919-108">Attributes</span></span>

<span data-ttu-id="1b919-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="1b919-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1b919-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="1b919-110">Child elements</span></span>

|<span data-ttu-id="1b919-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="1b919-111">**Element**</span></span>|<span data-ttu-id="1b919-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="1b919-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1b919-113">FolderId</span><span class="sxs-lookup"><span data-stu-id="1b919-113">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="1b919-114">Содержит идентификатор и ключ изменения папки.</span><span class="sxs-lookup"><span data-stu-id="1b919-114">Contains the identifier and change key of a folder.</span></span>  <br/> |
|[<span data-ttu-id="1b919-115">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="1b919-115">ParentFolderId</span></span>](parentfolderid.md) <br/> |<span data-ttu-id="1b919-116">Представляет идентификатор родительской папки, содержащей папку.</span><span class="sxs-lookup"><span data-stu-id="1b919-116">Represents the identifier of the parent folder that contains the folder.</span></span>  <br/> |
|[<span data-ttu-id="1b919-117">фолдеркласс</span><span class="sxs-lookup"><span data-stu-id="1b919-117">FolderClass</span></span>](folderclass.md) <br/> |<span data-ttu-id="1b919-118">Представляет класс папки для данной папки.</span><span class="sxs-lookup"><span data-stu-id="1b919-118">Represents the folder class for a given folder.</span></span>  <br/> |
|[<span data-ttu-id="1b919-119">DisplayName (строка)</span><span class="sxs-lookup"><span data-stu-id="1b919-119">DisplayName (string)</span></span>](displayname-string.md) <br/> |<span data-ttu-id="1b919-120">Содержит отображаемое имя папки.</span><span class="sxs-lookup"><span data-stu-id="1b919-120">Contains the display name of a folder.</span></span>  <br/> |
|[<span data-ttu-id="1b919-121">тоталкаунт</span><span class="sxs-lookup"><span data-stu-id="1b919-121">TotalCount</span></span>](totalcount.md) <br/> |<span data-ttu-id="1b919-122">Представляет общее количество элементов в заданной папке.</span><span class="sxs-lookup"><span data-stu-id="1b919-122">Represents the total count of items within a given folder.</span></span>  <br/> |
|[<span data-ttu-id="1b919-123">чилдфолдеркаунт</span><span class="sxs-lookup"><span data-stu-id="1b919-123">ChildFolderCount</span></span>](childfoldercount.md) <br/> |<span data-ttu-id="1b919-124">Представляет количество дочерних папок, содержащихся в папке.</span><span class="sxs-lookup"><span data-stu-id="1b919-124">Represents the number of child folders contained within a folder.</span></span> <span data-ttu-id="1b919-125">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1b919-125">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="1b919-126">ExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="1b919-126">ExtendedProperty</span></span>](extendedproperty.md) <br/> |<span data-ttu-id="1b919-127">Определяет расширенные свойства для папок.</span><span class="sxs-lookup"><span data-stu-id="1b919-127">Identifies extended properties on folders.</span></span>  <br/> |
|[<span data-ttu-id="1b919-128">манажедфолдеринформатион</span><span class="sxs-lookup"><span data-stu-id="1b919-128">ManagedFolderInformation</span></span>](managedfolderinformation.md) <br/> |<span data-ttu-id="1b919-129">Содержит сведения об управляемой папке.</span><span class="sxs-lookup"><span data-stu-id="1b919-129">Contains information about a managed folder.</span></span>  <br/> |
|[<span data-ttu-id="1b919-130">унреадкаунт</span><span class="sxs-lookup"><span data-stu-id="1b919-130">UnreadCount</span></span>](unreadcount.md) <br/> |<span data-ttu-id="1b919-131">Представляет количество непрочитанных элементов в заданной папке.</span><span class="sxs-lookup"><span data-stu-id="1b919-131">Represents the count of unread items within a given folder.</span></span>  <br/> |
|[<span data-ttu-id="1b919-132">сеарчпараметерс</span><span class="sxs-lookup"><span data-stu-id="1b919-132">SearchParameters</span></span>](searchparameters.md) <br/> |<span data-ttu-id="1b919-133">Содержит параметры, определяющие папку поиска.</span><span class="sxs-lookup"><span data-stu-id="1b919-133">Contains the parameters that define a search folder.</span></span>  <br/> |
|[<span data-ttu-id="1b919-134">PermissionSet (Пермиссионсеттипе)</span><span class="sxs-lookup"><span data-stu-id="1b919-134">PermissionSet (PermissionSetType)</span></span>](permissionset-permissionsettype.md) <br/> |<span data-ttu-id="1b919-135">Содержит все настроенные разрешения для папки.</span><span class="sxs-lookup"><span data-stu-id="1b919-135">Contains all the configured permissions for a folder.</span></span> <span data-ttu-id="1b919-136">Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="1b919-136">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span>  <br/> |
|[<span data-ttu-id="1b919-137">еффективеригхтс</span><span class="sxs-lookup"><span data-stu-id="1b919-137">EffectiveRights</span></span>](effectiverights.md) <br/> |<span data-ttu-id="1b919-138">Содержит права клиента на основе параметров разрешений для элемента или папки.</span><span class="sxs-lookup"><span data-stu-id="1b919-138">Contains the client's rights based on the permission settings for the item or folder.</span></span> <span data-ttu-id="1b919-139">Этот элемент доступен только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1b919-139">This element is read-only.</span></span> <span data-ttu-id="1b919-140">Этот элемент появился в Exchange 2007 с пакетом обновления 1.</span><span class="sxs-lookup"><span data-stu-id="1b919-140">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="1b919-141">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="1b919-141">Parent elements</span></span>

|<span data-ttu-id="1b919-142">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="1b919-142">**Element**</span></span>|<span data-ttu-id="1b919-143">**Описание**</span><span class="sxs-lookup"><span data-stu-id="1b919-143">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1b919-144">аппендтофолдерфиелд</span><span class="sxs-lookup"><span data-stu-id="1b919-144">AppendToFolderField</span></span>](appendtofolderfield.md) <br/> |<span data-ttu-id="1b919-145">Задает данные, добавляемые к свойству folder во время [операции операцию UpdateFolder](updatefolder-operation.md).</span><span class="sxs-lookup"><span data-stu-id="1b919-145">Specifies data to append to a folder property during an [UpdateFolder operation](updatefolder-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="1b919-146">Create (Фолдерсинк)</span><span class="sxs-lookup"><span data-stu-id="1b919-146">Create (FolderSync)</span></span>](create-foldersync.md) <br/> |<span data-ttu-id="1b919-147">Определяет одну папку для создания в локальном хранилище клиента.</span><span class="sxs-lookup"><span data-stu-id="1b919-147">Identifies a single folder to create in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="1b919-148">сетфолдерфиелд</span><span class="sxs-lookup"><span data-stu-id="1b919-148">SetFolderField</span></span>](setfolderfield.md) <br/> |<span data-ttu-id="1b919-149">Представляет обновление одного свойства папки в [операции операцию UpdateFolder](updatefolder-operation.md).</span><span class="sxs-lookup"><span data-stu-id="1b919-149">Represents an update to a single property on a folder in an [UpdateFolder operation](updatefolder-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="1b919-150">Обновление (Фолдерсинк)</span><span class="sxs-lookup"><span data-stu-id="1b919-150">Update (FolderSync)</span></span>](update-foldersync.md) <br/> |<span data-ttu-id="1b919-151">Определяет одну папку для обновления в локальном хранилище клиента.</span><span class="sxs-lookup"><span data-stu-id="1b919-151">Identifies a single folder to update in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="1b919-152">Folders</span><span class="sxs-lookup"><span data-stu-id="1b919-152">Folders</span></span>](folders-ex15websvcsotherref.md) <br/> |<span data-ttu-id="1b919-153">Содержит массив папок, используемых в операциях с папками.</span><span class="sxs-lookup"><span data-stu-id="1b919-153">Contains an array of folders used in folder operations.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="1b919-154">Примечания</span><span class="sxs-lookup"><span data-stu-id="1b919-154">Remarks</span></span>

 <span data-ttu-id="1b919-155">**SearchFolder** используется как для обычных папок поиска, так и для общедоступных папок поиска Майкрософтofficeoutlook и Outlook Web Access.</span><span class="sxs-lookup"><span data-stu-id="1b919-155">**SearchFolder** is used for both regular search folders and MicrosoftOfficeOutlook and Outlook Web Access visible search folders.</span></span> <span data-ttu-id="1b919-156">Чтобы папка поиска была видна в Outlook и Outlook Web Access, она должна быть создана в папке SearchFolders.</span><span class="sxs-lookup"><span data-stu-id="1b919-156">For a search folder to be visible to Outlook and Outlook Web Access, the folder must be created under the SearchFolders distinguished folder.</span></span> 
  
<span data-ttu-id="1b919-157">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="1b919-157">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1b919-158">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="1b919-158">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1b919-159">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="1b919-159">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="1b919-160">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="1b919-160">Schema Name</span></span>  <br/> |<span data-ttu-id="1b919-161">Схема Types</span><span class="sxs-lookup"><span data-stu-id="1b919-161">Types schema</span></span>  <br/> |
|<span data-ttu-id="1b919-162">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="1b919-162">Validation File</span></span>  <br/> |<span data-ttu-id="1b919-163">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="1b919-163">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="1b919-164">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="1b919-164">Can be Empty</span></span>  <br/> |<span data-ttu-id="1b919-165">False</span><span class="sxs-lookup"><span data-stu-id="1b919-165">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="1b919-166">См. также</span><span class="sxs-lookup"><span data-stu-id="1b919-166">See also</span></span>



- [<span data-ttu-id="1b919-167">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="1b919-167">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

