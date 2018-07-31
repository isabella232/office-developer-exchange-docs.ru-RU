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
ms.openlocfilehash: 320a7b821cc593e7dd60a8f8adb23bcd600f71f8
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/28/2018
ms.locfileid: "21353303"
---
# <a name="fieldorder"></a><span data-ttu-id="e2d27-103">FieldOrder</span><span class="sxs-lookup"><span data-stu-id="e2d27-103">FieldOrder</span></span>

<span data-ttu-id="e2d27-104">Элемент **FieldOrder** представляет одно поле, по которому будут отсортированы результаты и задает направление сортировки.</span><span class="sxs-lookup"><span data-stu-id="e2d27-104">The **FieldOrder** element represents a single field by which to sort results and indicates the direction for the sort.</span></span> 
  
```xml
<FieldOrder Order="">
   <FieldURI/>
</FieldOrder>
```

```xml
<FieldOrder Order="">
   <ExtendedFieldURI/> 
</FieldOrder>
```

```xml
<FieldOrder Order="">
   <IndexedFieldURI/>
</FieldOrder>
```

<span data-ttu-id="e2d27-105">**FieldOrderType**</span><span class="sxs-lookup"><span data-stu-id="e2d27-105">**FieldOrderType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="e2d27-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="e2d27-106">Attributes and elements</span></span>

<span data-ttu-id="e2d27-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="e2d27-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e2d27-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="e2d27-108">Attributes</span></span>

|<span data-ttu-id="e2d27-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="e2d27-109">**Attribute**</span></span>|<span data-ttu-id="e2d27-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="e2d27-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="e2d27-111">**Порядок**</span><span class="sxs-lookup"><span data-stu-id="e2d27-111">**Order**</span></span> <br/> | <span data-ttu-id="e2d27-112">Описывает направление сортировки.</span><span class="sxs-lookup"><span data-stu-id="e2d27-112">Describes the sort order direction.</span></span><br/><br/> <span data-ttu-id="e2d27-113">Ниже перечислены возможные значения.</span><span class="sxs-lookup"><span data-stu-id="e2d27-113">The following are the possible values:</span></span> <br/> <br/><span data-ttu-id="e2d27-114">-По возрастанию</span><span class="sxs-lookup"><span data-stu-id="e2d27-114">-  Ascending</span></span>  <br/><span data-ttu-id="e2d27-115">— По убыванию</span><span class="sxs-lookup"><span data-stu-id="e2d27-115">-  Descending</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="e2d27-116">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="e2d27-116">Child elements</span></span>

|<span data-ttu-id="e2d27-117">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="e2d27-117">**Element**</span></span>|<span data-ttu-id="e2d27-118">**Описание**</span><span class="sxs-lookup"><span data-stu-id="e2d27-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e2d27-119">FieldURI</span><span class="sxs-lookup"><span data-stu-id="e2d27-119">FieldURI</span></span>](fielduri.md) <br/> |<span data-ttu-id="e2d27-120">Идентифицирует часто упоминаемые свойства по URI.</span><span class="sxs-lookup"><span data-stu-id="e2d27-120">Identifies frequently referenced properties by URI.</span></span>  <br/> |
|[<span data-ttu-id="e2d27-121">IndexedFieldURI</span><span class="sxs-lookup"><span data-stu-id="e2d27-121">IndexedFieldURI</span></span>](indexedfielduri.md) <br/> |<span data-ttu-id="e2d27-122">Идентифицирует отдельных элементов словаря.</span><span class="sxs-lookup"><span data-stu-id="e2d27-122">Identifies individual members of a dictionary.</span></span>  <br/> |
|[<span data-ttu-id="e2d27-123">ExtendedFieldURI</span><span class="sxs-lookup"><span data-stu-id="e2d27-123">ExtendedFieldURI</span></span>](extendedfielduri.md) <br/> |<span data-ttu-id="e2d27-124">Задает свойства MAPI.</span><span class="sxs-lookup"><span data-stu-id="e2d27-124">Identifies MAPI properties.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="e2d27-125">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="e2d27-125">Parent elements</span></span>

|<span data-ttu-id="e2d27-126">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="e2d27-126">**Element**</span></span>|<span data-ttu-id="e2d27-127">**Описание**</span><span class="sxs-lookup"><span data-stu-id="e2d27-127">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e2d27-128">SortOrder</span><span class="sxs-lookup"><span data-stu-id="e2d27-128">SortOrder</span></span>](sortorder.md) <br/> |<span data-ttu-id="e2d27-129">Определяет способ сортировки в запросе FindItem элементов.</span><span class="sxs-lookup"><span data-stu-id="e2d27-129">Defines how items are sorted in a FindItem request.</span></span>  <br/> <span data-ttu-id="e2d27-130">Ниже приведен выражение XPath для этого элемента.`/FindItem/SortOrder`</span><span class="sxs-lookup"><span data-stu-id="e2d27-130">The following is the XPath expression to this element:  `/FindItem/SortOrder`</span></span> <br/> |
   
## <a name="remarks"></a><span data-ttu-id="e2d27-131">Замечания</span><span class="sxs-lookup"><span data-stu-id="e2d27-131">Remarks</span></span>

<span data-ttu-id="e2d27-132">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="e2d27-132">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e2d27-133">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="e2d27-133">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e2d27-134">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="e2d27-134">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="e2d27-135">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="e2d27-135">Schema Name</span></span>  <br/> |<span data-ttu-id="e2d27-136">Схема Types</span><span class="sxs-lookup"><span data-stu-id="e2d27-136">Types schema</span></span>  <br/> |
|<span data-ttu-id="e2d27-137">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="e2d27-137">Validation File</span></span>  <br/> |<span data-ttu-id="e2d27-138">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="e2d27-138">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="e2d27-139">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="e2d27-139">Can be Empty</span></span>  <br/> |<span data-ttu-id="e2d27-140">False</span><span class="sxs-lookup"><span data-stu-id="e2d27-140">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e2d27-141">См. также</span><span class="sxs-lookup"><span data-stu-id="e2d27-141">See also</span></span>

- [<span data-ttu-id="e2d27-142">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="e2d27-142">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

