---
title: StartDate (повторение)
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
# <a name="startdate-recurrence"></a><span data-ttu-id="80bc9-103">StartDate (повторение)</span><span class="sxs-lookup"><span data-stu-id="80bc9-103">StartDate (Recurrence)</span></span>

<span data-ttu-id="80bc9-104">Элемент **StartDate** представляет дату начала повторяющейся задачи или элемента календаря.</span><span class="sxs-lookup"><span data-stu-id="80bc9-104">The **StartDate** element represents the start date of a recurring task or calendar item.</span></span> 
  
```xml
<StartDate/>
```

<span data-ttu-id="80bc9-105">**Date**</span><span class="sxs-lookup"><span data-stu-id="80bc9-105">**Date**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="80bc9-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="80bc9-106">Attributes and elements</span></span>

<span data-ttu-id="80bc9-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="80bc9-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="80bc9-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="80bc9-108">Attributes</span></span>

<span data-ttu-id="80bc9-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="80bc9-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="80bc9-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="80bc9-110">Child elements</span></span>

<span data-ttu-id="80bc9-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="80bc9-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="80bc9-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="80bc9-112">Parent elements</span></span>

|<span data-ttu-id="80bc9-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="80bc9-113">**Element**</span></span>|<span data-ttu-id="80bc9-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="80bc9-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="80bc9-115">енддатерекурренце</span><span class="sxs-lookup"><span data-stu-id="80bc9-115">EndDateRecurrence</span></span>](enddaterecurrence.md) <br/> |<span data-ttu-id="80bc9-116">Описывает дату начала и дату окончания расписания повторения элемента.</span><span class="sxs-lookup"><span data-stu-id="80bc9-116">Describes the start date and the end date of an item recurrence pattern.</span></span>  <br/> |
|[<span data-ttu-id="80bc9-117">ноендрекурренце</span><span class="sxs-lookup"><span data-stu-id="80bc9-117">NoEndRecurrence</span></span>](noendrecurrence.md) <br/> |<span data-ttu-id="80bc9-118">Описывает дату начала для шаблона повторения элемента, у которого нет определенной конечной даты.</span><span class="sxs-lookup"><span data-stu-id="80bc9-118">Describes the start date of an item recurrence pattern that does not have a defined end date.</span></span>  <br/> |
|[<span data-ttu-id="80bc9-119">нумбередрекурренце</span><span class="sxs-lookup"><span data-stu-id="80bc9-119">NumberedRecurrence</span></span>](numberedrecurrence.md) <br/> |<span data-ttu-id="80bc9-120">Описывает дату начала и число повторений повторяющегося элемента.</span><span class="sxs-lookup"><span data-stu-id="80bc9-120">Describes the start date and the number of occurrences of a recurring item.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="80bc9-121">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="80bc9-121">Text value</span></span>

<span data-ttu-id="80bc9-122">Текстовое значение, представляющее дату, является обязательным при использовании этого элемента.</span><span class="sxs-lookup"><span data-stu-id="80bc9-122">A text value that represents a date is required if this element is used.</span></span> <span data-ttu-id="80bc9-123">Значение не может быть меньше Апр, 1, 1601 00:00:00.</span><span class="sxs-lookup"><span data-stu-id="80bc9-123">The value cannot be less than Apr, 1, 1601 00:00:00.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="80bc9-124">Примечания</span><span class="sxs-lookup"><span data-stu-id="80bc9-124">Remarks</span></span>

<span data-ttu-id="80bc9-125">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="80bc9-125">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="80bc9-126">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="80bc9-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="80bc9-127">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="80bc9-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="80bc9-128">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="80bc9-128">Schema name</span></span>  <br/> |<span data-ttu-id="80bc9-129">Схема Types</span><span class="sxs-lookup"><span data-stu-id="80bc9-129">Types schema</span></span>  <br/> |
|<span data-ttu-id="80bc9-130">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="80bc9-130">Validation file</span></span>  <br/> |<span data-ttu-id="80bc9-131">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="80bc9-131">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="80bc9-132">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="80bc9-132">Can be empty</span></span>  <br/> |<span data-ttu-id="80bc9-133">False</span><span class="sxs-lookup"><span data-stu-id="80bc9-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="80bc9-134">См. также</span><span class="sxs-lookup"><span data-stu-id="80bc9-134">See also</span></span>

- [<span data-ttu-id="80bc9-135">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="80bc9-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

