---
title: даилирекурренце
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DailyRecurrence
api_type:
- schema
ms.assetid: 0aaf265d-b723-49c6-8e9c-9ba60141e9ab
description: Элемент Даилирекурренце описывает частоту повторения элемента календаря или задачи в днях.
ms.openlocfilehash: d18a04ced19c87996c3a092f6668ab00c5a3f006
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462173"
---
# <a name="dailyrecurrence"></a><span data-ttu-id="f27e6-103">даилирекурренце</span><span class="sxs-lookup"><span data-stu-id="f27e6-103">DailyRecurrence</span></span>

<span data-ttu-id="f27e6-104">Элемент **даилирекурренце** описывает частоту повторения элемента календаря или задачи в днях.</span><span class="sxs-lookup"><span data-stu-id="f27e6-104">The **DailyRecurrence** element describes the frequency, in days, in which a calendar item or a task recurs.</span></span> 
  
```xml
<DailyRecurrence>
   <Interval/>
</DailyRecurrence>
```

<span data-ttu-id="f27e6-105">**даилирекурренцепаттернтипе**</span><span class="sxs-lookup"><span data-stu-id="f27e6-105">**DailyRecurrencePatternType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="f27e6-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="f27e6-106">Attributes and elements</span></span>

<span data-ttu-id="f27e6-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="f27e6-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f27e6-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="f27e6-108">Attributes</span></span>

<span data-ttu-id="f27e6-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="f27e6-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f27e6-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="f27e6-110">Child elements</span></span>

|<span data-ttu-id="f27e6-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="f27e6-111">**Element**</span></span>|<span data-ttu-id="f27e6-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="f27e6-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f27e6-113">Interval</span><span class="sxs-lookup"><span data-stu-id="f27e6-113">Interval</span></span>](interval.md) <br/> |<span data-ttu-id="f27e6-114">Определяет интервал (в днях) между двумя последовательными повторяющимися элементами.</span><span class="sxs-lookup"><span data-stu-id="f27e6-114">Defines the interval, in days, between two consecutive recurring items.</span></span> <span data-ttu-id="f27e6-115">Значение должно находиться в диапазоне от 1 до 999.</span><span class="sxs-lookup"><span data-stu-id="f27e6-115">The value must be in the range from 1 to 999.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f27e6-116">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="f27e6-116">Parent elements</span></span>

|<span data-ttu-id="f27e6-117">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="f27e6-117">**Element**</span></span>|<span data-ttu-id="f27e6-118">**Описание**</span><span class="sxs-lookup"><span data-stu-id="f27e6-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f27e6-119">Повторение (Таскрекурренцетипе)</span><span class="sxs-lookup"><span data-stu-id="f27e6-119">Recurrence (TaskRecurrenceType)</span></span>](recurrence-taskrecurrencetype.md) <br/> |<span data-ttu-id="f27e6-120">Содержит сведения о повторении для повторяющихся задач.</span><span class="sxs-lookup"><span data-stu-id="f27e6-120">Contains recurrence information for recurring tasks.</span></span>  <br/> |
|[<span data-ttu-id="f27e6-121">Повторение (RecurrenceType)</span><span class="sxs-lookup"><span data-stu-id="f27e6-121">Recurrence (RecurrenceType)</span></span>](recurrence-recurrencetype.md) <br/> |<span data-ttu-id="f27e6-122">Содержит шаблон повторения для элементов календаря и приглашений на собрание.</span><span class="sxs-lookup"><span data-stu-id="f27e6-122">Contains the recurrence pattern for calendar items and meeting requests.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="f27e6-123">Примечания</span><span class="sxs-lookup"><span data-stu-id="f27e6-123">Remarks</span></span>

<span data-ttu-id="f27e6-124">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="f27e6-124">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f27e6-125">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="f27e6-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f27e6-126">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="f27e6-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="f27e6-127">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="f27e6-127">Schema name</span></span>  <br/> |<span data-ttu-id="f27e6-128">Схема Types</span><span class="sxs-lookup"><span data-stu-id="f27e6-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="f27e6-129">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="f27e6-129">Validation file</span></span>  <br/> |<span data-ttu-id="f27e6-130">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="f27e6-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="f27e6-131">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="f27e6-131">Can be empty</span></span>  <br/> |<span data-ttu-id="f27e6-132">False</span><span class="sxs-lookup"><span data-stu-id="f27e6-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f27e6-133">См. также</span><span class="sxs-lookup"><span data-stu-id="f27e6-133">See also</span></span>

- [<span data-ttu-id="f27e6-134">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="f27e6-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

