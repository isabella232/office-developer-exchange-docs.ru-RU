---
title: OccurrenceItemId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- OccurrenceItemId
api_type:
- schema
ms.assetid: 4a15bbc3-5b93-4193-b9ec-da32f0a9a552
description: Элемент OccurrenceItemId определяет одно вхождение повторяющегося элемента.
ms.openlocfilehash: e3d7b6efc49775f54219ce0dc0ec39a34a95f8fd
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834639"
---
# <a name="occurrenceitemid"></a><span data-ttu-id="bba6a-103">OccurrenceItemId</span><span class="sxs-lookup"><span data-stu-id="bba6a-103">OccurrenceItemId</span></span>

<span data-ttu-id="bba6a-104">Элемент **OccurrenceItemId** определяет одно вхождение повторяющегося элемента.</span><span class="sxs-lookup"><span data-stu-id="bba6a-104">The **OccurrenceItemId** element identifies a single occurrence of a recurring item.</span></span> 
  
```XML
<OccurrenceItemId RecurringMasterId="" ChangeKey="" InstanceIndex=""/>
```

<span data-ttu-id="bba6a-105">**OccurrenceItemIdType**</span><span class="sxs-lookup"><span data-stu-id="bba6a-105">**OccurrenceItemIdType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="bba6a-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="bba6a-106">Attributes and elements</span></span>

<span data-ttu-id="bba6a-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="bba6a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="bba6a-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="bba6a-108">Attributes</span></span>

|<span data-ttu-id="bba6a-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="bba6a-109">**Attribute**</span></span>|<span data-ttu-id="bba6a-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="bba6a-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="bba6a-111">**RecurringMasterId**</span><span class="sxs-lookup"><span data-stu-id="bba6a-111">**RecurringMasterId**</span></span> <br/> |<span data-ttu-id="bba6a-112">Определяет повторяющиеся главных повторяющегося элемента.</span><span class="sxs-lookup"><span data-stu-id="bba6a-112">Identifies the recurring master of a recurring item.</span></span> <span data-ttu-id="bba6a-113">Этот атрибут является обязательным.</span><span class="sxs-lookup"><span data-stu-id="bba6a-113">This attribute is required.</span></span>  <br/> |
|<span data-ttu-id="bba6a-114">**ChangeKey**</span><span class="sxs-lookup"><span data-stu-id="bba6a-114">**ChangeKey**</span></span> <br/> |<span data-ttu-id="bba6a-115">Идентифицирует определенной версии образца повторения или вхождения элемента.</span><span class="sxs-lookup"><span data-stu-id="bba6a-115">Identifies a specific version of the recurring master or an item occurrence.</span></span> <span data-ttu-id="bba6a-116">Если изменить хозяином повторяющиеся или любой из его вхождения, изменяется **ChangeKey** .</span><span class="sxs-lookup"><span data-stu-id="bba6a-116">If either the recurring master or any of its occurrences change, the **ChangeKey** changes.</span></span> <span data-ttu-id="bba6a-117">**ChangeKey** подходит и для повторяющихся master и все вхождения.</span><span class="sxs-lookup"><span data-stu-id="bba6a-117">The **ChangeKey** is the same for the recurring master and all occurrences.</span></span>  <br/> |
|<span data-ttu-id="bba6a-118">**InstanceIndex**</span><span class="sxs-lookup"><span data-stu-id="bba6a-118">**InstanceIndex**</span></span> <br/> |<span data-ttu-id="bba6a-119">Определяет индекс экземпляра элемента.</span><span class="sxs-lookup"><span data-stu-id="bba6a-119">Identifies the index of the item occurrence.</span></span> <span data-ttu-id="bba6a-120">Этот атрибут является обязательным.</span><span class="sxs-lookup"><span data-stu-id="bba6a-120">This attribute is required.</span></span> <span data-ttu-id="bba6a-121">Это значение представляет собой целое число.</span><span class="sxs-lookup"><span data-stu-id="bba6a-121">This value represents an integer.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="bba6a-122">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="bba6a-122">Child elements</span></span>

<span data-ttu-id="bba6a-123">Нет.</span><span class="sxs-lookup"><span data-stu-id="bba6a-123">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="bba6a-124">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="bba6a-124">Parent elements</span></span>

