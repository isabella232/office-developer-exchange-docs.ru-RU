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
ms.openlocfilehash: 0d0d95849a2562e06b88872b2857cc5e6ca67af3
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761990"
---
# <a name="dayofmonth"></a><span data-ttu-id="ffd52-103">DayOfMonth</span><span class="sxs-lookup"><span data-stu-id="ffd52-103">DayOfMonth</span></span>

<span data-ttu-id="ffd52-104">Элемент **DayOfMonth** описывает день месяца, в который происходит повторяющийся элемент.</span><span class="sxs-lookup"><span data-stu-id="ffd52-104">The **DayOfMonth** element describes the day in a month that a recurring item occurs.</span></span> 
  
```xml
<DayOfMonth/>
```

<span data-ttu-id="ffd52-105">**int**</span><span class="sxs-lookup"><span data-stu-id="ffd52-105">**int**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="ffd52-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="ffd52-106">Attributes and elements</span></span>

<span data-ttu-id="ffd52-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="ffd52-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ffd52-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="ffd52-108">Attributes</span></span>

<span data-ttu-id="ffd52-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="ffd52-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ffd52-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="ffd52-110">Child elements</span></span>

<span data-ttu-id="ffd52-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="ffd52-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="ffd52-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="ffd52-112">Parent elements</span></span>

|<span data-ttu-id="ffd52-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="ffd52-113">**Element**</span></span>|<span data-ttu-id="ffd52-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="ffd52-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ffd52-115">абсолутэйеарлирекурренце</span><span class="sxs-lookup"><span data-stu-id="ffd52-115">AbsoluteYearlyRecurrence</span></span>](absoluteyearlyrecurrence.md) <br/> |<span data-ttu-id="ffd52-116">Представляет шаблон ежегодного повторения.</span><span class="sxs-lookup"><span data-stu-id="ffd52-116">Represents a yearly recurrence pattern.</span></span>  <br/> |
|[<span data-ttu-id="ffd52-117">абсолутемонслирекурренце</span><span class="sxs-lookup"><span data-stu-id="ffd52-117">AbsoluteMonthlyRecurrence</span></span>](absolutemonthlyrecurrence.md) <br/> |<span data-ttu-id="ffd52-118">Представляет ежемесячный шаблон повторения.</span><span class="sxs-lookup"><span data-stu-id="ffd52-118">Represents a monthly recurrence pattern.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="ffd52-119">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="ffd52-119">Text value</span></span>

<span data-ttu-id="ffd52-120">Требуется текстовое значение, представляющее целое число от 1 до 31.</span><span class="sxs-lookup"><span data-stu-id="ffd52-120">A text value that represents an integer in the range of 1 to 31 is required.</span></span> <span data-ttu-id="ffd52-121">Если для определенного месяца это значение превышает количество дней в месяце, подразумевается последний день месяца.</span><span class="sxs-lookup"><span data-stu-id="ffd52-121">If for a particular month this value is larger than the number of days in the month, the last day of the month is assumed.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="ffd52-122">Примечания</span><span class="sxs-lookup"><span data-stu-id="ffd52-122">Remarks</span></span>

<span data-ttu-id="ffd52-123">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="ffd52-123">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ffd52-124">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="ffd52-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ffd52-125">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="ffd52-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="ffd52-126">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="ffd52-126">Schema name</span></span>  <br/> |<span data-ttu-id="ffd52-127">Схема Types</span><span class="sxs-lookup"><span data-stu-id="ffd52-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="ffd52-128">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="ffd52-128">Validation file</span></span>  <br/> |<span data-ttu-id="ffd52-129">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="ffd52-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="ffd52-130">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="ffd52-130">Can be empty</span></span>  <br/> |<span data-ttu-id="ffd52-131">False</span><span class="sxs-lookup"><span data-stu-id="ffd52-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ffd52-132">См. также</span><span class="sxs-lookup"><span data-stu-id="ffd52-132">See also</span></span>

- [<span data-ttu-id="ffd52-133">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="ffd52-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

