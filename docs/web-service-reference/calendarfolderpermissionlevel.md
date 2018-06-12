---
title: CalendarFolderPermissionLevel
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CalendarFolderPermissionLevel
api_type:
- schema
ms.assetid: 2a5c9381-dc2c-4fc6-b9b5-893477d0970e
description: Элемент CalendarFolderPermissionLevel содержит разрешения для папки календаря по умолчанию. Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).
ms.openlocfilehash: 5d51fea522656910d8417e7f75214214e2c162c6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761644"
---
# <a name="calendarfolderpermissionlevel"></a><span data-ttu-id="fd178-104">CalendarFolderPermissionLevel</span><span class="sxs-lookup"><span data-stu-id="fd178-104">CalendarFolderPermissionLevel</span></span>

<span data-ttu-id="fd178-105">Элемент **CalendarFolderPermissionLevel** содержит разрешения для папки календаря по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="fd178-105">The **CalendarFolderPermissionLevel** element contains the permissions for the default Calendar folder.</span></span> <span data-ttu-id="fd178-106">Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="fd178-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<CalendarFolderPermissionLevel>
   None or Editor or Reviewer or Author or Custom
</CalendarFolderPermissionLevel>
```

 <span data-ttu-id="fd178-107">**DelegateFolderPermissionLevelType**</span><span class="sxs-lookup"><span data-stu-id="fd178-107">**DelegateFolderPermissionLevelType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="fd178-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="fd178-108">Attributes and elements</span></span>

<span data-ttu-id="fd178-109">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="fd178-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="fd178-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="fd178-110">Attributes</span></span>

<span data-ttu-id="fd178-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="fd178-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="fd178-112">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="fd178-112">Child elements</span></span>

<span data-ttu-id="fd178-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="fd178-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="fd178-114">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="fd178-114">Parent elements</span></span>

|<span data-ttu-id="fd178-115">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="fd178-115">**Element**</span></span>|<span data-ttu-id="fd178-116">**Описание**</span><span class="sxs-lookup"><span data-stu-id="fd178-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fd178-117">DelegatePermissions</span><span class="sxs-lookup"><span data-stu-id="fd178-117">DelegatePermissions</span></span>](delegatepermissions.md) <br/> |<span data-ttu-id="fd178-118">Содержит параметры уровня разрешений делегат для пользователя.</span><span class="sxs-lookup"><span data-stu-id="fd178-118">Contains the delegate permission level settings for a user.</span></span> <span data-ttu-id="fd178-119">Этот элемент появился в Exchange 2007 с пакетом обновления 1.</span><span class="sxs-lookup"><span data-stu-id="fd178-119">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="fd178-120">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="fd178-120">Text value</span></span>

<span data-ttu-id="fd178-121">В следующей таблице перечислены текстовые значения, которые представляют уровни разрешений.</span><span class="sxs-lookup"><span data-stu-id="fd178-121">The following table lists the text values that represent the permission levels.</span></span>
  
<span data-ttu-id="fd178-122">**Разрешение уровня текстовые значения**</span><span class="sxs-lookup"><span data-stu-id="fd178-122">**Permission level text values**</span></span>

|<span data-ttu-id="fd178-123">**Уровень разрешений**</span><span class="sxs-lookup"><span data-stu-id="fd178-123">**Permission level**</span></span>|<span data-ttu-id="fd178-124">**Описание**</span><span class="sxs-lookup"><span data-stu-id="fd178-124">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="fd178-125">Нет</span><span class="sxs-lookup"><span data-stu-id="fd178-125">None</span></span>  <br/> |<span data-ttu-id="fd178-126">Делегата не имеет доступа к разрешений для папки «Календарь».</span><span class="sxs-lookup"><span data-stu-id="fd178-126">The delegate user has no access permissions to the Calendar folder.</span></span>  <br/> |
|<span data-ttu-id="fd178-127">Редактор</span><span class="sxs-lookup"><span data-stu-id="fd178-127">Reviewer</span></span>  <br/> |<span data-ttu-id="fd178-128">Делегат пользователь может читать элементы в папке календаря.</span><span class="sxs-lookup"><span data-stu-id="fd178-128">The delegate user can read items in the Calendar folder.</span></span>  <br/> |
|<span data-ttu-id="fd178-129">Author</span><span class="sxs-lookup"><span data-stu-id="fd178-129">Author</span></span>  <br/> |<span data-ttu-id="fd178-130">Делегата можно читать и создавать элементы в папке календаря.</span><span class="sxs-lookup"><span data-stu-id="fd178-130">The delegate user can read and create items in the Calendar folder.</span></span>  <br/> |
|<span data-ttu-id="fd178-131">Редактор</span><span class="sxs-lookup"><span data-stu-id="fd178-131">Editor</span></span>  <br/> |<span data-ttu-id="fd178-132">Делегата могут читать, создавать и изменять элементы в папке календаря.</span><span class="sxs-lookup"><span data-stu-id="fd178-132">The delegate user can read, create, and modify items in the Calendar folder.</span></span>  <br/> |
|<span data-ttu-id="fd178-133">Пользовательский сервер</span><span class="sxs-lookup"><span data-stu-id="fd178-133">Custom</span></span>  <br/> |<span data-ttu-id="fd178-134">Делегата имеет пользовательские разрешения доступа к папке календаря.</span><span class="sxs-lookup"><span data-stu-id="fd178-134">The delegate user has custom access permissions to the Calendar folder.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="fd178-135">Замечания</span><span class="sxs-lookup"><span data-stu-id="fd178-135">Remarks</span></span>

<span data-ttu-id="fd178-136">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="fd178-136">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="fd178-137">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="fd178-137">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="fd178-138">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="fd178-138">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="fd178-139">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="fd178-139">Schema Name</span></span>  <br/> |<span data-ttu-id="fd178-140">Схема Types</span><span class="sxs-lookup"><span data-stu-id="fd178-140">Types schema</span></span>  <br/> |
|<span data-ttu-id="fd178-141">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="fd178-141">Validation File</span></span>  <br/> |<span data-ttu-id="fd178-142">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="fd178-142">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="fd178-143">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="fd178-143">Can be Empty</span></span>  <br/> |<span data-ttu-id="fd178-144">False</span><span class="sxs-lookup"><span data-stu-id="fd178-144">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="fd178-145">См. также</span><span class="sxs-lookup"><span data-stu-id="fd178-145">See also</span></span>



[<span data-ttu-id="fd178-146">Операция AddDelegate</span><span class="sxs-lookup"><span data-stu-id="fd178-146">AddDelegate operation</span></span>](adddelegate-operation.md)
  
[<span data-ttu-id="fd178-147">Операция UpdateDelegate</span><span class="sxs-lookup"><span data-stu-id="fd178-147">UpdateDelegate operation</span></span>](updatedelegate-operation.md)


- [<span data-ttu-id="fd178-148">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="fd178-148">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="fd178-149">Добавление делегатов</span><span class="sxs-lookup"><span data-stu-id="fd178-149">Adding Delegates</span></span>](http://msdn.microsoft.com/library/3a744150-66a3-4a13-9433-793603ba5038%28Office.15%29.aspx)