|<span data-ttu-id="bba6a-125">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="bba6a-125">**Element**</span></span>|<span data-ttu-id="bba6a-126">**Описание**</span><span class="sxs-lookup"><span data-stu-id="bba6a-126">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bba6a-127">GlobalItemIds</span><span class="sxs-lookup"><span data-stu-id="bba6a-127">GlobalItemIds</span></span>](globalitemids.md) <br/> |<span data-ttu-id="bba6a-128">Содержит коллекцию идентификаторов элементов для всех элементов беседы в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="bba6a-128">Contains the collection of item identifiers for all conversation items in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="bba6a-129">Что ItemID</span><span class="sxs-lookup"><span data-stu-id="bba6a-129">ItemIds</span></span>](itemids.md) <br/> | <span data-ttu-id="bba6a-130">Содержит уникальные идентификаторы элементов, элементы вхождений и повторяющиеся основные элементы, используемые для удаления, отправка, получение, перемещение и копирование элементов в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="bba6a-130">Contains the unique identities of items, occurrence items, and recurring master items that are used to delete, send, get, move, or copy items in the Exchange store.</span></span> <br/><br/><span data-ttu-id="bba6a-131">Ниже приведены выражения XPath для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="bba6a-131">The following are the XPath expressions to this element:</span></span> <br/><br/>  `/DeleteItem/ItemIds` <br/>  `/SendItem/ItemIds` <br/>  `/GetItem/ItemIds` <br/><br/><span data-ttu-id="bba6a-132">**Примечание**: [операция MoveItem](moveitem-operation.md) и [операции CopyItem](copyitem-operation.md) возможен только с элементами одного календаря и повторяющиеся основные элементы.</span><span class="sxs-lookup"><span data-stu-id="bba6a-132">**Note**:  [MoveItem operation](moveitem-operation.md) and [CopyItem operation](copyitem-operation.md) only work with single calendar items and recurring master items.</span></span> <span data-ttu-id="bba6a-133">Недопустимые вхождения элемента с помощью этих операций.</span><span class="sxs-lookup"><span data-stu-id="bba6a-133">Item occurrences are invalid with these operations.</span></span>           |
|[<span data-ttu-id="bba6a-134">ItemChange</span><span class="sxs-lookup"><span data-stu-id="bba6a-134">ItemChange</span></span>](itemchange.md) <br/> |<span data-ttu-id="bba6a-135">Содержит идентификатор элемента и обновления для применения к элементу.</span><span class="sxs-lookup"><span data-stu-id="bba6a-135">Contains an item identifier and the updates to apply to the item.</span></span><br/><br/> <span data-ttu-id="bba6a-136">Ниже приведен выражение XPath для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="bba6a-136">The following is the XPath expression to this element:</span></span>  <br/>  `/UpdateItem/ItemChanges/ItemChange[i]` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="bba6a-137">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="bba6a-137">Text value</span></span>

<span data-ttu-id="bba6a-138">Нет.</span><span class="sxs-lookup"><span data-stu-id="bba6a-138">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="bba6a-139">Замечания</span><span class="sxs-lookup"><span data-stu-id="bba6a-139">Remarks</span></span>

<span data-ttu-id="bba6a-140">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="bba6a-140">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="example"></a><span data-ttu-id="bba6a-141">Пример</span><span class="sxs-lookup"><span data-stu-id="bba6a-141">Example</span></span>

<span data-ttu-id="bba6a-142">Следующий пример определяет четвертый вхождение повторяющегося элемента, который имеет 34vswe4 удостоверений.</span><span class="sxs-lookup"><span data-stu-id="bba6a-142">The following example identifies the fourth occurrence of a recurring item that has the identity 34vswe4.</span></span>
  
```XML
<OccurrenceItemId RecurringMasterId="34vswe4" InstanceIndex="4" />
```

## <a name="element-information"></a><span data-ttu-id="bba6a-143">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="bba6a-143">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="bba6a-144">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="bba6a-144">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="bba6a-145">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="bba6a-145">Schema Name</span></span>  <br/> |<span data-ttu-id="bba6a-146">Схема Types</span><span class="sxs-lookup"><span data-stu-id="bba6a-146">Types schema</span></span>  <br/> |
|<span data-ttu-id="bba6a-147">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="bba6a-147">Validation File</span></span>  <br/> |<span data-ttu-id="bba6a-148">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="bba6a-148">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="bba6a-149">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="bba6a-149">Can be Empty</span></span>  <br/> |<span data-ttu-id="bba6a-150">False</span><span class="sxs-lookup"><span data-stu-id="bba6a-150">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="bba6a-151">См. также</span><span class="sxs-lookup"><span data-stu-id="bba6a-151">See also</span></span>

- [<span data-ttu-id="bba6a-152">RecurringMasterItemId</span><span class="sxs-lookup"><span data-stu-id="bba6a-152">RecurringMasterItemId</span></span>](recurringmasteritemid.md)
- [<span data-ttu-id="bba6a-153">FindConversation Operation</span><span class="sxs-lookup"><span data-stu-id="bba6a-153">FindConversation operation</span></span>](findconversation-operation.md)
- [<span data-ttu-id="bba6a-154">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="bba6a-154">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

