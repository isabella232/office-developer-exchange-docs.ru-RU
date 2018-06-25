---
title: StartDate (повторения)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- StartDate
api_type:
- schema
ms.assetid: bd65ac06-b3ac-4c9b-9568-3e4dc94378e7
description: Элемент StartDate представляет дату начала повторяющейся задачи или элемента календаря.
ms.openlocfilehash: 6a38e63bbcf010ab6dca8f66440a2b0a559cf88d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835551"
---
# <a name="startdate-recurrence"></a><span data-ttu-id="dd927-103">StartDate (повторения)</span><span class="sxs-lookup"><span data-stu-id="dd927-103">StartDate (Recurrence)</span></span>

<span data-ttu-id="dd927-104">Элемент **StartDate** представляет дату начала повторяющейся задачи или элемента календаря.</span><span class="sxs-lookup"><span data-stu-id="dd927-104">The **StartDate** element represents the start date of a recurring task or calendar item.</span></span> 
  
```xml
<StartDate/>
```

<span data-ttu-id="dd927-105">**Дата**</span><span class="sxs-lookup"><span data-stu-id="dd927-105">**Date**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="dd927-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="dd927-106">Attributes and elements</span></span>

<span data-ttu-id="dd927-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="dd927-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="dd927-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="dd927-108">Attributes</span></span>

<span data-ttu-id="dd927-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="dd927-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="dd927-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="dd927-110">Child elements</span></span>

<span data-ttu-id="dd927-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="dd927-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="dd927-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="dd927-112">Parent elements</span></span>

|<span data-ttu-id="dd927-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="dd927-113">**Element**</span></span>|<span data-ttu-id="dd927-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="dd927-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="dd927-115">EndDateRecurrence</span><span class="sxs-lookup"><span data-stu-id="dd927-115">EndDateRecurrence</span></span>](enddaterecurrence.md) <br/> |<span data-ttu-id="dd927-116">Описание, Дата начала и Дата окончания повторения элемента.</span><span class="sxs-lookup"><span data-stu-id="dd927-116">Describes the start date and the end date of an item recurrence pattern.</span></span>  <br/> |
|[<span data-ttu-id="dd927-117">NoEndRecurrence</span><span class="sxs-lookup"><span data-stu-id="dd927-117">NoEndRecurrence</span></span>](noendrecurrence.md) <br/> |<span data-ttu-id="dd927-118">Описывает дату начала повторения элемента, для которого не определенные дату.</span><span class="sxs-lookup"><span data-stu-id="dd927-118">Describes the start date of an item recurrence pattern that does not have a defined end date.</span></span>  <br/> |
|[<span data-ttu-id="dd927-119">NumberedRecurrence</span><span class="sxs-lookup"><span data-stu-id="dd927-119">NumberedRecurrence</span></span>](numberedrecurrence.md) <br/> |<span data-ttu-id="dd927-120">Описание, Дата начала и число вхождений повторяющегося элемента.</span><span class="sxs-lookup"><span data-stu-id="dd927-120">Describes the start date and the number of occurrences of a recurring item.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="dd927-121">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="dd927-121">Text value</span></span>

<span data-ttu-id="dd927-122">Текстовое значение, которое представляет дату является обязательным, если данный элемент используется.</span><span class="sxs-lookup"><span data-stu-id="dd927-122">A text value that represents a date is required if this element is used.</span></span> <span data-ttu-id="dd927-123">Значение не может быть меньше, чем апреля, 1 1601 00:00:00.</span><span class="sxs-lookup"><span data-stu-id="dd927-123">The value cannot be less than Apr, 1, 1601 00:00:00.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="dd927-124">Замечания</span><span class="sxs-lookup"><span data-stu-id="dd927-124">Remarks</span></span>

<span data-ttu-id="dd927-125">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="dd927-125">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="dd927-126">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="dd927-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="dd927-127">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="dd927-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="dd927-128">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="dd927-128">Schema name</span></span>  <br/> |<span data-ttu-id="dd927-129">Схема Types</span><span class="sxs-lookup"><span data-stu-id="dd927-129">Types schema</span></span>  <br/> |
|<span data-ttu-id="dd927-130">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="dd927-130">Validation file</span></span>  <br/> |<span data-ttu-id="dd927-131">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="dd927-131">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="dd927-132">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="dd927-132">Can be empty</span></span>  <br/> |<span data-ttu-id="dd927-133">False</span><span class="sxs-lookup"><span data-stu-id="dd927-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="dd927-134">См. также</span><span class="sxs-lookup"><span data-stu-id="dd927-134">See also</span></span>

- [<span data-ttu-id="dd927-135">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="dd927-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

