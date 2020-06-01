---
title: енддатерекурренце
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
description: Элемент Енддатерекурренце описывает дату начала и дату окончания расписания повторения элемента.
ms.openlocfilehash: e8ae72012e5bcac8d8b2a06b6d3a9b3a7caf30d7
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460150"
---
# <a name="enddaterecurrence"></a><span data-ttu-id="55199-103">енддатерекурренце</span><span class="sxs-lookup"><span data-stu-id="55199-103">EndDateRecurrence</span></span>

<span data-ttu-id="55199-104">Элемент **енддатерекурренце** описывает дату начала и дату окончания расписания повторения элемента.</span><span class="sxs-lookup"><span data-stu-id="55199-104">The **EndDateRecurrence** element describes the start date and the end date of an item recurrence pattern.</span></span> 
  
```xml
<EndDateRecurrence>
   <StartDate/>
   <EndDate/>
</EndDateRecurrence>
```

 <span data-ttu-id="55199-105">**енддатерекурренцеранжетипе**</span><span class="sxs-lookup"><span data-stu-id="55199-105">**EndDateRecurrenceRangeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="55199-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="55199-106">Attributes and elements</span></span>

<span data-ttu-id="55199-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="55199-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="55199-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="55199-108">Attributes</span></span>

<span data-ttu-id="55199-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="55199-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="55199-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="55199-110">Child elements</span></span>

|<span data-ttu-id="55199-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="55199-111">**Element**</span></span>|<span data-ttu-id="55199-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="55199-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="55199-113">StartDate (повторение)</span><span class="sxs-lookup"><span data-stu-id="55199-113">StartDate (Recurrence)</span></span>](startdate-recurrence.md) <br/> |<span data-ttu-id="55199-114">Представляет дату начала повторяющейся задачи или элемента календаря.</span><span class="sxs-lookup"><span data-stu-id="55199-114">Represents the start date of a recurring task or calendar item.</span></span>  <br/> |
|[<span data-ttu-id="55199-115">EndDate (повторение)</span><span class="sxs-lookup"><span data-stu-id="55199-115">EndDate (Recurrence)</span></span>](enddate-recurrence.md) <br/> |<span data-ttu-id="55199-116">Представляет дату окончания повторяющейся задачи или элемента календаря.</span><span class="sxs-lookup"><span data-stu-id="55199-116">Represents the end date of a recurring task or calendar item.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="55199-117">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="55199-117">Parent elements</span></span>

|<span data-ttu-id="55199-118">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="55199-118">**Element**</span></span>|<span data-ttu-id="55199-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="55199-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="55199-120">Повторение (RecurrenceType)</span><span class="sxs-lookup"><span data-stu-id="55199-120">Recurrence (RecurrenceType)</span></span>](recurrence-recurrencetype.md) <br/> |<span data-ttu-id="55199-121">Содержит шаблон повторения для элементов календаря и приглашений на собрание.</span><span class="sxs-lookup"><span data-stu-id="55199-121">Contains the recurrence pattern for calendar items and meeting requests.</span></span>  <br/> |
|[<span data-ttu-id="55199-122">Повторение (Таскрекурренцетипе)</span><span class="sxs-lookup"><span data-stu-id="55199-122">Recurrence (TaskRecurrenceType)</span></span>](recurrence-taskrecurrencetype.md) <br/> |<span data-ttu-id="55199-123">Содержит шаблон повторения для повторяющихся задач.</span><span class="sxs-lookup"><span data-stu-id="55199-123">Contains the recurrence pattern for recurring tasks.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="55199-124">Примечания</span><span class="sxs-lookup"><span data-stu-id="55199-124">Remarks</span></span>

<span data-ttu-id="55199-125">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="55199-125">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="55199-126">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="55199-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="55199-127">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="55199-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="55199-128">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="55199-128">Schema name</span></span>  <br/> |<span data-ttu-id="55199-129">Схема Types</span><span class="sxs-lookup"><span data-stu-id="55199-129">Types schema</span></span>  <br/> |
|<span data-ttu-id="55199-130">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="55199-130">Validation file</span></span>  <br/> |<span data-ttu-id="55199-131">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="55199-131">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="55199-132">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="55199-132">Can be empty</span></span>  <br/> |<span data-ttu-id="55199-133">False</span><span class="sxs-lookup"><span data-stu-id="55199-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="55199-134">См. также</span><span class="sxs-lookup"><span data-stu-id="55199-134">See also</span></span>



- [<span data-ttu-id="55199-135">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="55199-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

