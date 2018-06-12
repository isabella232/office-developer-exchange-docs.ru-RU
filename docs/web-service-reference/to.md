---
title: Чтобы
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- To
api_type:
- schema
ms.assetid: d14e46da-14bd-4a33-a78e-8ee314d9c1d8
description: Элемент кому указывает целевой перехода часового пояса. Целевой объект является период часовой пояс или группу переходы часового пояса.
ms.openlocfilehash: dc7df8ed3ddd6a9b4222ffab4c2b47b00ee4ba0c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19840194"
---
# <a name="to"></a><span data-ttu-id="931b6-104">Чтобы</span><span class="sxs-lookup"><span data-stu-id="931b6-104">To</span></span>

<span data-ttu-id="931b6-105">Элемент **для** указывает целевой перехода часового пояса.</span><span class="sxs-lookup"><span data-stu-id="931b6-105">The **To** element specifies the target of the time zone transition.</span></span> <span data-ttu-id="931b6-106">Целевой объект является период часовой пояс или группу переходы часового пояса.</span><span class="sxs-lookup"><span data-stu-id="931b6-106">The target is either a time zone period or a group of time zone transitions.</span></span> 
  
```xml
<To Kind=""/>
```

 <span data-ttu-id="931b6-107">**TransitionTargetType**</span><span class="sxs-lookup"><span data-stu-id="931b6-107">**TransitionTargetType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="931b6-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="931b6-108">Attributes and elements</span></span>

<span data-ttu-id="931b6-109">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="931b6-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="931b6-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="931b6-110">Attributes</span></span>

|<span data-ttu-id="931b6-111">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="931b6-111">**Attribute**</span></span>|<span data-ttu-id="931b6-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="931b6-112">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="931b6-113">Тип</span><span class="sxs-lookup"><span data-stu-id="931b6-113">Kind</span></span>  <br/> |<span data-ttu-id="931b6-114">Указывает целевой перехода часовой пояс — это часовой пояс периода или группы переходы часового пояса.</span><span class="sxs-lookup"><span data-stu-id="931b6-114">Indicates whether the time zone transition target is a time zone period or of a group of time zone transitions.</span></span>  <br/> |
   
#### <a name="kind-attribute-values"></a><span data-ttu-id="931b6-115">Атрибут вида значений</span><span class="sxs-lookup"><span data-stu-id="931b6-115">Kind attribute values</span></span>

|<span data-ttu-id="931b6-116">**Значение**</span><span class="sxs-lookup"><span data-stu-id="931b6-116">**Value**</span></span>|<span data-ttu-id="931b6-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="931b6-117">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="931b6-118">Точка</span><span class="sxs-lookup"><span data-stu-id="931b6-118">Period</span></span>  <br/> |<span data-ttu-id="931b6-119">Указывает, что целевой перехода часовой пояс периода часового пояса.</span><span class="sxs-lookup"><span data-stu-id="931b6-119">Specifies that the time zone transition target is a time zone period.</span></span>  <br/> |
|<span data-ttu-id="931b6-120">Группа</span><span class="sxs-lookup"><span data-stu-id="931b6-120">Group</span></span>  <br/> |<span data-ttu-id="931b6-121">Указывает, что целевой перехода часовой пояс группы переходы часового пояса.</span><span class="sxs-lookup"><span data-stu-id="931b6-121">Specifies that the time zone transition target is a group of time zone transitions.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="931b6-122">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="931b6-122">Child elements</span></span>

<span data-ttu-id="931b6-123">Нет.</span><span class="sxs-lookup"><span data-stu-id="931b6-123">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="931b6-124">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="931b6-124">Parent elements</span></span>

|<span data-ttu-id="931b6-125">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="931b6-125">**Element**</span></span>|<span data-ttu-id="931b6-126">**Описание**</span><span class="sxs-lookup"><span data-stu-id="931b6-126">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="931b6-127">AbsoluteDateTransition</span><span class="sxs-lookup"><span data-stu-id="931b6-127">AbsoluteDateTransition</span></span>](absolutedatetransition.md) <br/> |<span data-ttu-id="931b6-128">Представляет переход часовой пояс, который создается в конкретный день и в определенное время.</span><span class="sxs-lookup"><span data-stu-id="931b6-128">Represents a time zone transition that occurs on a specific date and at a specific time.</span></span>  <br/> |
|[<span data-ttu-id="931b6-129">RecurringDayTransition</span><span class="sxs-lookup"><span data-stu-id="931b6-129">RecurringDayTransition</span></span>](recurringdaytransition.md) <br/> |<span data-ttu-id="931b6-130">Представляет переход часового пояса, что происходит в тот же день каждый год.</span><span class="sxs-lookup"><span data-stu-id="931b6-130">Represents a time zone transition that occurs on the same day each year.</span></span>  <br/> |
|[<span data-ttu-id="931b6-131">RecurringDateTransition</span><span class="sxs-lookup"><span data-stu-id="931b6-131">RecurringDateTransition</span></span>](recurringdatetransition.md) <br/> |<span data-ttu-id="931b6-132">Представляет переход часового пояса, что происходит на указанном дня года.</span><span class="sxs-lookup"><span data-stu-id="931b6-132">Represents a time zone transition that occurs on a specified day of the year.</span></span>  <br/> |
|[<span data-ttu-id="931b6-133">Переход</span><span class="sxs-lookup"><span data-stu-id="931b6-133">Transition</span></span>](transition.md) <br/> |<span data-ttu-id="931b6-134">Представляет переход часового пояса.</span><span class="sxs-lookup"><span data-stu-id="931b6-134">Represents a time zone transition.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="931b6-135">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="931b6-135">Text value</span></span>

<span data-ttu-id="931b6-136">Текстовое значение — это строка, которая указывает уникальный идентификатор [периода](period.md) или [TransitionsGroup](transitionsgroup.md) , который является целевым для перехода часового пояса.</span><span class="sxs-lookup"><span data-stu-id="931b6-136">The text value is a string that specifies the unique identifier of the [Period](period.md) or [TransitionsGroup](transitionsgroup.md) that is the target of the time zone transition.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="931b6-137">Замечания</span><span class="sxs-lookup"><span data-stu-id="931b6-137">Remarks</span></span>

<span data-ttu-id="931b6-138">Схема, описывающая этот элемент находится в виртуальном каталоге EWS компьютера, на котором выполняется Microsoft Exchange Server с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="931b6-138">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="931b6-139">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="931b6-139">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="931b6-140">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="931b6-140">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="931b6-141">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="931b6-141">Schema Name</span></span>  <br/> |<span data-ttu-id="931b6-142">Схема Types</span><span class="sxs-lookup"><span data-stu-id="931b6-142">Types schema</span></span>  <br/> |
|<span data-ttu-id="931b6-143">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="931b6-143">Validation File</span></span>  <br/> |<span data-ttu-id="931b6-144">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="931b6-144">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="931b6-145">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="931b6-145">Can be Empty</span></span>  <br/> |<span data-ttu-id="931b6-146">False</span><span class="sxs-lookup"><span data-stu-id="931b6-146">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="931b6-147">См. также</span><span class="sxs-lookup"><span data-stu-id="931b6-147">See also</span></span>



- [<span data-ttu-id="931b6-148">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="931b6-148">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

