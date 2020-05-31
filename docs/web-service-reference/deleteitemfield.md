---
title: делетеитемфиелд
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
description: Элемент Делетеитемфиелд представляет операцию удаления данного свойства из элемента во время вызова UpdateItem.
ms.openlocfilehash: 571227eece8f717c1bf5da27cfab8ae50dfe3572
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/28/2018
ms.locfileid: "21353884"
---
# <a name="deleteitemfield"></a><span data-ttu-id="cf4a2-103">делетеитемфиелд</span><span class="sxs-lookup"><span data-stu-id="cf4a2-103">DeleteItemField</span></span>

<span data-ttu-id="cf4a2-104">Элемент **делетеитемфиелд** представляет операцию удаления данного свойства из элемента во время вызова UpdateItem.</span><span class="sxs-lookup"><span data-stu-id="cf4a2-104">The **DeleteItemField** element represents an operation to delete a given property from an item during an UpdateItem call.</span></span> 
 
- [<span data-ttu-id="cf4a2-105">UpdateItem</span><span class="sxs-lookup"><span data-stu-id="cf4a2-105">UpdateItem</span></span>](updateitem.md)  
- [<span data-ttu-id="cf4a2-106">итемчанжес</span><span class="sxs-lookup"><span data-stu-id="cf4a2-106">ItemChanges</span></span>](itemchanges.md) 
- [<span data-ttu-id="cf4a2-107">ItemChange</span><span class="sxs-lookup"><span data-stu-id="cf4a2-107">ItemChange</span></span>](itemchange.md) 
- [<span data-ttu-id="cf4a2-108">Обновления (элемент)</span><span class="sxs-lookup"><span data-stu-id="cf4a2-108">Updates (Item)</span></span>](updates-item.md) 
- [<span data-ttu-id="cf4a2-109">делетеитемфиелд</span><span class="sxs-lookup"><span data-stu-id="cf4a2-109">DeleteItemField</span></span>](deleteitemfield.md)
  
```xml
<DeleteItemField>
   <FieldURI/>
</DeleteItemField>
```

```xml
<DeleteItemField>
   <IndexedFieldURI/> 
</DeleteItemField>
```

```xml
<DeleteItemField>
   <ExtendedFieldURI/>
</DeleteItemField>
```

<span data-ttu-id="cf4a2-110">**делетеитемфиелдтипе**</span><span class="sxs-lookup"><span data-stu-id="cf4a2-110">**DeleteItemFieldType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="cf4a2-111">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="cf4a2-111">Attributes and elements</span></span>

<span data-ttu-id="cf4a2-112">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="cf4a2-112">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="cf4a2-113">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="cf4a2-113">Attributes</span></span>

<span data-ttu-id="cf4a2-114">Нет.</span><span class="sxs-lookup"><span data-stu-id="cf4a2-114">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="cf4a2-115">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="cf4a2-115">Child elements</span></span>

|<span data-ttu-id="cf4a2-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="cf4a2-116">**Element**</span></span>|<span data-ttu-id="cf4a2-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="cf4a2-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="cf4a2-118">фиелдури</span><span class="sxs-lookup"><span data-stu-id="cf4a2-118">FieldURI</span></span>](fielduri.md) <br/> |<span data-ttu-id="cf4a2-119">Определяет часто упоминаемые свойства по URI.</span><span class="sxs-lookup"><span data-stu-id="cf4a2-119">Identifies frequently referenced properties by URI.</span></span>  <br/> |
|[<span data-ttu-id="cf4a2-120">индекседфиелдури</span><span class="sxs-lookup"><span data-stu-id="cf4a2-120">IndexedFieldURI</span></span>](indexedfielduri.md) <br/> |<span data-ttu-id="cf4a2-121">Определяет отдельные элементы свойства Dictionary.</span><span class="sxs-lookup"><span data-stu-id="cf4a2-121">Identifies individual members of a dictionary property.</span></span>  <br/> |
|[<span data-ttu-id="cf4a2-122">екстендедфиелдури</span><span class="sxs-lookup"><span data-stu-id="cf4a2-122">ExtendedFieldURI</span></span>](extendedfielduri.md) <br/> |<span data-ttu-id="cf4a2-123">Определяет расширенные свойства MAPI.</span><span class="sxs-lookup"><span data-stu-id="cf4a2-123">Identifies extended MAPI properties.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="cf4a2-124">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="cf4a2-124">Parent elements</span></span>

|<span data-ttu-id="cf4a2-125">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="cf4a2-125">**Element**</span></span>|<span data-ttu-id="cf4a2-126">**Описание**</span><span class="sxs-lookup"><span data-stu-id="cf4a2-126">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="cf4a2-127">Обновления (элемент)</span><span class="sxs-lookup"><span data-stu-id="cf4a2-127">Updates (Item)</span></span>](updates-item.md) <br/> |<span data-ttu-id="cf4a2-128">Содержит набор элементов, определяющих Добавление, установку и удаление изменений свойств элемента.</span><span class="sxs-lookup"><span data-stu-id="cf4a2-128">Contains a set of elements that define append, set, and delete changes to item properties.</span></span>  <br/><br/><span data-ttu-id="cf4a2-129">Ниже приведено выражение XPath для этого элемента:</span><span class="sxs-lookup"><span data-stu-id="cf4a2-129">The following is the XPath expression to this element:</span></span><br/>`/UpdateItem/ItemChanges/ItemChange[i]/Updates` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="cf4a2-130">Примечания</span><span class="sxs-lookup"><span data-stu-id="cf4a2-130">Remarks</span></span>

<span data-ttu-id="cf4a2-131">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="cf4a2-131">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="cf4a2-132">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="cf4a2-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="cf4a2-133">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="cf4a2-133">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="cf4a2-134">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="cf4a2-134">Schema Name</span></span>  <br/> |<span data-ttu-id="cf4a2-135">Схема Types</span><span class="sxs-lookup"><span data-stu-id="cf4a2-135">types schema</span></span>  <br/> |
|<span data-ttu-id="cf4a2-136">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="cf4a2-136">Validation File</span></span>  <br/> |<span data-ttu-id="cf4a2-137">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="cf4a2-137">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="cf4a2-138">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="cf4a2-138">Can be Empty</span></span>  <br/> |<span data-ttu-id="cf4a2-139">False</span><span class="sxs-lookup"><span data-stu-id="cf4a2-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="cf4a2-140">См. также</span><span class="sxs-lookup"><span data-stu-id="cf4a2-140">See also</span></span>

- [<span data-ttu-id="cf4a2-141">Операция UpdateItem</span><span class="sxs-lookup"><span data-stu-id="cf4a2-141">UpdateItem operation</span></span>](updateitem-operation.md)

