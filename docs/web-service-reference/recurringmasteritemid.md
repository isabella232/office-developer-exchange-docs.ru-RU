---
title: RecurringMasterItemId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RecurringMasterItemId
api_type:
- schema
ms.assetid: 5800b58c-f3d7-4d8f-acc0-d13e02f4e258
description: Элемент RecurringMasterItemId определяет элемент шаблона повторения с учетом идентификаторы одного из его элементы, связанных с ними вхождение.
ms.openlocfilehash: ae59e33ece55d85435ece4c9030ccda32eb62eab
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835015"
---
# <a name="recurringmasteritemid"></a><span data-ttu-id="f414d-103">RecurringMasterItemId</span><span class="sxs-lookup"><span data-stu-id="f414d-103">RecurringMasterItemId</span></span>

<span data-ttu-id="f414d-104">Элемент **RecurringMasterItemId** определяет элемент шаблона повторения с учетом идентификаторы одного из его элементы, связанных с ними вхождение.</span><span class="sxs-lookup"><span data-stu-id="f414d-104">The **RecurringMasterItemId** element identifies a recurrence master item by identifying the identifiers of one of its related occurrence items.</span></span> 
  
```XML
<RecurringMasterItemId OccurrenceId="" ChangeKey="" />
```

 <span data-ttu-id="f414d-105">**RecurringMasterItemIdType**</span><span class="sxs-lookup"><span data-stu-id="f414d-105">**RecurringMasterItemIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f414d-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="f414d-106">Attributes and elements</span></span>

<span data-ttu-id="f414d-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="f414d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f414d-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="f414d-108">Attributes</span></span>

|<span data-ttu-id="f414d-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="f414d-109">**Attribute**</span></span>|<span data-ttu-id="f414d-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="f414d-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="f414d-111">**OccurrenceId**</span><span class="sxs-lookup"><span data-stu-id="f414d-111">**OccurrenceId**</span></span> <br/> |<span data-ttu-id="f414d-112">Определяет одно вхождение повторяющегося элемента шаблона.</span><span class="sxs-lookup"><span data-stu-id="f414d-112">Identifies a single occurrence of a recurring master item.</span></span> <span data-ttu-id="f414d-113">Этот атрибут является обязательным.</span><span class="sxs-lookup"><span data-stu-id="f414d-113">This attribute is required.</span></span>  <br/> |
|<span data-ttu-id="f414d-114">**ChangeKey**</span><span class="sxs-lookup"><span data-stu-id="f414d-114">**ChangeKey**</span></span> <br/> |<span data-ttu-id="f414d-115">Идентифицирует определенной версии одного экземпляра повторяющегося элемента шаблона.</span><span class="sxs-lookup"><span data-stu-id="f414d-115">Identifies a specific version of a single occurrence of a recurring master item.</span></span> <span data-ttu-id="f414d-116">Кроме того повторяющегося элемента шаблона также определены, так как он и одно вхождение будет содержать тем же ключом изменений.</span><span class="sxs-lookup"><span data-stu-id="f414d-116">Additionally, the recurring master item is also identified because it and the single occurrence will contain the same change key.</span></span> <span data-ttu-id="f414d-117">Этот атрибут является необязательным.</span><span class="sxs-lookup"><span data-stu-id="f414d-117">This attribute is optional.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="f414d-118">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="f414d-118">Child elements</span></span>

<span data-ttu-id="f414d-119">Нет.</span><span class="sxs-lookup"><span data-stu-id="f414d-119">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="f414d-120">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="f414d-120">Parent elements</span></span>

