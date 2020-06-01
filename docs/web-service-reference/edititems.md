---
title: едититемс
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- EditItems
api_type:
- schema
ms.assetid: 1cb14493-c999-4d66-b82c-ecb410dc1c00
description: Элемент Едититемс указывает, какие элементы папки у пользователя есть разрешение на изменение. Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).
ms.openlocfilehash: 0c3800b4d242dccb7455e0d0dea74e766db22854
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459253"
---
# <a name="edititems"></a><span data-ttu-id="a8881-104">едититемс</span><span class="sxs-lookup"><span data-stu-id="a8881-104">EditItems</span></span>

<span data-ttu-id="a8881-105">Элемент **едититемс** указывает, какие элементы папки у пользователя есть разрешение на изменение.</span><span class="sxs-lookup"><span data-stu-id="a8881-105">The **EditItems** element indicates which items in a folder a user has permission to edit.</span></span> <span data-ttu-id="a8881-106">Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="a8881-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<EditItems>None or Owned or All</EditItems>
```

 <span data-ttu-id="a8881-107">**пермиссионактионтипе**</span><span class="sxs-lookup"><span data-stu-id="a8881-107">**PermissionActionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a8881-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="a8881-108">Attributes and elements</span></span>

<span data-ttu-id="a8881-109">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="a8881-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a8881-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="a8881-110">Attributes</span></span>

<span data-ttu-id="a8881-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="a8881-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a8881-112">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="a8881-112">Child elements</span></span>

<span data-ttu-id="a8881-113">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="a8881-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="a8881-114">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="a8881-114">Parent elements</span></span>

|<span data-ttu-id="a8881-115">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="a8881-115">**Element**</span></span>|<span data-ttu-id="a8881-116">**Описание**</span><span class="sxs-lookup"><span data-stu-id="a8881-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a8881-117">Разрешение</span><span class="sxs-lookup"><span data-stu-id="a8881-117">Permission</span></span>](permission.md) <br/> |<span data-ttu-id="a8881-p103">Определяет доступ пользователя к папке. Этот элемент появился в Exchange 2007 с пакетом обновления 1.</span><span class="sxs-lookup"><span data-stu-id="a8881-p103">Defines the access that a user has to a folder. This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="a8881-120">календарпермиссион</span><span class="sxs-lookup"><span data-stu-id="a8881-120">CalendarPermission</span></span>](calendarpermission.md) <br/> |<span data-ttu-id="a8881-p104">Определяет доступ пользователя к папке календаря. Этот элемент появился в Exchange 2007 с пакетом обновления 1.</span><span class="sxs-lookup"><span data-stu-id="a8881-p104">Defines the access that a user has to a Calendar folder. This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="a8881-123">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="a8881-123">Text value</span></span>

<span data-ttu-id="a8881-124">В следующей таблице приведены возможные значения для элемента **едититемс** .</span><span class="sxs-lookup"><span data-stu-id="a8881-124">The following table lists the possible values for the **EditItems** element.</span></span> 
  
<span data-ttu-id="a8881-125">**Текстовые значения элементов Едититемс**</span><span class="sxs-lookup"><span data-stu-id="a8881-125">**EditItems element text values**</span></span>

|<span data-ttu-id="a8881-126">**Значение**</span><span class="sxs-lookup"><span data-stu-id="a8881-126">**Value**</span></span>|<span data-ttu-id="a8881-127">**Описание**</span><span class="sxs-lookup"><span data-stu-id="a8881-127">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="a8881-128">Нет</span><span class="sxs-lookup"><span data-stu-id="a8881-128">None</span></span>  <br/> |<span data-ttu-id="a8881-129">Указывает, что у пользователя нет разрешения на изменение элементов в папке.</span><span class="sxs-lookup"><span data-stu-id="a8881-129">Indicates that the user does not have permission to edit items in the folder.</span></span>  <br/> |
|<span data-ttu-id="a8881-130">Он</span><span class="sxs-lookup"><span data-stu-id="a8881-130">Owned</span></span>  <br/> |<span data-ttu-id="a8881-131">Указывает, что у пользователя есть разрешение на изменение элементов, которыми владеет пользователь в папке.</span><span class="sxs-lookup"><span data-stu-id="a8881-131">Indicates that the user has permission to edit the items that the user owns in the folder.</span></span>  <br/> |
|<span data-ttu-id="a8881-132">Все</span><span class="sxs-lookup"><span data-stu-id="a8881-132">All</span></span>  <br/> |<span data-ttu-id="a8881-133">Указывает, что у пользователя есть разрешение на изменение всех элементов в папке.</span><span class="sxs-lookup"><span data-stu-id="a8881-133">Indicates that the user has permission to edit all items in the folder.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="a8881-134">Примечания</span><span class="sxs-lookup"><span data-stu-id="a8881-134">Remarks</span></span>

<span data-ttu-id="a8881-135">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="a8881-135">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a8881-136">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="a8881-136">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a8881-137">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="a8881-137">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="a8881-138">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="a8881-138">Schema Name</span></span>  <br/> |<span data-ttu-id="a8881-139">Схема Types</span><span class="sxs-lookup"><span data-stu-id="a8881-139">Types schema</span></span>  <br/> |
|<span data-ttu-id="a8881-140">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="a8881-140">Validation File</span></span>  <br/> |<span data-ttu-id="a8881-141">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="a8881-141">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="a8881-142">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="a8881-142">Can be Empty</span></span>  <br/> |<span data-ttu-id="a8881-143">False</span><span class="sxs-lookup"><span data-stu-id="a8881-143">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a8881-144">См. также</span><span class="sxs-lookup"><span data-stu-id="a8881-144">See also</span></span>

- [<span data-ttu-id="a8881-145">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="a8881-145">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="a8881-146">Setting Folder-Level Permissions</span><span class="sxs-lookup"><span data-stu-id="a8881-146">Setting Folder-Level Permissions</span></span>](https://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

