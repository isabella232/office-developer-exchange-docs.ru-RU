---
title: NumberedRecurrence
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- NumberedRecurrence
api_type:
- schema
ms.assetid: 53746909-ef21-4764-8715-a7769b943cca
description: Элемент NumberedRecurrence описание, Дата начала и число вхождений повторяющегося элемента.
ms.openlocfilehash: 01fbf831fa7ff378221d4db3d873af730ac564d8
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834628"
---
# <a name="numberedrecurrence"></a><span data-ttu-id="d4bb6-103">NumberedRecurrence</span><span class="sxs-lookup"><span data-stu-id="d4bb6-103">NumberedRecurrence</span></span>

<span data-ttu-id="d4bb6-104">Элемент **NumberedRecurrence** описание, Дата начала и число вхождений повторяющегося элемента.</span><span class="sxs-lookup"><span data-stu-id="d4bb6-104">The **NumberedRecurrence** element describes the start date and the number of occurrences of a recurring item.</span></span> 
  
```xml
<NumberedRecurrence>
   <StartDate/>
   <NumberOfOccurrences/>
</NumberedRecurrence>
```

 <span data-ttu-id="d4bb6-105">**NumberedRecurrenceRangeType**</span><span class="sxs-lookup"><span data-stu-id="d4bb6-105">**NumberedRecurrenceRangeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d4bb6-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="d4bb6-106">Attributes and elements</span></span>

<span data-ttu-id="d4bb6-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="d4bb6-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d4bb6-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="d4bb6-108">Attributes</span></span>

<span data-ttu-id="d4bb6-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="d4bb6-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d4bb6-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="d4bb6-110">Child elements</span></span>

|<span data-ttu-id="d4bb6-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="d4bb6-111">**Element**</span></span>|<span data-ttu-id="d4bb6-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d4bb6-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d4bb6-113">StartDate (повторения)</span><span class="sxs-lookup"><span data-stu-id="d4bb6-113">StartDate (Recurrence)</span></span>](startdate-recurrence.md) <br/> |<span data-ttu-id="d4bb6-114">Представляет дату начала повторяющейся задачи или элемента календаря.</span><span class="sxs-lookup"><span data-stu-id="d4bb6-114">Represents the start date of a recurring task or calendar item.</span></span>  <br/> |
|[<span data-ttu-id="d4bb6-115">NumberOfOccurrences</span><span class="sxs-lookup"><span data-stu-id="d4bb6-115">NumberOfOccurrences</span></span>](numberofoccurrences.md) <br/> |<span data-ttu-id="d4bb6-116">Содержит число вхождений повторяющегося элемента.</span><span class="sxs-lookup"><span data-stu-id="d4bb6-116">Contains the number of occurrences of a recurring item.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d4bb6-117">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="d4bb6-117">Parent elements</span></span>

|<span data-ttu-id="d4bb6-118">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="d4bb6-118">**Element**</span></span>|<span data-ttu-id="d4bb6-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d4bb6-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d4bb6-120">Повторение (RecurrenceType)</span><span class="sxs-lookup"><span data-stu-id="d4bb6-120">Recurrence (RecurrenceType)</span></span>](recurrence-recurrencetype.md) <br/> |<span data-ttu-id="d4bb6-121">Содержит шаблон повторения для элементов календаря и приглашения на собрания.</span><span class="sxs-lookup"><span data-stu-id="d4bb6-121">Contains the recurrence pattern for calendar items and meeting requests.</span></span>  <br/> |
|[<span data-ttu-id="d4bb6-122">Повторение (TaskRecurrenceType)</span><span class="sxs-lookup"><span data-stu-id="d4bb6-122">Recurrence (TaskRecurrenceType)</span></span>](recurrence-taskrecurrencetype.md) <br/> |<span data-ttu-id="d4bb6-123">Содержит данные о повторении для повторяющихся задач.</span><span class="sxs-lookup"><span data-stu-id="d4bb6-123">Contains recurrence information for recurring tasks.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="d4bb6-124">Замечания</span><span class="sxs-lookup"><span data-stu-id="d4bb6-124">Remarks</span></span>

<span data-ttu-id="d4bb6-125">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="d4bb6-125">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d4bb6-126">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="d4bb6-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d4bb6-127">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="d4bb6-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d4bb6-128">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="d4bb6-128">Schema name</span></span>  <br/> |<span data-ttu-id="d4bb6-129">Схема Types</span><span class="sxs-lookup"><span data-stu-id="d4bb6-129">Types schema</span></span>  <br/> |
|<span data-ttu-id="d4bb6-130">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="d4bb6-130">Validation file</span></span>  <br/> |<span data-ttu-id="d4bb6-131">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="d4bb6-131">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d4bb6-132">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="d4bb6-132">Can be empty</span></span>  <br/> |<span data-ttu-id="d4bb6-133">False</span><span class="sxs-lookup"><span data-stu-id="d4bb6-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d4bb6-134">См. также</span><span class="sxs-lookup"><span data-stu-id="d4bb6-134">See also</span></span>



- [<span data-ttu-id="d4bb6-135">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="d4bb6-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

