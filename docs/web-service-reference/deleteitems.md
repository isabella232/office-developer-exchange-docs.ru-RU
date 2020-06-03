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
ms.openlocfilehash: a0bbefc8b021d047bb2e001669c3e92a6e2536ce
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44454409"
---
# <a name="deleteitems"></a><span data-ttu-id="d7d64-104">делетеитемс</span><span class="sxs-lookup"><span data-stu-id="d7d64-104">DeleteItems</span></span>

<span data-ttu-id="d7d64-105">Элемент **делетеитемс** указывает, какие элементы папки у пользователя есть разрешение на удаление.</span><span class="sxs-lookup"><span data-stu-id="d7d64-105">The **DeleteItems** element indicates which items in a folder a user has permission to delete.</span></span> <span data-ttu-id="d7d64-106">Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="d7d64-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<DeleteItems>None or Owned or All</DeleteItems>
```

 <span data-ttu-id="d7d64-107">**пермиссионактионтипе**</span><span class="sxs-lookup"><span data-stu-id="d7d64-107">**PermissionActionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d7d64-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="d7d64-108">Attributes and elements</span></span>

<span data-ttu-id="d7d64-109">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="d7d64-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d7d64-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="d7d64-110">Attributes</span></span>

<span data-ttu-id="d7d64-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="d7d64-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d7d64-112">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="d7d64-112">Child elements</span></span>

<span data-ttu-id="d7d64-113">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="d7d64-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="d7d64-114">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="d7d64-114">Parent elements</span></span>

|<span data-ttu-id="d7d64-115">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="d7d64-115">**Element**</span></span>|<span data-ttu-id="d7d64-116">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d7d64-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d7d64-117">Разрешение</span><span class="sxs-lookup"><span data-stu-id="d7d64-117">Permission</span></span>](permission.md) <br/> |<span data-ttu-id="d7d64-p103">Определяет доступ пользователя к папке. Этот элемент появился в Exchange 2007 с пакетом обновления 1.</span><span class="sxs-lookup"><span data-stu-id="d7d64-p103">Defines the access that a user has to a folder. This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="d7d64-120">календарпермиссион</span><span class="sxs-lookup"><span data-stu-id="d7d64-120">CalendarPermission</span></span>](calendarpermission.md) <br/> |<span data-ttu-id="d7d64-p104">Определяет доступ пользователя к папке календаря. Этот элемент появился в Exchange 2007 с пакетом обновления 1.</span><span class="sxs-lookup"><span data-stu-id="d7d64-p104">Defines the access that a user has to a Calendar folder. This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="d7d64-123">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="d7d64-123">Text value</span></span>

<span data-ttu-id="d7d64-124">В следующей таблице приведены возможные значения для элемента **делетеитемс** .</span><span class="sxs-lookup"><span data-stu-id="d7d64-124">The following table lists the possible values for the **DeleteItems** element.</span></span> 
  
<span data-ttu-id="d7d64-125">**Текстовые значения элементов Делетеитемс**</span><span class="sxs-lookup"><span data-stu-id="d7d64-125">**DeleteItems element text values**</span></span>

|<span data-ttu-id="d7d64-126">**Значение**</span><span class="sxs-lookup"><span data-stu-id="d7d64-126">**Value**</span></span>|<span data-ttu-id="d7d64-127">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d7d64-127">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="d7d64-128">Нет</span><span class="sxs-lookup"><span data-stu-id="d7d64-128">None</span></span>  <br/> |<span data-ttu-id="d7d64-129">Указывает, что у пользователя нет разрешения на удаление элементов в папке.</span><span class="sxs-lookup"><span data-stu-id="d7d64-129">Indicates that the user does not have permission to delete items in the folder.</span></span>  <br/> |
|<span data-ttu-id="d7d64-130">Он</span><span class="sxs-lookup"><span data-stu-id="d7d64-130">Owned</span></span>  <br/> |<span data-ttu-id="d7d64-131">Указывает, что у пользователя есть разрешение на удаление элементов, принадлежащих пользователю в папке.</span><span class="sxs-lookup"><span data-stu-id="d7d64-131">Indicates that the user has permission to delete the items that the user owns in the folder.</span></span>  <br/> |
|<span data-ttu-id="d7d64-132">Все</span><span class="sxs-lookup"><span data-stu-id="d7d64-132">All</span></span>  <br/> |<span data-ttu-id="d7d64-133">Указывает, что у пользователя есть разрешение на удаление всех элементов в папке.</span><span class="sxs-lookup"><span data-stu-id="d7d64-133">Indicates that the user has permission to delete all items in the folder.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="d7d64-134">Примечания</span><span class="sxs-lookup"><span data-stu-id="d7d64-134">Remarks</span></span>

<span data-ttu-id="d7d64-135">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="d7d64-135">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d7d64-136">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="d7d64-136">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d7d64-137">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="d7d64-137">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d7d64-138">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="d7d64-138">Schema Name</span></span>  <br/> |<span data-ttu-id="d7d64-139">Схема Types</span><span class="sxs-lookup"><span data-stu-id="d7d64-139">Types schema</span></span>  <br/> |
|<span data-ttu-id="d7d64-140">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="d7d64-140">Validation File</span></span>  <br/> |<span data-ttu-id="d7d64-141">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="d7d64-141">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d7d64-142">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="d7d64-142">Can be Empty</span></span>  <br/> |<span data-ttu-id="d7d64-143">False</span><span class="sxs-lookup"><span data-stu-id="d7d64-143">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d7d64-144">См. также</span><span class="sxs-lookup"><span data-stu-id="d7d64-144">See also</span></span>

- [<span data-ttu-id="d7d64-145">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="d7d64-145">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="d7d64-146">Setting Folder-Level Permissions</span><span class="sxs-lookup"><span data-stu-id="d7d64-146">Setting Folder-Level Permissions</span></span>](https://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

