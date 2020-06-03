---
title: Разрешение
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
description: Элемент permission определяет доступ пользователя к папке.
ms.openlocfilehash: 0f7515dbb06f8423f8d4d95e1391496e8ac73653
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459260"
---
# <a name="permission"></a><span data-ttu-id="f1cd0-103">Разрешение</span><span class="sxs-lookup"><span data-stu-id="f1cd0-103">Permission</span></span>

<span data-ttu-id="f1cd0-104">Элемент **Permission** определяет доступ пользователя к папке.</span><span class="sxs-lookup"><span data-stu-id="f1cd0-104">The **Permission** element defines the access that a user has to a folder.</span></span> 
  
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

 <span data-ttu-id="f1cd0-105">**пермиссионтипе**</span><span class="sxs-lookup"><span data-stu-id="f1cd0-105">**PermissionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f1cd0-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="f1cd0-106">Attributes and elements</span></span>

<span data-ttu-id="f1cd0-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="f1cd0-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f1cd0-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="f1cd0-108">Attributes</span></span>

<span data-ttu-id="f1cd0-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="f1cd0-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f1cd0-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="f1cd0-110">Child elements</span></span>

|<span data-ttu-id="f1cd0-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="f1cd0-111">**Element**</span></span>|<span data-ttu-id="f1cd0-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="f1cd0-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f1cd0-113">канкреатеитемс</span><span class="sxs-lookup"><span data-stu-id="f1cd0-113">CanCreateItems</span></span>](cancreateitems.md) <br/> |<span data-ttu-id="f1cd0-114">Указывает, имеет ли пользователь разрешение на создание элементов в папке.</span><span class="sxs-lookup"><span data-stu-id="f1cd0-114">Indicates whether a user has permission to create items in a folder.</span></span> <span data-ttu-id="f1cd0-115">Этот элемент появился в Exchange 2007 с пакетом обновления 1.</span><span class="sxs-lookup"><span data-stu-id="f1cd0-115">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="f1cd0-116">канкреатесубфолдерс</span><span class="sxs-lookup"><span data-stu-id="f1cd0-116">CanCreateSubFolders</span></span>](cancreatesubfolders.md) <br/> |<span data-ttu-id="f1cd0-117">Указывает, имеет ли пользователь разрешение на создание вложенных папок в папке.</span><span class="sxs-lookup"><span data-stu-id="f1cd0-117">Indicates whether a user has permission to create subfolders in a folder.</span></span> <span data-ttu-id="f1cd0-118">Этот элемент появился в Exchange 2007 с пакетом обновления 1.</span><span class="sxs-lookup"><span data-stu-id="f1cd0-118">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="f1cd0-119">делетеитемс</span><span class="sxs-lookup"><span data-stu-id="f1cd0-119">DeleteItems</span></span>](deleteitems.md) <br/> |<span data-ttu-id="f1cd0-120">Указывает, имеет ли пользователь разрешение на удаление элементов в папке.</span><span class="sxs-lookup"><span data-stu-id="f1cd0-120">Indicates whether a user has permission to delete items in a folder.</span></span> <span data-ttu-id="f1cd0-121">Этот элемент появился в Exchange 2007 с пакетом обновления 1.</span><span class="sxs-lookup"><span data-stu-id="f1cd0-121">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="f1cd0-122">едититемс</span><span class="sxs-lookup"><span data-stu-id="f1cd0-122">EditItems</span></span>](edititems.md) <br/> |<span data-ttu-id="f1cd0-123">Указывает, имеет ли пользователь разрешение на изменение элементов в папке.</span><span class="sxs-lookup"><span data-stu-id="f1cd0-123">Indicates whether a user has permission to edit items in a folder.</span></span> <span data-ttu-id="f1cd0-124">Этот элемент появился в Exchange 2007 с пакетом обновления 1.</span><span class="sxs-lookup"><span data-stu-id="f1cd0-124">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="f1cd0-125">исфолдерконтакт</span><span class="sxs-lookup"><span data-stu-id="f1cd0-125">IsFolderContact</span></span>](isfoldercontact.md) <br/> |<span data-ttu-id="f1cd0-126">Указывает, является ли пользователь контактом для папки.</span><span class="sxs-lookup"><span data-stu-id="f1cd0-126">Indicates whether a user is a contact for a folder.</span></span> <span data-ttu-id="f1cd0-127">Этот элемент появился в Exchange 2007 с пакетом обновления 1.</span><span class="sxs-lookup"><span data-stu-id="f1cd0-127">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="f1cd0-128">исфолдеровнер</span><span class="sxs-lookup"><span data-stu-id="f1cd0-128">IsFolderOwner</span></span>](isfolderowner.md) <br/> |<span data-ttu-id="f1cd0-129">Указывает, является ли пользователь владельцем папки.</span><span class="sxs-lookup"><span data-stu-id="f1cd0-129">Indicates whether a user is the owner of a folder.</span></span> <span data-ttu-id="f1cd0-130">Этот элемент появился в Exchange 2007 с пакетом обновления 1.</span><span class="sxs-lookup"><span data-stu-id="f1cd0-130">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="f1cd0-131">исфолдервисибле</span><span class="sxs-lookup"><span data-stu-id="f1cd0-131">IsFolderVisible</span></span>](isfoldervisible.md) <br/> |<span data-ttu-id="f1cd0-132">Указывает, может ли пользователь просматривать папку.</span><span class="sxs-lookup"><span data-stu-id="f1cd0-132">Indicates whether a user can view a folder.</span></span> <span data-ttu-id="f1cd0-133">Этот элемент появился в Exchange 2007 с пакетом обновления 1.</span><span class="sxs-lookup"><span data-stu-id="f1cd0-133">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="f1cd0-134">пермиссионлевел</span><span class="sxs-lookup"><span data-stu-id="f1cd0-134">PermissionLevel</span></span>](permissionlevel.md) <br/> |<span data-ttu-id="f1cd0-135">Представляет сочетание разрешений, которые пользователь имеет в папке.</span><span class="sxs-lookup"><span data-stu-id="f1cd0-135">Represents the combination of permissions that a user has on a folder.</span></span> <span data-ttu-id="f1cd0-136">Этот элемент появился в Exchange 2007 с пакетом обновления 1.</span><span class="sxs-lookup"><span data-stu-id="f1cd0-136">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="f1cd0-137">ReadItems (Пермиссионтипе)</span><span class="sxs-lookup"><span data-stu-id="f1cd0-137">ReadItems (PermissionType)</span></span>](readitems-permissiontype.md) <br/> |<span data-ttu-id="f1cd0-138">Указывает, имеет ли пользователь разрешение на чтение элементов в папке.</span><span class="sxs-lookup"><span data-stu-id="f1cd0-138">Indicates whether a user has permission to read items within a folder.</span></span> <span data-ttu-id="f1cd0-139">Этот элемент появился в Exchange 2007 с пакетом обновления 1.</span><span class="sxs-lookup"><span data-stu-id="f1cd0-139">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="f1cd0-140">UserId</span><span class="sxs-lookup"><span data-stu-id="f1cd0-140">UserId</span></span>](userid.md) <br/> |<span data-ttu-id="f1cd0-141">Определяет делегата или пользователя с разрешениями на доступ к папке.</span><span class="sxs-lookup"><span data-stu-id="f1cd0-141">Identifies a delegate user or a user who has folder access permissions.</span></span> <span data-ttu-id="f1cd0-142">Этот элемент появился в Exchange 2007 с пакетом обновления 1.</span><span class="sxs-lookup"><span data-stu-id="f1cd0-142">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f1cd0-143">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="f1cd0-143">Parent elements</span></span>

