---
title: ноендрекурренце
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
description: Элемент Ноендрекурренце описывает дату начала для шаблона повторения элемента, у которого нет определенной конечной даты.
ms.openlocfilehash: fc3eae170f5c07e31d7a80b45836efd07d74e543
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834537"
---
# <a name="noendrecurrence"></a><span data-ttu-id="5db46-103">ноендрекурренце</span><span class="sxs-lookup"><span data-stu-id="5db46-103">NoEndRecurrence</span></span>

<span data-ttu-id="5db46-104">Элемент **ноендрекурренце** описывает дату начала для шаблона повторения элемента, у которого нет определенной конечной даты.</span><span class="sxs-lookup"><span data-stu-id="5db46-104">The **NoEndRecurrence** element describes the start date of an item recurrence pattern that does not have a defined end date.</span></span> 
  
```xml
<NoEndRecurrence>
   <StartDate/>
</NoEndRecurrence>
```

 <span data-ttu-id="5db46-105">**ноендрекурренцеранжетипе**</span><span class="sxs-lookup"><span data-stu-id="5db46-105">**NoEndRecurrenceRangeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5db46-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="5db46-106">Attributes and elements</span></span>

<span data-ttu-id="5db46-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="5db46-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5db46-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="5db46-108">Attributes</span></span>

<span data-ttu-id="5db46-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="5db46-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5db46-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="5db46-110">Child elements</span></span>

|<span data-ttu-id="5db46-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="5db46-111">**Element**</span></span>|<span data-ttu-id="5db46-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="5db46-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5db46-113">StartDate (повторение)</span><span class="sxs-lookup"><span data-stu-id="5db46-113">StartDate (Recurrence)</span></span>](startdate-recurrence.md) <br/> |<span data-ttu-id="5db46-114">Представляет дату начала повторяющейся задачи или элемента календаря.</span><span class="sxs-lookup"><span data-stu-id="5db46-114">Represents the start date of a recurring task or calendar item.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="5db46-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="5db46-115">Parent elements</span></span>

|<span data-ttu-id="5db46-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="5db46-116">**Element**</span></span>|<span data-ttu-id="5db46-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="5db46-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5db46-118">Повторение (RecurrenceType)</span><span class="sxs-lookup"><span data-stu-id="5db46-118">Recurrence (RecurrenceType)</span></span>](recurrence-recurrencetype.md) <br/> |<span data-ttu-id="5db46-119">Содержит шаблон повторения для элементов календаря и приглашений на собрание.</span><span class="sxs-lookup"><span data-stu-id="5db46-119">Contains the recurrence pattern for calendar items and meeting requests.</span></span>  <br/> |
|[<span data-ttu-id="5db46-120">Повторение (Таскрекурренцетипе)</span><span class="sxs-lookup"><span data-stu-id="5db46-120">Recurrence (TaskRecurrenceType)</span></span>](recurrence-taskrecurrencetype.md) <br/> |<span data-ttu-id="5db46-121">Содержит сведения о повторении для повторяющихся задач.</span><span class="sxs-lookup"><span data-stu-id="5db46-121">Contains recurrence information for recurring tasks.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="5db46-122">Примечания</span><span class="sxs-lookup"><span data-stu-id="5db46-122">Remarks</span></span>

<span data-ttu-id="5db46-123">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="5db46-123">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5db46-124">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="5db46-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5db46-125">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="5db46-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="5db46-126">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="5db46-126">Schema name</span></span>  <br/> |<span data-ttu-id="5db46-127">Схема Types</span><span class="sxs-lookup"><span data-stu-id="5db46-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="5db46-128">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="5db46-128">Validation file</span></span>  <br/> |<span data-ttu-id="5db46-129">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="5db46-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="5db46-130">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="5db46-130">Can be empty</span></span>  <br/> |<span data-ttu-id="5db46-131">False</span><span class="sxs-lookup"><span data-stu-id="5db46-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="5db46-132">См. также</span><span class="sxs-lookup"><span data-stu-id="5db46-132">See also</span></span>



- [<span data-ttu-id="5db46-133">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="5db46-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

