---
title: DeleteItems
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DeleteItems
api_type:
- schema
ms.assetid: a5898bfc-f5ae-451d-9713-3e55864c690c
description: Элемент DeleteItems указывает, какие элементы в папке пользователь имеет разрешение на удаление. Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).
ms.openlocfilehash: 0be2154d1ceb6a995df8b27033fdc59bca81f9ef
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762052"
---
# <a name="deleteitems"></a><span data-ttu-id="a795a-104">DeleteItems</span><span class="sxs-lookup"><span data-stu-id="a795a-104">DeleteItems</span></span>

<span data-ttu-id="a795a-105">Элемент **DeleteItems** указывает, какие элементы в папке пользователь имеет разрешение на удаление.</span><span class="sxs-lookup"><span data-stu-id="a795a-105">The **DeleteItems** element indicates which items in a folder a user has permission to delete.</span></span> <span data-ttu-id="a795a-106">Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="a795a-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<DeleteItems>None or Owned or All</DeleteItems>
```

 <span data-ttu-id="a795a-107">**PermissionActionType**</span><span class="sxs-lookup"><span data-stu-id="a795a-107">**PermissionActionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a795a-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="a795a-108">Attributes and elements</span></span>

<span data-ttu-id="a795a-109">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="a795a-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a795a-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="a795a-110">Attributes</span></span>

<span data-ttu-id="a795a-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="a795a-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a795a-112">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="a795a-112">Child elements</span></span>

<span data-ttu-id="a795a-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="a795a-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="a795a-114">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="a795a-114">Parent elements</span></span>

|<span data-ttu-id="a795a-115">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="a795a-115">**Element**</span></span>|<span data-ttu-id="a795a-116">**Описание**</span><span class="sxs-lookup"><span data-stu-id="a795a-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a795a-117">Разрешение</span><span class="sxs-lookup"><span data-stu-id="a795a-117">Permission</span></span>](permission.md) <br/> |<span data-ttu-id="a795a-p103">Определяет доступ пользователя к папке. Этот элемент появился в Exchange 2007 с пакетом обновления 1.</span><span class="sxs-lookup"><span data-stu-id="a795a-p103">Defines the access that a user has to a folder. This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="a795a-120">CalendarPermission</span><span class="sxs-lookup"><span data-stu-id="a795a-120">CalendarPermission</span></span>](calendarpermission.md) <br/> |<span data-ttu-id="a795a-p104">Определяет доступ пользователя к папке календаря. Этот элемент появился в Exchange 2007 с пакетом обновления 1.</span><span class="sxs-lookup"><span data-stu-id="a795a-p104">Defines the access that a user has to a Calendar folder. This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="a795a-123">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="a795a-123">Text value</span></span>

<span data-ttu-id="a795a-124">В следующей таблице приведены возможные значения для элемента **DeleteItems** .</span><span class="sxs-lookup"><span data-stu-id="a795a-124">The following table lists the possible values for the **DeleteItems** element.</span></span> 
  
<span data-ttu-id="a795a-125">**DeleteItems элемент текстовые значения**</span><span class="sxs-lookup"><span data-stu-id="a795a-125">**DeleteItems element text values**</span></span>

|<span data-ttu-id="a795a-126">**Значение**</span><span class="sxs-lookup"><span data-stu-id="a795a-126">**Value**</span></span>|<span data-ttu-id="a795a-127">**Описание**</span><span class="sxs-lookup"><span data-stu-id="a795a-127">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="a795a-128">Нет</span><span class="sxs-lookup"><span data-stu-id="a795a-128">None</span></span>  <br/> |<span data-ttu-id="a795a-129">Указывает, что пользователь не имеет разрешения на удаление элементов в папке.</span><span class="sxs-lookup"><span data-stu-id="a795a-129">Indicates that the user does not have permission to delete items in the folder.</span></span>  <br/> |
|<span data-ttu-id="a795a-130">Владельцем</span><span class="sxs-lookup"><span data-stu-id="a795a-130">Owned</span></span>  <br/> |<span data-ttu-id="a795a-131">Указывает, что пользователь имеет разрешения на удаление элементов, которые принадлежат пользователю в папке.</span><span class="sxs-lookup"><span data-stu-id="a795a-131">Indicates that the user has permission to delete the items that the user owns in the folder.</span></span>  <br/> |
|<span data-ttu-id="a795a-132">Все</span><span class="sxs-lookup"><span data-stu-id="a795a-132">All</span></span>  <br/> |<span data-ttu-id="a795a-133">Указывает, что пользователь имеет разрешения на удаление всех элементов в папке.</span><span class="sxs-lookup"><span data-stu-id="a795a-133">Indicates that the user has permission to delete all items in the folder.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="a795a-134">Замечания</span><span class="sxs-lookup"><span data-stu-id="a795a-134">Remarks</span></span>

<span data-ttu-id="a795a-135">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="a795a-135">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a795a-136">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="a795a-136">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a795a-137">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="a795a-137">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="a795a-138">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="a795a-138">Schema Name</span></span>  <br/> |<span data-ttu-id="a795a-139">Схема Types</span><span class="sxs-lookup"><span data-stu-id="a795a-139">Types schema</span></span>  <br/> |
|<span data-ttu-id="a795a-140">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="a795a-140">Validation File</span></span>  <br/> |<span data-ttu-id="a795a-141">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="a795a-141">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="a795a-142">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="a795a-142">Can be Empty</span></span>  <br/> |<span data-ttu-id="a795a-143">False</span><span class="sxs-lookup"><span data-stu-id="a795a-143">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a795a-144">См. также</span><span class="sxs-lookup"><span data-stu-id="a795a-144">See also</span></span>

- [<span data-ttu-id="a795a-145">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="a795a-145">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="a795a-146">Setting Folder-Level Permissions</span><span class="sxs-lookup"><span data-stu-id="a795a-146">Setting Folder-Level Permissions</span></span>](http://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

