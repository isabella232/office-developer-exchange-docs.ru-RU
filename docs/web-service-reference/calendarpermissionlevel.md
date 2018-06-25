---
title: CalendarPermissionLevel
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CalendarPermissionLevel
api_type:
- schema
ms.assetid: 6ac2b792-4326-4a3f-b6cb-977bf523b5b2
description: Элемент CalendarPermissionLevel представляет уровень разрешений, который пользователь имеет папки календаря. Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).
ms.openlocfilehash: 646e4df3b70350a16cdd1f3e134260c2984a5161
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761654"
---
# <a name="calendarpermissionlevel"></a><span data-ttu-id="7ff07-104">CalendarPermissionLevel</span><span class="sxs-lookup"><span data-stu-id="7ff07-104">CalendarPermissionLevel</span></span>

<span data-ttu-id="7ff07-105">Элемент **CalendarPermissionLevel** представляет уровень разрешений, который пользователь имеет папки календаря.</span><span class="sxs-lookup"><span data-stu-id="7ff07-105">The **CalendarPermissionLevel** element represents the permission level that a user has on a Calendar folder.</span></span> <span data-ttu-id="7ff07-106">Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="7ff07-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<CalendarPermissionLevel>None or Owner or PublishingEditor or Editor or PublishingAuthor or Author or NoneditingAuthor or Reviewer or Contributor or FreeBusyTimeOnly or FreeBusyTimeAndSubjectAndLocation or Custom</CalendarPermissionLevel>
```

 <span data-ttu-id="7ff07-107">**CalendarPermissionLevelType**</span><span class="sxs-lookup"><span data-stu-id="7ff07-107">**CalendarPermissionLevelType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7ff07-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="7ff07-108">Attributes and elements</span></span>

<span data-ttu-id="7ff07-109">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="7ff07-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7ff07-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="7ff07-110">Attributes</span></span>

<span data-ttu-id="7ff07-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="7ff07-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7ff07-112">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="7ff07-112">Child elements</span></span>

<span data-ttu-id="7ff07-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="7ff07-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="7ff07-114">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="7ff07-114">Parent elements</span></span>

|<span data-ttu-id="7ff07-115">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="7ff07-115">**Element**</span></span>|<span data-ttu-id="7ff07-116">**Описание**</span><span class="sxs-lookup"><span data-stu-id="7ff07-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7ff07-117">CalendarPermission</span><span class="sxs-lookup"><span data-stu-id="7ff07-117">CalendarPermission</span></span>](calendarpermission.md) <br/> |<span data-ttu-id="7ff07-p103">Определяет доступ пользователя к папке календаря. Этот элемент появился в Exchange 2007 с пакетом обновления 1.</span><span class="sxs-lookup"><span data-stu-id="7ff07-p103">Defines the access that a user has to a Calendar folder. This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="7ff07-120">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="7ff07-120">Text value</span></span>

<span data-ttu-id="7ff07-121">В следующей таблице приведены возможные значения для элемента **CalendarPermissionLevel** .</span><span class="sxs-lookup"><span data-stu-id="7ff07-121">The following table lists the possible values for the **CalendarPermissionLevel** element.</span></span> 
  
<span data-ttu-id="7ff07-122">**CalendarPermissionLevel элемент текстовые значения**</span><span class="sxs-lookup"><span data-stu-id="7ff07-122">**CalendarPermissionLevel element text values**</span></span>

|<span data-ttu-id="7ff07-123">**Значение**</span><span class="sxs-lookup"><span data-stu-id="7ff07-123">**Value**</span></span>|<span data-ttu-id="7ff07-124">**Описание**</span><span class="sxs-lookup"><span data-stu-id="7ff07-124">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="7ff07-125">Нет</span><span class="sxs-lookup"><span data-stu-id="7ff07-125">None</span></span>  <br/> |<span data-ttu-id="7ff07-126">Указывает, что пользователь не имеет разрешений на папку.</span><span class="sxs-lookup"><span data-stu-id="7ff07-126">Indicates that the user has no permissions on the folder.</span></span>  <br/> |
|<span data-ttu-id="7ff07-127">Owner</span><span class="sxs-lookup"><span data-stu-id="7ff07-127">Owner</span></span>  <br/> |<span data-ttu-id="7ff07-128">Указывает, что пользователя можно создавать, читать, изменить и удаление всех элементов в папке и создавать вложенные папки.</span><span class="sxs-lookup"><span data-stu-id="7ff07-128">Indicates that the user can create, read, edit, and delete all items in the folder, and create subfolders.</span></span> <span data-ttu-id="7ff07-129">Пользователь является владельцем папки и папки контактов.</span><span class="sxs-lookup"><span data-stu-id="7ff07-129">The user is both folder owner and folder contact.</span></span>  <br/> |
|<span data-ttu-id="7ff07-130">PublishingEditor</span><span class="sxs-lookup"><span data-stu-id="7ff07-130">PublishingEditor</span></span>  <br/> |<span data-ttu-id="7ff07-131">Указывает, что пользователя можно создавать, читать, изменить и удаление всех элементов в папке и создавать вложенные папки.</span><span class="sxs-lookup"><span data-stu-id="7ff07-131">Indicates that the user can create, read, edit, and delete all items in the folder, and create subfolders.</span></span>  <br/> |
|<span data-ttu-id="7ff07-132">Редактор</span><span class="sxs-lookup"><span data-stu-id="7ff07-132">Editor</span></span>  <br/> |<span data-ttu-id="7ff07-133">Указывает, можно, что пользователь создание, чтение, изменение и удаление всех элементов в папке.</span><span class="sxs-lookup"><span data-stu-id="7ff07-133">Indicates that the user can create, read, edit and delete all items in the folder.</span></span>  <br/> |
|<span data-ttu-id="7ff07-134">PublishingAuthor</span><span class="sxs-lookup"><span data-stu-id="7ff07-134">PublishingAuthor</span></span>  <br/> |<span data-ttu-id="7ff07-135">Указывает, что пользователя можно создавать и читать все элементы в папке, изменять и удалять только элементы, которые пользователь создает и создавать вложенные папки.</span><span class="sxs-lookup"><span data-stu-id="7ff07-135">Indicates that the user can create and read all items in the folder, edit and delete only items that the user creates, and create subfolders.</span></span>  <br/> |
|<span data-ttu-id="7ff07-136">Author</span><span class="sxs-lookup"><span data-stu-id="7ff07-136">Author</span></span>  <br/> |<span data-ttu-id="7ff07-137">Указывает, что пользователь создавать и читать все элементы в папке и редактировать и удалять только элементы, которые пользователь создает.</span><span class="sxs-lookup"><span data-stu-id="7ff07-137">Indicates that the user can create and read all items in the folder, and edit and delete only items that the user creates.</span></span>  <br/> |
|<span data-ttu-id="7ff07-138">NoneditingAuthor</span><span class="sxs-lookup"><span data-stu-id="7ff07-138">NoneditingAuthor</span></span>  <br/> |<span data-ttu-id="7ff07-139">Указывает, что пользователь создавать и читать все элементы в папке и удалить только элементы, которые пользователь создает.</span><span class="sxs-lookup"><span data-stu-id="7ff07-139">Indicates that the user can create and read all items in the folder, and delete only items that the user creates.</span></span>  <br/> |
|<span data-ttu-id="7ff07-140">Редактор</span><span class="sxs-lookup"><span data-stu-id="7ff07-140">Reviewer</span></span>  <br/> |<span data-ttu-id="7ff07-141">Указывает, что пользователи могут читать все элементы в папке.</span><span class="sxs-lookup"><span data-stu-id="7ff07-141">Indicates that the user can read all items in the folder.</span></span>  <br/> |
|<span data-ttu-id="7ff07-142">Участник</span><span class="sxs-lookup"><span data-stu-id="7ff07-142">Contributor</span></span>  <br/> |<span data-ttu-id="7ff07-143">Указывает, что пользователь может создавать элементы в папке.</span><span class="sxs-lookup"><span data-stu-id="7ff07-143">Indicates that the user can create items in the folder.</span></span> <span data-ttu-id="7ff07-144">Содержимое папки не отображаются.</span><span class="sxs-lookup"><span data-stu-id="7ff07-144">The contents of the folder do not appear.</span></span>  <br/> |
|<span data-ttu-id="7ff07-145">FreeBusyTimeOnly</span><span class="sxs-lookup"><span data-stu-id="7ff07-145">FreeBusyTimeOnly</span></span>  <br/> |<span data-ttu-id="7ff07-146">Указывает, что пользователь может просматривать только занятости в календаре.</span><span class="sxs-lookup"><span data-stu-id="7ff07-146">Indicates that the user can view only free/busy time within the calendar.</span></span>  <br/> |
|<span data-ttu-id="7ff07-147">FreeBusyTimeAndSubjectAndLocation</span><span class="sxs-lookup"><span data-stu-id="7ff07-147">FreeBusyTimeAndSubjectAndLocation</span></span>  <br/> |<span data-ttu-id="7ff07-148">Указывает, что пользователь может просматривать занятости в календаре и тему и место встречи.</span><span class="sxs-lookup"><span data-stu-id="7ff07-148">Indicates that the user can view free/busy time within the calendar and the subject and location of appointments.</span></span>  <br/> |
|<span data-ttu-id="7ff07-149">Пользовательский сервер</span><span class="sxs-lookup"><span data-stu-id="7ff07-149">Custom</span></span>  <br/> |<span data-ttu-id="7ff07-150">Указывает, что пользователь имеет пользовательские разрешения доступа в общей папке.</span><span class="sxs-lookup"><span data-stu-id="7ff07-150">Indicates that the user has custom access permissions on the folder.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="7ff07-151">Замечания</span><span class="sxs-lookup"><span data-stu-id="7ff07-151">Remarks</span></span>

<span data-ttu-id="7ff07-152">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="7ff07-152">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7ff07-153">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="7ff07-153">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7ff07-154">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="7ff07-154">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="7ff07-155">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="7ff07-155">Schema Name</span></span>  <br/> |<span data-ttu-id="7ff07-156">Схема Types</span><span class="sxs-lookup"><span data-stu-id="7ff07-156">Types schema</span></span>  <br/> |
|<span data-ttu-id="7ff07-157">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="7ff07-157">Validation File</span></span>  <br/> |<span data-ttu-id="7ff07-158">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="7ff07-158">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="7ff07-159">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="7ff07-159">Can be Empty</span></span>  <br/> |<span data-ttu-id="7ff07-160">False</span><span class="sxs-lookup"><span data-stu-id="7ff07-160">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7ff07-161">См. также</span><span class="sxs-lookup"><span data-stu-id="7ff07-161">See also</span></span>



- [<span data-ttu-id="7ff07-162">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="7ff07-162">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="7ff07-163">Setting Folder-Level Permissions</span><span class="sxs-lookup"><span data-stu-id="7ff07-163">Setting Folder-Level Permissions</span></span>](http://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

