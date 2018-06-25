---
title: TasksFolderPermissionLevel
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- TasksFolderPermissionLevel
api_type:
- schema
ms.assetid: 0f70b79b-3443-4048-b410-692d4e2464fc
description: Элемент TasksFolderPermissionLevel содержит разрешения для папки задач по умолчанию. Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).
ms.openlocfilehash: 49807896f9175bafbef106c41d1c9dff8f6178c4
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19840137"
---
# <a name="tasksfolderpermissionlevel"></a><span data-ttu-id="7907b-104">TasksFolderPermissionLevel</span><span class="sxs-lookup"><span data-stu-id="7907b-104">TasksFolderPermissionLevel</span></span>

<span data-ttu-id="7907b-105">Элемент **TasksFolderPermissionLevel** содержит разрешения для папки задач по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="7907b-105">The **TasksFolderPermissionLevel** element contains the permissions for the default Tasks folder.</span></span> <span data-ttu-id="7907b-106">Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="7907b-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<TasksFolderPermissionLevel>
   None or Editor or Reviewer or Author or Custom
</TasksFolderPermissionLevel>
```

<span data-ttu-id="7907b-107">**DelegateFolderPermissionLevelType**</span><span class="sxs-lookup"><span data-stu-id="7907b-107">**DelegateFolderPermissionLevelType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="7907b-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="7907b-108">Attributes and elements</span></span>

<span data-ttu-id="7907b-109">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="7907b-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7907b-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="7907b-110">Attributes</span></span>

<span data-ttu-id="7907b-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="7907b-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7907b-112">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="7907b-112">Child elements</span></span>

<span data-ttu-id="7907b-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="7907b-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="7907b-114">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="7907b-114">Parent elements</span></span>

|<span data-ttu-id="7907b-115">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="7907b-115">**Element**</span></span>|<span data-ttu-id="7907b-116">**Описание**</span><span class="sxs-lookup"><span data-stu-id="7907b-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7907b-117">DelegatePermissions</span><span class="sxs-lookup"><span data-stu-id="7907b-117">DelegatePermissions</span></span>](delegatepermissions.md) <br/> |<span data-ttu-id="7907b-118">Содержит параметры уровня разрешений делегат для пользователя.</span><span class="sxs-lookup"><span data-stu-id="7907b-118">Contains the delegate permission level settings for a user.</span></span> <span data-ttu-id="7907b-119">Этот элемент появился в Exchange 2007 с пакетом обновления 1.</span><span class="sxs-lookup"><span data-stu-id="7907b-119">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="7907b-120">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="7907b-120">Text value</span></span>

<span data-ttu-id="7907b-121">В следующей таблице перечислены текстовые значения, которые представляют уровни разрешений.</span><span class="sxs-lookup"><span data-stu-id="7907b-121">The following table lists the text values that represent the permission levels.</span></span>
  
<span data-ttu-id="7907b-122">**Разрешение уровня текстовые значения**</span><span class="sxs-lookup"><span data-stu-id="7907b-122">**Permission level text values**</span></span>

|<span data-ttu-id="7907b-123">**Уровень разрешений**</span><span class="sxs-lookup"><span data-stu-id="7907b-123">**Permission level**</span></span>|<span data-ttu-id="7907b-124">**Описание**</span><span class="sxs-lookup"><span data-stu-id="7907b-124">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="7907b-125">Нет</span><span class="sxs-lookup"><span data-stu-id="7907b-125">None</span></span>  <br/> |<span data-ttu-id="7907b-126">Делегата не имеет доступа к разрешений на папку.</span><span class="sxs-lookup"><span data-stu-id="7907b-126">The delegate user has no access permissions to the Tasks folder.</span></span>  <br/> |
|<span data-ttu-id="7907b-127">Редактор</span><span class="sxs-lookup"><span data-stu-id="7907b-127">Reviewer</span></span>  <br/> |<span data-ttu-id="7907b-128">Делегат пользователь может читать элементы в папке задач.</span><span class="sxs-lookup"><span data-stu-id="7907b-128">The delegate user can read items in the Tasks folder.</span></span>  <br/> |
|<span data-ttu-id="7907b-129">Author</span><span class="sxs-lookup"><span data-stu-id="7907b-129">Author</span></span>  <br/> |<span data-ttu-id="7907b-130">Делегата можно читать и создавать элементы в папке заданий.</span><span class="sxs-lookup"><span data-stu-id="7907b-130">The delegate user can read and create items in the Tasks folder.</span></span>  <br/> |
|<span data-ttu-id="7907b-131">Редактор</span><span class="sxs-lookup"><span data-stu-id="7907b-131">Editor</span></span>  <br/> |<span data-ttu-id="7907b-132">Делегата могут читать, создавать и изменять элементы в папке задач.</span><span class="sxs-lookup"><span data-stu-id="7907b-132">The delegate user can read, create, and modify items in the Tasks folder.</span></span>  <br/> |
|<span data-ttu-id="7907b-133">Пользовательский сервер</span><span class="sxs-lookup"><span data-stu-id="7907b-133">Custom</span></span>  <br/> |<span data-ttu-id="7907b-134">Делегата имеет пользовательские разрешения доступа к папке задачи.</span><span class="sxs-lookup"><span data-stu-id="7907b-134">The delegate user has custom access permissions to the Tasks folder.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="7907b-135">Замечания</span><span class="sxs-lookup"><span data-stu-id="7907b-135">Remarks</span></span>

<span data-ttu-id="7907b-136">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="7907b-136">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7907b-137">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="7907b-137">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7907b-138">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="7907b-138">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="7907b-139">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="7907b-139">Schema Name</span></span>  <br/> |<span data-ttu-id="7907b-140">Схема Types</span><span class="sxs-lookup"><span data-stu-id="7907b-140">Types schema</span></span>  <br/> |
|<span data-ttu-id="7907b-141">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="7907b-141">Validation File</span></span>  <br/> |<span data-ttu-id="7907b-142">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="7907b-142">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="7907b-143">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="7907b-143">Can be Empty</span></span>  <br/> |<span data-ttu-id="7907b-144">False</span><span class="sxs-lookup"><span data-stu-id="7907b-144">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7907b-145">См. также</span><span class="sxs-lookup"><span data-stu-id="7907b-145">See also</span></span>

- [<span data-ttu-id="7907b-146">Операция AddDelegate</span><span class="sxs-lookup"><span data-stu-id="7907b-146">AddDelegate operation</span></span>](adddelegate-operation.md)
- [<span data-ttu-id="7907b-147">Операция UpdateDelegate</span><span class="sxs-lookup"><span data-stu-id="7907b-147">UpdateDelegate operation</span></span>](updatedelegate-operation.md)
- [<span data-ttu-id="7907b-148">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="7907b-148">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="7907b-149">Добавление делегатов</span><span class="sxs-lookup"><span data-stu-id="7907b-149">Adding Delegates</span></span>](http://msdn.microsoft.com/library/3a744150-66a3-4a13-9433-793603ba5038%28Office.15%29.aspx)

