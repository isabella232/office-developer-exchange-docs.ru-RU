---
title: итемидс
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
description: Элемент Итемидс содержит уникальные идентификаторы элементов, элементы вхождений и повторяющиеся элементы шаблона, которые используются для удаления, отправки, получения, перемещения или копирования элементов в хранилище Exchange.
ms.openlocfilehash: bbd594ce2610bd625b0e16a0383fda552ee9eb19
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460605"
---
# <a name="itemids"></a><span data-ttu-id="9df2f-103">итемидс</span><span class="sxs-lookup"><span data-stu-id="9df2f-103">ItemIds</span></span>
  
<span data-ttu-id="9df2f-104">Элемент **итемидс** содержит уникальные идентификаторы элементов, элементы вхождений и повторяющиеся элементы шаблона, которые используются для удаления, отправки, получения, перемещения или копирования элементов в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="9df2f-104">The **ItemIds** element contains the unique identities of items, occurrence items, and recurring master items that are used to delete, send, get, move, or copy items in the Exchange store.</span></span>
  
```xml
<ItemIds>
   <ItemId/>
   <OccurrenceItemId/>
   <RecurringMasterItemId/>
</ItemIds>
```

<span data-ttu-id="9df2f-105">**нонемптяррайофбасеитемидстипе**</span><span class="sxs-lookup"><span data-stu-id="9df2f-105">**NonEmptyArrayOfBaseItemIdsType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="9df2f-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="9df2f-106">Attributes and elements</span></span>

<span data-ttu-id="9df2f-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="9df2f-107">The following sections describe attributes, child elements, and parent elements.</span></span> 
  
### <a name="attributes"></a><span data-ttu-id="9df2f-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="9df2f-108">Attributes</span></span>

<span data-ttu-id="9df2f-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="9df2f-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9df2f-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="9df2f-110">Child elements</span></span>

|<span data-ttu-id="9df2f-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="9df2f-111">**Element**</span></span>|<span data-ttu-id="9df2f-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="9df2f-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9df2f-113">Идентификатор</span><span class="sxs-lookup"><span data-stu-id="9df2f-113">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="9df2f-114">Содержит уникальный идентификатор и ключ изменения элемента в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="9df2f-114">Contains the unique identifier and change key of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="9df2f-115">оккурренцеитемид</span><span class="sxs-lookup"><span data-stu-id="9df2f-115">OccurrenceItemId</span></span>](occurrenceitemid.md) <br/> |<span data-ttu-id="9df2f-116">Определяет один экземпляр повторяющегося элемента.</span><span class="sxs-lookup"><span data-stu-id="9df2f-116">Identifies a single occurrence of a recurring item.</span></span>  <br/> |
|[<span data-ttu-id="9df2f-117">рекуррингмастеритемид</span><span class="sxs-lookup"><span data-stu-id="9df2f-117">RecurringMasterItemId</span></span>](recurringmasteritemid.md) <br/> |<span data-ttu-id="9df2f-118">Определяет элемент шаблона повторения, определив один из идентификаторов связанных элементов вхождения.</span><span class="sxs-lookup"><span data-stu-id="9df2f-118">Identifies a recurrence master item by identifying one of its related occurrence items' identifiers.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="9df2f-119">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="9df2f-119">Parent elements</span></span>

