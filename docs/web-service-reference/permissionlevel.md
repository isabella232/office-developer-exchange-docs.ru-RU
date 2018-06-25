---
title: PermissionLevel
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- PermissionLevel
api_type:
- schema
ms.assetid: 87978600-3523-451e-a725-ef092c543e2a
description: Элемент PermissionLevel представляет уровень разрешений, который пользователь имеет на папку. Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).
ms.openlocfilehash: 7cc734f5807fe039467065315c220341f47d3fb4
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834730"
---
# <a name="permissionlevel"></a><span data-ttu-id="edd88-104">PermissionLevel</span><span class="sxs-lookup"><span data-stu-id="edd88-104">PermissionLevel</span></span>

<span data-ttu-id="edd88-105">Элемент **PermissionLevel** представляет уровень разрешений, который пользователь имеет на папку.</span><span class="sxs-lookup"><span data-stu-id="edd88-105">The **PermissionLevel** element represents the permission level that a user has on a folder.</span></span> <span data-ttu-id="edd88-106">Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="edd88-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<PermissionLevel>None or Owner or PublishingEditor or Editor or PublishingAuthor or Author or NoneditingAuthor or Reviewer or Contributor or Custom</PermissionLevel>
```

 <span data-ttu-id="edd88-107">**PermissionLevelType**</span><span class="sxs-lookup"><span data-stu-id="edd88-107">**PermissionLevelType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="edd88-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="edd88-108">Attributes and elements</span></span>

<span data-ttu-id="edd88-109">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="edd88-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="edd88-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="edd88-110">Attributes</span></span>

<span data-ttu-id="edd88-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="edd88-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="edd88-112">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="edd88-112">Child elements</span></span>

<span data-ttu-id="edd88-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="edd88-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="edd88-114">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="edd88-114">Parent elements</span></span>

|<span data-ttu-id="edd88-115">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="edd88-115">**Element**</span></span>|<span data-ttu-id="edd88-116">**Описание**</span><span class="sxs-lookup"><span data-stu-id="edd88-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="edd88-117">Разрешение</span><span class="sxs-lookup"><span data-stu-id="edd88-117">Permission</span></span>](permission.md) <br/> |<span data-ttu-id="edd88-p103">Определяет доступ пользователя к папке. Этот элемент появился в Exchange 2007 с пакетом обновления 1.</span><span class="sxs-lookup"><span data-stu-id="edd88-p103">Defines the access that a user has to a folder. This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="edd88-120">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="edd88-120">Text value</span></span>

<span data-ttu-id="edd88-121">В следующей таблице приведены возможные значения для элемента **PermissionLevel** .</span><span class="sxs-lookup"><span data-stu-id="edd88-121">The following table lists the possible values for the **PermissionLevel** element.</span></span> 
  
<span data-ttu-id="edd88-122">**PermissionLevel элемент текстовые значения**</span><span class="sxs-lookup"><span data-stu-id="edd88-122">**PermissionLevel element text values**</span></span>

|<span data-ttu-id="edd88-123">**Значение**</span><span class="sxs-lookup"><span data-stu-id="edd88-123">**Value**</span></span>|<span data-ttu-id="edd88-124">**Описание**</span><span class="sxs-lookup"><span data-stu-id="edd88-124">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="edd88-125">Нет</span><span class="sxs-lookup"><span data-stu-id="edd88-125">None</span></span>  <br/> |<span data-ttu-id="edd88-126">Указывает, что пользователь не имеет разрешений на папку.</span><span class="sxs-lookup"><span data-stu-id="edd88-126">Indicates that the user has no permissions on the folder.</span></span>  <br/> |
|<span data-ttu-id="edd88-127">Owner</span><span class="sxs-lookup"><span data-stu-id="edd88-127">Owner</span></span>  <br/> |<span data-ttu-id="edd88-128">Указывает, что пользователя можно создавать, читать, изменить и удаление всех элементов в папке и создавать вложенные папки.</span><span class="sxs-lookup"><span data-stu-id="edd88-128">Indicates that the user can create, read, edit, and delete all items in the folder, and create subfolders.</span></span> <span data-ttu-id="edd88-129">Пользователь является владельцем папки и папки контактов.</span><span class="sxs-lookup"><span data-stu-id="edd88-129">The user is both folder owner and folder contact.</span></span>  <br/> |
|<span data-ttu-id="edd88-130">PublishingEditor</span><span class="sxs-lookup"><span data-stu-id="edd88-130">PublishingEditor</span></span>  <br/> |<span data-ttu-id="edd88-131">Указывает, что пользователя можно создавать, читать, изменить и удаление всех элементов в папке и создавать вложенные папки.</span><span class="sxs-lookup"><span data-stu-id="edd88-131">Indicates that the user can create, read, edit, and delete all items in the folder, and create subfolders.</span></span>  <br/> |
|<span data-ttu-id="edd88-132">Редактор</span><span class="sxs-lookup"><span data-stu-id="edd88-132">Editor</span></span>  <br/> |<span data-ttu-id="edd88-133">Указывает, что пользователь создание, чтение, изменение и удаление всех элементов в папке.</span><span class="sxs-lookup"><span data-stu-id="edd88-133">Indicates that the user can create, read, edit, and delete all items in the folder.</span></span>  <br/> |
|<span data-ttu-id="edd88-134">PublishingAuthor</span><span class="sxs-lookup"><span data-stu-id="edd88-134">PublishingAuthor</span></span>  <br/> |<span data-ttu-id="edd88-135">Указывает, что пользователя можно создавать и читать все элементы в папке, изменять и удалять только элементы, которые пользователь создает и создавать вложенные папки.</span><span class="sxs-lookup"><span data-stu-id="edd88-135">Indicates that the user can create and read all items in the folder, edit and delete only items that the user creates, and create subfolders.</span></span>  <br/> |
|<span data-ttu-id="edd88-136">Author</span><span class="sxs-lookup"><span data-stu-id="edd88-136">Author</span></span>  <br/> |<span data-ttu-id="edd88-137">Указывает, что пользователь создавать и читать все элементы в папке и редактировать и удалять только элементы, которые пользователь создает.</span><span class="sxs-lookup"><span data-stu-id="edd88-137">Indicates that the user can create and read all items in the folder, and edit and delete only items that the user creates.</span></span>  <br/> |
|<span data-ttu-id="edd88-138">NoneditingAuthor</span><span class="sxs-lookup"><span data-stu-id="edd88-138">NoneditingAuthor</span></span>  <br/> |<span data-ttu-id="edd88-139">Указывает, что пользователь создавать и читать все элементы в папке и удалить только элементы, которые пользователь создает.</span><span class="sxs-lookup"><span data-stu-id="edd88-139">Indicates that the user can create and read all items in the folder, and delete only items that the user creates.</span></span>  <br/> |
|<span data-ttu-id="edd88-140">Редактор</span><span class="sxs-lookup"><span data-stu-id="edd88-140">Reviewer</span></span>  <br/> |<span data-ttu-id="edd88-141">Указывает, что пользователи могут читать все элементы в папке.</span><span class="sxs-lookup"><span data-stu-id="edd88-141">Indicates that the user can read all items in the folder.</span></span>  <br/> |
|<span data-ttu-id="edd88-142">Участник</span><span class="sxs-lookup"><span data-stu-id="edd88-142">Contributor</span></span>  <br/> |<span data-ttu-id="edd88-143">Указывает, что пользователь может создавать элементы в папке.</span><span class="sxs-lookup"><span data-stu-id="edd88-143">Indicates that the user can create items in the folder.</span></span> <span data-ttu-id="edd88-144">Содержимое папки не отображаются.</span><span class="sxs-lookup"><span data-stu-id="edd88-144">The contents of the folder do not appear.</span></span>  <br/> |
|<span data-ttu-id="edd88-145">Пользовательский сервер</span><span class="sxs-lookup"><span data-stu-id="edd88-145">Custom</span></span>  <br/> |<span data-ttu-id="edd88-146">Указывает, что пользователь имеет пользовательские разрешения доступа в общей папке.</span><span class="sxs-lookup"><span data-stu-id="edd88-146">Indicates that the user has custom access permissions on the folder.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="edd88-147">Замечания</span><span class="sxs-lookup"><span data-stu-id="edd88-147">Remarks</span></span>

<span data-ttu-id="edd88-148">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="edd88-148">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="edd88-149">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="edd88-149">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="edd88-150">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="edd88-150">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="edd88-151">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="edd88-151">Schema Name</span></span>  <br/> |<span data-ttu-id="edd88-152">Схема Types</span><span class="sxs-lookup"><span data-stu-id="edd88-152">Types schema</span></span>  <br/> |
|<span data-ttu-id="edd88-153">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="edd88-153">Validation File</span></span>  <br/> |<span data-ttu-id="edd88-154">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="edd88-154">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="edd88-155">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="edd88-155">Can be Empty</span></span>  <br/> |<span data-ttu-id="edd88-156">False</span><span class="sxs-lookup"><span data-stu-id="edd88-156">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="edd88-157">См. также</span><span class="sxs-lookup"><span data-stu-id="edd88-157">See also</span></span>



- [<span data-ttu-id="edd88-158">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="edd88-158">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="edd88-159">Setting Folder-Level Permissions</span><span class="sxs-lookup"><span data-stu-id="edd88-159">Setting Folder-Level Permissions</span></span>](http://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

