---
title: ItemIds
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ItemIds
api_type:
- schema
ms.assetid: 6b82122b-5544-4adf-91b7-ef2db7d5046f
description: Что ItemID элемент содержит уникальные идентификаторы элементов, элементы вхождений и повторяющиеся основные элементы, используемые для удаления, отправка, получение, перемещение и копирование элементов в хранилище Exchange.
ms.openlocfilehash: 1bd4d6f4593a7c3b418561269d8b29707cc6030c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19834155"
---
# <a name="itemids"></a><span data-ttu-id="5d134-103">ItemIds</span><span class="sxs-lookup"><span data-stu-id="5d134-103">ItemIds</span></span>
  
<span data-ttu-id="5d134-104">**Что ItemID** элемент содержит уникальные идентификаторы элементов, элементы вхождений и повторяющиеся основные элементы, используемые для удаления, отправка, получение, перемещение и копирование элементов в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="5d134-104">The **ItemIds** element contains the unique identities of items, occurrence items, and recurring master items that are used to delete, send, get, move, or copy items in the Exchange store.</span></span>
  
```xml
<ItemIds>
   <ItemId/>
   <OccurrenceItemId/>
   <RecurringMasterItemId/>
</ItemIds>
```

<span data-ttu-id="5d134-105">**NonEmptyArrayOfBaseItemIdsType**</span><span class="sxs-lookup"><span data-stu-id="5d134-105">**NonEmptyArrayOfBaseItemIdsType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="5d134-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="5d134-106">Attributes and elements</span></span>

<span data-ttu-id="5d134-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="5d134-107">The following sections describe attributes, child elements, and parent elements.</span></span> 
  
### <a name="attributes"></a><span data-ttu-id="5d134-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="5d134-108">Attributes</span></span>

<span data-ttu-id="5d134-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="5d134-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5d134-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="5d134-110">Child elements</span></span>

|<span data-ttu-id="5d134-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="5d134-111">**Element**</span></span>|<span data-ttu-id="5d134-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="5d134-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5d134-113">Идентификатор элемента</span><span class="sxs-lookup"><span data-stu-id="5d134-113">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="5d134-114">Содержит уникальный идентификатор и меняет ключ элемента в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="5d134-114">Contains the unique identifier and change key of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="5d134-115">OccurrenceItemId</span><span class="sxs-lookup"><span data-stu-id="5d134-115">OccurrenceItemId</span></span>](occurrenceitemid.md) <br/> |<span data-ttu-id="5d134-116">Определяет одно вхождение повторяющегося элемента.</span><span class="sxs-lookup"><span data-stu-id="5d134-116">Identifies a single occurrence of a recurring item.</span></span>  <br/> |
|[<span data-ttu-id="5d134-117">RecurringMasterItemId</span><span class="sxs-lookup"><span data-stu-id="5d134-117">RecurringMasterItemId</span></span>](recurringmasteritemid.md) <br/> |<span data-ttu-id="5d134-118">Идентифицирует элемент шаблона повторения, указав один из его появления связанные элементы идентификаторов.</span><span class="sxs-lookup"><span data-stu-id="5d134-118">Identifies a recurrence master item by identifying one of its related occurrence items' identifiers.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="5d134-119">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="5d134-119">Parent elements</span></span>

