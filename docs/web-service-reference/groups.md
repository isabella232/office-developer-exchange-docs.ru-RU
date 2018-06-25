---
title: Группы
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Groups
api_type:
- schema
ms.assetid: 6b6b2d67-219d-4dfb-a4ed-d627b1cfb33f
description: Элемент Groups содержит коллекцию групп, найденных с критерии поиска и объединение, который идентифицируется в запросе FindItem операции.
ms.openlocfilehash: 406a1974899e89243f52ba7a56afcc172c4f3df6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833786"
---
# <a name="groups"></a><span data-ttu-id="44678-103">Группы</span><span class="sxs-lookup"><span data-stu-id="44678-103">Groups</span></span>

<span data-ttu-id="44678-104">Элемент **Groups** содержит коллекцию групп, найденных с критерии поиска и объединение, который идентифицируется в запросе на [операции FindItem](finditem-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="44678-104">The **Groups** element contains a collection of groups that are found with the search and aggregation criteria that is identified in the [FindItem operation](finditem-operation.md) request.</span></span> 
  
```xml
<Groups>
   <GroupedItems/>
</Groups>
```

 <span data-ttu-id="44678-105">**ArrayOfGroupedItemsType**</span><span class="sxs-lookup"><span data-stu-id="44678-105">**ArrayOfGroupedItemsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="44678-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="44678-106">Attributes and elements</span></span>

<span data-ttu-id="44678-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="44678-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="44678-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="44678-108">Attributes</span></span>

<span data-ttu-id="44678-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="44678-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="44678-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="44678-110">Child elements</span></span>

|<span data-ttu-id="44678-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="44678-111">**Element**</span></span>|<span data-ttu-id="44678-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="44678-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="44678-113">GroupedItems</span><span class="sxs-lookup"><span data-stu-id="44678-113">GroupedItems</span></span>](groupeditems.md) <br/> |<span data-ttu-id="44678-114">Представляет коллекцию элементов, которые являются результатом сгруппированных [операции FindItem](finditem-operation.md) вызова.</span><span class="sxs-lookup"><span data-stu-id="44678-114">Represents a collection of items that are the result of a grouped [FindItem operation](finditem-operation.md) call.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="44678-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="44678-115">Parent elements</span></span>

|<span data-ttu-id="44678-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="44678-116">**Element**</span></span>|<span data-ttu-id="44678-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="44678-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="44678-118">RootFolder (FindItemResponseMessage)</span><span class="sxs-lookup"><span data-stu-id="44678-118">RootFolder (FindItemResponseMessage)</span></span>](rootfolder-finditemresponsemessage.md) <br/> |<span data-ttu-id="44678-119">Содержит результаты поиска в одной корневой папке во время [операции FindItem](finditem-operation.md) операции.</span><span class="sxs-lookup"><span data-stu-id="44678-119">Contains the results from a search of a single root folder during a [FindItem operation](finditem-operation.md) operation.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="44678-120">Замечания</span><span class="sxs-lookup"><span data-stu-id="44678-120">Remarks</span></span>

<span data-ttu-id="44678-121">Один экземпляр [GroupedItems](groupeditems.md) произойдет для каждую отдельную группу в результатах.</span><span class="sxs-lookup"><span data-stu-id="44678-121">One [GroupedItems](groupeditems.md) instance will occur for each distinct group within the result.</span></span> 
  
<span data-ttu-id="44678-122">Схема, описывающая этот элемент находится в виртуальном каталоге EWS компьютера, на котором выполняется Microsoft Exchange Server 2010 с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="44678-122">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="44678-123">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="44678-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="44678-124">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="44678-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="44678-125">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="44678-125">Schema name</span></span>  <br/> |<span data-ttu-id="44678-126">Схема Types</span><span class="sxs-lookup"><span data-stu-id="44678-126">Types schema</span></span>  <br/> |
|<span data-ttu-id="44678-127">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="44678-127">Validation file</span></span>  <br/> |<span data-ttu-id="44678-128">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="44678-128">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="44678-129">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="44678-129">Can be empty</span></span>  <br/> |<span data-ttu-id="44678-130">False</span><span class="sxs-lookup"><span data-stu-id="44678-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="44678-131">См. также</span><span class="sxs-lookup"><span data-stu-id="44678-131">See also</span></span>



[<span data-ttu-id="44678-132">FindItem Operation</span><span class="sxs-lookup"><span data-stu-id="44678-132">FindItem operation</span></span>](finditem-operation.md)


[<span data-ttu-id="44678-133">Поиск элементов</span><span class="sxs-lookup"><span data-stu-id="44678-133">Finding Items</span></span>](http://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)

