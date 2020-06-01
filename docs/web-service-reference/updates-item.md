---
title: Обновления (элемент)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Updates
api_type:
- schema
ms.assetid: 5c1a855e-390d-4713-9d10-6e86ca392814
description: Элемент Updates содержит набор элементов, определяющих Добавление, установку и удаление изменений свойств элемента.
ms.openlocfilehash: 6902ea4d3d3d9adc074745d5642cdfa6d91a9163
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44456355"
---
# <a name="updates-item"></a><span data-ttu-id="a1d98-103">Обновления (элемент)</span><span class="sxs-lookup"><span data-stu-id="a1d98-103">Updates (Item)</span></span>

<span data-ttu-id="a1d98-104">Элемент **Updates** содержит набор элементов, определяющих Добавление, установку и удаление изменений свойств элемента.</span><span class="sxs-lookup"><span data-stu-id="a1d98-104">The **Updates** element contains a set of elements that define append, set, and delete changes to item properties.</span></span> 
  
- [<span data-ttu-id="a1d98-105">UpdateItem</span><span class="sxs-lookup"><span data-stu-id="a1d98-105">UpdateItem</span></span>](updateitem.md)
  
- [<span data-ttu-id="a1d98-106">итемчанжес</span><span class="sxs-lookup"><span data-stu-id="a1d98-106">ItemChanges</span></span>](itemchanges.md)
  
- [<span data-ttu-id="a1d98-107">ItemChange</span><span class="sxs-lookup"><span data-stu-id="a1d98-107">ItemChange</span></span>](itemchange.md)
  
- [<span data-ttu-id="a1d98-108">Обновления (элемент)</span><span class="sxs-lookup"><span data-stu-id="a1d98-108">Updates (Item)</span></span>](updates-item.md)
  
```xml
<Updates>
   <AppendToItemField/>
   <SetItemField/>
   <DeleteItemField/>
</Updates>
```

<span data-ttu-id="a1d98-109">**нонемптяррайофитемчанжедескриптионстипе**</span><span class="sxs-lookup"><span data-stu-id="a1d98-109">**NonEmptyArrayOfItemChangeDescriptionsType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="a1d98-110">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="a1d98-110">Attributes and elements</span></span>

<span data-ttu-id="a1d98-111">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="a1d98-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a1d98-112">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="a1d98-112">Attributes</span></span>

<span data-ttu-id="a1d98-113">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="a1d98-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a1d98-114">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="a1d98-114">Child elements</span></span>

|<span data-ttu-id="a1d98-115">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="a1d98-115">**Element**</span></span>|<span data-ttu-id="a1d98-116">**Описание**</span><span class="sxs-lookup"><span data-stu-id="a1d98-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a1d98-117">аппендтоитемфиелд</span><span class="sxs-lookup"><span data-stu-id="a1d98-117">AppendToItemField</span></span>](appendtoitemfield.md) <br/> |<span data-ttu-id="a1d98-118">Представляет данные, добавляемые к одному свойству элемента во время [операции UpdateItem](updateitem-operation.md).</span><span class="sxs-lookup"><span data-stu-id="a1d98-118">Represents data to append to a single property of an item during an [UpdateItem operation](updateitem-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="a1d98-119">сетитемфиелд</span><span class="sxs-lookup"><span data-stu-id="a1d98-119">SetItemField</span></span>](setitemfield.md) <br/> |<span data-ttu-id="a1d98-120">Представляет обновление одного свойства элемента в [операции UpdateItem](updateitem-operation.md).</span><span class="sxs-lookup"><span data-stu-id="a1d98-120">Represents an update to a single property of an item in an [UpdateItem operation](updateitem-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="a1d98-121">делетеитемфиелд</span><span class="sxs-lookup"><span data-stu-id="a1d98-121">DeleteItemField</span></span>](deleteitemfield.md) <br/> |<span data-ttu-id="a1d98-122">Представляет операцию удаления данного свойства из элемента во время [операции UpdateItem](updateitem-operation.md).</span><span class="sxs-lookup"><span data-stu-id="a1d98-122">Represents an operation to delete a given property from an item during an [UpdateItem operation](updateitem-operation.md).</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="a1d98-123">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="a1d98-123">Parent elements</span></span>

|<span data-ttu-id="a1d98-124">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="a1d98-124">**Element**</span></span>|<span data-ttu-id="a1d98-125">**Описание**</span><span class="sxs-lookup"><span data-stu-id="a1d98-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a1d98-126">ItemChange</span><span class="sxs-lookup"><span data-stu-id="a1d98-126">ItemChange</span></span>](itemchange.md) <br/> |<span data-ttu-id="a1d98-127">Содержит идентификатор элемента и обновления, применяемые к элементу.</span><span class="sxs-lookup"><span data-stu-id="a1d98-127">Contains an item identifier and the updates to apply to the item.</span></span>  <br/> <span data-ttu-id="a1d98-128">Ниже приведено выражение XPath для этого элемента:`/UpdateItem/ItemChanges/ItemChange[i]`</span><span class="sxs-lookup"><span data-stu-id="a1d98-128">The following is the XPath expression to this element:  `/UpdateItem/ItemChanges/ItemChange[i]`</span></span> <br/> |
   
## <a name="remarks"></a><span data-ttu-id="a1d98-129">Примечания</span><span class="sxs-lookup"><span data-stu-id="a1d98-129">Remarks</span></span>

<span data-ttu-id="a1d98-130">Обновления, определенные этим элементом, выполняются над элементом, идентифицируемым элементами [ItemId](itemid.md), [оккурренцеитемид](occurrenceitemid.md)или [рекуррингмастеритемид](recurringmasteritemid.md) .</span><span class="sxs-lookup"><span data-stu-id="a1d98-130">The updates that are defined by this element are performed on the item that is identified by the [ItemId](itemid.md), [OccurrenceItemId](occurrenceitemid.md), or [RecurringMasterItemId](recurringmasteritemid.md) elements.</span></span> 
  
<span data-ttu-id="a1d98-131">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="a1d98-131">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a1d98-132">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="a1d98-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a1d98-133">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="a1d98-133">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="a1d98-134">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="a1d98-134">Schema Name</span></span>  <br/> |<span data-ttu-id="a1d98-135">Схема Types</span><span class="sxs-lookup"><span data-stu-id="a1d98-135">types schema</span></span>  <br/> |
|<span data-ttu-id="a1d98-136">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="a1d98-136">Validation File</span></span>  <br/> |<span data-ttu-id="a1d98-137">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="a1d98-137">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="a1d98-138">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="a1d98-138">Can be Empty</span></span>  <br/> |<span data-ttu-id="a1d98-139">False</span><span class="sxs-lookup"><span data-stu-id="a1d98-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a1d98-140">См. также</span><span class="sxs-lookup"><span data-stu-id="a1d98-140">See also</span></span>

- [<span data-ttu-id="a1d98-141">Операция UpdateItem</span><span class="sxs-lookup"><span data-stu-id="a1d98-141">UpdateItem operation</span></span>](updateitem-operation.md)
- [<span data-ttu-id="a1d98-142">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="a1d98-142">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

