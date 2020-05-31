---
title: дистингуишедграупби
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DistinguishedGroupBy
api_type:
- schema
ms.assetid: 6ff3ac48-02ba-40ec-a71b-c401bb2b127c
description: Элемент Дистингуишедграупби предоставляет стандартные группирования для запросов FindItem.
ms.openlocfilehash: 0635366447675bf28dedf3af4f7d76094ee5e0a4
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762187"
---
# <a name="distinguishedgroupby"></a><span data-ttu-id="f4616-103">дистингуишедграупби</span><span class="sxs-lookup"><span data-stu-id="f4616-103">DistinguishedGroupBy</span></span>

<span data-ttu-id="f4616-104">Элемент **дистингуишедграупби** предоставляет стандартные группирования для запросов FindItem.</span><span class="sxs-lookup"><span data-stu-id="f4616-104">The **DistinguishedGroupBy** element provides standard groupings for FindItem queries.</span></span> 
  
- [<span data-ttu-id="f4616-105">FindItem</span><span class="sxs-lookup"><span data-stu-id="f4616-105">FindItem</span></span>](finditem.md) 
- [<span data-ttu-id="f4616-106">дистингуишедграупби</span><span class="sxs-lookup"><span data-stu-id="f4616-106">DistinguishedGroupBy</span></span>](distinguishedgroupby.md)
  
```xml
<DistinguishedGroupBy>
   <StandardGroupBy/>
</DistinguishedGroupBy>
```

 <span data-ttu-id="f4616-107">**дистингуишедграупбитипе**</span><span class="sxs-lookup"><span data-stu-id="f4616-107">**DistinguishedGroupByType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f4616-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="f4616-108">Attributes and elements</span></span>

<span data-ttu-id="f4616-109">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="f4616-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f4616-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="f4616-110">Attributes</span></span>

<span data-ttu-id="f4616-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="f4616-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f4616-112">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="f4616-112">Child elements</span></span>

|<span data-ttu-id="f4616-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="f4616-113">**Element**</span></span>|<span data-ttu-id="f4616-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="f4616-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f4616-115">стандардграупби</span><span class="sxs-lookup"><span data-stu-id="f4616-115">StandardGroupBy</span></span>](standardgroupby.md) <br/> |<span data-ttu-id="f4616-116">Представляет стандартные механизмы группирования и агрегирования для операции сгруппированной операции FindItem.</span><span class="sxs-lookup"><span data-stu-id="f4616-116">Represents the standard grouping and aggregating mechanisms for a grouped FindItem operation.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f4616-117">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="f4616-117">Parent elements</span></span>

|<span data-ttu-id="f4616-118">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="f4616-118">**Element**</span></span>|<span data-ttu-id="f4616-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="f4616-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f4616-120">FindItem</span><span class="sxs-lookup"><span data-stu-id="f4616-120">FindItem</span></span>](finditem.md) <br/> |<span data-ttu-id="f4616-121">Определяет запрос на поиск элементов в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="f4616-121">Defines a request to find items in a mailbox.</span></span><br/><br/><span data-ttu-id="f4616-122">Ниже приведено выражение XPath для этого элемента:`/FindItem`</span><span class="sxs-lookup"><span data-stu-id="f4616-122">The following is the XPath expression to this element:  `/FindItem`</span></span> <br/> |
   
## <a name="remarks"></a><span data-ttu-id="f4616-123">Примечания</span><span class="sxs-lookup"><span data-stu-id="f4616-123">Remarks</span></span>

<span data-ttu-id="f4616-124">Элемент **дистингуишедграупби** можно добавить в операцию FindItem при условии, что результаты должны быть сгруппированы, а одна из стандартных групп соответствует требованиям к группированию.</span><span class="sxs-lookup"><span data-stu-id="f4616-124">The **DistinguishedGroupBy** element can be added to a FindItem operation when the results must come backed grouped and when one of the standard groups meets the grouping requirements.</span></span> <span data-ttu-id="f4616-125">Если не указан ни элемент **дистингуишедграупби** , ни элемент [GroupBy](groupby.md) , результаты FindItem будут отходиться на несгруппированные результаты.</span><span class="sxs-lookup"><span data-stu-id="f4616-125">If neither the **DistinguishedGroupBy** element nor the [GroupBy](groupby.md) element is specified, FindItem results will come back ungrouped.</span></span> 
  
<span data-ttu-id="f4616-126">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="f4616-126">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f4616-127">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="f4616-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f4616-128">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="f4616-128">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="f4616-129">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="f4616-129">Schema Name</span></span>  <br/> |<span data-ttu-id="f4616-130">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="f4616-130">Messages schema</span></span>  <br/> |
|<span data-ttu-id="f4616-131">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="f4616-131">Validation File</span></span>  <br/> |<span data-ttu-id="f4616-132">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="f4616-132">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="f4616-133">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="f4616-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="f4616-134">False</span><span class="sxs-lookup"><span data-stu-id="f4616-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f4616-135">См. также</span><span class="sxs-lookup"><span data-stu-id="f4616-135">See also</span></span>

- [<span data-ttu-id="f4616-136">Операция FindItem</span><span class="sxs-lookup"><span data-stu-id="f4616-136">FindItem operation</span></span>](finditem-operation.md)
- [<span data-ttu-id="f4616-137">Поиск элементов</span><span class="sxs-lookup"><span data-stu-id="f4616-137">Finding Items</span></span>](http://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)

