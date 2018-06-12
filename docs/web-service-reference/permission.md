---
title: Permission
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Permission
api_type:
- schema
ms.assetid: b8d0429a-0e58-4480-9847-4901970c7033
description: Элемент разрешений определяет доступ пользователя к папке.
ms.openlocfilehash: 600d60f481c4f1d407c3a39ab65d6ddcf46d04e7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19834735"
---
# <a name="permission"></a><span data-ttu-id="54d27-103">Разрешение</span><span class="sxs-lookup"><span data-stu-id="54d27-103">Permission</span></span>

<span data-ttu-id="54d27-104">Элемент **разрешений** определяет доступ пользователя к папке.</span><span class="sxs-lookup"><span data-stu-id="54d27-104">The **Permission** element defines the access that a user has to a folder.</span></span> 
  
```XML
<Permission>
   <CanCreateItems/>
   <CanCreateSubfolders/>
   <IsFolderOwner/>
   <IsFolderVisible/>
   <IsFolderContact/>
   <EditItems/>
   <DeleteItems/>
   <PermissionLevel/>
   <ReadItems/>
   <UserId/>
</Permission>
```

 <span data-ttu-id="54d27-105">**PermissionType**</span><span class="sxs-lookup"><span data-stu-id="54d27-105">**PermissionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="54d27-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="54d27-106">Attributes and elements</span></span>

<span data-ttu-id="54d27-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="54d27-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="54d27-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="54d27-108">Attributes</span></span>

<span data-ttu-id="54d27-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="54d27-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="54d27-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="54d27-110">Child elements</span></span>

|<span data-ttu-id="54d27-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="54d27-111">**Element**</span></span>|<span data-ttu-id="54d27-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="54d27-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="54d27-113">CanCreateItems</span><span class="sxs-lookup"><span data-stu-id="54d27-113">CanCreateItems</span></span>](cancreateitems.md) <br/> |<span data-ttu-id="54d27-114">Указывает, является ли пользователь имеет право на создание элементов в папке.</span><span class="sxs-lookup"><span data-stu-id="54d27-114">Indicates whether a user has permission to create items in a folder.</span></span> <span data-ttu-id="54d27-115">Этот элемент появился в Exchange 2007 с пакетом обновления 1.</span><span class="sxs-lookup"><span data-stu-id="54d27-115">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="54d27-116">CanCreateSubFolders</span><span class="sxs-lookup"><span data-stu-id="54d27-116">CanCreateSubFolders</span></span>](cancreatesubfolders.md) <br/> |<span data-ttu-id="54d27-117">Указывает, является ли пользователь имеет право на создание вложенных папок в папке.</span><span class="sxs-lookup"><span data-stu-id="54d27-117">Indicates whether a user has permission to create subfolders in a folder.</span></span> <span data-ttu-id="54d27-118">Этот элемент появился в Exchange 2007 с пакетом обновления 1.</span><span class="sxs-lookup"><span data-stu-id="54d27-118">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="54d27-119">DeleteItems</span><span class="sxs-lookup"><span data-stu-id="54d27-119">DeleteItems</span></span>](deleteitems.md) <br/> |<span data-ttu-id="54d27-120">Указывает, является ли пользователь имеет разрешения на удаление элементов в папке.</span><span class="sxs-lookup"><span data-stu-id="54d27-120">Indicates whether a user has permission to delete items in a folder.</span></span> <span data-ttu-id="54d27-121">Этот элемент появился в Exchange 2007 с пакетом обновления 1.</span><span class="sxs-lookup"><span data-stu-id="54d27-121">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="54d27-122">EditItems</span><span class="sxs-lookup"><span data-stu-id="54d27-122">EditItems</span></span>](edititems.md) <br/> |<span data-ttu-id="54d27-123">Указывает, является ли пользователь имеет разрешения на редактирование элементов в папке.</span><span class="sxs-lookup"><span data-stu-id="54d27-123">Indicates whether a user has permission to edit items in a folder.</span></span> <span data-ttu-id="54d27-124">Этот элемент появился в Exchange 2007 с пакетом обновления 1.</span><span class="sxs-lookup"><span data-stu-id="54d27-124">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="54d27-125">IsFolderContact</span><span class="sxs-lookup"><span data-stu-id="54d27-125">IsFolderContact</span></span>](isfoldercontact.md) <br/> |<span data-ttu-id="54d27-126">Указывает, является ли пользователь является контактом для папки.</span><span class="sxs-lookup"><span data-stu-id="54d27-126">Indicates whether a user is a contact for a folder.</span></span> <span data-ttu-id="54d27-127">Этот элемент появился в Exchange 2007 с пакетом обновления 1.</span><span class="sxs-lookup"><span data-stu-id="54d27-127">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="54d27-128">IsFolderOwner</span><span class="sxs-lookup"><span data-stu-id="54d27-128">IsFolderOwner</span></span>](isfolderowner.md) <br/> |<span data-ttu-id="54d27-129">Указывает, является ли пользователь является владельцем папки.</span><span class="sxs-lookup"><span data-stu-id="54d27-129">Indicates whether a user is the owner of a folder.</span></span> <span data-ttu-id="54d27-130">Этот элемент появился в Exchange 2007 с пакетом обновления 1.</span><span class="sxs-lookup"><span data-stu-id="54d27-130">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="54d27-131">IsFolderVisible</span><span class="sxs-lookup"><span data-stu-id="54d27-131">IsFolderVisible</span></span>](isfoldervisible.md) <br/> |<span data-ttu-id="54d27-132">Указывает, может ли пользователь просматривать папки.</span><span class="sxs-lookup"><span data-stu-id="54d27-132">Indicates whether a user can view a folder.</span></span> <span data-ttu-id="54d27-133">Этот элемент появился в Exchange 2007 с пакетом обновления 1.</span><span class="sxs-lookup"><span data-stu-id="54d27-133">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="54d27-134">PermissionLevel</span><span class="sxs-lookup"><span data-stu-id="54d27-134">PermissionLevel</span></span>](permissionlevel.md) <br/> |<span data-ttu-id="54d27-135">Представляет комбинации разрешений, которыми пользователь обладает на папку.</span><span class="sxs-lookup"><span data-stu-id="54d27-135">Represents the combination of permissions that a user has on a folder.</span></span> <span data-ttu-id="54d27-136">Этот элемент появился в Exchange 2007 с пакетом обновления 1.</span><span class="sxs-lookup"><span data-stu-id="54d27-136">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="54d27-137">ReadItems (PermissionType)</span><span class="sxs-lookup"><span data-stu-id="54d27-137">ReadItems (PermissionType)</span></span>](readitems-permissiontype.md) <br/> |<span data-ttu-id="54d27-138">Указывает, является ли пользователь имеет разрешение на чтение элементов в папке.</span><span class="sxs-lookup"><span data-stu-id="54d27-138">Indicates whether a user has permission to read items within a folder.</span></span> <span data-ttu-id="54d27-139">Этот элемент появился в Exchange 2007 с пакетом обновления 1.</span><span class="sxs-lookup"><span data-stu-id="54d27-139">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="54d27-140">Идентификатор пользователя</span><span class="sxs-lookup"><span data-stu-id="54d27-140">UserId</span></span>](userid.md) <br/> |<span data-ttu-id="54d27-141">Идентифицирует пользователя делегатом или пользователь, имеющий права доступа к папкам.</span><span class="sxs-lookup"><span data-stu-id="54d27-141">Identifies a delegate user or a user who has folder access permissions.</span></span> <span data-ttu-id="54d27-142">Этот элемент появился в Exchange 2007 с пакетом обновления 1.</span><span class="sxs-lookup"><span data-stu-id="54d27-142">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="54d27-143">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="54d27-143">Parent elements</span></span>

