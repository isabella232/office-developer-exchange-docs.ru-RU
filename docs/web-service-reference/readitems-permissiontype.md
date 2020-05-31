---
title: ReadItems (Пермиссионтипе)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ReadItems
api_type:
- schema
ms.assetid: 0a11a802-28e2-436b-b5a9-30fd064675a6
description: Элемент ReadItems указывает, имеет ли пользователь разрешение на чтение элементов в папке. Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).
ms.openlocfilehash: bf266c77106f25b90ffd174e25fb0c3972ab91cb
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834961"
---
# <a name="readitems-permissiontype"></a><span data-ttu-id="61375-104">ReadItems (Пермиссионтипе)</span><span class="sxs-lookup"><span data-stu-id="61375-104">ReadItems (PermissionType)</span></span>

<span data-ttu-id="61375-105">Элемент **ReadItems** указывает, имеет ли пользователь разрешение на чтение элементов в папке.</span><span class="sxs-lookup"><span data-stu-id="61375-105">The **ReadItems** element indicates whether a user has permission to read items within a folder.</span></span> <span data-ttu-id="61375-106">Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="61375-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<ReadItems>None or FullDetails</ReadItems>
```

 <span data-ttu-id="61375-107">**пермиссионреадакцесстипе**</span><span class="sxs-lookup"><span data-stu-id="61375-107">**PermissionReadAccessType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="61375-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="61375-108">Attributes and elements</span></span>

<span data-ttu-id="61375-109">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="61375-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="61375-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="61375-110">Attributes</span></span>

<span data-ttu-id="61375-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="61375-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="61375-112">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="61375-112">Child elements</span></span>

<span data-ttu-id="61375-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="61375-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="61375-114">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="61375-114">Parent elements</span></span>

|<span data-ttu-id="61375-115">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="61375-115">**Element**</span></span>|<span data-ttu-id="61375-116">**Описание**</span><span class="sxs-lookup"><span data-stu-id="61375-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="61375-117">Разрешение</span><span class="sxs-lookup"><span data-stu-id="61375-117">Permission</span></span>](permission.md) <br/> |<span data-ttu-id="61375-p103">Определяет доступ пользователя к папке. Этот элемент появился в Exchange 2007 с пакетом обновления 1.</span><span class="sxs-lookup"><span data-stu-id="61375-p103">Defines the access that a user has to a folder. This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="61375-120">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="61375-120">Text value</span></span>

<span data-ttu-id="61375-121">В следующей таблице приведены возможные значения для элемента **ReadItems** .</span><span class="sxs-lookup"><span data-stu-id="61375-121">The following table lists the possible values for the **ReadItems** element.</span></span> 
  
<span data-ttu-id="61375-122">**Текстовые значения элементов ReadItems**</span><span class="sxs-lookup"><span data-stu-id="61375-122">**ReadItems element text values**</span></span>

|<span data-ttu-id="61375-123">**Значение**</span><span class="sxs-lookup"><span data-stu-id="61375-123">**Value**</span></span>|<span data-ttu-id="61375-124">**Описание**</span><span class="sxs-lookup"><span data-stu-id="61375-124">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="61375-125">Нет</span><span class="sxs-lookup"><span data-stu-id="61375-125">None</span></span>  <br/> |<span data-ttu-id="61375-126">Указывает, что у пользователя нет разрешения на чтение элементов в папке.</span><span class="sxs-lookup"><span data-stu-id="61375-126">Indicates that the user does not have permission to read items in the folder.</span></span>  <br/> |
|<span data-ttu-id="61375-127">фуллдетаилс</span><span class="sxs-lookup"><span data-stu-id="61375-127">FullDetails</span></span>  <br/> |<span data-ttu-id="61375-128">Указывает, что у пользователя есть разрешение на чтение всех элементов в папке.</span><span class="sxs-lookup"><span data-stu-id="61375-128">Indicates that the user has permission to read all items in the folder.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="61375-129">Примечания</span><span class="sxs-lookup"><span data-stu-id="61375-129">Remarks</span></span>

<span data-ttu-id="61375-130">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="61375-130">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="61375-131">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="61375-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="61375-132">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="61375-132">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="61375-133">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="61375-133">Schema Name</span></span>  <br/> |<span data-ttu-id="61375-134">Схема Types</span><span class="sxs-lookup"><span data-stu-id="61375-134">Types schema</span></span>  <br/> |
|<span data-ttu-id="61375-135">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="61375-135">Validation File</span></span>  <br/> |<span data-ttu-id="61375-136">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="61375-136">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="61375-137">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="61375-137">Can be Empty</span></span>  <br/> |<span data-ttu-id="61375-138">False</span><span class="sxs-lookup"><span data-stu-id="61375-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="61375-139">См. также</span><span class="sxs-lookup"><span data-stu-id="61375-139">See also</span></span>



- [<span data-ttu-id="61375-140">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="61375-140">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="61375-141">Setting Folder-Level Permissions</span><span class="sxs-lookup"><span data-stu-id="61375-141">Setting Folder-Level Permissions</span></span>](http://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

