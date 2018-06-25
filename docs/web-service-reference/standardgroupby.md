---
title: StandardGroupBy
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- StandardGroupBy
api_type:
- schema
ms.assetid: 04a84f71-b7eb-44dc-ac2c-ed504b52c463
description: Элемент StandardGroupBy представляет стандартный группировки и сбор механизмы для группированных FindItem операции.
ms.openlocfilehash: 8e2ec72a79ebafc2e5757d6dcebb27c0c53ec0b5
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835542"
---
# <a name="standardgroupby"></a><span data-ttu-id="6de63-103">StandardGroupBy</span><span class="sxs-lookup"><span data-stu-id="6de63-103">StandardGroupBy</span></span>

<span data-ttu-id="6de63-104">Элемент **StandardGroupBy** представляет стандартный группировки и сбор механизмы для группированных FindItem операции.</span><span class="sxs-lookup"><span data-stu-id="6de63-104">The **StandardGroupBy** element represents the standard grouping and aggregating mechanisms for a grouped FindItem operation.</span></span> 
  
[<span data-ttu-id="6de63-105">FindItem</span><span class="sxs-lookup"><span data-stu-id="6de63-105">FindItem</span></span>](finditem.md)
  
[<span data-ttu-id="6de63-106">DistinguishedGroupBy</span><span class="sxs-lookup"><span data-stu-id="6de63-106">DistinguishedGroupBy</span></span>](distinguishedgroupby.md)
  
[<span data-ttu-id="6de63-107">StandardGroupBy</span><span class="sxs-lookup"><span data-stu-id="6de63-107">StandardGroupBy</span></span>](standardgroupby.md)
  
```xml
<StandardGroupBy/>
```

 <span data-ttu-id="6de63-108">**StandardGroupByType**</span><span class="sxs-lookup"><span data-stu-id="6de63-108">**StandardGroupByType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6de63-109">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="6de63-109">Attributes and elements</span></span>

<span data-ttu-id="6de63-110">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="6de63-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6de63-111">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="6de63-111">Attributes</span></span>

<span data-ttu-id="6de63-112">Нет.</span><span class="sxs-lookup"><span data-stu-id="6de63-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6de63-113">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="6de63-113">Child elements</span></span>

<span data-ttu-id="6de63-114">Нет.</span><span class="sxs-lookup"><span data-stu-id="6de63-114">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="6de63-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="6de63-115">Parent elements</span></span>

|<span data-ttu-id="6de63-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="6de63-116">**Element**</span></span>|<span data-ttu-id="6de63-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="6de63-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6de63-118">DistinguishedGroupBy</span><span class="sxs-lookup"><span data-stu-id="6de63-118">DistinguishedGroupBy</span></span>](distinguishedgroupby.md) <br/> |<span data-ttu-id="6de63-119">Содержит стандартные группы для запросов FindItem.</span><span class="sxs-lookup"><span data-stu-id="6de63-119">Provides standard groupings for FindItem queries.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="6de63-120">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="6de63-120">Text value</span></span>

<span data-ttu-id="6de63-121">Текстовое значение является обязательным.</span><span class="sxs-lookup"><span data-stu-id="6de63-121">A text value is required.</span></span> <span data-ttu-id="6de63-122">Только одно значение, которое может использоваться для этого элемента — **ConversationTopic**.</span><span class="sxs-lookup"><span data-stu-id="6de63-122">The only value that can be used for this element is **ConversationTopic**.</span></span> <span data-ttu-id="6de63-123">**ConversationTopic** группы сообщений: ConversationTopic и статистические выражения на элемент: DateTimeReceived (максимум).</span><span class="sxs-lookup"><span data-stu-id="6de63-123">**ConversationTopic** groups by message:ConversationTopic and aggregates on item:DateTimeReceived (maximum).</span></span> <span data-ttu-id="6de63-124">Дополнительные сведения о объединение можно [AggregateOn](aggregateon.md).</span><span class="sxs-lookup"><span data-stu-id="6de63-124">For more information about aggregation, see [AggregateOn](aggregateon.md).</span></span>
  
## <a name="remarks"></a><span data-ttu-id="6de63-125">Замечания</span><span class="sxs-lookup"><span data-stu-id="6de63-125">Remarks</span></span>

<span data-ttu-id="6de63-126">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="6de63-126">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6de63-127">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="6de63-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6de63-128">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="6de63-128">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="6de63-129">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="6de63-129">Schema Name</span></span>  <br/> |<span data-ttu-id="6de63-130">Схема Types</span><span class="sxs-lookup"><span data-stu-id="6de63-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="6de63-131">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="6de63-131">Validation File</span></span>  <br/> |<span data-ttu-id="6de63-132">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="6de63-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="6de63-133">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="6de63-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="6de63-134">False</span><span class="sxs-lookup"><span data-stu-id="6de63-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6de63-135">См. также</span><span class="sxs-lookup"><span data-stu-id="6de63-135">See also</span></span>



[<span data-ttu-id="6de63-136">FindItem Operation</span><span class="sxs-lookup"><span data-stu-id="6de63-136">FindItem operation</span></span>](finditem-operation.md)
  
[<span data-ttu-id="6de63-137">FindItem</span><span class="sxs-lookup"><span data-stu-id="6de63-137">FindItem</span></span>](finditem.md)


[<span data-ttu-id="6de63-138">Поиск элементов</span><span class="sxs-lookup"><span data-stu-id="6de63-138">Finding Items</span></span>](http://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)

