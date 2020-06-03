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
ms.openlocfilehash: e6f5ee8a1130d7c040f3ddd94021eff6d4a758b0
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44455676"
---
# <a name="deleteitemfield"></a><span data-ttu-id="9c2a1-103">делетеитемфиелд</span><span class="sxs-lookup"><span data-stu-id="9c2a1-103">DeleteItemField</span></span>

<span data-ttu-id="9c2a1-104">Элемент **делетеитемфиелд** представляет операцию удаления данного свойства из элемента во время вызова UpdateItem.</span><span class="sxs-lookup"><span data-stu-id="9c2a1-104">The **DeleteItemField** element represents an operation to delete a given property from an item during an UpdateItem call.</span></span> 
 
- [<span data-ttu-id="9c2a1-105">UpdateItem</span><span class="sxs-lookup"><span data-stu-id="9c2a1-105">UpdateItem</span></span>](updateitem.md)  
- [<span data-ttu-id="9c2a1-106">итемчанжес</span><span class="sxs-lookup"><span data-stu-id="9c2a1-106">ItemChanges</span></span>](itemchanges.md) 
- [<span data-ttu-id="9c2a1-107">ItemChange</span><span class="sxs-lookup"><span data-stu-id="9c2a1-107">ItemChange</span></span>](itemchange.md) 
- [<span data-ttu-id="9c2a1-108">Обновления (элемент)</span><span class="sxs-lookup"><span data-stu-id="9c2a1-108">Updates (Item)</span></span>](updates-item.md) 
- [<span data-ttu-id="9c2a1-109">делетеитемфиелд</span><span class="sxs-lookup"><span data-stu-id="9c2a1-109">DeleteItemField</span></span>](deleteitemfield.md)
  
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

<span data-ttu-id="9c2a1-110">**делетеитемфиелдтипе**</span><span class="sxs-lookup"><span data-stu-id="9c2a1-110">**DeleteItemFieldType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="9c2a1-111">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="9c2a1-111">Attributes and elements</span></span>

<span data-ttu-id="9c2a1-112">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="9c2a1-112">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9c2a1-113">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="9c2a1-113">Attributes</span></span>

<span data-ttu-id="9c2a1-114">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="9c2a1-114">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9c2a1-115">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="9c2a1-115">Child elements</span></span>

|<span data-ttu-id="9c2a1-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="9c2a1-116">**Element**</span></span>|<span data-ttu-id="9c2a1-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="9c2a1-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9c2a1-118">фиелдури</span><span class="sxs-lookup"><span data-stu-id="9c2a1-118">FieldURI</span></span>](fielduri.md) <br/> |<span data-ttu-id="9c2a1-119">Определяет часто упоминаемые свойства по URI.</span><span class="sxs-lookup"><span data-stu-id="9c2a1-119">Identifies frequently referenced properties by URI.</span></span>  <br/> |
|[<span data-ttu-id="9c2a1-120">индекседфиелдури</span><span class="sxs-lookup"><span data-stu-id="9c2a1-120">IndexedFieldURI</span></span>](indexedfielduri.md) <br/> |<span data-ttu-id="9c2a1-121">Определяет отдельные элементы свойства Dictionary.</span><span class="sxs-lookup"><span data-stu-id="9c2a1-121">Identifies individual members of a dictionary property.</span></span>  <br/> |
|[<span data-ttu-id="9c2a1-122">екстендедфиелдури</span><span class="sxs-lookup"><span data-stu-id="9c2a1-122">ExtendedFieldURI</span></span>](extendedfielduri.md) <br/> |<span data-ttu-id="9c2a1-123">Определяет расширенные свойства MAPI.</span><span class="sxs-lookup"><span data-stu-id="9c2a1-123">Identifies extended MAPI properties.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="9c2a1-124">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="9c2a1-124">Parent elements</span></span>

|<span data-ttu-id="9c2a1-125">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="9c2a1-125">**Element**</span></span>|<span data-ttu-id="9c2a1-126">**Описание**</span><span class="sxs-lookup"><span data-stu-id="9c2a1-126">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9c2a1-127">Обновления (элемент)</span><span class="sxs-lookup"><span data-stu-id="9c2a1-127">Updates (Item)</span></span>](updates-item.md) <br/> |<span data-ttu-id="9c2a1-128">Содержит набор элементов, определяющих Добавление, установку и удаление изменений свойств элемента.</span><span class="sxs-lookup"><span data-stu-id="9c2a1-128">Contains a set of elements that define append, set, and delete changes to item properties.</span></span>  <br/><br/><span data-ttu-id="9c2a1-129">Ниже приведено выражение XPath для этого элемента:</span><span class="sxs-lookup"><span data-stu-id="9c2a1-129">The following is the XPath expression to this element:</span></span><br/>`/UpdateItem/ItemChanges/ItemChange[i]/Updates` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="9c2a1-130">Примечания</span><span class="sxs-lookup"><span data-stu-id="9c2a1-130">Remarks</span></span>

<span data-ttu-id="9c2a1-131">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="9c2a1-131">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9c2a1-132">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="9c2a1-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9c2a1-133">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="9c2a1-133">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="9c2a1-134">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="9c2a1-134">Schema Name</span></span>  <br/> |<span data-ttu-id="9c2a1-135">Схема Types</span><span class="sxs-lookup"><span data-stu-id="9c2a1-135">types schema</span></span>  <br/> |
|<span data-ttu-id="9c2a1-136">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="9c2a1-136">Validation File</span></span>  <br/> |<span data-ttu-id="9c2a1-137">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="9c2a1-137">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="9c2a1-138">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="9c2a1-138">Can be Empty</span></span>  <br/> |<span data-ttu-id="9c2a1-139">False</span><span class="sxs-lookup"><span data-stu-id="9c2a1-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9c2a1-140">См. также</span><span class="sxs-lookup"><span data-stu-id="9c2a1-140">See also</span></span>

- [<span data-ttu-id="9c2a1-141">Операция UpdateItem</span><span class="sxs-lookup"><span data-stu-id="9c2a1-141">UpdateItem operation</span></span>](updateitem-operation.md)

