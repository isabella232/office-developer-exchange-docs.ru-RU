---
title: абсолутемонслирекурренце
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AbsoluteMonthlyRecurrence
api_type:
- schema
ms.assetid: 178fa0ae-9dfc-417f-933c-d657d31c2161
description: Элемент Абсолутемонслирекурренце представляет месячный шаблон повторения.
ms.openlocfilehash: 3176cd30a1cfe7b2310f960ce377ab7a277e795a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460437"
---
# <a name="absolutemonthlyrecurrence"></a><span data-ttu-id="c5d99-103">абсолутемонслирекурренце</span><span class="sxs-lookup"><span data-stu-id="c5d99-103">AbsoluteMonthlyRecurrence</span></span>

<span data-ttu-id="c5d99-104">Элемент **абсолутемонслирекурренце** представляет месячный шаблон повторения.</span><span class="sxs-lookup"><span data-stu-id="c5d99-104">The **AbsoluteMonthlyRecurrence** element represents a monthly recurrence pattern.</span></span> 
  
```xml
<AbsoluteMonthlyRecurrence>
   <Interval/>
   <DayOfMonth/>
</AbsoluteMonthlyRecurrence>
```

 <span data-ttu-id="c5d99-105">**абсолутемонслирекурренцепаттернтипе**</span><span class="sxs-lookup"><span data-stu-id="c5d99-105">**AbsoluteMonthlyRecurrencePatternType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c5d99-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="c5d99-106">Attributes and elements</span></span>

<span data-ttu-id="c5d99-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="c5d99-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c5d99-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="c5d99-108">Attributes</span></span>

<span data-ttu-id="c5d99-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="c5d99-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c5d99-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="c5d99-110">Child elements</span></span>

|<span data-ttu-id="c5d99-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="c5d99-111">**Element**</span></span>|<span data-ttu-id="c5d99-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="c5d99-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c5d99-113">DayOfMonth</span><span class="sxs-lookup"><span data-stu-id="c5d99-113">DayOfMonth</span></span>](dayofmonth.md) <br/> |<span data-ttu-id="c5d99-114">Описывает день месяца, в который происходит повторяющийся элемент.</span><span class="sxs-lookup"><span data-stu-id="c5d99-114">Describes the day in a month that a recurring item occurs.</span></span> <span data-ttu-id="c5d99-115">Диапазон значений этого свойства — от 1 до 31.</span><span class="sxs-lookup"><span data-stu-id="c5d99-115">The range of values for this property is 1 to 31.</span></span> <span data-ttu-id="c5d99-116">Если для определенного месяца это значение превышает количество дней в месяце, для этого свойства подразумевается последний день месяца.</span><span class="sxs-lookup"><span data-stu-id="c5d99-116">If for a particular month this value is larger than the number of days in the month, the last day of the month is assumed for this property.</span></span>  <br/> |
|[<span data-ttu-id="c5d99-117">Interval</span><span class="sxs-lookup"><span data-stu-id="c5d99-117">Interval</span></span>](interval.md) <br/> |<span data-ttu-id="c5d99-118">Определяет интервал между двумя последовательными повторяющимися элементами.</span><span class="sxs-lookup"><span data-stu-id="c5d99-118">Defines the interval between two consecutive recurring items.</span></span> <span data-ttu-id="c5d99-119">Например, если элемент **Interval** имеет значение 5, повторяющийся элемент повторяется каждые 5 месяцев.</span><span class="sxs-lookup"><span data-stu-id="c5d99-119">For example, if the **Interval** element has a value of 5, the recurring item occurs every 5 months.</span></span> <span data-ttu-id="c5d99-120">Диапазон допустимых значений: от 1 до 99.</span><span class="sxs-lookup"><span data-stu-id="c5d99-120">The range of valid values is from 1 to 99.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="c5d99-121">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="c5d99-121">Parent elements</span></span>

|<span data-ttu-id="c5d99-122">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="c5d99-122">**Element**</span></span>|<span data-ttu-id="c5d99-123">**Описание**</span><span class="sxs-lookup"><span data-stu-id="c5d99-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c5d99-124">Повторение (Таскрекурренцетипе)</span><span class="sxs-lookup"><span data-stu-id="c5d99-124">Recurrence (TaskRecurrenceType)</span></span>](recurrence-taskrecurrencetype.md) <br/> |<span data-ttu-id="c5d99-125">Содержит сведения о повторении для повторяющихся задач.</span><span class="sxs-lookup"><span data-stu-id="c5d99-125">Contains recurrence information for recurring tasks.</span></span>  <br/> |
|[<span data-ttu-id="c5d99-126">Повторение (RecurrenceType)</span><span class="sxs-lookup"><span data-stu-id="c5d99-126">Recurrence (RecurrenceType)</span></span>](recurrence-recurrencetype.md) <br/> |<span data-ttu-id="c5d99-127">Содержит шаблон повторения для элементов календаря и приглашений на собрание.</span><span class="sxs-lookup"><span data-stu-id="c5d99-127">Contains the recurrence pattern for calendar items and meeting requests.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="c5d99-128">Примечания</span><span class="sxs-lookup"><span data-stu-id="c5d99-128">Remarks</span></span>

<span data-ttu-id="c5d99-129">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="c5d99-129">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c5d99-130">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="c5d99-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c5d99-131">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="c5d99-131">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="c5d99-132">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="c5d99-132">Schema Name</span></span>  <br/> |<span data-ttu-id="c5d99-133">Схема Types</span><span class="sxs-lookup"><span data-stu-id="c5d99-133">Types schema</span></span>  <br/> |
|<span data-ttu-id="c5d99-134">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="c5d99-134">Validation File</span></span>  <br/> |<span data-ttu-id="c5d99-135">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="c5d99-135">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="c5d99-136">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="c5d99-136">Can Be Empty</span></span>  <br/> |<span data-ttu-id="c5d99-137">False</span><span class="sxs-lookup"><span data-stu-id="c5d99-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c5d99-138">См. также</span><span class="sxs-lookup"><span data-stu-id="c5d99-138">See also</span></span>

- [<span data-ttu-id="c5d99-139">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="c5d99-139">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

