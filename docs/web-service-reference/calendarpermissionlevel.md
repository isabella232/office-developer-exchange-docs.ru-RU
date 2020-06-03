---
title: календарпермиссионлевел
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
description: Элемент Календарпермиссионлевел представляет уровень разрешений, который пользователь имеет в папке календаря. Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).
ms.openlocfilehash: 670f78e0b3cef7a40339c83d84916871f8969536
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44527182"
---
# <a name="calendarpermissionlevel"></a><span data-ttu-id="2cfc5-104">календарпермиссионлевел</span><span class="sxs-lookup"><span data-stu-id="2cfc5-104">CalendarPermissionLevel</span></span>

<span data-ttu-id="2cfc5-105">Элемент **календарпермиссионлевел** представляет уровень разрешений, который пользователь имеет в папке календаря.</span><span class="sxs-lookup"><span data-stu-id="2cfc5-105">The **CalendarPermissionLevel** element represents the permission level that a user has on a Calendar folder.</span></span> <span data-ttu-id="2cfc5-106">Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="2cfc5-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<CalendarPermissionLevel>None or Owner or PublishingEditor or Editor or PublishingAuthor or Author or NoneditingAuthor or Reviewer or Contributor or FreeBusyTimeOnly or FreeBusyTimeAndSubjectAndLocation or Custom</CalendarPermissionLevel>
```

 <span data-ttu-id="2cfc5-107">**календарпермиссионлевелтипе**</span><span class="sxs-lookup"><span data-stu-id="2cfc5-107">**CalendarPermissionLevelType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2cfc5-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="2cfc5-108">Attributes and elements</span></span>

<span data-ttu-id="2cfc5-109">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="2cfc5-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2cfc5-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="2cfc5-110">Attributes</span></span>

<span data-ttu-id="2cfc5-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="2cfc5-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2cfc5-112">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="2cfc5-112">Child elements</span></span>

<span data-ttu-id="2cfc5-113">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="2cfc5-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="2cfc5-114">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="2cfc5-114">Parent elements</span></span>

|<span data-ttu-id="2cfc5-115">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="2cfc5-115">**Element**</span></span>|<span data-ttu-id="2cfc5-116">**Описание**</span><span class="sxs-lookup"><span data-stu-id="2cfc5-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2cfc5-117">календарпермиссион</span><span class="sxs-lookup"><span data-stu-id="2cfc5-117">CalendarPermission</span></span>](calendarpermission.md) <br/> |<span data-ttu-id="2cfc5-p103">Определяет доступ пользователя к папке календаря. Этот элемент появился в Exchange 2007 с пакетом обновления 1.</span><span class="sxs-lookup"><span data-stu-id="2cfc5-p103">Defines the access that a user has to a Calendar folder. This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="2cfc5-120">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="2cfc5-120">Text value</span></span>

<span data-ttu-id="2cfc5-121">В следующей таблице приведены возможные значения для элемента **календарпермиссионлевел** .</span><span class="sxs-lookup"><span data-stu-id="2cfc5-121">The following table lists the possible values for the **CalendarPermissionLevel** element.</span></span> 
  
<span data-ttu-id="2cfc5-122">**Текстовые значения элементов Календарпермиссионлевел**</span><span class="sxs-lookup"><span data-stu-id="2cfc5-122">**CalendarPermissionLevel element text values**</span></span>

|<span data-ttu-id="2cfc5-123">**Значение**</span><span class="sxs-lookup"><span data-stu-id="2cfc5-123">**Value**</span></span>|<span data-ttu-id="2cfc5-124">**Описание**</span><span class="sxs-lookup"><span data-stu-id="2cfc5-124">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="2cfc5-125">Нет</span><span class="sxs-lookup"><span data-stu-id="2cfc5-125">None</span></span>  <br/> |<span data-ttu-id="2cfc5-126">Указывает, что у пользователя нет разрешений на доступ к папке.</span><span class="sxs-lookup"><span data-stu-id="2cfc5-126">Indicates that the user has no permissions on the folder.</span></span>  <br/> |
|<span data-ttu-id="2cfc5-127">Владелец</span><span class="sxs-lookup"><span data-stu-id="2cfc5-127">Owner</span></span>  <br/> |<span data-ttu-id="2cfc5-128">Указывает, что пользователь может создавать, читать, редактировать и удалять все элементы в папке, а также создавать вложенные папки.</span><span class="sxs-lookup"><span data-stu-id="2cfc5-128">Indicates that the user can create, read, edit, and delete all items in the folder, and create subfolders.</span></span> <span data-ttu-id="2cfc5-129">Пользователь является владельцем папки и ее контактом.</span><span class="sxs-lookup"><span data-stu-id="2cfc5-129">The user is both folder owner and folder contact.</span></span>  <br/> |
|<span data-ttu-id="2cfc5-130">PublishingEditor</span><span class="sxs-lookup"><span data-stu-id="2cfc5-130">PublishingEditor</span></span>  <br/> |<span data-ttu-id="2cfc5-131">Указывает, что пользователь может создавать, читать, редактировать и удалять все элементы в папке, а также создавать вложенные папки.</span><span class="sxs-lookup"><span data-stu-id="2cfc5-131">Indicates that the user can create, read, edit, and delete all items in the folder, and create subfolders.</span></span>  <br/> |
|<span data-ttu-id="2cfc5-132">Корректор</span><span class="sxs-lookup"><span data-stu-id="2cfc5-132">Editor</span></span>  <br/> |<span data-ttu-id="2cfc5-133">Указывает, что пользователь может создавать, читать, редактировать и удалять все элементы в папке.</span><span class="sxs-lookup"><span data-stu-id="2cfc5-133">Indicates that the user can create, read, edit and delete all items in the folder.</span></span>  <br/> |
|<span data-ttu-id="2cfc5-134">PublishingAuthor</span><span class="sxs-lookup"><span data-stu-id="2cfc5-134">PublishingAuthor</span></span>  <br/> |<span data-ttu-id="2cfc5-135">Указывает, что пользователь может создавать и читать все элементы в папке, изменять и удалять только те элементы, которые создает пользователь, и создавать вложенные папки.</span><span class="sxs-lookup"><span data-stu-id="2cfc5-135">Indicates that the user can create and read all items in the folder, edit and delete only items that the user creates, and create subfolders.</span></span>  <br/> |
|<span data-ttu-id="2cfc5-136">Автор</span><span class="sxs-lookup"><span data-stu-id="2cfc5-136">Author</span></span>  <br/> |<span data-ttu-id="2cfc5-137">Указывает, что пользователь может создавать и читать все элементы в папке, а также изменять и удалять только те элементы, которые создает пользователь.</span><span class="sxs-lookup"><span data-stu-id="2cfc5-137">Indicates that the user can create and read all items in the folder, and edit and delete only items that the user creates.</span></span>  <br/> |
|<span data-ttu-id="2cfc5-138">Noneditingauthorcreateitems</span><span class="sxs-lookup"><span data-stu-id="2cfc5-138">NoneditingAuthor</span></span>  <br/> |<span data-ttu-id="2cfc5-139">Указывает, что пользователь может создавать и читать все элементы в папке, а также удалять только те элементы, которые создает пользователь.</span><span class="sxs-lookup"><span data-stu-id="2cfc5-139">Indicates that the user can create and read all items in the folder, and delete only items that the user creates.</span></span>  <br/> |
|<span data-ttu-id="2cfc5-140">Reviewer</span><span class="sxs-lookup"><span data-stu-id="2cfc5-140">Reviewer</span></span>  <br/> |<span data-ttu-id="2cfc5-141">Указывает, что пользователь может читать все элементы в папке.</span><span class="sxs-lookup"><span data-stu-id="2cfc5-141">Indicates that the user can read all items in the folder.</span></span>  <br/> |
|<span data-ttu-id="2cfc5-142">Участник</span><span class="sxs-lookup"><span data-stu-id="2cfc5-142">Contributor</span></span>  <br/> |<span data-ttu-id="2cfc5-143">Указывает, что пользователь может создавать элементы в папке.</span><span class="sxs-lookup"><span data-stu-id="2cfc5-143">Indicates that the user can create items in the folder.</span></span> <span data-ttu-id="2cfc5-144">Содержимое папки не отображается.</span><span class="sxs-lookup"><span data-stu-id="2cfc5-144">The contents of the folder do not appear.</span></span>  <br/> |
|<span data-ttu-id="2cfc5-145">фрибуситимеонли</span><span class="sxs-lookup"><span data-stu-id="2cfc5-145">FreeBusyTimeOnly</span></span>  <br/> |<span data-ttu-id="2cfc5-146">Указывает, что пользователь может просматривать только время занятости в календаре.</span><span class="sxs-lookup"><span data-stu-id="2cfc5-146">Indicates that the user can view only free/busy time within the calendar.</span></span>  <br/> |
|<span data-ttu-id="2cfc5-147">фрибуситимеандсубжектандлокатион</span><span class="sxs-lookup"><span data-stu-id="2cfc5-147">FreeBusyTimeAndSubjectAndLocation</span></span>  <br/> |<span data-ttu-id="2cfc5-148">Указывает, что пользователь может просматривать сведения о занятости в календаре и теме и местоположении встреч.</span><span class="sxs-lookup"><span data-stu-id="2cfc5-148">Indicates that the user can view free/busy time within the calendar and the subject and location of appointments.</span></span>  <br/> |
|<span data-ttu-id="2cfc5-149">Пользовательские</span><span class="sxs-lookup"><span data-stu-id="2cfc5-149">Custom</span></span>  <br/> |<span data-ttu-id="2cfc5-150">Указывает, что пользователь имеет пользовательские разрешения на доступ к папке.</span><span class="sxs-lookup"><span data-stu-id="2cfc5-150">Indicates that the user has custom access permissions on the folder.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="2cfc5-151">Примечания</span><span class="sxs-lookup"><span data-stu-id="2cfc5-151">Remarks</span></span>

<span data-ttu-id="2cfc5-152">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="2cfc5-152">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2cfc5-153">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="2cfc5-153">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2cfc5-154">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="2cfc5-154">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="2cfc5-155">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="2cfc5-155">Schema Name</span></span>  <br/> |<span data-ttu-id="2cfc5-156">Схема Types</span><span class="sxs-lookup"><span data-stu-id="2cfc5-156">Types schema</span></span>  <br/> |
|<span data-ttu-id="2cfc5-157">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="2cfc5-157">Validation File</span></span>  <br/> |<span data-ttu-id="2cfc5-158">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="2cfc5-158">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="2cfc5-159">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="2cfc5-159">Can be Empty</span></span>  <br/> |<span data-ttu-id="2cfc5-160">False</span><span class="sxs-lookup"><span data-stu-id="2cfc5-160">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="2cfc5-161">См. также</span><span class="sxs-lookup"><span data-stu-id="2cfc5-161">See also</span></span>



- [<span data-ttu-id="2cfc5-162">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="2cfc5-162">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="2cfc5-163">Setting Folder-Level Permissions</span><span class="sxs-lookup"><span data-stu-id="2cfc5-163">Setting Folder-Level Permissions</span></span>](https://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

