---
title: День месяца
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DayOfMonth
api_type:
- schema
ms.assetid: 09b7504e-08d8-42f9-88cc-a2a37a2e2b8b
description: Элемент день месяца описывает день месяца, которая происходит повторяющегося элемента.
ms.openlocfilehash: 0d0d95849a2562e06b88872b2857cc5e6ca67af3
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761990"
---
# <a name="dayofmonth"></a><span data-ttu-id="5bd8d-103">День месяца</span><span class="sxs-lookup"><span data-stu-id="5bd8d-103">DayOfMonth</span></span>

<span data-ttu-id="5bd8d-104">Элемент **день месяца** описывает день месяца, которая происходит повторяющегося элемента.</span><span class="sxs-lookup"><span data-stu-id="5bd8d-104">The **DayOfMonth** element describes the day in a month that a recurring item occurs.</span></span> 
  
```xml
<DayOfMonth/>
```

<span data-ttu-id="5bd8d-105">**int**</span><span class="sxs-lookup"><span data-stu-id="5bd8d-105">**int**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="5bd8d-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="5bd8d-106">Attributes and elements</span></span>

<span data-ttu-id="5bd8d-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="5bd8d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5bd8d-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="5bd8d-108">Attributes</span></span>

<span data-ttu-id="5bd8d-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="5bd8d-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5bd8d-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="5bd8d-110">Child elements</span></span>

<span data-ttu-id="5bd8d-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="5bd8d-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="5bd8d-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="5bd8d-112">Parent elements</span></span>

|<span data-ttu-id="5bd8d-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="5bd8d-113">**Element**</span></span>|<span data-ttu-id="5bd8d-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="5bd8d-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5bd8d-115">AbsoluteYearlyRecurrence</span><span class="sxs-lookup"><span data-stu-id="5bd8d-115">AbsoluteYearlyRecurrence</span></span>](absoluteyearlyrecurrence.md) <br/> |<span data-ttu-id="5bd8d-116">Представляет шаблон повторения ежегодно.</span><span class="sxs-lookup"><span data-stu-id="5bd8d-116">Represents a yearly recurrence pattern.</span></span>  <br/> |
|[<span data-ttu-id="5bd8d-117">AbsoluteMonthlyRecurrence</span><span class="sxs-lookup"><span data-stu-id="5bd8d-117">AbsoluteMonthlyRecurrence</span></span>](absolutemonthlyrecurrence.md) <br/> |<span data-ttu-id="5bd8d-118">Представляет шаблон повторения ежемесячно.</span><span class="sxs-lookup"><span data-stu-id="5bd8d-118">Represents a monthly recurrence pattern.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="5bd8d-119">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="5bd8d-119">Text value</span></span>

<span data-ttu-id="5bd8d-120">Текстовое значение, которое представляет целое число в диапазоне от 1 до 31 является обязательным.</span><span class="sxs-lookup"><span data-stu-id="5bd8d-120">A text value that represents an integer in the range of 1 to 31 is required.</span></span> <span data-ttu-id="5bd8d-121">Если за определенный месяц это значение больше, чем число дней в месяце, подразумевается последний день месяца.</span><span class="sxs-lookup"><span data-stu-id="5bd8d-121">If for a particular month this value is larger than the number of days in the month, the last day of the month is assumed.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="5bd8d-122">Замечания</span><span class="sxs-lookup"><span data-stu-id="5bd8d-122">Remarks</span></span>

<span data-ttu-id="5bd8d-123">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="5bd8d-123">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5bd8d-124">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="5bd8d-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5bd8d-125">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="5bd8d-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="5bd8d-126">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="5bd8d-126">Schema name</span></span>  <br/> |<span data-ttu-id="5bd8d-127">Схема Types</span><span class="sxs-lookup"><span data-stu-id="5bd8d-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="5bd8d-128">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="5bd8d-128">Validation file</span></span>  <br/> |<span data-ttu-id="5bd8d-129">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="5bd8d-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="5bd8d-130">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="5bd8d-130">Can be empty</span></span>  <br/> |<span data-ttu-id="5bd8d-131">False</span><span class="sxs-lookup"><span data-stu-id="5bd8d-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="5bd8d-132">См. также</span><span class="sxs-lookup"><span data-stu-id="5bd8d-132">See also</span></span>

- [<span data-ttu-id="5bd8d-133">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="5bd8d-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

