---
title: DeleteItemField
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DeleteItemField
api_type:
- schema
ms.assetid: 3893be6a-49a7-49f6-bf53-c7f819ec3f87
description: Элемент DeleteItemField представляет операцию для удаления заданного свойства из элемента во время вызова UpdateItem.
ms.openlocfilehash: 2388bd10379211a31890b7c4f27920431ce444c8
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762044"
---
# <a name="deleteitemfield"></a><span data-ttu-id="c71de-103">DeleteItemField</span><span class="sxs-lookup"><span data-stu-id="c71de-103">DeleteItemField</span></span>

<span data-ttu-id="c71de-104">Элемент **DeleteItemField** представляет операцию для удаления заданного свойства из элемента во время вызова UpdateItem.</span><span class="sxs-lookup"><span data-stu-id="c71de-104">The **DeleteItemField** element represents an operation to delete a given property from an item during an UpdateItem call.</span></span> 
 
- [<span data-ttu-id="c71de-105">UpdateItem</span><span class="sxs-lookup"><span data-stu-id="c71de-105">UpdateItem</span></span>](updateitem.md)  
- [<span data-ttu-id="c71de-106">ItemChanges</span><span class="sxs-lookup"><span data-stu-id="c71de-106">ItemChanges</span></span>](itemchanges.md) 
- [<span data-ttu-id="c71de-107">ItemChange</span><span class="sxs-lookup"><span data-stu-id="c71de-107">ItemChange</span></span>](itemchange.md) 
- [<span data-ttu-id="c71de-108">Обновления (элемент)</span><span class="sxs-lookup"><span data-stu-id="c71de-108">Updates (Item)</span></span>](updates-item.md) 
- [<span data-ttu-id="c71de-109">DeleteItemField</span><span class="sxs-lookup"><span data-stu-id="c71de-109">DeleteItemField</span></span>](deleteitemfield.md)
  
```xml
<DeleteItemField>
   <FieldURI/>
</DeleteItemField>
```

 <span data-ttu-id="c71de-110">**DeleteItemFieldType**</span><span class="sxs-lookup"><span data-stu-id="c71de-110">**DeleteItemFieldType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c71de-111">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="c71de-111">Attributes and elements</span></span>

<span data-ttu-id="c71de-112">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="c71de-112">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c71de-113">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="c71de-113">Attributes</span></span>

<span data-ttu-id="c71de-114">Нет.</span><span class="sxs-lookup"><span data-stu-id="c71de-114">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c71de-115">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="c71de-115">Child elements</span></span>

|<span data-ttu-id="c71de-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="c71de-116">**Element**</span></span>|<span data-ttu-id="c71de-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="c71de-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c71de-118">FieldURI</span><span class="sxs-lookup"><span data-stu-id="c71de-118">FieldURI</span></span>](fielduri.md) <br/> |<span data-ttu-id="c71de-119">Идентифицирует часто упоминаемые свойства по URI.</span><span class="sxs-lookup"><span data-stu-id="c71de-119">Identifies frequently referenced properties by URI.</span></span>  <br/> |
|[<span data-ttu-id="c71de-120">IndexedFieldURI</span><span class="sxs-lookup"><span data-stu-id="c71de-120">IndexedFieldURI</span></span>](indexedfielduri.md) <br/> |<span data-ttu-id="c71de-121">Идентифицирует отдельным членам свойства словаря.</span><span class="sxs-lookup"><span data-stu-id="c71de-121">Identifies individual members of a dictionary property.</span></span>  <br/> |
|[<span data-ttu-id="c71de-122">ExtendedFieldURI</span><span class="sxs-lookup"><span data-stu-id="c71de-122">ExtendedFieldURI</span></span>](extendedfielduri.md) <br/> |<span data-ttu-id="c71de-123">Задает расширенные свойства MAPI.</span><span class="sxs-lookup"><span data-stu-id="c71de-123">Identifies extended MAPI properties.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="c71de-124">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="c71de-124">Parent elements</span></span>

|<span data-ttu-id="c71de-125">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="c71de-125">**Element**</span></span>|<span data-ttu-id="c71de-126">**Описание**</span><span class="sxs-lookup"><span data-stu-id="c71de-126">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c71de-127">Обновления (элемент)</span><span class="sxs-lookup"><span data-stu-id="c71de-127">Updates (Item)</span></span>](updates-item.md) <br/> |<span data-ttu-id="c71de-128">Содержит набор элементов, которые определяют добавьте, Установка и удаление изменения свойств элемента.</span><span class="sxs-lookup"><span data-stu-id="c71de-128">Contains a set of elements that define append, set, and delete changes to item properties.</span></span>  <br/><br/><span data-ttu-id="c71de-129">Ниже приведен выражение XPath для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="c71de-129">The following is the XPath expression to this element:</span></span><br/>`/UpdateItem/ItemChanges/ItemChange[i]/Updates` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="c71de-130">Замечания</span><span class="sxs-lookup"><span data-stu-id="c71de-130">Remarks</span></span>

<span data-ttu-id="c71de-131">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="c71de-131">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c71de-132">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="c71de-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c71de-133">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="c71de-133">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="c71de-134">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="c71de-134">Schema Name</span></span>  <br/> |<span data-ttu-id="c71de-135">типы схемы</span><span class="sxs-lookup"><span data-stu-id="c71de-135">types schema</span></span>  <br/> |
|<span data-ttu-id="c71de-136">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="c71de-136">Validation File</span></span>  <br/> |<span data-ttu-id="c71de-137">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="c71de-137">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="c71de-138">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="c71de-138">Can be Empty</span></span>  <br/> |<span data-ttu-id="c71de-139">False</span><span class="sxs-lookup"><span data-stu-id="c71de-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c71de-140">См. также</span><span class="sxs-lookup"><span data-stu-id="c71de-140">See also</span></span>

- [<span data-ttu-id="c71de-141">UpdateItem Operation</span><span class="sxs-lookup"><span data-stu-id="c71de-141">UpdateItem operation</span></span>](updateitem-operation.md)