|<span data-ttu-id="54d27-144">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="54d27-144">**Element**</span></span>|<span data-ttu-id="54d27-145">**Описание**</span><span class="sxs-lookup"><span data-stu-id="54d27-145">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="54d27-146">Разрешения</span><span class="sxs-lookup"><span data-stu-id="54d27-146">Permissions</span></span>](permissions.md) <br/> |<span data-ttu-id="54d27-147">Содержит все настроенные разрешения для папки.</span><span class="sxs-lookup"><span data-stu-id="54d27-147">Contains all the configured permissions for a folder.</span></span> <span data-ttu-id="54d27-148">Этот элемент появился в Exchange 2007 с пакетом обновления 1.</span><span class="sxs-lookup"><span data-stu-id="54d27-148">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="54d27-149">Замечания</span><span class="sxs-lookup"><span data-stu-id="54d27-149">Remarks</span></span>

<span data-ttu-id="54d27-150">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="54d27-150">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
<span data-ttu-id="54d27-151">Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="54d27-151">This element was introduced in Exchange Server 2007 Service Pack 1 (SP1).</span></span>
  
### <a name="version-differences"></a><span data-ttu-id="54d27-152">Различия версий</span><span class="sxs-lookup"><span data-stu-id="54d27-152">Version differences</span></span>

<span data-ttu-id="54d27-153">Для приложений, предназначенных для Exchange Online, Exchange Online в составе Office 365 или более в локальной версии Exchange, начиная с Exchange 2013 разрешения папок не возвращаются при [BaseShape](baseshape.md) элемент имеет значение **AllProperties** в запросе [GetFolder](getfolder-operation.md) операции.</span><span class="sxs-lookup"><span data-stu-id="54d27-153">For applications that target Exchange Online, Exchange Online as part of Office 365, or an on-premises version of Exchange starting with Exchange 2013, folder permissions are not returned when the [BaseShape](baseshape.md) element has a value of **AllProperties** in the [GetFolder](getfolder-operation.md) operation request.</span></span> <span data-ttu-id="54d27-154">Для получения разрешений для папки, добавьте в элемент [AdditionalProperties](additionalproperties.md) в запросе **GetFolder** элемент [PermissionSet (PermissionSetType)](permissionset-permissionsettype.md) .</span><span class="sxs-lookup"><span data-stu-id="54d27-154">To retrieve folder permissions, add the [PermissionSet (PermissionSetType)](permissionset-permissionsettype.md) element to the [AdditionalProperties](additionalproperties.md) element in the **GetFolder** request.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="54d27-155">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="54d27-155">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="54d27-156">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="54d27-156">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="54d27-157">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="54d27-157">Schema Name</span></span>  <br/> |<span data-ttu-id="54d27-158">Схема Types</span><span class="sxs-lookup"><span data-stu-id="54d27-158">Types schema</span></span>  <br/> |
|<span data-ttu-id="54d27-159">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="54d27-159">Validation File</span></span>  <br/> |<span data-ttu-id="54d27-160">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="54d27-160">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="54d27-161">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="54d27-161">Can be Empty</span></span>  <br/> |<span data-ttu-id="54d27-162">False</span><span class="sxs-lookup"><span data-stu-id="54d27-162">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="54d27-163">См. также</span><span class="sxs-lookup"><span data-stu-id="54d27-163">See also</span></span>



- [<span data-ttu-id="54d27-164">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="54d27-164">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="54d27-165">Setting Folder-Level Permissions</span><span class="sxs-lookup"><span data-stu-id="54d27-165">Setting Folder-Level Permissions</span></span>](http://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

