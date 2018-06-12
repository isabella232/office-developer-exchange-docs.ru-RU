---
title: SortOrder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SortOrder
api_type:
- schema
ms.assetid: c2413f0b-8c03-46ae-9990-13338b3c53a6
description: Элемент SortOrder определяет способ сортировки в запросе FindItem или FindConversation элементов.
ms.openlocfilehash: e20e5eab7972616c90079786abd78a0f7fedfebe
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19835519"
---
# <a name="sortorder"></a><span data-ttu-id="ddf7b-103">SortOrder</span><span class="sxs-lookup"><span data-stu-id="ddf7b-103">SortOrder</span></span>

<span data-ttu-id="ddf7b-104">Элемент **SortOrder** определяет способ сортировки в запросе **FindItem** или **FindConversation** элементов.</span><span class="sxs-lookup"><span data-stu-id="ddf7b-104">The **SortOrder** element defines how items are sorted in a **FindItem** or **FindConversation** request.</span></span> 
  
```xml
<SortOrder>
   <FieldOrder/>
</SortOrder>
```

 <span data-ttu-id="ddf7b-105">**NonEmptyArrayOfFieldOrdersType**</span><span class="sxs-lookup"><span data-stu-id="ddf7b-105">**NonEmptyArrayOfFieldOrdersType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ddf7b-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="ddf7b-106">Attributes and elements</span></span>

<span data-ttu-id="ddf7b-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="ddf7b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ddf7b-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="ddf7b-108">Attributes</span></span>

<span data-ttu-id="ddf7b-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="ddf7b-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ddf7b-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="ddf7b-110">Child elements</span></span>

|<span data-ttu-id="ddf7b-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="ddf7b-111">**Element**</span></span>|<span data-ttu-id="ddf7b-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="ddf7b-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ddf7b-113">FieldOrder</span><span class="sxs-lookup"><span data-stu-id="ddf7b-113">FieldOrder</span></span>](fieldorder.md) <br/> |<span data-ttu-id="ddf7b-114">Представляет одно поле, по которому будут отсортированы результаты и задает направление сортировки.</span><span class="sxs-lookup"><span data-stu-id="ddf7b-114">Represents a single field by which to sort results and indicates the direction for the sort.</span></span> <span data-ttu-id="ddf7b-115">Один или несколько из этих элементов могут быть включены.</span><span class="sxs-lookup"><span data-stu-id="ddf7b-115">One or more of these elements may be included.</span></span> <span data-ttu-id="ddf7b-116">Элементы [FieldOrder](fieldorder.md) применяются в порядке, указанном для сортировки.</span><span class="sxs-lookup"><span data-stu-id="ddf7b-116">[FieldOrder](fieldorder.md) elements are applied in the order specified for sorting.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="ddf7b-117">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="ddf7b-117">Parent elements</span></span>

|<span data-ttu-id="ddf7b-118">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="ddf7b-118">**Element**</span></span>|<span data-ttu-id="ddf7b-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="ddf7b-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ddf7b-120">FindItem</span><span class="sxs-lookup"><span data-stu-id="ddf7b-120">FindItem</span></span>](finditem.md) <br/> |<span data-ttu-id="ddf7b-121">Определяет запрос для поиска элементов в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="ddf7b-121">Defines a request to find items in a mailbox.</span></span>  <br/> <span data-ttu-id="ddf7b-122">Ниже приведен выражение XPath для этого элемента.`/FindItem`</span><span class="sxs-lookup"><span data-stu-id="ddf7b-122">The following is the XPath expression to this element:  `/FindItem`</span></span> <br/> |
|[<span data-ttu-id="ddf7b-123">FindConversation</span><span class="sxs-lookup"><span data-stu-id="ddf7b-123">FindConversation</span></span>](findconversation.md) <br/> |<span data-ttu-id="ddf7b-124">Определяет запрос на поиск бесед в почтовый ящик.</span><span class="sxs-lookup"><span data-stu-id="ddf7b-124">Defines a request to find conversations in a mailbox.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="ddf7b-125">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="ddf7b-125">Text value</span></span>

<span data-ttu-id="ddf7b-126">Нет.</span><span class="sxs-lookup"><span data-stu-id="ddf7b-126">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="ddf7b-127">Замечания</span><span class="sxs-lookup"><span data-stu-id="ddf7b-127">Remarks</span></span>

<span data-ttu-id="ddf7b-128">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="ddf7b-128">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ddf7b-129">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="ddf7b-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ddf7b-130">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="ddf7b-130">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="ddf7b-131">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="ddf7b-131">Schema Name</span></span>  <br/> |<span data-ttu-id="ddf7b-132">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="ddf7b-132">Messages schema</span></span>  <br/> |
|<span data-ttu-id="ddf7b-133">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="ddf7b-133">Validation File</span></span>  <br/> |<span data-ttu-id="ddf7b-134">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="ddf7b-134">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="ddf7b-135">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="ddf7b-135">Can be Empty</span></span>  <br/> |<span data-ttu-id="ddf7b-136">False</span><span class="sxs-lookup"><span data-stu-id="ddf7b-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ddf7b-137">См. также</span><span class="sxs-lookup"><span data-stu-id="ddf7b-137">See also</span></span>



[<span data-ttu-id="ddf7b-138">FindItem Operation</span><span class="sxs-lookup"><span data-stu-id="ddf7b-138">FindItem operation</span></span>](finditem-operation.md)
  
[<span data-ttu-id="ddf7b-139">FindConversation Operation</span><span class="sxs-lookup"><span data-stu-id="ddf7b-139">FindConversation operation</span></span>](findconversation-operation.md)


- [<span data-ttu-id="ddf7b-140">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="ddf7b-140">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

