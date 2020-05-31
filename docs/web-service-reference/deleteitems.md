---
title: делетеитемс
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
description: Элемент Делетеитемс указывает, какие элементы папки у пользователя есть разрешение на удаление. Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).
ms.openlocfilehash: 0be2154d1ceb6a995df8b27033fdc59bca81f9ef
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762052"
---
# <a name="deleteitems"></a><span data-ttu-id="c334c-104">делетеитемс</span><span class="sxs-lookup"><span data-stu-id="c334c-104">DeleteItems</span></span>

<span data-ttu-id="c334c-105">Элемент **делетеитемс** указывает, какие элементы папки у пользователя есть разрешение на удаление.</span><span class="sxs-lookup"><span data-stu-id="c334c-105">The **DeleteItems** element indicates which items in a folder a user has permission to delete.</span></span> <span data-ttu-id="c334c-106">Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="c334c-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<DeleteItems>None or Owned or All</DeleteItems>
```

 <span data-ttu-id="c334c-107">**пермиссионактионтипе**</span><span class="sxs-lookup"><span data-stu-id="c334c-107">**PermissionActionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c334c-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="c334c-108">Attributes and elements</span></span>

<span data-ttu-id="c334c-109">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="c334c-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c334c-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="c334c-110">Attributes</span></span>

<span data-ttu-id="c334c-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="c334c-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c334c-112">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="c334c-112">Child elements</span></span>

<span data-ttu-id="c334c-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="c334c-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="c334c-114">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="c334c-114">Parent elements</span></span>

|<span data-ttu-id="c334c-115">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="c334c-115">**Element**</span></span>|<span data-ttu-id="c334c-116">**Описание**</span><span class="sxs-lookup"><span data-stu-id="c334c-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c334c-117">Разрешение</span><span class="sxs-lookup"><span data-stu-id="c334c-117">Permission</span></span>](permission.md) <br/> |<span data-ttu-id="c334c-p103">Определяет доступ пользователя к папке. Этот элемент появился в Exchange 2007 с пакетом обновления 1.</span><span class="sxs-lookup"><span data-stu-id="c334c-p103">Defines the access that a user has to a folder. This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="c334c-120">календарпермиссион</span><span class="sxs-lookup"><span data-stu-id="c334c-120">CalendarPermission</span></span>](calendarpermission.md) <br/> |<span data-ttu-id="c334c-p104">Определяет доступ пользователя к папке календаря. Этот элемент появился в Exchange 2007 с пакетом обновления 1.</span><span class="sxs-lookup"><span data-stu-id="c334c-p104">Defines the access that a user has to a Calendar folder. This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="c334c-123">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="c334c-123">Text value</span></span>

<span data-ttu-id="c334c-124">В следующей таблице приведены возможные значения для элемента **делетеитемс** .</span><span class="sxs-lookup"><span data-stu-id="c334c-124">The following table lists the possible values for the **DeleteItems** element.</span></span> 
  
<span data-ttu-id="c334c-125">**Текстовые значения элементов Делетеитемс**</span><span class="sxs-lookup"><span data-stu-id="c334c-125">**DeleteItems element text values**</span></span>

|<span data-ttu-id="c334c-126">**Значение**</span><span class="sxs-lookup"><span data-stu-id="c334c-126">**Value**</span></span>|<span data-ttu-id="c334c-127">**Описание**</span><span class="sxs-lookup"><span data-stu-id="c334c-127">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="c334c-128">Нет</span><span class="sxs-lookup"><span data-stu-id="c334c-128">None</span></span>  <br/> |<span data-ttu-id="c334c-129">Указывает, что у пользователя нет разрешения на удаление элементов в папке.</span><span class="sxs-lookup"><span data-stu-id="c334c-129">Indicates that the user does not have permission to delete items in the folder.</span></span>  <br/> |
|<span data-ttu-id="c334c-130">Он</span><span class="sxs-lookup"><span data-stu-id="c334c-130">Owned</span></span>  <br/> |<span data-ttu-id="c334c-131">Указывает, что у пользователя есть разрешение на удаление элементов, принадлежащих пользователю в папке.</span><span class="sxs-lookup"><span data-stu-id="c334c-131">Indicates that the user has permission to delete the items that the user owns in the folder.</span></span>  <br/> |
|<span data-ttu-id="c334c-132">Все</span><span class="sxs-lookup"><span data-stu-id="c334c-132">All</span></span>  <br/> |<span data-ttu-id="c334c-133">Указывает, что у пользователя есть разрешение на удаление всех элементов в папке.</span><span class="sxs-lookup"><span data-stu-id="c334c-133">Indicates that the user has permission to delete all items in the folder.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="c334c-134">Примечания</span><span class="sxs-lookup"><span data-stu-id="c334c-134">Remarks</span></span>

<span data-ttu-id="c334c-135">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="c334c-135">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c334c-136">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="c334c-136">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c334c-137">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="c334c-137">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="c334c-138">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="c334c-138">Schema Name</span></span>  <br/> |<span data-ttu-id="c334c-139">Схема Types</span><span class="sxs-lookup"><span data-stu-id="c334c-139">Types schema</span></span>  <br/> |
|<span data-ttu-id="c334c-140">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="c334c-140">Validation File</span></span>  <br/> |<span data-ttu-id="c334c-141">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="c334c-141">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="c334c-142">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="c334c-142">Can be Empty</span></span>  <br/> |<span data-ttu-id="c334c-143">False</span><span class="sxs-lookup"><span data-stu-id="c334c-143">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c334c-144">См. также</span><span class="sxs-lookup"><span data-stu-id="c334c-144">See also</span></span>

- [<span data-ttu-id="c334c-145">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="c334c-145">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="c334c-146">Setting Folder-Level Permissions</span><span class="sxs-lookup"><span data-stu-id="c334c-146">Setting Folder-Level Permissions</span></span>](http://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

