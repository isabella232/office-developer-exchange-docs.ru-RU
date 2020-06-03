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
ms.openlocfilehash: 997b4f603198e6d05a011c4ef6bac7fe4dfbfe52
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529436"
---
# <a name="contactsfolder"></a><span data-ttu-id="a6c5b-103">контактсфолдер</span><span class="sxs-lookup"><span data-stu-id="a6c5b-103">ContactsFolder</span></span>

<span data-ttu-id="a6c5b-104">Элемент **контактсфолдер** представляет папку Contacts, содержащуюся в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="a6c5b-104">The **ContactsFolder** element represents a contacts folder that is contained in a mailbox.</span></span> 
  
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

 <span data-ttu-id="a6c5b-105">**контактсфолдертипе**</span><span class="sxs-lookup"><span data-stu-id="a6c5b-105">**ContactsFolderType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a6c5b-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="a6c5b-106">Attributes and elements</span></span>

<span data-ttu-id="a6c5b-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="a6c5b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a6c5b-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="a6c5b-108">Attributes</span></span>

<span data-ttu-id="a6c5b-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="a6c5b-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a6c5b-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="a6c5b-110">Child elements</span></span>

|<span data-ttu-id="a6c5b-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="a6c5b-111">**Element**</span></span>|<span data-ttu-id="a6c5b-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="a6c5b-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a6c5b-113">FolderId</span><span class="sxs-lookup"><span data-stu-id="a6c5b-113">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="a6c5b-114">Содержит идентификатор и ключ изменения папки "Контакты".</span><span class="sxs-lookup"><span data-stu-id="a6c5b-114">Contains the identifier and change key of a contacts folder.</span></span>  <br/> |
|[<span data-ttu-id="a6c5b-115">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="a6c5b-115">ParentFolderId</span></span>](parentfolderid.md) <br/> |<span data-ttu-id="a6c5b-116">Представляет идентификатор родительской папки, содержащей папку "Контакты".</span><span class="sxs-lookup"><span data-stu-id="a6c5b-116">Represents the identifier of the parent folder that contains the contacts folder.</span></span>  <br/> |
|[<span data-ttu-id="a6c5b-117">фолдеркласс</span><span class="sxs-lookup"><span data-stu-id="a6c5b-117">FolderClass</span></span>](folderclass.md) <br/> |<span data-ttu-id="a6c5b-118">Представляет класс папки для папки "Контакты".</span><span class="sxs-lookup"><span data-stu-id="a6c5b-118">Represents the folder class for a contacts folder.</span></span>  <br/> |
|[<span data-ttu-id="a6c5b-119">DisplayName (строка)</span><span class="sxs-lookup"><span data-stu-id="a6c5b-119">DisplayName (string)</span></span>](displayname-string.md) <br/> |<span data-ttu-id="a6c5b-120">Содержит отображаемое имя папки контактов.</span><span class="sxs-lookup"><span data-stu-id="a6c5b-120">Contains the display name of a contacts folder.</span></span>  <br/> |
|[<span data-ttu-id="a6c5b-121">тоталкаунт</span><span class="sxs-lookup"><span data-stu-id="a6c5b-121">TotalCount</span></span>](totalcount.md) <br/> |<span data-ttu-id="a6c5b-122">Представляет общее количество элементов в папке "Контакты".</span><span class="sxs-lookup"><span data-stu-id="a6c5b-122">Represents the total count of items within a contacts folder.</span></span>  <br/> |
|[<span data-ttu-id="a6c5b-123">чилдфолдеркаунт</span><span class="sxs-lookup"><span data-stu-id="a6c5b-123">ChildFolderCount</span></span>](childfoldercount.md) <br/> |<span data-ttu-id="a6c5b-124">Представляет количество дочерних папок, содержащихся в папке "Контакты".</span><span class="sxs-lookup"><span data-stu-id="a6c5b-124">Represents the number of child folders that are contained within a contacts folder.</span></span> <span data-ttu-id="a6c5b-125">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a6c5b-125">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="a6c5b-126">ExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="a6c5b-126">ExtendedProperty</span></span>](extendedproperty.md) <br/> |<span data-ttu-id="a6c5b-127">Определяет расширенные свойства для папок контактов.</span><span class="sxs-lookup"><span data-stu-id="a6c5b-127">Identifies extended properties on contacts folders.</span></span>  <br/> |
|[<span data-ttu-id="a6c5b-128">манажедфолдеринформатион</span><span class="sxs-lookup"><span data-stu-id="a6c5b-128">ManagedFolderInformation</span></span>](managedfolderinformation.md) <br/> |<span data-ttu-id="a6c5b-129">Содержит сведения об управляемой папке.</span><span class="sxs-lookup"><span data-stu-id="a6c5b-129">Contains information about a managed folder.</span></span>  <br/> |
|[<span data-ttu-id="a6c5b-130">еффективеригхтс</span><span class="sxs-lookup"><span data-stu-id="a6c5b-130">EffectiveRights</span></span>](effectiverights.md) <br/> |<span data-ttu-id="a6c5b-131">Содержит права клиента на основе параметров разрешений для элемента или папки.</span><span class="sxs-lookup"><span data-stu-id="a6c5b-131">Contains the client's rights based on the permission settings for the item or folder.</span></span>  <br/> |
|[<span data-ttu-id="a6c5b-132">Шаринжеффективеригхтс (Пермиссионреадакцесстипе)</span><span class="sxs-lookup"><span data-stu-id="a6c5b-132">SharingEffectiveRights (PermissionReadAccessType)</span></span>](sharingeffectiverights-permissionreadaccesstype.md) <br/> |<span data-ttu-id="a6c5b-133">Указывает разрешения, назначенные пользователю для данных контакта, к которым предоставлен общий доступ.</span><span class="sxs-lookup"><span data-stu-id="a6c5b-133">Indicates the permissions that the user has for the contact data that is being shared.</span></span>  <br/> |
|[<span data-ttu-id="a6c5b-134">PermissionSet (Пермиссионсеттипе)</span><span class="sxs-lookup"><span data-stu-id="a6c5b-134">PermissionSet (PermissionSetType)</span></span>](permissionset-permissionsettype.md) <br/> |<span data-ttu-id="a6c5b-135">Содержит все настроенные разрешения для папки.</span><span class="sxs-lookup"><span data-stu-id="a6c5b-135">Contains all the configured permissions for a folder.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="a6c5b-136">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="a6c5b-136">Parent elements</span></span>

