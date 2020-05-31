---
title: оккурренцеитемид
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
description: Элемент Оккурренцеитемид определяет один экземпляр повторяющегося элемента.
ms.openlocfilehash: 073639ecbca6ffda872e9253b7c7e44c3541f13b
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/28/2018
ms.locfileid: "21353464"
---
# <a name="occurrenceitemid"></a><span data-ttu-id="bea10-103">оккурренцеитемид</span><span class="sxs-lookup"><span data-stu-id="bea10-103">OccurrenceItemId</span></span>

<span data-ttu-id="bea10-104">Элемент **оккурренцеитемид** определяет один экземпляр повторяющегося элемента.</span><span class="sxs-lookup"><span data-stu-id="bea10-104">The **OccurrenceItemId** element identifies a single occurrence of a recurring item.</span></span> 
  
```XML
<OccurrenceItemId RecurringMasterId="" ChangeKey="" InstanceIndex=""/>
```

<span data-ttu-id="bea10-105">**оккурренцеитемидтипе**</span><span class="sxs-lookup"><span data-stu-id="bea10-105">**OccurrenceItemIdType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="bea10-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="bea10-106">Attributes and elements</span></span>

<span data-ttu-id="bea10-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="bea10-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="bea10-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="bea10-108">Attributes</span></span>

|<span data-ttu-id="bea10-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="bea10-109">**Attribute**</span></span>|<span data-ttu-id="bea10-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="bea10-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="bea10-111">**рекуррингмастерид**</span><span class="sxs-lookup"><span data-stu-id="bea10-111">**RecurringMasterId**</span></span> <br/> |<span data-ttu-id="bea10-112">Определяет шаблон повторяющегося элемента повторяющегося элемента.</span><span class="sxs-lookup"><span data-stu-id="bea10-112">Identifies the recurring master of a recurring item.</span></span> <span data-ttu-id="bea10-113">Этот атрибут является обязательным.</span><span class="sxs-lookup"><span data-stu-id="bea10-113">This attribute is required.</span></span>  <br/> |
|<span data-ttu-id="bea10-114">**чанжекэй**</span><span class="sxs-lookup"><span data-stu-id="bea10-114">**ChangeKey**</span></span> <br/> |<span data-ttu-id="bea10-115">Определяет определенную версию шаблона повторения или вхождение элемента.</span><span class="sxs-lookup"><span data-stu-id="bea10-115">Identifies a specific version of the recurring master or an item occurrence.</span></span> <span data-ttu-id="bea10-116">При изменении одного или обоих его повторений **чанжекэй** изменяется.</span><span class="sxs-lookup"><span data-stu-id="bea10-116">If either the recurring master or any of its occurrences change, the **ChangeKey** changes.</span></span> <span data-ttu-id="bea10-117">**Чанжекэй** одинаково для шаблона повторения и всех вхождений.</span><span class="sxs-lookup"><span data-stu-id="bea10-117">The **ChangeKey** is the same for the recurring master and all occurrences.</span></span>  <br/> |
|<span data-ttu-id="bea10-118">**инстанцеиндекс**</span><span class="sxs-lookup"><span data-stu-id="bea10-118">**InstanceIndex**</span></span> <br/> |<span data-ttu-id="bea10-119">Определяет индекс экземпляра элемента.</span><span class="sxs-lookup"><span data-stu-id="bea10-119">Identifies the index of the item occurrence.</span></span> <span data-ttu-id="bea10-120">Этот атрибут является обязательным.</span><span class="sxs-lookup"><span data-stu-id="bea10-120">This attribute is required.</span></span> <span data-ttu-id="bea10-121">Это значение представляет целое число.</span><span class="sxs-lookup"><span data-stu-id="bea10-121">This value represents an integer.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="bea10-122">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="bea10-122">Child elements</span></span>

<span data-ttu-id="bea10-123">Нет.</span><span class="sxs-lookup"><span data-stu-id="bea10-123">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="bea10-124">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="bea10-124">Parent elements</span></span>

