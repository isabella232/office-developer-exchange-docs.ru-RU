---
title: DailyRecurrence
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
description: Элемент DailyRecurrence описывает период в днях, в которых повторяется элемента календаря или задачи.
ms.openlocfilehash: d02c1f7425372d60c10b40527dc5f0d65f923b45
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761958"
---
# <a name="dailyrecurrence"></a><span data-ttu-id="29a25-103">DailyRecurrence</span><span class="sxs-lookup"><span data-stu-id="29a25-103">DailyRecurrence</span></span>

<span data-ttu-id="29a25-104">Элемент **DailyRecurrence** описывает период в днях, в которых повторяется элемента календаря или задачи.</span><span class="sxs-lookup"><span data-stu-id="29a25-104">The **DailyRecurrence** element describes the frequency, in days, in which a calendar item or a task recurs.</span></span> 
  
```xml
<DailyRecurrence>
   <Interval/>
</DailyRecurrence>
```

<span data-ttu-id="29a25-105">**DailyRecurrencePatternType**</span><span class="sxs-lookup"><span data-stu-id="29a25-105">**DailyRecurrencePatternType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="29a25-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="29a25-106">Attributes and elements</span></span>

<span data-ttu-id="29a25-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="29a25-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="29a25-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="29a25-108">Attributes</span></span>

<span data-ttu-id="29a25-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="29a25-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="29a25-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="29a25-110">Child elements</span></span>

|<span data-ttu-id="29a25-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="29a25-111">**Element**</span></span>|<span data-ttu-id="29a25-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="29a25-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="29a25-113">Интервал</span><span class="sxs-lookup"><span data-stu-id="29a25-113">Interval</span></span>](interval.md) <br/> |<span data-ttu-id="29a25-114">Задает интервал в днях между двумя последовательными повторяющихся элементов.</span><span class="sxs-lookup"><span data-stu-id="29a25-114">Defines the interval, in days, between two consecutive recurring items.</span></span> <span data-ttu-id="29a25-115">Значение должно быть в диапазоне от 1 до 999.</span><span class="sxs-lookup"><span data-stu-id="29a25-115">The value must be in the range from 1 to 999.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="29a25-116">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="29a25-116">Parent elements</span></span>

|<span data-ttu-id="29a25-117">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="29a25-117">**Element**</span></span>|<span data-ttu-id="29a25-118">**Описание**</span><span class="sxs-lookup"><span data-stu-id="29a25-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="29a25-119">Повторение (TaskRecurrenceType)</span><span class="sxs-lookup"><span data-stu-id="29a25-119">Recurrence (TaskRecurrenceType)</span></span>](recurrence-taskrecurrencetype.md) <br/> |<span data-ttu-id="29a25-120">Содержит данные о повторении для повторяющихся задач.</span><span class="sxs-lookup"><span data-stu-id="29a25-120">Contains recurrence information for recurring tasks.</span></span>  <br/> |
|[<span data-ttu-id="29a25-121">Повторение (RecurrenceType)</span><span class="sxs-lookup"><span data-stu-id="29a25-121">Recurrence (RecurrenceType)</span></span>](recurrence-recurrencetype.md) <br/> |<span data-ttu-id="29a25-122">Содержит шаблон повторения для элементов календаря и приглашения на собрания.</span><span class="sxs-lookup"><span data-stu-id="29a25-122">Contains the recurrence pattern for calendar items and meeting requests.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="29a25-123">Замечания</span><span class="sxs-lookup"><span data-stu-id="29a25-123">Remarks</span></span>

<span data-ttu-id="29a25-124">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="29a25-124">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="29a25-125">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="29a25-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="29a25-126">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="29a25-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="29a25-127">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="29a25-127">Schema name</span></span>  <br/> |<span data-ttu-id="29a25-128">Схема Types</span><span class="sxs-lookup"><span data-stu-id="29a25-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="29a25-129">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="29a25-129">Validation file</span></span>  <br/> |<span data-ttu-id="29a25-130">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="29a25-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="29a25-131">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="29a25-131">Can be empty</span></span>  <br/> |<span data-ttu-id="29a25-132">False</span><span class="sxs-lookup"><span data-stu-id="29a25-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="29a25-133">См. также</span><span class="sxs-lookup"><span data-stu-id="29a25-133">See also</span></span>

- [<span data-ttu-id="29a25-134">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="29a25-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