|<span data-ttu-id="a6c5b-137">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="a6c5b-137">**Element**</span></span>|<span data-ttu-id="a6c5b-138">**Описание**</span><span class="sxs-lookup"><span data-stu-id="a6c5b-138">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a6c5b-139">аппендтофолдерфиелд</span><span class="sxs-lookup"><span data-stu-id="a6c5b-139">AppendToFolderField</span></span>](appendtofolderfield.md) <br/> |<span data-ttu-id="a6c5b-140">Задает данные, добавляемые к свойству folder во время [операции операцию UpdateFolder](updatefolder-operation.md).</span><span class="sxs-lookup"><span data-stu-id="a6c5b-140">Specifies data to append to a folder property during an [UpdateFolder operation](updatefolder-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="a6c5b-141">Create (Фолдерсинк)</span><span class="sxs-lookup"><span data-stu-id="a6c5b-141">Create (FolderSync)</span></span>](create-foldersync.md) <br/> |<span data-ttu-id="a6c5b-142">Определяет одну папку для создания в локальном хранилище клиента.</span><span class="sxs-lookup"><span data-stu-id="a6c5b-142">Identifies a single folder to create in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="a6c5b-143">сетфолдерфиелд</span><span class="sxs-lookup"><span data-stu-id="a6c5b-143">SetFolderField</span></span>](setfolderfield.md) <br/> |<span data-ttu-id="a6c5b-144">Представляет обновление одного свойства папки в [операции операцию UpdateFolder](updatefolder-operation.md).</span><span class="sxs-lookup"><span data-stu-id="a6c5b-144">Represents an update to a single property on a folder in an [UpdateFolder operation](updatefolder-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="a6c5b-145">Обновление (Фолдерсинк)</span><span class="sxs-lookup"><span data-stu-id="a6c5b-145">Update (FolderSync)</span></span>](update-foldersync.md) <br/> |<span data-ttu-id="a6c5b-146">Определяет одну папку для обновления в локальном хранилище клиента.</span><span class="sxs-lookup"><span data-stu-id="a6c5b-146">Identifies a single folder to update in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="a6c5b-147">Folders</span><span class="sxs-lookup"><span data-stu-id="a6c5b-147">Folders</span></span>](folders-ex15websvcsotherref.md) <br/> |<span data-ttu-id="a6c5b-148">Содержит массив папок, используемых в операциях с папками.</span><span class="sxs-lookup"><span data-stu-id="a6c5b-148">Contains an array of folders that are used in folder operations.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="a6c5b-149">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="a6c5b-149">Text value</span></span>

<span data-ttu-id="a6c5b-150">Нет.</span><span class="sxs-lookup"><span data-stu-id="a6c5b-150">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="a6c5b-151">Примечания</span><span class="sxs-lookup"><span data-stu-id="a6c5b-151">Remarks</span></span>

<span data-ttu-id="a6c5b-152">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="a6c5b-152">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a6c5b-153">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="a6c5b-153">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a6c5b-154">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="a6c5b-154">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="a6c5b-155">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="a6c5b-155">Schema Name</span></span>  <br/> |<span data-ttu-id="a6c5b-156">Схема Types</span><span class="sxs-lookup"><span data-stu-id="a6c5b-156">Types schema</span></span>  <br/> |
|<span data-ttu-id="a6c5b-157">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="a6c5b-157">Validation File</span></span>  <br/> |<span data-ttu-id="a6c5b-158">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="a6c5b-158">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="a6c5b-159">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="a6c5b-159">Can be Empty</span></span>  <br/> |<span data-ttu-id="a6c5b-160">False</span><span class="sxs-lookup"><span data-stu-id="a6c5b-160">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a6c5b-161">См. также</span><span class="sxs-lookup"><span data-stu-id="a6c5b-161">See also</span></span>



- [<span data-ttu-id="a6c5b-162">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="a6c5b-162">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

