---
title: контактсфолдер
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ContactsFolder
api_type:
- schema
ms.assetid: 6c299de8-2087-4aeb-8e66-2bc7586509a6
description: Элемент Контактсфолдер представляет папку Contacts, содержащуюся в почтовом ящике.
ms.openlocfilehash: 01302f00d84cfff9713e3b188b7799c537fc0629
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761739"
---
# <a name="contactsfolder"></a><span data-ttu-id="eb65c-103">контактсфолдер</span><span class="sxs-lookup"><span data-stu-id="eb65c-103">ContactsFolder</span></span>

<span data-ttu-id="eb65c-104">Элемент **контактсфолдер** представляет папку Contacts, содержащуюся в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="eb65c-104">The **ContactsFolder** element represents a contacts folder that is contained in a mailbox.</span></span> 
  
```xml
<ContactsFolder>
   <FolderId/>
   <ParentFolderId/>
   <FolderClass/>
   <DisplayName/>
   <TotalCount/>
   <ChildFolderCount/>
   <ExtendedProperty/>
   <ManagedFolderInformation/>
   <EffectiveRights/>
   <SharingEffectiveRights/>
   <PermissionSet/>
</ContactsFolder>
```

 <span data-ttu-id="eb65c-105">**контактсфолдертипе**</span><span class="sxs-lookup"><span data-stu-id="eb65c-105">**ContactsFolderType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="eb65c-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="eb65c-106">Attributes and elements</span></span>

<span data-ttu-id="eb65c-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="eb65c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="eb65c-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="eb65c-108">Attributes</span></span>

<span data-ttu-id="eb65c-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="eb65c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="eb65c-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="eb65c-110">Child elements</span></span>

|<span data-ttu-id="eb65c-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="eb65c-111">**Element**</span></span>|<span data-ttu-id="eb65c-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="eb65c-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="eb65c-113">FolderId</span><span class="sxs-lookup"><span data-stu-id="eb65c-113">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="eb65c-114">Содержит идентификатор и ключ изменения папки "Контакты".</span><span class="sxs-lookup"><span data-stu-id="eb65c-114">Contains the identifier and change key of a contacts folder.</span></span>  <br/> |
|[<span data-ttu-id="eb65c-115">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="eb65c-115">ParentFolderId</span></span>](parentfolderid.md) <br/> |<span data-ttu-id="eb65c-116">Представляет идентификатор родительской папки, содержащей папку "Контакты".</span><span class="sxs-lookup"><span data-stu-id="eb65c-116">Represents the identifier of the parent folder that contains the contacts folder.</span></span>  <br/> |
|[<span data-ttu-id="eb65c-117">фолдеркласс</span><span class="sxs-lookup"><span data-stu-id="eb65c-117">FolderClass</span></span>](folderclass.md) <br/> |<span data-ttu-id="eb65c-118">Представляет класс папки для папки "Контакты".</span><span class="sxs-lookup"><span data-stu-id="eb65c-118">Represents the folder class for a contacts folder.</span></span>  <br/> |
|[<span data-ttu-id="eb65c-119">DisplayName (строка)</span><span class="sxs-lookup"><span data-stu-id="eb65c-119">DisplayName (string)</span></span>](displayname-string.md) <br/> |<span data-ttu-id="eb65c-120">Содержит отображаемое имя папки контактов.</span><span class="sxs-lookup"><span data-stu-id="eb65c-120">Contains the display name of a contacts folder.</span></span>  <br/> |
|[<span data-ttu-id="eb65c-121">тоталкаунт</span><span class="sxs-lookup"><span data-stu-id="eb65c-121">TotalCount</span></span>](totalcount.md) <br/> |<span data-ttu-id="eb65c-122">Представляет общее количество элементов в папке "Контакты".</span><span class="sxs-lookup"><span data-stu-id="eb65c-122">Represents the total count of items within a contacts folder.</span></span>  <br/> |
|[<span data-ttu-id="eb65c-123">чилдфолдеркаунт</span><span class="sxs-lookup"><span data-stu-id="eb65c-123">ChildFolderCount</span></span>](childfoldercount.md) <br/> |<span data-ttu-id="eb65c-124">Представляет количество дочерних папок, содержащихся в папке "Контакты".</span><span class="sxs-lookup"><span data-stu-id="eb65c-124">Represents the number of child folders that are contained within a contacts folder.</span></span> <span data-ttu-id="eb65c-125">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="eb65c-125">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="eb65c-126">ExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="eb65c-126">ExtendedProperty</span></span>](extendedproperty.md) <br/> |<span data-ttu-id="eb65c-127">Определяет расширенные свойства для папок контактов.</span><span class="sxs-lookup"><span data-stu-id="eb65c-127">Identifies extended properties on contacts folders.</span></span>  <br/> |
|[<span data-ttu-id="eb65c-128">манажедфолдеринформатион</span><span class="sxs-lookup"><span data-stu-id="eb65c-128">ManagedFolderInformation</span></span>](managedfolderinformation.md) <br/> |<span data-ttu-id="eb65c-129">Содержит сведения об управляемой папке.</span><span class="sxs-lookup"><span data-stu-id="eb65c-129">Contains information about a managed folder.</span></span>  <br/> |
|[<span data-ttu-id="eb65c-130">еффективеригхтс</span><span class="sxs-lookup"><span data-stu-id="eb65c-130">EffectiveRights</span></span>](effectiverights.md) <br/> |<span data-ttu-id="eb65c-131">Содержит права клиента на основе параметров разрешений для элемента или папки.</span><span class="sxs-lookup"><span data-stu-id="eb65c-131">Contains the client's rights based on the permission settings for the item or folder.</span></span>  <br/> |
|[<span data-ttu-id="eb65c-132">Шаринжеффективеригхтс (Пермиссионреадакцесстипе)</span><span class="sxs-lookup"><span data-stu-id="eb65c-132">SharingEffectiveRights (PermissionReadAccessType)</span></span>](sharingeffectiverights-permissionreadaccesstype.md) <br/> |<span data-ttu-id="eb65c-133">Указывает разрешения, назначенные пользователю для данных контакта, к которым предоставлен общий доступ.</span><span class="sxs-lookup"><span data-stu-id="eb65c-133">Indicates the permissions that the user has for the contact data that is being shared.</span></span>  <br/> |
|[<span data-ttu-id="eb65c-134">PermissionSet (Пермиссионсеттипе)</span><span class="sxs-lookup"><span data-stu-id="eb65c-134">PermissionSet (PermissionSetType)</span></span>](permissionset-permissionsettype.md) <br/> |<span data-ttu-id="eb65c-135">Содержит все настроенные разрешения для папки.</span><span class="sxs-lookup"><span data-stu-id="eb65c-135">Contains all the configured permissions for a folder.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="eb65c-136">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="eb65c-136">Parent elements</span></span>

