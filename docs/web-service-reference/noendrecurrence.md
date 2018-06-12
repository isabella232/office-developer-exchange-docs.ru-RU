---
title: NoEndRecurrence
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- NoEndRecurrence
api_type:
- schema
ms.assetid: ab2ebd9c-388e-45f1-abf9-56e293ef123b
description: Элемент NoEndRecurrence описывает дату начала повторения элемента, для которого не определенные дату.
ms.openlocfilehash: fc3eae170f5c07e31d7a80b45836efd07d74e543
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19834537"
---
# <a name="noendrecurrence"></a><span data-ttu-id="4cc3a-103">NoEndRecurrence</span><span class="sxs-lookup"><span data-stu-id="4cc3a-103">NoEndRecurrence</span></span>

<span data-ttu-id="4cc3a-104">Элемент **NoEndRecurrence** описывает дату начала повторения элемента, для которого не определенные дату.</span><span class="sxs-lookup"><span data-stu-id="4cc3a-104">The **NoEndRecurrence** element describes the start date of an item recurrence pattern that does not have a defined end date.</span></span> 
  
```xml
<NoEndRecurrence>
   <StartDate/>
</NoEndRecurrence>
```

 <span data-ttu-id="4cc3a-105">**NoEndRecurrenceRangeType**</span><span class="sxs-lookup"><span data-stu-id="4cc3a-105">**NoEndRecurrenceRangeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4cc3a-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="4cc3a-106">Attributes and elements</span></span>

<span data-ttu-id="4cc3a-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="4cc3a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4cc3a-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="4cc3a-108">Attributes</span></span>

<span data-ttu-id="4cc3a-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="4cc3a-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4cc3a-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="4cc3a-110">Child elements</span></span>

|<span data-ttu-id="4cc3a-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="4cc3a-111">**Element**</span></span>|<span data-ttu-id="4cc3a-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="4cc3a-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4cc3a-113">StartDate (повторения)</span><span class="sxs-lookup"><span data-stu-id="4cc3a-113">StartDate (Recurrence)</span></span>](startdate-recurrence.md) <br/> |<span data-ttu-id="4cc3a-114">Представляет дату начала повторяющейся задачи или элемента календаря.</span><span class="sxs-lookup"><span data-stu-id="4cc3a-114">Represents the start date of a recurring task or calendar item.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="4cc3a-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="4cc3a-115">Parent elements</span></span>

|<span data-ttu-id="4cc3a-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="4cc3a-116">**Element**</span></span>|<span data-ttu-id="4cc3a-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="4cc3a-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4cc3a-118">Повторение (RecurrenceType)</span><span class="sxs-lookup"><span data-stu-id="4cc3a-118">Recurrence (RecurrenceType)</span></span>](recurrence-recurrencetype.md) <br/> |<span data-ttu-id="4cc3a-119">Содержит шаблон повторения для элементов календаря и приглашения на собрания.</span><span class="sxs-lookup"><span data-stu-id="4cc3a-119">Contains the recurrence pattern for calendar items and meeting requests.</span></span>  <br/> |
|[<span data-ttu-id="4cc3a-120">Повторение (TaskRecurrenceType)</span><span class="sxs-lookup"><span data-stu-id="4cc3a-120">Recurrence (TaskRecurrenceType)</span></span>](recurrence-taskrecurrencetype.md) <br/> |<span data-ttu-id="4cc3a-121">Содержит данные о повторении для повторяющихся задач.</span><span class="sxs-lookup"><span data-stu-id="4cc3a-121">Contains recurrence information for recurring tasks.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="4cc3a-122">Замечания</span><span class="sxs-lookup"><span data-stu-id="4cc3a-122">Remarks</span></span>

<span data-ttu-id="4cc3a-123">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="4cc3a-123">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4cc3a-124">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="4cc3a-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4cc3a-125">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="4cc3a-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="4cc3a-126">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="4cc3a-126">Schema name</span></span>  <br/> |<span data-ttu-id="4cc3a-127">Схема Types</span><span class="sxs-lookup"><span data-stu-id="4cc3a-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="4cc3a-128">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="4cc3a-128">Validation file</span></span>  <br/> |<span data-ttu-id="4cc3a-129">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="4cc3a-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="4cc3a-130">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="4cc3a-130">Can be empty</span></span>  <br/> |<span data-ttu-id="4cc3a-131">False</span><span class="sxs-lookup"><span data-stu-id="4cc3a-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="4cc3a-132">См. также</span><span class="sxs-lookup"><span data-stu-id="4cc3a-132">See also</span></span>



- [<span data-ttu-id="4cc3a-133">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="4cc3a-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

