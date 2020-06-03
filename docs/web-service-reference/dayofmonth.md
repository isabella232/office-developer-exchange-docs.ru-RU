---
title: DayOfMonth
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
description: Элемент DayOfMonth описывает день месяца, в который происходит повторяющийся элемент.
ms.openlocfilehash: dc333a46283d5e8eba3a79f62f8c22c22f56e190
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44442831"
---
# <a name="dayofmonth"></a><span data-ttu-id="83dd2-103">DayOfMonth</span><span class="sxs-lookup"><span data-stu-id="83dd2-103">DayOfMonth</span></span>

<span data-ttu-id="83dd2-104">Элемент **DayOfMonth** описывает день месяца, в который происходит повторяющийся элемент.</span><span class="sxs-lookup"><span data-stu-id="83dd2-104">The **DayOfMonth** element describes the day in a month that a recurring item occurs.</span></span> 
  
```xml
<DayOfMonth/>
```

<span data-ttu-id="83dd2-105">**int**</span><span class="sxs-lookup"><span data-stu-id="83dd2-105">**int**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="83dd2-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="83dd2-106">Attributes and elements</span></span>

<span data-ttu-id="83dd2-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="83dd2-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="83dd2-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="83dd2-108">Attributes</span></span>

<span data-ttu-id="83dd2-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="83dd2-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="83dd2-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="83dd2-110">Child elements</span></span>

<span data-ttu-id="83dd2-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="83dd2-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="83dd2-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="83dd2-112">Parent elements</span></span>

|<span data-ttu-id="83dd2-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="83dd2-113">**Element**</span></span>|<span data-ttu-id="83dd2-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="83dd2-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="83dd2-115">абсолутэйеарлирекурренце</span><span class="sxs-lookup"><span data-stu-id="83dd2-115">AbsoluteYearlyRecurrence</span></span>](absoluteyearlyrecurrence.md) <br/> |<span data-ttu-id="83dd2-116">Представляет шаблон ежегодного повторения.</span><span class="sxs-lookup"><span data-stu-id="83dd2-116">Represents a yearly recurrence pattern.</span></span>  <br/> |
|[<span data-ttu-id="83dd2-117">абсолутемонслирекурренце</span><span class="sxs-lookup"><span data-stu-id="83dd2-117">AbsoluteMonthlyRecurrence</span></span>](absolutemonthlyrecurrence.md) <br/> |<span data-ttu-id="83dd2-118">Представляет ежемесячный шаблон повторения.</span><span class="sxs-lookup"><span data-stu-id="83dd2-118">Represents a monthly recurrence pattern.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="83dd2-119">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="83dd2-119">Text value</span></span>

<span data-ttu-id="83dd2-120">Требуется текстовое значение, представляющее целое число от 1 до 31.</span><span class="sxs-lookup"><span data-stu-id="83dd2-120">A text value that represents an integer in the range of 1 to 31 is required.</span></span> <span data-ttu-id="83dd2-121">Если для определенного месяца это значение превышает количество дней в месяце, подразумевается последний день месяца.</span><span class="sxs-lookup"><span data-stu-id="83dd2-121">If for a particular month this value is larger than the number of days in the month, the last day of the month is assumed.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="83dd2-122">Примечания</span><span class="sxs-lookup"><span data-stu-id="83dd2-122">Remarks</span></span>

<span data-ttu-id="83dd2-123">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="83dd2-123">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="83dd2-124">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="83dd2-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="83dd2-125">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="83dd2-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="83dd2-126">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="83dd2-126">Schema name</span></span>  <br/> |<span data-ttu-id="83dd2-127">Схема Types</span><span class="sxs-lookup"><span data-stu-id="83dd2-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="83dd2-128">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="83dd2-128">Validation file</span></span>  <br/> |<span data-ttu-id="83dd2-129">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="83dd2-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="83dd2-130">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="83dd2-130">Can be empty</span></span>  <br/> |<span data-ttu-id="83dd2-131">False</span><span class="sxs-lookup"><span data-stu-id="83dd2-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="83dd2-132">См. также</span><span class="sxs-lookup"><span data-stu-id="83dd2-132">See also</span></span>

- [<span data-ttu-id="83dd2-133">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="83dd2-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

