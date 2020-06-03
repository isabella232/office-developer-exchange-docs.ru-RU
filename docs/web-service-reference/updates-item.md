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
ms.lasthandoff: 06/03/2020
ms.locfileid: "44456355"
---
# <a name="updates-item"></a><span data-ttu-id="ad989-103">Обновления (элемент)</span><span class="sxs-lookup"><span data-stu-id="ad989-103">Updates (Item)</span></span>

<span data-ttu-id="ad989-104">Элемент **Updates** содержит набор элементов, определяющих Добавление, установку и удаление изменений свойств элемента.</span><span class="sxs-lookup"><span data-stu-id="ad989-104">The **Updates** element contains a set of elements that define append, set, and delete changes to item properties.</span></span> 
  
- [<span data-ttu-id="ad989-105">UpdateItem</span><span class="sxs-lookup"><span data-stu-id="ad989-105">UpdateItem</span></span>](updateitem.md)
  
- [<span data-ttu-id="ad989-106">итемчанжес</span><span class="sxs-lookup"><span data-stu-id="ad989-106">ItemChanges</span></span>](itemchanges.md)
  
- [<span data-ttu-id="ad989-107">ItemChange</span><span class="sxs-lookup"><span data-stu-id="ad989-107">ItemChange</span></span>](itemchange.md)
  
- [<span data-ttu-id="ad989-108">Обновления (элемент)</span><span class="sxs-lookup"><span data-stu-id="ad989-108">Updates (Item)</span></span>](updates-item.md)
  
```xml
<Updates>
   <AppendToItemField/>
   <SetItemField/>
   <DeleteItemField/>
</Updates>
```

<span data-ttu-id="ad989-109">**нонемптяррайофитемчанжедескриптионстипе**</span><span class="sxs-lookup"><span data-stu-id="ad989-109">**NonEmptyArrayOfItemChangeDescriptionsType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="ad989-110">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="ad989-110">Attributes and elements</span></span>

<span data-ttu-id="ad989-111">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="ad989-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ad989-112">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="ad989-112">Attributes</span></span>

<span data-ttu-id="ad989-113">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="ad989-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ad989-114">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="ad989-114">Child elements</span></span>

|<span data-ttu-id="ad989-115">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="ad989-115">**Element**</span></span>|<span data-ttu-id="ad989-116">**Описание**</span><span class="sxs-lookup"><span data-stu-id="ad989-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ad989-117">аппендтоитемфиелд</span><span class="sxs-lookup"><span data-stu-id="ad989-117">AppendToItemField</span></span>](appendtoitemfield.md) <br/> |<span data-ttu-id="ad989-118">Представляет данные, добавляемые к одному свойству элемента во время [операции UpdateItem](updateitem-operation.md).</span><span class="sxs-lookup"><span data-stu-id="ad989-118">Represents data to append to a single property of an item during an [UpdateItem operation](updateitem-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="ad989-119">сетитемфиелд</span><span class="sxs-lookup"><span data-stu-id="ad989-119">SetItemField</span></span>](setitemfield.md) <br/> |<span data-ttu-id="ad989-120">Представляет обновление одного свойства элемента в [операции UpdateItem](updateitem-operation.md).</span><span class="sxs-lookup"><span data-stu-id="ad989-120">Represents an update to a single property of an item in an [UpdateItem operation](updateitem-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="ad989-121">делетеитемфиелд</span><span class="sxs-lookup"><span data-stu-id="ad989-121">DeleteItemField</span></span>](deleteitemfield.md) <br/> |<span data-ttu-id="ad989-122">Представляет операцию удаления данного свойства из элемента во время [операции UpdateItem](updateitem-operation.md).</span><span class="sxs-lookup"><span data-stu-id="ad989-122">Represents an operation to delete a given property from an item during an [UpdateItem operation](updateitem-operation.md).</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="ad989-123">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="ad989-123">Parent elements</span></span>

|<span data-ttu-id="ad989-124">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="ad989-124">**Element**</span></span>|<span data-ttu-id="ad989-125">**Описание**</span><span class="sxs-lookup"><span data-stu-id="ad989-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ad989-126">ItemChange</span><span class="sxs-lookup"><span data-stu-id="ad989-126">ItemChange</span></span>](itemchange.md) <br/> |<span data-ttu-id="ad989-127">Содержит идентификатор элемента и обновления, применяемые к элементу.</span><span class="sxs-lookup"><span data-stu-id="ad989-127">Contains an item identifier and the updates to apply to the item.</span></span>  <br/> <span data-ttu-id="ad989-128">Ниже приведено выражение XPath для этого элемента:`/UpdateItem/ItemChanges/ItemChange[i]`</span><span class="sxs-lookup"><span data-stu-id="ad989-128">The following is the XPath expression to this element:  `/UpdateItem/ItemChanges/ItemChange[i]`</span></span> <br/> |
   
## <a name="remarks"></a><span data-ttu-id="ad989-129">Примечания</span><span class="sxs-lookup"><span data-stu-id="ad989-129">Remarks</span></span>

<span data-ttu-id="ad989-130">Обновления, определенные этим элементом, выполняются над элементом, идентифицируемым элементами [ItemId](itemid.md), [оккурренцеитемид](occurrenceitemid.md)или [рекуррингмастеритемид](recurringmasteritemid.md) .</span><span class="sxs-lookup"><span data-stu-id="ad989-130">The updates that are defined by this element are performed on the item that is identified by the [ItemId](itemid.md), [OccurrenceItemId](occurrenceitemid.md), or [RecurringMasterItemId](recurringmasteritemid.md) elements.</span></span> 
  
<span data-ttu-id="ad989-131">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="ad989-131">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ad989-132">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="ad989-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ad989-133">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="ad989-133">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="ad989-134">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="ad989-134">Schema Name</span></span>  <br/> |<span data-ttu-id="ad989-135">Схема Types</span><span class="sxs-lookup"><span data-stu-id="ad989-135">types schema</span></span>  <br/> |
|<span data-ttu-id="ad989-136">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="ad989-136">Validation File</span></span>  <br/> |<span data-ttu-id="ad989-137">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="ad989-137">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="ad989-138">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="ad989-138">Can be Empty</span></span>  <br/> |<span data-ttu-id="ad989-139">False</span><span class="sxs-lookup"><span data-stu-id="ad989-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ad989-140">См. также</span><span class="sxs-lookup"><span data-stu-id="ad989-140">See also</span></span>

- [<span data-ttu-id="ad989-141">Операция UpdateItem</span><span class="sxs-lookup"><span data-stu-id="ad989-141">UpdateItem operation</span></span>](updateitem-operation.md)
- [<span data-ttu-id="ad989-142">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="ad989-142">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

