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
description: Элемент SortOrder определяет порядок сортировки элементов в запросе FindItem или FindConversation.
ms.openlocfilehash: e20e5eab7972616c90079786abd78a0f7fedfebe
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835519"
---
# <a name="sortorder"></a><span data-ttu-id="b7e89-103">SortOrder</span><span class="sxs-lookup"><span data-stu-id="b7e89-103">SortOrder</span></span>

<span data-ttu-id="b7e89-104">Элемент **SortOrder** определяет порядок сортировки элементов в запросе **FindItem** или **FindConversation** .</span><span class="sxs-lookup"><span data-stu-id="b7e89-104">The **SortOrder** element defines how items are sorted in a **FindItem** or **FindConversation** request.</span></span> 
  
```xml
<SortOrder>
   <FieldOrder/>
</SortOrder>
```

 <span data-ttu-id="b7e89-105">**нонемптяррайоффиелдордерстипе**</span><span class="sxs-lookup"><span data-stu-id="b7e89-105">**NonEmptyArrayOfFieldOrdersType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b7e89-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="b7e89-106">Attributes and elements</span></span>

<span data-ttu-id="b7e89-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="b7e89-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b7e89-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="b7e89-108">Attributes</span></span>

<span data-ttu-id="b7e89-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="b7e89-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b7e89-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="b7e89-110">Child elements</span></span>

|<span data-ttu-id="b7e89-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="b7e89-111">**Element**</span></span>|<span data-ttu-id="b7e89-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="b7e89-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b7e89-113">фиелдордер</span><span class="sxs-lookup"><span data-stu-id="b7e89-113">FieldOrder</span></span>](fieldorder.md) <br/> |<span data-ttu-id="b7e89-114">Представляет одно поле для сортировки результатов и указывает направление сортировки.</span><span class="sxs-lookup"><span data-stu-id="b7e89-114">Represents a single field by which to sort results and indicates the direction for the sort.</span></span> <span data-ttu-id="b7e89-115">Можно включить один или несколько из этих элементов.</span><span class="sxs-lookup"><span data-stu-id="b7e89-115">One or more of these elements may be included.</span></span> <span data-ttu-id="b7e89-116">Элементы [фиелдордер](fieldorder.md) применяются в порядке, указанном для сортировки.</span><span class="sxs-lookup"><span data-stu-id="b7e89-116">[FieldOrder](fieldorder.md) elements are applied in the order specified for sorting.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="b7e89-117">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="b7e89-117">Parent elements</span></span>

|<span data-ttu-id="b7e89-118">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="b7e89-118">**Element**</span></span>|<span data-ttu-id="b7e89-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="b7e89-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b7e89-120">FindItem</span><span class="sxs-lookup"><span data-stu-id="b7e89-120">FindItem</span></span>](finditem.md) <br/> |<span data-ttu-id="b7e89-121">Определяет запрос на поиск элементов в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="b7e89-121">Defines a request to find items in a mailbox.</span></span>  <br/> <span data-ttu-id="b7e89-122">Ниже приведено выражение XPath для этого элемента:`/FindItem`</span><span class="sxs-lookup"><span data-stu-id="b7e89-122">The following is the XPath expression to this element:  `/FindItem`</span></span> <br/> |
|[<span data-ttu-id="b7e89-123">FindConversation</span><span class="sxs-lookup"><span data-stu-id="b7e89-123">FindConversation</span></span>](findconversation.md) <br/> |<span data-ttu-id="b7e89-124">Определяет запрос на поиск бесед в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="b7e89-124">Defines a request to find conversations in a mailbox.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="b7e89-125">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="b7e89-125">Text value</span></span>

<span data-ttu-id="b7e89-126">Нет.</span><span class="sxs-lookup"><span data-stu-id="b7e89-126">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="b7e89-127">Примечания</span><span class="sxs-lookup"><span data-stu-id="b7e89-127">Remarks</span></span>

<span data-ttu-id="b7e89-128">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="b7e89-128">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b7e89-129">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="b7e89-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b7e89-130">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="b7e89-130">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="b7e89-131">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="b7e89-131">Schema Name</span></span>  <br/> |<span data-ttu-id="b7e89-132">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="b7e89-132">Messages schema</span></span>  <br/> |
|<span data-ttu-id="b7e89-133">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="b7e89-133">Validation File</span></span>  <br/> |<span data-ttu-id="b7e89-134">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="b7e89-134">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="b7e89-135">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="b7e89-135">Can be Empty</span></span>  <br/> |<span data-ttu-id="b7e89-136">False</span><span class="sxs-lookup"><span data-stu-id="b7e89-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b7e89-137">См. также</span><span class="sxs-lookup"><span data-stu-id="b7e89-137">See also</span></span>



[<span data-ttu-id="b7e89-138">Операция FindItem</span><span class="sxs-lookup"><span data-stu-id="b7e89-138">FindItem operation</span></span>](finditem-operation.md)
  
[<span data-ttu-id="b7e89-139">Операция FindConversation</span><span class="sxs-lookup"><span data-stu-id="b7e89-139">FindConversation operation</span></span>](findconversation-operation.md)


- [<span data-ttu-id="b7e89-140">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="b7e89-140">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

