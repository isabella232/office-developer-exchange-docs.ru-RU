---
title: рекуррингмастеритемид
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
description: Элемент Рекуррингмастеритемид определяет элемент шаблона повторения, определяя идентификаторы одного из связанных элементов вхождения.
ms.openlocfilehash: 896a9ce95d619e7bb44c8158288bc4f62ce417d9
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529884"
---
# <a name="recurringmasteritemid"></a><span data-ttu-id="8c63c-103">рекуррингмастеритемид</span><span class="sxs-lookup"><span data-stu-id="8c63c-103">RecurringMasterItemId</span></span>

<span data-ttu-id="8c63c-104">Элемент **рекуррингмастеритемид** определяет элемент шаблона повторения, определяя идентификаторы одного из связанных элементов вхождения.</span><span class="sxs-lookup"><span data-stu-id="8c63c-104">The **RecurringMasterItemId** element identifies a recurrence master item by identifying the identifiers of one of its related occurrence items.</span></span> 
  
```XML
<RecurringMasterItemId OccurrenceId="" ChangeKey="" />
```

 <span data-ttu-id="8c63c-105">**рекуррингмастеритемидтипе**</span><span class="sxs-lookup"><span data-stu-id="8c63c-105">**RecurringMasterItemIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="8c63c-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="8c63c-106">Attributes and elements</span></span>

<span data-ttu-id="8c63c-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="8c63c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8c63c-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="8c63c-108">Attributes</span></span>

|<span data-ttu-id="8c63c-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="8c63c-109">**Attribute**</span></span>|<span data-ttu-id="8c63c-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="8c63c-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="8c63c-111">**оккурренцеид**</span><span class="sxs-lookup"><span data-stu-id="8c63c-111">**OccurrenceId**</span></span> <br/> |<span data-ttu-id="8c63c-112">Определяет один экземпляр повторяющегося элемента шаблона.</span><span class="sxs-lookup"><span data-stu-id="8c63c-112">Identifies a single occurrence of a recurring master item.</span></span> <span data-ttu-id="8c63c-113">Этот атрибут является обязательным.</span><span class="sxs-lookup"><span data-stu-id="8c63c-113">This attribute is required.</span></span>  <br/> |
|<span data-ttu-id="8c63c-114">**чанжекэй**</span><span class="sxs-lookup"><span data-stu-id="8c63c-114">**ChangeKey**</span></span> <br/> |<span data-ttu-id="8c63c-115">Определяет конкретную версию одного экземпляра повторяющегося элемента шаблона.</span><span class="sxs-lookup"><span data-stu-id="8c63c-115">Identifies a specific version of a single occurrence of a recurring master item.</span></span> <span data-ttu-id="8c63c-116">Кроме того, также идентифицируется шаблон повторяющегося элемента, так как он и один экземпляр будут содержать один и тот же ключ изменения.</span><span class="sxs-lookup"><span data-stu-id="8c63c-116">Additionally, the recurring master item is also identified because it and the single occurrence will contain the same change key.</span></span> <span data-ttu-id="8c63c-117">Этот атрибут является необязательным.</span><span class="sxs-lookup"><span data-stu-id="8c63c-117">This attribute is optional.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="8c63c-118">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="8c63c-118">Child elements</span></span>

<span data-ttu-id="8c63c-119">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="8c63c-119">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="8c63c-120">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="8c63c-120">Parent elements</span></span>

