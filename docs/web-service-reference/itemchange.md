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
description: Элемент Итемчанже содержит идентификатор элемента и обновления, применяемые к элементу.
ms.openlocfilehash: 916ef1ba2c7a709ec1fd80ababd72999506773c4
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459919"
---
# <a name="itemchange"></a><span data-ttu-id="ea3fe-103">ItemChange</span><span class="sxs-lookup"><span data-stu-id="ea3fe-103">ItemChange</span></span>

<span data-ttu-id="ea3fe-104">Элемент **итемчанже** содержит идентификатор элемента и обновления, применяемые к элементу.</span><span class="sxs-lookup"><span data-stu-id="ea3fe-104">The **ItemChange** element contains an item identifier and the updates to apply to the item.</span></span> 
  
- [<span data-ttu-id="ea3fe-105">UpdateItem</span><span class="sxs-lookup"><span data-stu-id="ea3fe-105">UpdateItem</span></span>](updateitem.md) 
- [<span data-ttu-id="ea3fe-106">итемчанжес</span><span class="sxs-lookup"><span data-stu-id="ea3fe-106">ItemChanges</span></span>](itemchanges.md)
- [<span data-ttu-id="ea3fe-107">ItemChange</span><span class="sxs-lookup"><span data-stu-id="ea3fe-107">ItemChange</span></span>](itemchange.md)
  
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

<span data-ttu-id="ea3fe-108">**итемчанжетипе**</span><span class="sxs-lookup"><span data-stu-id="ea3fe-108">**ItemChangeType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="ea3fe-109">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="ea3fe-109">Attributes and elements</span></span>

<span data-ttu-id="ea3fe-110">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="ea3fe-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ea3fe-111">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="ea3fe-111">Attributes</span></span>

<span data-ttu-id="ea3fe-112">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="ea3fe-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ea3fe-113">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="ea3fe-113">Child elements</span></span>

|<span data-ttu-id="ea3fe-114">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="ea3fe-114">**Element**</span></span>|<span data-ttu-id="ea3fe-115">**Описание**</span><span class="sxs-lookup"><span data-stu-id="ea3fe-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ea3fe-116">Идентификатор</span><span class="sxs-lookup"><span data-stu-id="ea3fe-116">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="ea3fe-117">Содержит уникальный идентификатор и ключ изменения элемента в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="ea3fe-117">Contains the unique identifier and change key of an item in the Exchange store.</span></span> <span data-ttu-id="ea3fe-118">Этот элемент является обязательным, если элемент [оккурренцеитемид](occurrenceitemid.md) или [рекуррингмастеритемид](recurringmasteritemid.md) не используется.</span><span class="sxs-lookup"><span data-stu-id="ea3fe-118">This element is required if the [OccurrenceItemId](occurrenceitemid.md) or [RecurringMasterItemId](recurringmasteritemid.md) element is not used.</span></span>  <br/> |
|[<span data-ttu-id="ea3fe-119">оккурренцеитемид</span><span class="sxs-lookup"><span data-stu-id="ea3fe-119">OccurrenceItemId</span></span>](occurrenceitemid.md) <br/> |<span data-ttu-id="ea3fe-120">Определяет один экземпляр повторяющегося элемента.</span><span class="sxs-lookup"><span data-stu-id="ea3fe-120">Identifies a single occurrence of a recurring item.</span></span> <span data-ttu-id="ea3fe-121">Этот элемент является обязательным при использовании.</span><span class="sxs-lookup"><span data-stu-id="ea3fe-121">This element is required if used.</span></span> <span data-ttu-id="ea3fe-122">Этот элемент является обязательным, если элемент [рекуррингмастеритемид](recurringmasteritemid.md) или [ItemId](itemid.md) не используется.</span><span class="sxs-lookup"><span data-stu-id="ea3fe-122">This element is required if the [RecurringMasterItemId](recurringmasteritemid.md) or [ItemId](itemid.md) element is not used.</span></span>  <br/> |
|[<span data-ttu-id="ea3fe-123">рекуррингмастеритемид</span><span class="sxs-lookup"><span data-stu-id="ea3fe-123">RecurringMasterItemId</span></span>](recurringmasteritemid.md) <br/> |<span data-ttu-id="ea3fe-124">Определяет элемент шаблона повторения, определив один из идентификаторов связанных элементов вхождения.</span><span class="sxs-lookup"><span data-stu-id="ea3fe-124">Identifies a recurrence master item by identifying one of its related occurrence items' identifiers.</span></span> <span data-ttu-id="ea3fe-125">Этот элемент является обязательным при использовании.</span><span class="sxs-lookup"><span data-stu-id="ea3fe-125">This element is required if used.</span></span> <span data-ttu-id="ea3fe-126">Этот элемент является обязательным, если элемент [оккурренцеитемид](occurrenceitemid.md) или [ItemId](itemid.md) не используется.</span><span class="sxs-lookup"><span data-stu-id="ea3fe-126">This element is required if the [OccurrenceItemId](occurrenceitemid.md) or [ItemId](itemid.md) element is not used.</span></span>  <br/> |
|[<span data-ttu-id="ea3fe-127">Обновления (элемент)</span><span class="sxs-lookup"><span data-stu-id="ea3fe-127">Updates (Item)</span></span>](updates-item.md) <br/> |<span data-ttu-id="ea3fe-128">Содержит массив, определяющий Добавление, установку и удаление изменений свойств элемента.</span><span class="sxs-lookup"><span data-stu-id="ea3fe-128">Contains an array that defines append, set, and delete changes to item properties.</span></span> <span data-ttu-id="ea3fe-129">Этот элемент обязательный.</span><span class="sxs-lookup"><span data-stu-id="ea3fe-129">This element is required.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="ea3fe-130">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="ea3fe-130">Parent elements</span></span>

