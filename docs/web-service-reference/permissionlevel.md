---
title: пермиссионлевел
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
description: Элемент Пермиссионлевел представляет уровень разрешений, который пользователь имеет в папке. Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).
ms.openlocfilehash: e1e441c53b5c40c16051eb852a6b35a8af7476e2
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458042"
---
# <a name="permissionlevel"></a><span data-ttu-id="0170f-104">пермиссионлевел</span><span class="sxs-lookup"><span data-stu-id="0170f-104">PermissionLevel</span></span>

<span data-ttu-id="0170f-105">Элемент **пермиссионлевел** представляет уровень разрешений, который пользователь имеет в папке.</span><span class="sxs-lookup"><span data-stu-id="0170f-105">The **PermissionLevel** element represents the permission level that a user has on a folder.</span></span> <span data-ttu-id="0170f-106">Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="0170f-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<PermissionLevel>None or Owner or PublishingEditor or Editor or PublishingAuthor or Author or NoneditingAuthor or Reviewer or Contributor or Custom</PermissionLevel>
```

 <span data-ttu-id="0170f-107">**пермиссионлевелтипе**</span><span class="sxs-lookup"><span data-stu-id="0170f-107">**PermissionLevelType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0170f-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="0170f-108">Attributes and elements</span></span>

<span data-ttu-id="0170f-109">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="0170f-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0170f-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="0170f-110">Attributes</span></span>

<span data-ttu-id="0170f-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="0170f-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0170f-112">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="0170f-112">Child elements</span></span>

<span data-ttu-id="0170f-113">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="0170f-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="0170f-114">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="0170f-114">Parent elements</span></span>

|<span data-ttu-id="0170f-115">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="0170f-115">**Element**</span></span>|<span data-ttu-id="0170f-116">**Описание**</span><span class="sxs-lookup"><span data-stu-id="0170f-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0170f-117">Разрешение</span><span class="sxs-lookup"><span data-stu-id="0170f-117">Permission</span></span>](permission.md) <br/> |<span data-ttu-id="0170f-p103">Определяет доступ пользователя к папке. Этот элемент появился в Exchange 2007 с пакетом обновления 1.</span><span class="sxs-lookup"><span data-stu-id="0170f-p103">Defines the access that a user has to a folder. This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="0170f-120">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="0170f-120">Text value</span></span>

<span data-ttu-id="0170f-121">В следующей таблице приведены возможные значения для элемента **пермиссионлевел** .</span><span class="sxs-lookup"><span data-stu-id="0170f-121">The following table lists the possible values for the **PermissionLevel** element.</span></span> 
  
<span data-ttu-id="0170f-122">**Текстовые значения элементов Пермиссионлевел**</span><span class="sxs-lookup"><span data-stu-id="0170f-122">**PermissionLevel element text values**</span></span>

|<span data-ttu-id="0170f-123">**Значение**</span><span class="sxs-lookup"><span data-stu-id="0170f-123">**Value**</span></span>|<span data-ttu-id="0170f-124">**Описание**</span><span class="sxs-lookup"><span data-stu-id="0170f-124">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="0170f-125">Нет</span><span class="sxs-lookup"><span data-stu-id="0170f-125">None</span></span>  <br/> |<span data-ttu-id="0170f-126">Указывает, что у пользователя нет разрешений на доступ к папке.</span><span class="sxs-lookup"><span data-stu-id="0170f-126">Indicates that the user has no permissions on the folder.</span></span>  <br/> |
|<span data-ttu-id="0170f-127">Владелец</span><span class="sxs-lookup"><span data-stu-id="0170f-127">Owner</span></span>  <br/> |<span data-ttu-id="0170f-128">Указывает, что пользователь может создавать, читать, редактировать и удалять все элементы в папке, а также создавать вложенные папки.</span><span class="sxs-lookup"><span data-stu-id="0170f-128">Indicates that the user can create, read, edit, and delete all items in the folder, and create subfolders.</span></span> <span data-ttu-id="0170f-129">Пользователь является владельцем папки и ее контактом.</span><span class="sxs-lookup"><span data-stu-id="0170f-129">The user is both folder owner and folder contact.</span></span>  <br/> |
|<span data-ttu-id="0170f-130">PublishingEditor</span><span class="sxs-lookup"><span data-stu-id="0170f-130">PublishingEditor</span></span>  <br/> |<span data-ttu-id="0170f-131">Указывает, что пользователь может создавать, читать, редактировать и удалять все элементы в папке, а также создавать вложенные папки.</span><span class="sxs-lookup"><span data-stu-id="0170f-131">Indicates that the user can create, read, edit, and delete all items in the folder, and create subfolders.</span></span>  <br/> |
|<span data-ttu-id="0170f-132">Корректор</span><span class="sxs-lookup"><span data-stu-id="0170f-132">Editor</span></span>  <br/> |<span data-ttu-id="0170f-133">Указывает, что пользователь может создавать, читать, редактировать и удалять все элементы в папке.</span><span class="sxs-lookup"><span data-stu-id="0170f-133">Indicates that the user can create, read, edit, and delete all items in the folder.</span></span>  <br/> |
|<span data-ttu-id="0170f-134">PublishingAuthor</span><span class="sxs-lookup"><span data-stu-id="0170f-134">PublishingAuthor</span></span>  <br/> |<span data-ttu-id="0170f-135">Указывает, что пользователь может создавать и читать все элементы в папке, изменять и удалять только те элементы, которые создает пользователь, и создавать вложенные папки.</span><span class="sxs-lookup"><span data-stu-id="0170f-135">Indicates that the user can create and read all items in the folder, edit and delete only items that the user creates, and create subfolders.</span></span>  <br/> |
|<span data-ttu-id="0170f-136">Автор</span><span class="sxs-lookup"><span data-stu-id="0170f-136">Author</span></span>  <br/> |<span data-ttu-id="0170f-137">Указывает, что пользователь может создавать и читать все элементы в папке, а также изменять и удалять только те элементы, которые создает пользователь.</span><span class="sxs-lookup"><span data-stu-id="0170f-137">Indicates that the user can create and read all items in the folder, and edit and delete only items that the user creates.</span></span>  <br/> |
|<span data-ttu-id="0170f-138">Noneditingauthorcreateitems</span><span class="sxs-lookup"><span data-stu-id="0170f-138">NoneditingAuthor</span></span>  <br/> |<span data-ttu-id="0170f-139">Указывает, что пользователь может создавать и читать все элементы в папке, а также удалять только те элементы, которые создает пользователь.</span><span class="sxs-lookup"><span data-stu-id="0170f-139">Indicates that the user can create and read all items in the folder, and delete only items that the user creates.</span></span>  <br/> |
|<span data-ttu-id="0170f-140">Reviewer</span><span class="sxs-lookup"><span data-stu-id="0170f-140">Reviewer</span></span>  <br/> |<span data-ttu-id="0170f-141">Указывает, что пользователь может читать все элементы в папке.</span><span class="sxs-lookup"><span data-stu-id="0170f-141">Indicates that the user can read all items in the folder.</span></span>  <br/> |
|<span data-ttu-id="0170f-142">Участник</span><span class="sxs-lookup"><span data-stu-id="0170f-142">Contributor</span></span>  <br/> |<span data-ttu-id="0170f-143">Указывает, что пользователь может создавать элементы в папке.</span><span class="sxs-lookup"><span data-stu-id="0170f-143">Indicates that the user can create items in the folder.</span></span> <span data-ttu-id="0170f-144">Содержимое папки не отображается.</span><span class="sxs-lookup"><span data-stu-id="0170f-144">The contents of the folder do not appear.</span></span>  <br/> |
|<span data-ttu-id="0170f-145">Пользовательские</span><span class="sxs-lookup"><span data-stu-id="0170f-145">Custom</span></span>  <br/> |<span data-ttu-id="0170f-146">Указывает, что пользователь имеет пользовательские разрешения на доступ к папке.</span><span class="sxs-lookup"><span data-stu-id="0170f-146">Indicates that the user has custom access permissions on the folder.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="0170f-147">Примечания</span><span class="sxs-lookup"><span data-stu-id="0170f-147">Remarks</span></span>

<span data-ttu-id="0170f-148">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="0170f-148">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0170f-149">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="0170f-149">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0170f-150">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="0170f-150">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="0170f-151">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="0170f-151">Schema Name</span></span>  <br/> |<span data-ttu-id="0170f-152">Схема Types</span><span class="sxs-lookup"><span data-stu-id="0170f-152">Types schema</span></span>  <br/> |
|<span data-ttu-id="0170f-153">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="0170f-153">Validation File</span></span>  <br/> |<span data-ttu-id="0170f-154">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="0170f-154">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="0170f-155">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="0170f-155">Can be Empty</span></span>  <br/> |<span data-ttu-id="0170f-156">False</span><span class="sxs-lookup"><span data-stu-id="0170f-156">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0170f-157">См. также</span><span class="sxs-lookup"><span data-stu-id="0170f-157">See also</span></span>



- [<span data-ttu-id="0170f-158">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="0170f-158">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="0170f-159">Setting Folder-Level Permissions</span><span class="sxs-lookup"><span data-stu-id="0170f-159">Setting Folder-Level Permissions</span></span>](https://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