|<span data-ttu-id="f414d-121">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="f414d-121">**Element**</span></span>|<span data-ttu-id="f414d-122">**Описание**</span><span class="sxs-lookup"><span data-stu-id="f414d-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f414d-123">GlobalItemIds</span><span class="sxs-lookup"><span data-stu-id="f414d-123">GlobalItemIds</span></span>](globalitemids.md) <br/> |<span data-ttu-id="f414d-124">Содержит коллекцию идентификаторов элементов для всех элементов беседы в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="f414d-124">Contains the collection of item identifiers for all conversation items in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="f414d-125">ItemChange</span><span class="sxs-lookup"><span data-stu-id="f414d-125">ItemChange</span></span>](itemchange.md) <br/> |<span data-ttu-id="f414d-126">Содержит идентификатор элемента и обновления для применения к элементу.</span><span class="sxs-lookup"><span data-stu-id="f414d-126">Contains an item identifier and the updates to apply to the item.</span></span> <br/> <br/> <span data-ttu-id="f414d-127">Ниже приведен выражение XPath для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="f414d-127">The following is the XPath expression to this element:</span></span> <br/> <br/>  `/UpdateItem/ItemChanges/ItemChange[i]` <br/> |
|[<span data-ttu-id="f414d-128">Что ItemID</span><span class="sxs-lookup"><span data-stu-id="f414d-128">ItemIds</span></span>](itemids.md) <br/> | <span data-ttu-id="f414d-129">Содержит уникальные идентификаторы элементов, элементы вхождений и повторяющиеся основные элементы, используемые для удаления, отправка, получение, перемещение и копирование элементов в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="f414d-129">Contains the unique identities of items, occurrence items, and recurring master items that are used to delete, send, get, move, or copy items in the Exchange store.</span></span> <br/> <br/>  <span data-ttu-id="f414d-130">Ниже приведены выражения XPath для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="f414d-130">The following are the XPath expressions to this element:</span></span>  <br/><br/>  `/DeleteItem/ItemIds` <br/>  `/SendItem/ItemIds` <br/>  `/GetItem/ItemIds` <br/>  `/MoveItem/ItemIds` <br/>  `/CopyItem//ItemIds` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="f414d-131">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="f414d-131">Text value</span></span>

<span data-ttu-id="f414d-132">Нет.</span><span class="sxs-lookup"><span data-stu-id="f414d-132">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="f414d-133">Замечания</span><span class="sxs-lookup"><span data-stu-id="f414d-133">Remarks</span></span>

<span data-ttu-id="f414d-134">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="f414d-134">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="example"></a><span data-ttu-id="f414d-135">Пример</span><span class="sxs-lookup"><span data-stu-id="f414d-135">Example</span></span>

<span data-ttu-id="f414d-136">Следующий пример определяет повторяющиеся главных элемент, указав один из его вхождения, содержащие 56lkjh6 идентификатор.</span><span class="sxs-lookup"><span data-stu-id="f414d-136">The following example identifies the recurring master item by identifying one of its occurrences with the identifier 56lkjh6.</span></span>
  
```XML
<RecurringMasterItemId OccurrenceId="56lkjh6" />
```

## <a name="element-information"></a><span data-ttu-id="f414d-137">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="f414d-137">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f414d-138">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="f414d-138">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="f414d-139">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="f414d-139">Schema Name</span></span>  <br/> |<span data-ttu-id="f414d-140">Схема Types</span><span class="sxs-lookup"><span data-stu-id="f414d-140">Types schema</span></span>  <br/> |
|<span data-ttu-id="f414d-141">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="f414d-141">Validation File</span></span>  <br/> |<span data-ttu-id="f414d-142">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="f414d-142">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="f414d-143">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="f414d-143">Can be Empty</span></span>  <br/> |<span data-ttu-id="f414d-144">False</span><span class="sxs-lookup"><span data-stu-id="f414d-144">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f414d-145">См. также</span><span class="sxs-lookup"><span data-stu-id="f414d-145">See also</span></span>

- [<span data-ttu-id="f414d-146">OccurrenceItemId</span><span class="sxs-lookup"><span data-stu-id="f414d-146">OccurrenceItemId</span></span>](occurrenceitemid.md)
- [<span data-ttu-id="f414d-147">FindConversation Operation</span><span class="sxs-lookup"><span data-stu-id="f414d-147">FindConversation operation</span></span>](findconversation-operation.md)

