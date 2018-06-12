---
title: GroupIndex
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GroupIndex
api_type:
- schema
ms.assetid: 7a596ff7-6cc3-4626-a52c-538a92202337
description: Элемент GroupIndex представляет значение свойства, которое используется для группирования элементов для текущей группы элементов в ходе вызова FindItem операции.
ms.openlocfilehash: 8b23f5142a15c099c30209ea48cd04f4af4e8c6a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833762"
---
# <a name="groupindex"></a><span data-ttu-id="021a8-103">GroupIndex</span><span class="sxs-lookup"><span data-stu-id="021a8-103">GroupIndex</span></span>

<span data-ttu-id="021a8-104">Элемент **GroupIndex** представляет значение свойства, которое используется для группирования элементов для текущей группы элементов в ходе [операции FindItem](finditem-operation.md) вызова.</span><span class="sxs-lookup"><span data-stu-id="021a8-104">The **GroupIndex** element represents the property value that is used to group items for the current group of items in a [FindItem operation](finditem-operation.md) call.</span></span> 
  
[<span data-ttu-id="021a8-105">FindItemResponse</span><span class="sxs-lookup"><span data-stu-id="021a8-105">FindItemResponse</span></span>](finditemresponse.md)
  
[<span data-ttu-id="021a8-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="021a8-106">ResponseMessages</span></span>](responsemessages.md)
  
[<span data-ttu-id="021a8-107">FindItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="021a8-107">FindItemResponseMessage</span></span>](finditemresponsemessage.md)
  
[<span data-ttu-id="021a8-108">RootFolder (FindItemResponseMessage)</span><span class="sxs-lookup"><span data-stu-id="021a8-108">RootFolder (FindItemResponseMessage)</span></span>](rootfolder-finditemresponsemessage.md)
  
[<span data-ttu-id="021a8-109">Группы</span><span class="sxs-lookup"><span data-stu-id="021a8-109">Groups</span></span>](groups.md)
  
[<span data-ttu-id="021a8-110">GroupedItems</span><span class="sxs-lookup"><span data-stu-id="021a8-110">GroupedItems</span></span>](groupeditems.md)
  
[<span data-ttu-id="021a8-111">GroupIndex</span><span class="sxs-lookup"><span data-stu-id="021a8-111">GroupIndex</span></span>](groupindex.md)
  
```xml
<GroupIndex/>
```

 <span data-ttu-id="021a8-112">**string**</span><span class="sxs-lookup"><span data-stu-id="021a8-112">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="021a8-113">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="021a8-113">Attributes and elements</span></span>

<span data-ttu-id="021a8-114">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="021a8-114">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="021a8-115">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="021a8-115">Attributes</span></span>

<span data-ttu-id="021a8-116">Нет.</span><span class="sxs-lookup"><span data-stu-id="021a8-116">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="021a8-117">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="021a8-117">Child elements</span></span>

<span data-ttu-id="021a8-118">Нет.</span><span class="sxs-lookup"><span data-stu-id="021a8-118">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="021a8-119">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="021a8-119">Parent elements</span></span>

|<span data-ttu-id="021a8-120">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="021a8-120">**Element**</span></span>|<span data-ttu-id="021a8-121">**Описание**</span><span class="sxs-lookup"><span data-stu-id="021a8-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="021a8-122">GroupedItems</span><span class="sxs-lookup"><span data-stu-id="021a8-122">GroupedItems</span></span>](groupeditems.md) <br/> |<span data-ttu-id="021a8-123">Представляет коллекцию элементов, которые являются результатом сгруппированных [операции FindItem](finditem-operation.md) вызова.</span><span class="sxs-lookup"><span data-stu-id="021a8-123">Represents a collection of items that are the result of a grouped [FindItem operation](finditem-operation.md) call.</span></span>  <br/> <span data-ttu-id="021a8-124">Ниже приведен выражение XPath для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="021a8-124">The following is the XPath expression to this element:</span></span>  <br/>  `/FindItemResponse/ResponseMessages/FindItemResponseMessage/RootFolder/Groups/GroupedItems[i]` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="021a8-125">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="021a8-125">Text value</span></span>

<span data-ttu-id="021a8-126">Текстовое значение является обязательным.</span><span class="sxs-lookup"><span data-stu-id="021a8-126">A text value is required.</span></span> <span data-ttu-id="021a8-127">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="021a8-127">This property is read-only.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="021a8-128">Замечания</span><span class="sxs-lookup"><span data-stu-id="021a8-128">Remarks</span></span>

<span data-ttu-id="021a8-129">Этот элемент имеет место только в ответ на [операцию FindItem](finditem-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="021a8-129">This element only occurs in a [FindItem operation](finditem-operation.md) response.</span></span> 
  
<span data-ttu-id="021a8-130">Схема, описывающая этот элемент находится в виртуальном каталоге EWS компьютера, на котором выполняется Microsoft Exchange Server 2010 с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="021a8-130">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="021a8-131">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="021a8-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="021a8-132">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="021a8-132">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="021a8-133">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="021a8-133">Schema name</span></span>  <br/> |<span data-ttu-id="021a8-134">Схема Types</span><span class="sxs-lookup"><span data-stu-id="021a8-134">Types schema</span></span>  <br/> |
|<span data-ttu-id="021a8-135">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="021a8-135">Validation file</span></span>  <br/> |<span data-ttu-id="021a8-136">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="021a8-136">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="021a8-137">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="021a8-137">Can be empty</span></span>  <br/> |<span data-ttu-id="021a8-138">False</span><span class="sxs-lookup"><span data-stu-id="021a8-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="021a8-139">См. также</span><span class="sxs-lookup"><span data-stu-id="021a8-139">See also</span></span>



[<span data-ttu-id="021a8-140">FindItem Operation</span><span class="sxs-lookup"><span data-stu-id="021a8-140">FindItem operation</span></span>](finditem-operation.md)


[<span data-ttu-id="021a8-141">Поиск элементов</span><span class="sxs-lookup"><span data-stu-id="021a8-141">Finding Items</span></span>](http://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)

