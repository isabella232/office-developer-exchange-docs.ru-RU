---
title: GroupedItems
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GroupedItems
api_type:
- schema
ms.assetid: 53170df4-4272-4b37-b23f-cd8e2d4a7396
description: Элемент GroupedItems представляет коллекцию элементов, которые являются результатом сгруппированных вызова операции FindItem.
ms.openlocfilehash: f8aed9b78fc54307f44b96a45e5c31a4cc76ab50
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833756"
---
# <a name="groupeditems"></a><span data-ttu-id="049e1-103">GroupedItems</span><span class="sxs-lookup"><span data-stu-id="049e1-103">GroupedItems</span></span>

<span data-ttu-id="049e1-104">Элемент **GroupedItems** представляет коллекцию элементов, которые являются результатом сгруппированных [операции FindItem](finditem-operation.md) вызова.</span><span class="sxs-lookup"><span data-stu-id="049e1-104">The **GroupedItems** element represents a collection of items that are the result of a grouped [FindItem operation](finditem-operation.md) call.</span></span> 
  
[<span data-ttu-id="049e1-105">FindItemResponse</span><span class="sxs-lookup"><span data-stu-id="049e1-105">FindItemResponse</span></span>](finditemresponse.md)
  
[<span data-ttu-id="049e1-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="049e1-106">ResponseMessages</span></span>](responsemessages.md)
  
[<span data-ttu-id="049e1-107">FindItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="049e1-107">FindItemResponseMessage</span></span>](finditemresponsemessage.md)
  
[<span data-ttu-id="049e1-108">RootFolder (FindItemResponseMessage)</span><span class="sxs-lookup"><span data-stu-id="049e1-108">RootFolder (FindItemResponseMessage)</span></span>](rootfolder-finditemresponsemessage.md)
  
[<span data-ttu-id="049e1-109">Группы</span><span class="sxs-lookup"><span data-stu-id="049e1-109">Groups</span></span>](groups.md)
  
[<span data-ttu-id="049e1-110">GroupedItems</span><span class="sxs-lookup"><span data-stu-id="049e1-110">GroupedItems</span></span>](groupeditems.md)
  
```xml
<GroupedItems>
   <GroupIndex/>
   <Items/>
</GroupedItems>
```

 <span data-ttu-id="049e1-111">**GroupedItemsType**</span><span class="sxs-lookup"><span data-stu-id="049e1-111">**GroupedItemsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="049e1-112">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="049e1-112">Attributes and elements</span></span>

<span data-ttu-id="049e1-113">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="049e1-113">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="049e1-114">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="049e1-114">Attributes</span></span>

<span data-ttu-id="049e1-115">Нет.</span><span class="sxs-lookup"><span data-stu-id="049e1-115">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="049e1-116">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="049e1-116">Child elements</span></span>

|<span data-ttu-id="049e1-117">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="049e1-117">**Element**</span></span>|<span data-ttu-id="049e1-118">**Описание**</span><span class="sxs-lookup"><span data-stu-id="049e1-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="049e1-119">GroupIndex</span><span class="sxs-lookup"><span data-stu-id="049e1-119">GroupIndex</span></span>](groupindex.md) <br/> |<span data-ttu-id="049e1-120">Представляет значение свойства, используемое для группировки элементов в сгруппированных [операции FindItem](finditem-operation.md) вызова.</span><span class="sxs-lookup"><span data-stu-id="049e1-120">Represents the property value that is used to group items in a grouped [FindItem operation](finditem-operation.md) call.</span></span>  <br/> |
|[<span data-ttu-id="049e1-121">Элементы</span><span class="sxs-lookup"><span data-stu-id="049e1-121">Items</span></span>](items.md) <br/> |<span data-ttu-id="049e1-122">Содержит массив сгруппированные элементы.</span><span class="sxs-lookup"><span data-stu-id="049e1-122">Contains an array of grouped items.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="049e1-123">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="049e1-123">Parent elements</span></span>

|<span data-ttu-id="049e1-124">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="049e1-124">**Element**</span></span>|<span data-ttu-id="049e1-125">**Описание**</span><span class="sxs-lookup"><span data-stu-id="049e1-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="049e1-126">Группы</span><span class="sxs-lookup"><span data-stu-id="049e1-126">Groups</span></span>](groups.md) <br/> |<span data-ttu-id="049e1-127">Содержит коллекцию групп, которые находятся с критерии поиска и объединение, который идентифицируется в запрос [FindItem операции](finditem-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="049e1-127">Contains a collection of groups that are found with the search and aggregation criteria that is identified in the [FindItem operation](finditem-operation.md) request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="049e1-128">Замечания</span><span class="sxs-lookup"><span data-stu-id="049e1-128">Remarks</span></span>

<span data-ttu-id="049e1-129">Схема, описывающая этот элемент находится в виртуальном каталоге EWS компьютера, на котором выполняется Microsoft Exchange Server 2010 с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="049e1-129">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="049e1-130">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="049e1-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="049e1-131">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="049e1-131">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="049e1-132">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="049e1-132">Schema name</span></span>  <br/> |<span data-ttu-id="049e1-133">Схема Types</span><span class="sxs-lookup"><span data-stu-id="049e1-133">Types schema</span></span>  <br/> |
|<span data-ttu-id="049e1-134">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="049e1-134">Validation file</span></span>  <br/> |<span data-ttu-id="049e1-135">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="049e1-135">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="049e1-136">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="049e1-136">Can be empty</span></span>  <br/> |<span data-ttu-id="049e1-137">False</span><span class="sxs-lookup"><span data-stu-id="049e1-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="049e1-138">См. также</span><span class="sxs-lookup"><span data-stu-id="049e1-138">See also</span></span>



[<span data-ttu-id="049e1-139">FindItem Operation</span><span class="sxs-lookup"><span data-stu-id="049e1-139">FindItem operation</span></span>](finditem-operation.md)


[<span data-ttu-id="049e1-140">Поиск элементов</span><span class="sxs-lookup"><span data-stu-id="049e1-140">Finding Items</span></span>](http://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)

