---
title: ItemChange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ItemChange
api_type:
- schema
ms.assetid: 5cb43b02-d444-4d9c-9075-cdc5a4427daf
description: Элемент ItemChange содержит идентификатор элемента и обновления, чтобы применить к элементу.
ms.openlocfilehash: 42484c8deecb106e05023215342af3c7d996d852
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/28/2018
ms.locfileid: "21353513"
---
# <a name="itemchange"></a><span data-ttu-id="aad5c-103">ItemChange</span><span class="sxs-lookup"><span data-stu-id="aad5c-103">ItemChange</span></span>

<span data-ttu-id="aad5c-104">Элемент **ItemChange** содержит идентификатор элемента и обновления, чтобы применить к элементу.</span><span class="sxs-lookup"><span data-stu-id="aad5c-104">The **ItemChange** element contains an item identifier and the updates to apply to the item.</span></span> 
  
- [<span data-ttu-id="aad5c-105">UpdateItem</span><span class="sxs-lookup"><span data-stu-id="aad5c-105">UpdateItem</span></span>](updateitem.md) 
- [<span data-ttu-id="aad5c-106">ItemChanges</span><span class="sxs-lookup"><span data-stu-id="aad5c-106">ItemChanges</span></span>](itemchanges.md)
- [<span data-ttu-id="aad5c-107">ItemChange</span><span class="sxs-lookup"><span data-stu-id="aad5c-107">ItemChange</span></span>](itemchange.md)
  
```xml
<ItemChange>
   <ItemId/>
   <Updates>...</Updates>
</ItemChange>
```

```xml
<ItemChange>
   <OccurrenceItemId>...</OccurrenceItemId>
   <Updates>...</Updates>
</ItemChange>
```

```xml
<ItemChange>
   <RecurringMasterItemId>...</RecurringMasterItemId>
   <Updates>...</Updates>
</ItemChange>
```

<span data-ttu-id="aad5c-108">**ItemChangeType**</span><span class="sxs-lookup"><span data-stu-id="aad5c-108">**ItemChangeType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="aad5c-109">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="aad5c-109">Attributes and elements</span></span>

<span data-ttu-id="aad5c-110">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="aad5c-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="aad5c-111">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="aad5c-111">Attributes</span></span>

<span data-ttu-id="aad5c-112">Нет.</span><span class="sxs-lookup"><span data-stu-id="aad5c-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="aad5c-113">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="aad5c-113">Child elements</span></span>

|<span data-ttu-id="aad5c-114">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="aad5c-114">**Element**</span></span>|<span data-ttu-id="aad5c-115">**Описание**</span><span class="sxs-lookup"><span data-stu-id="aad5c-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="aad5c-116">Идентификатор элемента</span><span class="sxs-lookup"><span data-stu-id="aad5c-116">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="aad5c-117">Содержит уникальный идентификатор и меняет ключ элемента в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="aad5c-117">Contains the unique identifier and change key of an item in the Exchange store.</span></span> <span data-ttu-id="aad5c-118">Этот элемент является обязательным, если элемент [OccurrenceItemId](occurrenceitemid.md) или [RecurringMasterItemId](recurringmasteritemid.md) не используется.</span><span class="sxs-lookup"><span data-stu-id="aad5c-118">This element is required if the [OccurrenceItemId](occurrenceitemid.md) or [RecurringMasterItemId](recurringmasteritemid.md) element is not used.</span></span>  <br/> |
|[<span data-ttu-id="aad5c-119">OccurrenceItemId</span><span class="sxs-lookup"><span data-stu-id="aad5c-119">OccurrenceItemId</span></span>](occurrenceitemid.md) <br/> |<span data-ttu-id="aad5c-120">Определяет одно вхождение повторяющегося элемента.</span><span class="sxs-lookup"><span data-stu-id="aad5c-120">Identifies a single occurrence of a recurring item.</span></span> <span data-ttu-id="aad5c-121">Этот элемент является обязательным, если используется.</span><span class="sxs-lookup"><span data-stu-id="aad5c-121">This element is required if used.</span></span> <span data-ttu-id="aad5c-122">Этот элемент является обязательным, если элемент [RecurringMasterItemId](recurringmasteritemid.md) или [ItemId](itemid.md) не используется.</span><span class="sxs-lookup"><span data-stu-id="aad5c-122">This element is required if the [RecurringMasterItemId](recurringmasteritemid.md) or [ItemId](itemid.md) element is not used.</span></span>  <br/> |
|[<span data-ttu-id="aad5c-123">RecurringMasterItemId</span><span class="sxs-lookup"><span data-stu-id="aad5c-123">RecurringMasterItemId</span></span>](recurringmasteritemid.md) <br/> |<span data-ttu-id="aad5c-124">Идентифицирует элемент шаблона повторения, указав один из его появления связанные элементы идентификаторов.</span><span class="sxs-lookup"><span data-stu-id="aad5c-124">Identifies a recurrence master item by identifying one of its related occurrence items' identifiers.</span></span> <span data-ttu-id="aad5c-125">Этот элемент является обязательным, если используется.</span><span class="sxs-lookup"><span data-stu-id="aad5c-125">This element is required if used.</span></span> <span data-ttu-id="aad5c-126">Этот элемент является обязательным, если элемент [OccurrenceItemId](occurrenceitemid.md) или [ItemId](itemid.md) не используется.</span><span class="sxs-lookup"><span data-stu-id="aad5c-126">This element is required if the [OccurrenceItemId](occurrenceitemid.md) or [ItemId](itemid.md) element is not used.</span></span>  <br/> |
|[<span data-ttu-id="aad5c-127">Updates (Item)</span><span class="sxs-lookup"><span data-stu-id="aad5c-127">Updates (Item)</span></span>](updates-item.md) <br/> |<span data-ttu-id="aad5c-128">Содержит массив, определяющий добавьте, Установка и удаление изменения свойств элемента.</span><span class="sxs-lookup"><span data-stu-id="aad5c-128">Contains an array that defines append, set, and delete changes to item properties.</span></span> <span data-ttu-id="aad5c-129">Этот элемент обязательный.</span><span class="sxs-lookup"><span data-stu-id="aad5c-129">This element is required.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="aad5c-130">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="aad5c-130">Parent elements</span></span>

