---
title: DayOfWeekIndex
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DayOfWeekIndex
api_type:
- schema
ms.assetid: 82420338-a1f7-4887-b338-b2d93b2c2bf1
description: Элемент DayOfWeekIndex описывает неделю в месяц используется в относительный повторения.
ms.openlocfilehash: 4987685d0c3cefdfad4f5be1368776a5b859bf94
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761999"
---
# <a name="dayofweekindex"></a><span data-ttu-id="257fb-103">DayOfWeekIndex</span><span class="sxs-lookup"><span data-stu-id="257fb-103">DayOfWeekIndex</span></span>

<span data-ttu-id="257fb-104">Элемент **DayOfWeekIndex** описывает неделю в месяц используется в относительный повторения.</span><span class="sxs-lookup"><span data-stu-id="257fb-104">The **DayOfWeekIndex** element describes which week in a month is used in a relative recurrence pattern.</span></span> 
  
```xml
<DayOfWeekIndex/>
```

<span data-ttu-id="257fb-105">**DayOfWeekIndexType**</span><span class="sxs-lookup"><span data-stu-id="257fb-105">**DayOfWeekIndexType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="257fb-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="257fb-106">Attributes and elements</span></span>

<span data-ttu-id="257fb-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="257fb-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="257fb-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="257fb-108">Attributes</span></span>

<span data-ttu-id="257fb-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="257fb-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="257fb-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="257fb-110">Child elements</span></span>

<span data-ttu-id="257fb-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="257fb-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="257fb-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="257fb-112">Parent elements</span></span>

|<span data-ttu-id="257fb-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="257fb-113">**Element**</span></span>|<span data-ttu-id="257fb-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="257fb-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="257fb-115">RelativeYearlyRecurrence</span><span class="sxs-lookup"><span data-stu-id="257fb-115">RelativeYearlyRecurrence</span></span>](relativeyearlyrecurrence.md) <br/> |<span data-ttu-id="257fb-116">Описывает относительное ежегодно повторяющейся.</span><span class="sxs-lookup"><span data-stu-id="257fb-116">Describes a relative yearly recurrence pattern.</span></span>  <br/> |
|[<span data-ttu-id="257fb-117">RelativeMonthlyRecurrence</span><span class="sxs-lookup"><span data-stu-id="257fb-117">RelativeMonthlyRecurrence</span></span>](relativemonthlyrecurrence.md) <br/> |<span data-ttu-id="257fb-118">Описывает относительное ежемесячный шаблона повторения.</span><span class="sxs-lookup"><span data-stu-id="257fb-118">Describes a relative monthly recurrence pattern.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="257fb-119">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="257fb-119">Text value</span></span>

<span data-ttu-id="257fb-120">Текстовое значение является обязательным.</span><span class="sxs-lookup"><span data-stu-id="257fb-120">A text value is required.</span></span> <span data-ttu-id="257fb-121">Ниже перечислены возможные значения.</span><span class="sxs-lookup"><span data-stu-id="257fb-121">The following are the possible values:</span></span>
  
- <span data-ttu-id="257fb-122">Первый</span><span class="sxs-lookup"><span data-stu-id="257fb-122">First</span></span>    
- <span data-ttu-id="257fb-123">Второй </span><span class="sxs-lookup"><span data-stu-id="257fb-123">Second</span></span>    
- <span data-ttu-id="257fb-124">Третья</span><span class="sxs-lookup"><span data-stu-id="257fb-124">Third</span></span>    
- <span data-ttu-id="257fb-125">Четвертый</span><span class="sxs-lookup"><span data-stu-id="257fb-125">Fourth</span></span>    
- <span data-ttu-id="257fb-126">Последний</span><span class="sxs-lookup"><span data-stu-id="257fb-126">Last</span></span>
    
## <a name="remarks"></a><span data-ttu-id="257fb-127">Замечания</span><span class="sxs-lookup"><span data-stu-id="257fb-127">Remarks</span></span>

<span data-ttu-id="257fb-128">Например второй понедельник месяца может произойти в третьей недели месяца.</span><span class="sxs-lookup"><span data-stu-id="257fb-128">For example, the second Monday of a month may occur in the third week of that month.</span></span> <span data-ttu-id="257fb-129">Если месяца начинается в пятницу, первой недели, месяца только содержит несколько дней и не содержит понедельник.</span><span class="sxs-lookup"><span data-stu-id="257fb-129">If a month starts on a Friday, the first week of the month only contains a few days and does not contain a Monday.</span></span> <span data-ttu-id="257fb-130">Таким образом первый понедельник бы в второй недели.</span><span class="sxs-lookup"><span data-stu-id="257fb-130">Therefore, the first Monday would have to occur in the second week.</span></span>
  
<span data-ttu-id="257fb-131">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="257fb-131">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="257fb-132">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="257fb-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="257fb-133">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="257fb-133">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="257fb-134">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="257fb-134">Schema name</span></span>  <br/> |<span data-ttu-id="257fb-135">Схема Types</span><span class="sxs-lookup"><span data-stu-id="257fb-135">Types schema</span></span>  <br/> |
|<span data-ttu-id="257fb-136">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="257fb-136">Validation file</span></span>  <br/> |<span data-ttu-id="257fb-137">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="257fb-137">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="257fb-138">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="257fb-138">Can be empty</span></span>  <br/> |<span data-ttu-id="257fb-139">False</span><span class="sxs-lookup"><span data-stu-id="257fb-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="257fb-140">См. также</span><span class="sxs-lookup"><span data-stu-id="257fb-140">See also</span></span>

- [<span data-ttu-id="257fb-141">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="257fb-141">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

