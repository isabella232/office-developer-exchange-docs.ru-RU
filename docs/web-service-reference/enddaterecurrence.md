---
title: EndDateRecurrence
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- EndDateRecurrence
api_type:
- schema
ms.assetid: a5ee2504-db84-49ee-870c-cca9269f2e26
description: Элемент EndDateRecurrence описание, Дата начала и Дата окончания повторения элемента.
ms.openlocfilehash: 73450bf69c6b122e806d85011975159e348ad740
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762350"
---
# <a name="enddaterecurrence"></a><span data-ttu-id="ad380-103">EndDateRecurrence</span><span class="sxs-lookup"><span data-stu-id="ad380-103">EndDateRecurrence</span></span>

<span data-ttu-id="ad380-104">Элемент **EndDateRecurrence** описание, Дата начала и Дата окончания повторения элемента.</span><span class="sxs-lookup"><span data-stu-id="ad380-104">The **EndDateRecurrence** element describes the start date and the end date of an item recurrence pattern.</span></span> 
  
```xml
<EndDateRecurrence>
   <StartDate/>
   <EndDate/>
</EndDateRecurrence>
```

 <span data-ttu-id="ad380-105">**EndDateRecurrenceRangeType**</span><span class="sxs-lookup"><span data-stu-id="ad380-105">**EndDateRecurrenceRangeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ad380-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="ad380-106">Attributes and elements</span></span>

<span data-ttu-id="ad380-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="ad380-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ad380-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="ad380-108">Attributes</span></span>

<span data-ttu-id="ad380-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="ad380-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ad380-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="ad380-110">Child elements</span></span>

|<span data-ttu-id="ad380-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="ad380-111">**Element**</span></span>|<span data-ttu-id="ad380-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="ad380-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ad380-113">StartDate (повторения)</span><span class="sxs-lookup"><span data-stu-id="ad380-113">StartDate (Recurrence)</span></span>](startdate-recurrence.md) <br/> |<span data-ttu-id="ad380-114">Представляет дату начала повторяющейся задачи или элемента календаря.</span><span class="sxs-lookup"><span data-stu-id="ad380-114">Represents the start date of a recurring task or calendar item.</span></span>  <br/> |
|[<span data-ttu-id="ad380-115">Дата окончания (повторения)</span><span class="sxs-lookup"><span data-stu-id="ad380-115">EndDate (Recurrence)</span></span>](enddate-recurrence.md) <br/> |<span data-ttu-id="ad380-116">Представляет дату окончания повторяющейся задачи или элемента календаря.</span><span class="sxs-lookup"><span data-stu-id="ad380-116">Represents the end date of a recurring task or calendar item.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="ad380-117">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="ad380-117">Parent elements</span></span>

|<span data-ttu-id="ad380-118">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="ad380-118">**Element**</span></span>|<span data-ttu-id="ad380-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="ad380-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ad380-120">Повторение (RecurrenceType)</span><span class="sxs-lookup"><span data-stu-id="ad380-120">Recurrence (RecurrenceType)</span></span>](recurrence-recurrencetype.md) <br/> |<span data-ttu-id="ad380-121">Содержит шаблон повторения для элементов календаря и приглашения на собрания.</span><span class="sxs-lookup"><span data-stu-id="ad380-121">Contains the recurrence pattern for calendar items and meeting requests.</span></span>  <br/> |
|[<span data-ttu-id="ad380-122">Повторение (TaskRecurrenceType)</span><span class="sxs-lookup"><span data-stu-id="ad380-122">Recurrence (TaskRecurrenceType)</span></span>](recurrence-taskrecurrencetype.md) <br/> |<span data-ttu-id="ad380-123">Содержит шаблон повторения для повторяющихся задач.</span><span class="sxs-lookup"><span data-stu-id="ad380-123">Contains the recurrence pattern for recurring tasks.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="ad380-124">Замечания</span><span class="sxs-lookup"><span data-stu-id="ad380-124">Remarks</span></span>

<span data-ttu-id="ad380-125">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="ad380-125">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ad380-126">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="ad380-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ad380-127">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="ad380-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="ad380-128">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="ad380-128">Schema name</span></span>  <br/> |<span data-ttu-id="ad380-129">Схема Types</span><span class="sxs-lookup"><span data-stu-id="ad380-129">Types schema</span></span>  <br/> |
|<span data-ttu-id="ad380-130">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="ad380-130">Validation file</span></span>  <br/> |<span data-ttu-id="ad380-131">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="ad380-131">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="ad380-132">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="ad380-132">Can be empty</span></span>  <br/> |<span data-ttu-id="ad380-133">False</span><span class="sxs-lookup"><span data-stu-id="ad380-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ad380-134">См. также</span><span class="sxs-lookup"><span data-stu-id="ad380-134">See also</span></span>



- [<span data-ttu-id="ad380-135">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="ad380-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

