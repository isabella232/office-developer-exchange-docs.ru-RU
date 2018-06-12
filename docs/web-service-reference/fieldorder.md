---
title: FieldOrder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FieldOrder
api_type:
- schema
ms.assetid: b9364842-bbe2-4221-afef-bf5022bc89ec
description: Элемент FieldOrder представляет одно поле, по которому будут отсортированы результаты и задает направление сортировки.
ms.openlocfilehash: 10e28f066f7fa6799bf6b03b694d98825f95626d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762529"
---
# <a name="fieldorder"></a><span data-ttu-id="c05df-103">FieldOrder</span><span class="sxs-lookup"><span data-stu-id="c05df-103">FieldOrder</span></span>

<span data-ttu-id="c05df-104">Элемент **FieldOrder** представляет одно поле, по которому будут отсортированы результаты и задает направление сортировки.</span><span class="sxs-lookup"><span data-stu-id="c05df-104">The **FieldOrder** element represents a single field by which to sort results and indicates the direction for the sort.</span></span> 
  
```xml
<FieldOrder Order="">
   <FieldURI/>
</FieldOrder>
```

 <span data-ttu-id="c05df-105">**FieldOrderType**</span><span class="sxs-lookup"><span data-stu-id="c05df-105">**FieldOrderType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c05df-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="c05df-106">Attributes and elements</span></span>

<span data-ttu-id="c05df-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="c05df-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c05df-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="c05df-108">Attributes</span></span>

|<span data-ttu-id="c05df-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="c05df-109">**Attribute**</span></span>|<span data-ttu-id="c05df-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="c05df-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="c05df-111">**Порядок**</span><span class="sxs-lookup"><span data-stu-id="c05df-111">**Order**</span></span> <br/> | <span data-ttu-id="c05df-112">Описывает направление сортировки.</span><span class="sxs-lookup"><span data-stu-id="c05df-112">Describes the sort order direction.</span></span><br/><br/> <span data-ttu-id="c05df-113">Ниже перечислены возможные значения.</span><span class="sxs-lookup"><span data-stu-id="c05df-113">The following are the possible values:</span></span> <br/> <br/><span data-ttu-id="c05df-114">-По возрастанию</span><span class="sxs-lookup"><span data-stu-id="c05df-114">-  Ascending</span></span>  <br/><span data-ttu-id="c05df-115">— По убыванию</span><span class="sxs-lookup"><span data-stu-id="c05df-115">-  Descending</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="c05df-116">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="c05df-116">Child elements</span></span>

|<span data-ttu-id="c05df-117">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="c05df-117">**Element**</span></span>|<span data-ttu-id="c05df-118">**Описание**</span><span class="sxs-lookup"><span data-stu-id="c05df-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c05df-119">FieldURI</span><span class="sxs-lookup"><span data-stu-id="c05df-119">FieldURI</span></span>](fielduri.md) <br/> |<span data-ttu-id="c05df-120">Идентифицирует часто упоминаемые свойства по URI.</span><span class="sxs-lookup"><span data-stu-id="c05df-120">Identifies frequently referenced properties by URI.</span></span>  <br/> |
|[<span data-ttu-id="c05df-121">IndexedFieldURI</span><span class="sxs-lookup"><span data-stu-id="c05df-121">IndexedFieldURI</span></span>](indexedfielduri.md) <br/> |<span data-ttu-id="c05df-122">Идентифицирует отдельных элементов словаря.</span><span class="sxs-lookup"><span data-stu-id="c05df-122">Identifies individual members of a dictionary.</span></span>  <br/> |
|[<span data-ttu-id="c05df-123">ExtendedFieldURI</span><span class="sxs-lookup"><span data-stu-id="c05df-123">ExtendedFieldURI</span></span>](extendedfielduri.md) <br/> |<span data-ttu-id="c05df-124">Задает свойства MAPI.</span><span class="sxs-lookup"><span data-stu-id="c05df-124">Identifies MAPI properties.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="c05df-125">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="c05df-125">Parent elements</span></span>

|<span data-ttu-id="c05df-126">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="c05df-126">**Element**</span></span>|<span data-ttu-id="c05df-127">**Описание**</span><span class="sxs-lookup"><span data-stu-id="c05df-127">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c05df-128">SortOrder</span><span class="sxs-lookup"><span data-stu-id="c05df-128">SortOrder</span></span>](sortorder.md) <br/> |<span data-ttu-id="c05df-129">Определяет способ сортировки в запросе FindItem элементов.</span><span class="sxs-lookup"><span data-stu-id="c05df-129">Defines how items are sorted in a FindItem request.</span></span>  <br/> <span data-ttu-id="c05df-130">Ниже приведен выражение XPath для этого элемента.`/FindItem/SortOrder`</span><span class="sxs-lookup"><span data-stu-id="c05df-130">The following is the XPath expression to this element:  `/FindItem/SortOrder`</span></span> <br/> |
   
## <a name="remarks"></a><span data-ttu-id="c05df-131">Замечания</span><span class="sxs-lookup"><span data-stu-id="c05df-131">Remarks</span></span>

<span data-ttu-id="c05df-132">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="c05df-132">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c05df-133">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="c05df-133">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c05df-134">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="c05df-134">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="c05df-135">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="c05df-135">Schema Name</span></span>  <br/> |<span data-ttu-id="c05df-136">Схема Types</span><span class="sxs-lookup"><span data-stu-id="c05df-136">Types schema</span></span>  <br/> |
|<span data-ttu-id="c05df-137">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="c05df-137">Validation File</span></span>  <br/> |<span data-ttu-id="c05df-138">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="c05df-138">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="c05df-139">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="c05df-139">Can be Empty</span></span>  <br/> |<span data-ttu-id="c05df-140">False</span><span class="sxs-lookup"><span data-stu-id="c05df-140">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c05df-141">См. также</span><span class="sxs-lookup"><span data-stu-id="c05df-141">See also</span></span>

- [<span data-ttu-id="c05df-142">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="c05df-142">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