|<span data-ttu-id="9df2f-120">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="9df2f-120">**Element**</span></span>|<span data-ttu-id="9df2f-121">**Описание**</span><span class="sxs-lookup"><span data-stu-id="9df2f-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9df2f-122">Беседы (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="9df2f-122">Conversation (ConversationType)</span></span>](conversation-conversationtype.md) <br/> |<span data-ttu-id="9df2f-123">Представляет одну беседу.</span><span class="sxs-lookup"><span data-stu-id="9df2f-123">Represents a single conversation.</span></span>  <br/> |
|[<span data-ttu-id="9df2f-124">DeleteItem</span><span class="sxs-lookup"><span data-stu-id="9df2f-124">DeleteItem</span></span>](deleteitem.md) <br/> |<span data-ttu-id="9df2f-125">Определяет запрос на удаление элементов в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="9df2f-125">Defines a request to delete items in the Exchange store.</span></span>  <br/> <span data-ttu-id="9df2f-126">Ниже приведено выражение XPath для этого элемента:</span><span class="sxs-lookup"><span data-stu-id="9df2f-126">The following is the XPath expression to this element:</span></span>  <br/>  `/DeleteItem` <br/> |
|[<span data-ttu-id="9df2f-127">SendItem</span><span class="sxs-lookup"><span data-stu-id="9df2f-127">SendItem</span></span>](senditem.md) <br/> |<span data-ttu-id="9df2f-128">Корневой элемент, определяющий запрос на отправку элементов в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="9df2f-128">The root element that defines a request to send items in the Exchange store.</span></span>  <br/> <span data-ttu-id="9df2f-129">Ниже приведено выражение XPath для этого элемента:</span><span class="sxs-lookup"><span data-stu-id="9df2f-129">The following is the XPath expression to this element:</span></span>  <br/>  `/SendItem` <br/> |
|[<span data-ttu-id="9df2f-130">GetItem</span><span class="sxs-lookup"><span data-stu-id="9df2f-130">GetItem</span></span>](getitem.md) <br/> |<span data-ttu-id="9df2f-131">Определяет запрос на получение элементов из хранилища Exchange.</span><span class="sxs-lookup"><span data-stu-id="9df2f-131">Defines a request to get items from the Exchange store.</span></span>  <br/> <span data-ttu-id="9df2f-132">Ниже приведено выражение XPath для этого элемента:</span><span class="sxs-lookup"><span data-stu-id="9df2f-132">The following is the XPath expression to this element:</span></span>  <br/>  `/GetItem` <br/> |
|[<span data-ttu-id="9df2f-133">MoveItem</span><span class="sxs-lookup"><span data-stu-id="9df2f-133">MoveItem</span></span>](moveitem.md) <br/> |<span data-ttu-id="9df2f-134">Определяет запрос на перемещение элементов в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="9df2f-134">Defines a request to move items in the Exchange store.</span></span>  <br/> <span data-ttu-id="9df2f-135">Ниже приведено выражение XPath для этого элемента:</span><span class="sxs-lookup"><span data-stu-id="9df2f-135">The following is the XPath expression to this element:</span></span>  <br/>  `/MoveItem` <br/> |
|[<span data-ttu-id="9df2f-136">CopyItem</span><span class="sxs-lookup"><span data-stu-id="9df2f-136">CopyItem</span></span>](copyitem.md) <br/> |<span data-ttu-id="9df2f-137">Определяет запрос на копирование элементов в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="9df2f-137">Defines a request to copy items in the Exchange store.</span></span>  <br/> <span data-ttu-id="9df2f-138">Ниже приведено выражение XPath для этого элемента:</span><span class="sxs-lookup"><span data-stu-id="9df2f-138">The following is the XPath expression to this element:</span></span>  <br/>  `/CopyItem` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="9df2f-139">Примечания</span><span class="sxs-lookup"><span data-stu-id="9df2f-139">Remarks</span></span>

<span data-ttu-id="9df2f-140">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="9df2f-140">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9df2f-141">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="9df2f-141">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9df2f-142">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="9df2f-142">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="9df2f-143">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="9df2f-143">Schema Name</span></span>  <br/> |<span data-ttu-id="9df2f-144">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="9df2f-144">Messages schema</span></span>  <br/> |
|<span data-ttu-id="9df2f-145">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="9df2f-145">Validation File</span></span>  <br/> |<span data-ttu-id="9df2f-146">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="9df2f-146">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="9df2f-147">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="9df2f-147">Can be Empty</span></span>  <br/> |<span data-ttu-id="9df2f-148">False</span><span class="sxs-lookup"><span data-stu-id="9df2f-148">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9df2f-149">См. также</span><span class="sxs-lookup"><span data-stu-id="9df2f-149">See also</span></span>

- [<span data-ttu-id="9df2f-150">Операция DeleteItem</span><span class="sxs-lookup"><span data-stu-id="9df2f-150">DeleteItem operation</span></span>](deleteitem-operation.md)
- [<span data-ttu-id="9df2f-151">Операция SendItem</span><span class="sxs-lookup"><span data-stu-id="9df2f-151">SendItem operation</span></span>](senditem-operation.md) 
- [<span data-ttu-id="9df2f-152">Операция GetItem</span><span class="sxs-lookup"><span data-stu-id="9df2f-152">GetItem operation</span></span>](getitem-operation.md)
- [<span data-ttu-id="9df2f-153">Операция MoveItem</span><span class="sxs-lookup"><span data-stu-id="9df2f-153">MoveItem operation</span></span>](moveitem-operation.md)
- [<span data-ttu-id="9df2f-154">Операция CopyItem</span><span class="sxs-lookup"><span data-stu-id="9df2f-154">CopyItem operation</span></span>](copyitem-operation.md)
- [<span data-ttu-id="9df2f-155">Операция FindConversation</span><span class="sxs-lookup"><span data-stu-id="9df2f-155">FindConversation operation</span></span>](findconversation-operation.md)