|<span data-ttu-id="eb65c-137">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="eb65c-137">**Element**</span></span>|<span data-ttu-id="eb65c-138">**Описание**</span><span class="sxs-lookup"><span data-stu-id="eb65c-138">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="eb65c-139">аппендтофолдерфиелд</span><span class="sxs-lookup"><span data-stu-id="eb65c-139">AppendToFolderField</span></span>](appendtofolderfield.md) <br/> |<span data-ttu-id="eb65c-140">Задает данные, добавляемые к свойству folder во время [операции операцию UpdateFolder](updatefolder-operation.md).</span><span class="sxs-lookup"><span data-stu-id="eb65c-140">Specifies data to append to a folder property during an [UpdateFolder operation](updatefolder-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="eb65c-141">Create (Фолдерсинк)</span><span class="sxs-lookup"><span data-stu-id="eb65c-141">Create (FolderSync)</span></span>](create-foldersync.md) <br/> |<span data-ttu-id="eb65c-142">Определяет одну папку для создания в локальном хранилище клиента.</span><span class="sxs-lookup"><span data-stu-id="eb65c-142">Identifies a single folder to create in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="eb65c-143">сетфолдерфиелд</span><span class="sxs-lookup"><span data-stu-id="eb65c-143">SetFolderField</span></span>](setfolderfield.md) <br/> |<span data-ttu-id="eb65c-144">Представляет обновление одного свойства папки в [операции операцию UpdateFolder](updatefolder-operation.md).</span><span class="sxs-lookup"><span data-stu-id="eb65c-144">Represents an update to a single property on a folder in an [UpdateFolder operation](updatefolder-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="eb65c-145">Обновление (Фолдерсинк)</span><span class="sxs-lookup"><span data-stu-id="eb65c-145">Update (FolderSync)</span></span>](update-foldersync.md) <br/> |<span data-ttu-id="eb65c-146">Определяет одну папку для обновления в локальном хранилище клиента.</span><span class="sxs-lookup"><span data-stu-id="eb65c-146">Identifies a single folder to update in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="eb65c-147">Folders</span><span class="sxs-lookup"><span data-stu-id="eb65c-147">Folders</span></span>](folders-ex15websvcsotherref.md) <br/> |<span data-ttu-id="eb65c-148">Содержит массив папок, используемых в операциях с папками.</span><span class="sxs-lookup"><span data-stu-id="eb65c-148">Contains an array of folders that are used in folder operations.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="eb65c-149">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="eb65c-149">Text value</span></span>

<span data-ttu-id="eb65c-150">Нет.</span><span class="sxs-lookup"><span data-stu-id="eb65c-150">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="eb65c-151">Примечания</span><span class="sxs-lookup"><span data-stu-id="eb65c-151">Remarks</span></span>

<span data-ttu-id="eb65c-152">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="eb65c-152">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="eb65c-153">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="eb65c-153">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="eb65c-154">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="eb65c-154">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="eb65c-155">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="eb65c-155">Schema Name</span></span>  <br/> |<span data-ttu-id="eb65c-156">Схема Types</span><span class="sxs-lookup"><span data-stu-id="eb65c-156">Types schema</span></span>  <br/> |
|<span data-ttu-id="eb65c-157">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="eb65c-157">Validation File</span></span>  <br/> |<span data-ttu-id="eb65c-158">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="eb65c-158">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="eb65c-159">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="eb65c-159">Can be Empty</span></span>  <br/> |<span data-ttu-id="eb65c-160">False</span><span class="sxs-lookup"><span data-stu-id="eb65c-160">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="eb65c-161">См. также</span><span class="sxs-lookup"><span data-stu-id="eb65c-161">See also</span></span>



- [<span data-ttu-id="eb65c-162">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="eb65c-162">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

