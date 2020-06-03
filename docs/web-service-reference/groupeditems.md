---
title: граупедитемс
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
description: Элемент Граупедитемс представляет коллекцию элементов, которые являются результатом вызова сгруппированной операции FindItem.
ms.openlocfilehash: 0ee1ca3c6d0cf98e2daefa60a1cb1fd096cda478
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530813"
---
# <a name="groupeditems"></a><span data-ttu-id="13a08-103">граупедитемс</span><span class="sxs-lookup"><span data-stu-id="13a08-103">GroupedItems</span></span>

<span data-ttu-id="13a08-104">Элемент **граупедитемс** представляет коллекцию элементов, которые являются результатом вызова сгруппированной [операции FindItem](finditem-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="13a08-104">The **GroupedItems** element represents a collection of items that are the result of a grouped [FindItem operation](finditem-operation.md) call.</span></span> 
  
[<span data-ttu-id="13a08-105">финдитемреспонсе</span><span class="sxs-lookup"><span data-stu-id="13a08-105">FindItemResponse</span></span>](finditemresponse.md)
  
[<span data-ttu-id="13a08-106">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="13a08-106">ResponseMessages</span></span>](responsemessages.md)
  
[<span data-ttu-id="13a08-107">финдитемреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="13a08-107">FindItemResponseMessage</span></span>](finditemresponsemessage.md)
  
[<span data-ttu-id="13a08-108">Рутфолдер (Финдитемреспонсемессаже)</span><span class="sxs-lookup"><span data-stu-id="13a08-108">RootFolder (FindItemResponseMessage)</span></span>](rootfolder-finditemresponsemessage.md)
  
[<span data-ttu-id="13a08-109">Groups</span><span class="sxs-lookup"><span data-stu-id="13a08-109">Groups</span></span>](groups.md)
  
[<span data-ttu-id="13a08-110">граупедитемс</span><span class="sxs-lookup"><span data-stu-id="13a08-110">GroupedItems</span></span>](groupeditems.md)
  
```xml
<GroupedItems>
   <GroupIndex/>
   <Items/>
</GroupedItems>
```

 <span data-ttu-id="13a08-111">**граупедитемстипе**</span><span class="sxs-lookup"><span data-stu-id="13a08-111">**GroupedItemsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="13a08-112">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="13a08-112">Attributes and elements</span></span>

<span data-ttu-id="13a08-113">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="13a08-113">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="13a08-114">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="13a08-114">Attributes</span></span>

<span data-ttu-id="13a08-115">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="13a08-115">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="13a08-116">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="13a08-116">Child elements</span></span>

|<span data-ttu-id="13a08-117">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="13a08-117">**Element**</span></span>|<span data-ttu-id="13a08-118">**Описание**</span><span class="sxs-lookup"><span data-stu-id="13a08-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="13a08-119">граупиндекс</span><span class="sxs-lookup"><span data-stu-id="13a08-119">GroupIndex</span></span>](groupindex.md) <br/> |<span data-ttu-id="13a08-120">Представляет значение свойства, используемое для группировки элементов в сгруппированном вызове [операции FindItem](finditem-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="13a08-120">Represents the property value that is used to group items in a grouped [FindItem operation](finditem-operation.md) call.</span></span>  <br/> |
|[<span data-ttu-id="13a08-121">Items</span><span class="sxs-lookup"><span data-stu-id="13a08-121">Items</span></span>](items.md) <br/> |<span data-ttu-id="13a08-122">Содержит массив сгруппированных элементов.</span><span class="sxs-lookup"><span data-stu-id="13a08-122">Contains an array of grouped items.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="13a08-123">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="13a08-123">Parent elements</span></span>

|<span data-ttu-id="13a08-124">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="13a08-124">**Element**</span></span>|<span data-ttu-id="13a08-125">**Описание**</span><span class="sxs-lookup"><span data-stu-id="13a08-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="13a08-126">Groups</span><span class="sxs-lookup"><span data-stu-id="13a08-126">Groups</span></span>](groups.md) <br/> |<span data-ttu-id="13a08-127">Содержит коллекцию групп, найденных с помощью критериев поиска и объединения, которые определены в запросе [операции FindItem](finditem-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="13a08-127">Contains a collection of groups that are found with the search and aggregation criteria that is identified in the [FindItem operation](finditem-operation.md) request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="13a08-128">Примечания</span><span class="sxs-lookup"><span data-stu-id="13a08-128">Remarks</span></span>

<span data-ttu-id="13a08-129">Схема, описывающая этот элемент, находится в виртуальном каталоге EWS компьютера под управлением Microsoft Exchange Server 2010, на котором установлена роль сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="13a08-129">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="13a08-130">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="13a08-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="13a08-131">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="13a08-131">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="13a08-132">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="13a08-132">Schema name</span></span>  <br/> |<span data-ttu-id="13a08-133">Схема Types</span><span class="sxs-lookup"><span data-stu-id="13a08-133">Types schema</span></span>  <br/> |
|<span data-ttu-id="13a08-134">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="13a08-134">Validation file</span></span>  <br/> |<span data-ttu-id="13a08-135">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="13a08-135">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="13a08-136">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="13a08-136">Can be empty</span></span>  <br/> |<span data-ttu-id="13a08-137">False</span><span class="sxs-lookup"><span data-stu-id="13a08-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="13a08-138">См. также</span><span class="sxs-lookup"><span data-stu-id="13a08-138">See also</span></span>



[<span data-ttu-id="13a08-139">Операция FindItem</span><span class="sxs-lookup"><span data-stu-id="13a08-139">FindItem operation</span></span>](finditem-operation.md)


[<span data-ttu-id="13a08-140">Поиск элементов</span><span class="sxs-lookup"><span data-stu-id="13a08-140">Finding Items</span></span>](https://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)