|<span data-ttu-id="ea3fe-131">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="ea3fe-131">**Element**</span></span>|<span data-ttu-id="ea3fe-132">**Описание**</span><span class="sxs-lookup"><span data-stu-id="ea3fe-132">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ea3fe-133">итемчанжес</span><span class="sxs-lookup"><span data-stu-id="ea3fe-133">ItemChanges</span></span>](itemchanges.md) <br/> |<span data-ttu-id="ea3fe-134">Содержит массив элементов [итемчанже](itemchange.md) , определяющих элементы и обновления, которые необходимо применить к элементам.</span><span class="sxs-lookup"><span data-stu-id="ea3fe-134">Contains an array of [ItemChange](itemchange.md) elements that identify items and the updates to apply to the items.</span></span>  <br/> <span data-ttu-id="ea3fe-135">Ниже приведено выражение XPath для этого элемента:</span><span class="sxs-lookup"><span data-stu-id="ea3fe-135">The following is the XPath expression to this element:</span></span>  <br/>  `/UpdateItem/ItemChanges` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="ea3fe-136">Примечания</span><span class="sxs-lookup"><span data-stu-id="ea3fe-136">Remarks</span></span>

<span data-ttu-id="ea3fe-137">В элементе **итемчанже** можно использовать только один элемент [ItemId](itemid.md), [оккурренцеитемид](occurrenceitemid.md)или [рекуррингмастеритемид](recurringmasteritemid.md) .</span><span class="sxs-lookup"><span data-stu-id="ea3fe-137">Only a single [ItemId](itemid.md), [OccurrenceItemId](occurrenceitemid.md), or [RecurringMasterItemId](recurringmasteritemid.md) element can be used in an **ItemChange** element.</span></span> 
  
<span data-ttu-id="ea3fe-138">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="ea3fe-138">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ea3fe-139">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="ea3fe-139">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ea3fe-140">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="ea3fe-140">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="ea3fe-141">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="ea3fe-141">Schema Name</span></span>  <br/> |<span data-ttu-id="ea3fe-142">Схема Types</span><span class="sxs-lookup"><span data-stu-id="ea3fe-142">Types schema</span></span>  <br/> |
|<span data-ttu-id="ea3fe-143">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="ea3fe-143">Validation File</span></span>  <br/> |<span data-ttu-id="ea3fe-144">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="ea3fe-144">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="ea3fe-145">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="ea3fe-145">Can be Empty</span></span>  <br/> |<span data-ttu-id="ea3fe-146">False</span><span class="sxs-lookup"><span data-stu-id="ea3fe-146">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ea3fe-147">См. также</span><span class="sxs-lookup"><span data-stu-id="ea3fe-147">See also</span></span>

- [<span data-ttu-id="ea3fe-148">Операция UpdateItem</span><span class="sxs-lookup"><span data-stu-id="ea3fe-148">UpdateItem operation</span></span>](updateitem-operation.md)