|<span data-ttu-id="bea10-125">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="bea10-125">**Element**</span></span>|<span data-ttu-id="bea10-126">**Описание**</span><span class="sxs-lookup"><span data-stu-id="bea10-126">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bea10-127">глобалитемидс</span><span class="sxs-lookup"><span data-stu-id="bea10-127">GlobalItemIds</span></span>](globalitemids.md) <br/> |<span data-ttu-id="bea10-128">Содержит коллекцию идентификаторов элементов для всех элементов бесед в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="bea10-128">Contains the collection of item identifiers for all conversation items in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="bea10-129">итемидс</span><span class="sxs-lookup"><span data-stu-id="bea10-129">ItemIds</span></span>](itemids.md) <br/> | <span data-ttu-id="bea10-130">Содержит уникальные идентификаторы элементов, элементы вхождений и повторяющиеся элементы шаблона, которые используются для удаления, отправки, получения, перемещения или копирования элементов в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="bea10-130">Contains the unique identities of items, occurrence items, and recurring master items that are used to delete, send, get, move, or copy items in the Exchange store.</span></span> <br/><br/><span data-ttu-id="bea10-131">Ниже приведены выражения XPath для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="bea10-131">The following are the XPath expressions to this element:</span></span> <br/><br/>  `/DeleteItem/ItemIds` <br/>  `/SendItem/ItemIds` <br/>  `/GetItem/ItemIds` <br/><br/><span data-ttu-id="bea10-132">**Note**: [Операция MoveItem](moveitem-operation.md) и [CopyItem](copyitem-operation.md) работают только с одними элементами календаря и повторяющимися элементами шаблона.</span><span class="sxs-lookup"><span data-stu-id="bea10-132">**NOTE**: [MoveItem operation](moveitem-operation.md) and [CopyItem operation](copyitem-operation.md) only work with single calendar items and recurring master items.</span></span> <span data-ttu-id="bea10-133">Недопустимые вхождения элементов для этих операций.</span><span class="sxs-lookup"><span data-stu-id="bea10-133">Item occurrences are invalid with these operations.</span></span>           |
|[<span data-ttu-id="bea10-134">ItemChange</span><span class="sxs-lookup"><span data-stu-id="bea10-134">ItemChange</span></span>](itemchange.md) <br/> |<span data-ttu-id="bea10-135">Содержит идентификатор элемента и обновления, применяемые к элементу.</span><span class="sxs-lookup"><span data-stu-id="bea10-135">Contains an item identifier and the updates to apply to the item.</span></span><br/><br/> <span data-ttu-id="bea10-136">Ниже приведено выражение XPath для этого элемента:</span><span class="sxs-lookup"><span data-stu-id="bea10-136">The following is the XPath expression to this element:</span></span>  <br/>  `/UpdateItem/ItemChanges/ItemChange[i]` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="bea10-137">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="bea10-137">Text value</span></span>

<span data-ttu-id="bea10-138">Нет.</span><span class="sxs-lookup"><span data-stu-id="bea10-138">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="bea10-139">Примечания</span><span class="sxs-lookup"><span data-stu-id="bea10-139">Remarks</span></span>

<span data-ttu-id="bea10-140">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="bea10-140">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="example"></a><span data-ttu-id="bea10-141">Пример</span><span class="sxs-lookup"><span data-stu-id="bea10-141">Example</span></span>

<span data-ttu-id="bea10-142">В приведенном ниже примере показано, как определить Четвертый экземпляр повторяющегося элемента с идентификатором 34vswe4.</span><span class="sxs-lookup"><span data-stu-id="bea10-142">The following example identifies the fourth occurrence of a recurring item that has the identity 34vswe4.</span></span>
  
```XML
<OccurrenceItemId RecurringMasterId="34vswe4" InstanceIndex="4" />
```

## <a name="element-information"></a><span data-ttu-id="bea10-143">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="bea10-143">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="bea10-144">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="bea10-144">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="bea10-145">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="bea10-145">Schema Name</span></span>  <br/> |<span data-ttu-id="bea10-146">Схема Types</span><span class="sxs-lookup"><span data-stu-id="bea10-146">Types schema</span></span>  <br/> |
|<span data-ttu-id="bea10-147">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="bea10-147">Validation File</span></span>  <br/> |<span data-ttu-id="bea10-148">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="bea10-148">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="bea10-149">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="bea10-149">Can be Empty</span></span>  <br/> |<span data-ttu-id="bea10-150">False</span><span class="sxs-lookup"><span data-stu-id="bea10-150">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="bea10-151">См. также</span><span class="sxs-lookup"><span data-stu-id="bea10-151">See also</span></span>

- [<span data-ttu-id="bea10-152">рекуррингмастеритемид</span><span class="sxs-lookup"><span data-stu-id="bea10-152">RecurringMasterItemId</span></span>](recurringmasteritemid.md)
- [<span data-ttu-id="bea10-153">Операция FindConversation</span><span class="sxs-lookup"><span data-stu-id="bea10-153">FindConversation operation</span></span>](findconversation-operation.md)
- [<span data-ttu-id="bea10-154">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="bea10-154">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