|<span data-ttu-id="f1cd0-144">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="f1cd0-144">**Element**</span></span>|<span data-ttu-id="f1cd0-145">**Описание**</span><span class="sxs-lookup"><span data-stu-id="f1cd0-145">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f1cd0-146">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f1cd0-146">Permissions</span></span>](permissions.md) <br/> |<span data-ttu-id="f1cd0-147">Содержит все настроенные разрешения для папки.</span><span class="sxs-lookup"><span data-stu-id="f1cd0-147">Contains all the configured permissions for a folder.</span></span> <span data-ttu-id="f1cd0-148">Этот элемент появился в Exchange 2007 с пакетом обновления 1.</span><span class="sxs-lookup"><span data-stu-id="f1cd0-148">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="f1cd0-149">Примечания</span><span class="sxs-lookup"><span data-stu-id="f1cd0-149">Remarks</span></span>

<span data-ttu-id="f1cd0-150">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="f1cd0-150">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
<span data-ttu-id="f1cd0-151">Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="f1cd0-151">This element was introduced in Exchange Server 2007 Service Pack 1 (SP1).</span></span>
  
### <a name="version-differences"></a><span data-ttu-id="f1cd0-152">Различия версий</span><span class="sxs-lookup"><span data-stu-id="f1cd0-152">Version differences</span></span>

<span data-ttu-id="f1cd0-153">Для приложений, предназначенных для Exchange Online, Exchange Online в составе Office 365, или локальной версии Exchange, начиная с Exchange 2013, разрешения для папки не возвращаются, если элемент [басешапе](baseshape.md) имеет значение **аллпропертиес** в запросе операции- [папки](getfolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="f1cd0-153">For applications that target Exchange Online, Exchange Online as part of Office 365, or an on-premises version of Exchange starting with Exchange 2013, folder permissions are not returned when the [BaseShape](baseshape.md) element has a value of **AllProperties** in the [GetFolder](getfolder-operation.md) operation request.</span></span> <span data-ttu-id="f1cd0-154">Чтобы получить разрешения для папки, добавьте элемент [PermissionSet (пермиссионсеттипе)](permissionset-permissionsettype.md) в элемент [аддитионалпропертиес](additionalproperties.md) в запросе на получение **папки** .</span><span class="sxs-lookup"><span data-stu-id="f1cd0-154">To retrieve folder permissions, add the [PermissionSet (PermissionSetType)](permissionset-permissionsettype.md) element to the [AdditionalProperties](additionalproperties.md) element in the **GetFolder** request.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="f1cd0-155">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="f1cd0-155">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f1cd0-156">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="f1cd0-156">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="f1cd0-157">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="f1cd0-157">Schema Name</span></span>  <br/> |<span data-ttu-id="f1cd0-158">Схема Types</span><span class="sxs-lookup"><span data-stu-id="f1cd0-158">Types schema</span></span>  <br/> |
|<span data-ttu-id="f1cd0-159">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="f1cd0-159">Validation File</span></span>  <br/> |<span data-ttu-id="f1cd0-160">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="f1cd0-160">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="f1cd0-161">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="f1cd0-161">Can be Empty</span></span>  <br/> |<span data-ttu-id="f1cd0-162">False</span><span class="sxs-lookup"><span data-stu-id="f1cd0-162">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f1cd0-163">См. также</span><span class="sxs-lookup"><span data-stu-id="f1cd0-163">See also</span></span>



- [<span data-ttu-id="f1cd0-164">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="f1cd0-164">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="f1cd0-165">Setting Folder-Level Permissions</span><span class="sxs-lookup"><span data-stu-id="f1cd0-165">Setting Folder-Level Permissions</span></span>](https://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

