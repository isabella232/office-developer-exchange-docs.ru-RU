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
description: Элемент Groups содержит коллекцию групп, которые обнаружены с помощью критериев поиска и объединения, которые определены в запросе операции FindItem.
ms.openlocfilehash: 915d9dffd6d8cec1def6634e6b70642d563b5242
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530791"
---
# <a name="groups"></a><span data-ttu-id="388ee-103">Группы</span><span class="sxs-lookup"><span data-stu-id="388ee-103">Groups</span></span>

<span data-ttu-id="388ee-104">Элемент **Groups** содержит коллекцию групп, которые обнаружены с помощью критериев поиска и объединения, которые определены в запросе [операции FindItem](finditem-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="388ee-104">The **Groups** element contains a collection of groups that are found with the search and aggregation criteria that is identified in the [FindItem operation](finditem-operation.md) request.</span></span> 
  
```xml
<Groups>
   <GroupedItems/>
</Groups>
```

 <span data-ttu-id="388ee-105">**аррайофграупедитемстипе**</span><span class="sxs-lookup"><span data-stu-id="388ee-105">**ArrayOfGroupedItemsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="388ee-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="388ee-106">Attributes and elements</span></span>

<span data-ttu-id="388ee-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="388ee-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="388ee-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="388ee-108">Attributes</span></span>

<span data-ttu-id="388ee-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="388ee-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="388ee-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="388ee-110">Child elements</span></span>

|<span data-ttu-id="388ee-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="388ee-111">**Element**</span></span>|<span data-ttu-id="388ee-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="388ee-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="388ee-113">граупедитемс</span><span class="sxs-lookup"><span data-stu-id="388ee-113">GroupedItems</span></span>](groupeditems.md) <br/> |<span data-ttu-id="388ee-114">Представляет коллекцию элементов, которая является результатом сгруппированного вызова [операции FindItem](finditem-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="388ee-114">Represents a collection of items that are the result of a grouped [FindItem operation](finditem-operation.md) call.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="388ee-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="388ee-115">Parent elements</span></span>

|<span data-ttu-id="388ee-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="388ee-116">**Element**</span></span>|<span data-ttu-id="388ee-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="388ee-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="388ee-118">Рутфолдер (Финдитемреспонсемессаже)</span><span class="sxs-lookup"><span data-stu-id="388ee-118">RootFolder (FindItemResponseMessage)</span></span>](rootfolder-finditemresponsemessage.md) <br/> |<span data-ttu-id="388ee-119">Содержит результаты поиска в одной корневой папке во время операции [FindItem](finditem-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="388ee-119">Contains the results from a search of a single root folder during a [FindItem operation](finditem-operation.md) operation.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="388ee-120">Примечания</span><span class="sxs-lookup"><span data-stu-id="388ee-120">Remarks</span></span>

<span data-ttu-id="388ee-121">Один экземпляр [граупедитемс](groupeditems.md) будет выполняться для каждой отдельной группы в результате.</span><span class="sxs-lookup"><span data-stu-id="388ee-121">One [GroupedItems](groupeditems.md) instance will occur for each distinct group within the result.</span></span> 
  
<span data-ttu-id="388ee-122">Схема, описывающая этот элемент, находится в виртуальном каталоге EWS компьютера под управлением Microsoft Exchange Server 2010, на котором установлена роль сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="388ee-122">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="388ee-123">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="388ee-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="388ee-124">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="388ee-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="388ee-125">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="388ee-125">Schema name</span></span>  <br/> |<span data-ttu-id="388ee-126">Схема Types</span><span class="sxs-lookup"><span data-stu-id="388ee-126">Types schema</span></span>  <br/> |
|<span data-ttu-id="388ee-127">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="388ee-127">Validation file</span></span>  <br/> |<span data-ttu-id="388ee-128">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="388ee-128">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="388ee-129">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="388ee-129">Can be empty</span></span>  <br/> |<span data-ttu-id="388ee-130">False</span><span class="sxs-lookup"><span data-stu-id="388ee-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="388ee-131">См. также</span><span class="sxs-lookup"><span data-stu-id="388ee-131">See also</span></span>



[<span data-ttu-id="388ee-132">Операция FindItem</span><span class="sxs-lookup"><span data-stu-id="388ee-132">FindItem operation</span></span>](finditem-operation.md)


[<span data-ttu-id="388ee-133">Поиск элементов</span><span class="sxs-lookup"><span data-stu-id="388ee-133">Finding Items</span></span>](https://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)