|<span data-ttu-id="aad5c-131">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="aad5c-131">**Element**</span></span>|<span data-ttu-id="aad5c-132">**Описание**</span><span class="sxs-lookup"><span data-stu-id="aad5c-132">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="aad5c-133">ItemChanges</span><span class="sxs-lookup"><span data-stu-id="aad5c-133">ItemChanges</span></span>](itemchanges.md) <br/> |<span data-ttu-id="aad5c-134">Содержит массив элементов [ItemChange](itemchange.md) , чтобы указать элементы и обновления, чтобы применить к элементам.</span><span class="sxs-lookup"><span data-stu-id="aad5c-134">Contains an array of [ItemChange](itemchange.md) elements that identify items and the updates to apply to the items.</span></span>  <br/> <span data-ttu-id="aad5c-135">Ниже приведен выражение XPath для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="aad5c-135">The following is the XPath expression to this element:</span></span>  <br/>  `/UpdateItem/ItemChanges` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="aad5c-136">Замечания</span><span class="sxs-lookup"><span data-stu-id="aad5c-136">Remarks</span></span>

<span data-ttu-id="aad5c-137">Можно использовать только один элемент [ItemId](itemid.md), [OccurrenceItemId](occurrenceitemid.md)или [RecurringMasterItemId](recurringmasteritemid.md) в элементе **ItemChange** .</span><span class="sxs-lookup"><span data-stu-id="aad5c-137">Only a single [ItemId](itemid.md), [OccurrenceItemId](occurrenceitemid.md), or [RecurringMasterItemId](recurringmasteritemid.md) element can be used in an **ItemChange** element.</span></span> 
  
<span data-ttu-id="aad5c-138">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="aad5c-138">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="aad5c-139">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="aad5c-139">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="aad5c-140">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="aad5c-140">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="aad5c-141">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="aad5c-141">Schema Name</span></span>  <br/> |<span data-ttu-id="aad5c-142">Схема Types</span><span class="sxs-lookup"><span data-stu-id="aad5c-142">Types schema</span></span>  <br/> |
|<span data-ttu-id="aad5c-143">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="aad5c-143">Validation File</span></span>  <br/> |<span data-ttu-id="aad5c-144">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="aad5c-144">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="aad5c-145">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="aad5c-145">Can be Empty</span></span>  <br/> |<span data-ttu-id="aad5c-146">False</span><span class="sxs-lookup"><span data-stu-id="aad5c-146">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="aad5c-147">См. также</span><span class="sxs-lookup"><span data-stu-id="aad5c-147">See also</span></span>

- [<span data-ttu-id="aad5c-148">Операция UpdateItem</span><span class="sxs-lookup"><span data-stu-id="aad5c-148">UpdateItem operation</span></span>](updateitem-operation.md)