|<span data-ttu-id="5d134-120">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="5d134-120">**Element**</span></span>|<span data-ttu-id="5d134-121">**Описание**</span><span class="sxs-lookup"><span data-stu-id="5d134-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5d134-122">Беседы (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="5d134-122">Conversation (ConversationType)</span></span>](conversation-conversationtype.md) <br/> |<span data-ttu-id="5d134-123">Представляет одну беседу.</span><span class="sxs-lookup"><span data-stu-id="5d134-123">Represents a single conversation.</span></span>  <br/> |
|[<span data-ttu-id="5d134-124">DeleteItem</span><span class="sxs-lookup"><span data-stu-id="5d134-124">DeleteItem</span></span>](deleteitem.md) <br/> |<span data-ttu-id="5d134-125">Определяет запрос на удаление элементов в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="5d134-125">Defines a request to delete items in the Exchange store.</span></span>  <br/> <span data-ttu-id="5d134-126">Ниже приведен выражение XPath для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="5d134-126">The following is the XPath expression to this element:</span></span>  <br/>  `/DeleteItem` <br/> |
|[<span data-ttu-id="5d134-127">SendItem</span><span class="sxs-lookup"><span data-stu-id="5d134-127">SendItem</span></span>](senditem.md) <br/> |<span data-ttu-id="5d134-128">Корневой элемент, который определяет запрос на отправку элементов в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="5d134-128">The root element that defines a request to send items in the Exchange store.</span></span>  <br/> <span data-ttu-id="5d134-129">Ниже приведен выражение XPath для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="5d134-129">The following is the XPath expression to this element:</span></span>  <br/>  `/SendItem` <br/> |
|[<span data-ttu-id="5d134-130">GetItem</span><span class="sxs-lookup"><span data-stu-id="5d134-130">GetItem</span></span>](getitem.md) <br/> |<span data-ttu-id="5d134-131">Определяет запрос на получение элементов из хранилища Exchange.</span><span class="sxs-lookup"><span data-stu-id="5d134-131">Defines a request to get items from the Exchange store.</span></span>  <br/> <span data-ttu-id="5d134-132">Ниже приведен выражение XPath для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="5d134-132">The following is the XPath expression to this element:</span></span>  <br/>  `/GetItem` <br/> |
|[<span data-ttu-id="5d134-133">MoveItem</span><span class="sxs-lookup"><span data-stu-id="5d134-133">MoveItem</span></span>](moveitem.md) <br/> |<span data-ttu-id="5d134-134">Определяет запрос на перемещение элементов в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="5d134-134">Defines a request to move items in the Exchange store.</span></span>  <br/> <span data-ttu-id="5d134-135">Ниже приведен выражение XPath для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="5d134-135">The following is the XPath expression to this element:</span></span>  <br/>  `/MoveItem` <br/> |
|[<span data-ttu-id="5d134-136">CopyItem</span><span class="sxs-lookup"><span data-stu-id="5d134-136">CopyItem</span></span>](copyitem.md) <br/> |<span data-ttu-id="5d134-137">Определяет запрос для копирования элементов в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="5d134-137">Defines a request to copy items in the Exchange store.</span></span>  <br/> <span data-ttu-id="5d134-138">Ниже приведен выражение XPath для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="5d134-138">The following is the XPath expression to this element:</span></span>  <br/>  `/CopyItem` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="5d134-139">Замечания</span><span class="sxs-lookup"><span data-stu-id="5d134-139">Remarks</span></span>

<span data-ttu-id="5d134-140">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="5d134-140">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5d134-141">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="5d134-141">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5d134-142">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="5d134-142">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="5d134-143">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="5d134-143">Schema Name</span></span>  <br/> |<span data-ttu-id="5d134-144">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="5d134-144">Messages schema</span></span>  <br/> |
|<span data-ttu-id="5d134-145">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="5d134-145">Validation File</span></span>  <br/> |<span data-ttu-id="5d134-146">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="5d134-146">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="5d134-147">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="5d134-147">Can be Empty</span></span>  <br/> |<span data-ttu-id="5d134-148">False</span><span class="sxs-lookup"><span data-stu-id="5d134-148">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="5d134-149">См. также</span><span class="sxs-lookup"><span data-stu-id="5d134-149">See also</span></span>

- [<span data-ttu-id="5d134-150">Операция DeleteItem</span><span class="sxs-lookup"><span data-stu-id="5d134-150">DeleteItem operation</span></span>](deleteitem-operation.md)
- [<span data-ttu-id="5d134-151">SendItem Operation</span><span class="sxs-lookup"><span data-stu-id="5d134-151">SendItem operation</span></span>](senditem-operation.md) 
- [<span data-ttu-id="5d134-152">GetItem Operation</span><span class="sxs-lookup"><span data-stu-id="5d134-152">GetItem operation</span></span>](getitem-operation.md)
- [<span data-ttu-id="5d134-153">MoveItem Operation</span><span class="sxs-lookup"><span data-stu-id="5d134-153">MoveItem operation</span></span>](moveitem-operation.md)
- [<span data-ttu-id="5d134-154">CopyItem Operation</span><span class="sxs-lookup"><span data-stu-id="5d134-154">CopyItem operation</span></span>](copyitem-operation.md)
- [<span data-ttu-id="5d134-155">FindConversation Operation</span><span class="sxs-lookup"><span data-stu-id="5d134-155">FindConversation operation</span></span>](findconversation-operation.md)

