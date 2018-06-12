---
title: CanCreateItems
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CanCreateItems
api_type:
- schema
ms.assetid: c4574e9a-3c42-40a1-a5f9-79b6560e9b30
description: Элемент CanCreateItems указывает, является ли пользователь имеет право на создание элементов в папке. Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).
ms.openlocfilehash: 313699a15ef3038dd9114c18b76b29aba15e5ab7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761669"
---
# <a name="cancreateitems"></a><span data-ttu-id="2ab2e-104">CanCreateItems</span><span class="sxs-lookup"><span data-stu-id="2ab2e-104">CanCreateItems</span></span>

<span data-ttu-id="2ab2e-105">Элемент **CanCreateItems** указывает, является ли пользователь имеет право на создание элементов в папке.</span><span class="sxs-lookup"><span data-stu-id="2ab2e-105">The **CanCreateItems** element indicates whether a user has permission to create items in a folder.</span></span> <span data-ttu-id="2ab2e-106">Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="2ab2e-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<CanCreateItems/>
```

 <span data-ttu-id="2ab2e-107">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="2ab2e-107">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2ab2e-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="2ab2e-108">Attributes and elements</span></span>

<span data-ttu-id="2ab2e-109">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="2ab2e-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2ab2e-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="2ab2e-110">Attributes</span></span>

<span data-ttu-id="2ab2e-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="2ab2e-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2ab2e-112">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="2ab2e-112">Child elements</span></span>

<span data-ttu-id="2ab2e-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="2ab2e-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="2ab2e-114">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="2ab2e-114">Parent elements</span></span>

|<span data-ttu-id="2ab2e-115">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="2ab2e-115">**Element**</span></span>|<span data-ttu-id="2ab2e-116">**Описание**</span><span class="sxs-lookup"><span data-stu-id="2ab2e-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2ab2e-117">Разрешение</span><span class="sxs-lookup"><span data-stu-id="2ab2e-117">Permission</span></span>](permission.md) <br/> |<span data-ttu-id="2ab2e-p103">Определяет доступ пользователя к папке. Этот элемент появился в Exchange 2007 с пакетом обновления 1.</span><span class="sxs-lookup"><span data-stu-id="2ab2e-p103">Defines the access that a user has to a folder. This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="2ab2e-120">CalendarPermission</span><span class="sxs-lookup"><span data-stu-id="2ab2e-120">CalendarPermission</span></span>](calendarpermission.md) <br/> |<span data-ttu-id="2ab2e-p104">Определяет доступ пользователя к папке календаря. Этот элемент появился в Exchange 2007 с пакетом обновления 1.</span><span class="sxs-lookup"><span data-stu-id="2ab2e-p104">Defines the access that a user has to a Calendar folder. This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="2ab2e-123">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="2ab2e-123">Text value</span></span>

<span data-ttu-id="2ab2e-124">Текстовое значение **true,** указывает, что пользователь может создавать элементы в папке.</span><span class="sxs-lookup"><span data-stu-id="2ab2e-124">A text value of **true** indicates that the user can create items in the folder.</span></span> <span data-ttu-id="2ab2e-125">Значение **false** указывает, что пользователь не может создавать элементы в папке.</span><span class="sxs-lookup"><span data-stu-id="2ab2e-125">A value of **false** indicates that the user cannot create items in the folder.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="2ab2e-126">Замечания</span><span class="sxs-lookup"><span data-stu-id="2ab2e-126">Remarks</span></span>

<span data-ttu-id="2ab2e-127">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="2ab2e-127">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2ab2e-128">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="2ab2e-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2ab2e-129">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="2ab2e-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="2ab2e-130">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="2ab2e-130">Schema Name</span></span>  <br/> |<span data-ttu-id="2ab2e-131">Схема Types</span><span class="sxs-lookup"><span data-stu-id="2ab2e-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="2ab2e-132">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="2ab2e-132">Validation File</span></span>  <br/> |<span data-ttu-id="2ab2e-133">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="2ab2e-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="2ab2e-134">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="2ab2e-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="2ab2e-135">False</span><span class="sxs-lookup"><span data-stu-id="2ab2e-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="2ab2e-136">См. также</span><span class="sxs-lookup"><span data-stu-id="2ab2e-136">See also</span></span>



- [<span data-ttu-id="2ab2e-137">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="2ab2e-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="2ab2e-138">Setting Folder-Level Permissions</span><span class="sxs-lookup"><span data-stu-id="2ab2e-138">Setting Folder-Level Permissions</span></span>](http://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