|<span data-ttu-id="8c63c-121">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="8c63c-121">**Element**</span></span>|<span data-ttu-id="8c63c-122">**Описание**</span><span class="sxs-lookup"><span data-stu-id="8c63c-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8c63c-123">глобалитемидс</span><span class="sxs-lookup"><span data-stu-id="8c63c-123">GlobalItemIds</span></span>](globalitemids.md) <br/> |<span data-ttu-id="8c63c-124">Содержит коллекцию идентификаторов элементов для всех элементов бесед в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="8c63c-124">Contains the collection of item identifiers for all conversation items in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="8c63c-125">ItemChange</span><span class="sxs-lookup"><span data-stu-id="8c63c-125">ItemChange</span></span>](itemchange.md) <br/> |<span data-ttu-id="8c63c-126">Содержит идентификатор элемента и обновления, применяемые к элементу.</span><span class="sxs-lookup"><span data-stu-id="8c63c-126">Contains an item identifier and the updates to apply to the item.</span></span> <br/> <br/> <span data-ttu-id="8c63c-127">Ниже приведено выражение XPath для этого элемента:</span><span class="sxs-lookup"><span data-stu-id="8c63c-127">The following is the XPath expression to this element:</span></span> <br/> <br/>  `/UpdateItem/ItemChanges/ItemChange[i]` <br/> |
|[<span data-ttu-id="8c63c-128">итемидс</span><span class="sxs-lookup"><span data-stu-id="8c63c-128">ItemIds</span></span>](itemids.md) <br/> | <span data-ttu-id="8c63c-129">Содержит уникальные идентификаторы элементов, элементы вхождений и повторяющиеся элементы шаблона, которые используются для удаления, отправки, получения, перемещения или копирования элементов в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="8c63c-129">Contains the unique identities of items, occurrence items, and recurring master items that are used to delete, send, get, move, or copy items in the Exchange store.</span></span> <br/> <br/>  <span data-ttu-id="8c63c-130">Ниже приведены выражения XPath для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="8c63c-130">The following are the XPath expressions to this element:</span></span>  <br/><br/>  `/DeleteItem/ItemIds` <br/>  `/SendItem/ItemIds` <br/>  `/GetItem/ItemIds` <br/>  `/MoveItem/ItemIds` <br/>  `/CopyItem//ItemIds` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="8c63c-131">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="8c63c-131">Text value</span></span>

<span data-ttu-id="8c63c-132">Нет.</span><span class="sxs-lookup"><span data-stu-id="8c63c-132">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="8c63c-133">Примечания</span><span class="sxs-lookup"><span data-stu-id="8c63c-133">Remarks</span></span>

<span data-ttu-id="8c63c-134">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="8c63c-134">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="example"></a><span data-ttu-id="8c63c-135">Пример</span><span class="sxs-lookup"><span data-stu-id="8c63c-135">Example</span></span>

<span data-ttu-id="8c63c-136">В примере ниже показано, как определить шаблон повторяющегося элемента, определив один из его экземпляров с идентификатором 56lkjh6.</span><span class="sxs-lookup"><span data-stu-id="8c63c-136">The following example identifies the recurring master item by identifying one of its occurrences with the identifier 56lkjh6.</span></span>
  
```XML
<RecurringMasterItemId OccurrenceId="56lkjh6" />
```

## <a name="element-information"></a><span data-ttu-id="8c63c-137">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="8c63c-137">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8c63c-138">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="8c63c-138">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="8c63c-139">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="8c63c-139">Schema Name</span></span>  <br/> |<span data-ttu-id="8c63c-140">Схема Types</span><span class="sxs-lookup"><span data-stu-id="8c63c-140">Types schema</span></span>  <br/> |
|<span data-ttu-id="8c63c-141">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="8c63c-141">Validation File</span></span>  <br/> |<span data-ttu-id="8c63c-142">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="8c63c-142">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="8c63c-143">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="8c63c-143">Can be Empty</span></span>  <br/> |<span data-ttu-id="8c63c-144">False</span><span class="sxs-lookup"><span data-stu-id="8c63c-144">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="8c63c-145">См. также</span><span class="sxs-lookup"><span data-stu-id="8c63c-145">See also</span></span>

- [<span data-ttu-id="8c63c-146">оккурренцеитемид</span><span class="sxs-lookup"><span data-stu-id="8c63c-146">OccurrenceItemId</span></span>](occurrenceitemid.md)
- [<span data-ttu-id="8c63c-147">Операция FindConversation</span><span class="sxs-lookup"><span data-stu-id="8c63c-147">FindConversation operation</span></span>](findconversation-operation.md)

