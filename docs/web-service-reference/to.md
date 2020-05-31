---
title: To
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
description: Элемент to указывает целевой объект перехода часового пояса. Целевой объект — это период времени часового пояса или группа переходов часового пояса.
ms.openlocfilehash: dc7df8ed3ddd6a9b4222ffab4c2b47b00ee4ba0c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19840194"
---
# <a name="to"></a><span data-ttu-id="bee9d-104">To</span><span class="sxs-lookup"><span data-stu-id="bee9d-104">To</span></span>

<span data-ttu-id="bee9d-105">Элемент **to** указывает целевой объект перехода часового пояса.</span><span class="sxs-lookup"><span data-stu-id="bee9d-105">The **To** element specifies the target of the time zone transition.</span></span> <span data-ttu-id="bee9d-106">Целевой объект — это период времени часового пояса или группа переходов часового пояса.</span><span class="sxs-lookup"><span data-stu-id="bee9d-106">The target is either a time zone period or a group of time zone transitions.</span></span> 
  
```xml
<To Kind=""/>
```

 <span data-ttu-id="bee9d-107">**транситионтаржеттипе**</span><span class="sxs-lookup"><span data-stu-id="bee9d-107">**TransitionTargetType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="bee9d-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="bee9d-108">Attributes and elements</span></span>

<span data-ttu-id="bee9d-109">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="bee9d-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="bee9d-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="bee9d-110">Attributes</span></span>

|<span data-ttu-id="bee9d-111">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="bee9d-111">**Attribute**</span></span>|<span data-ttu-id="bee9d-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="bee9d-112">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="bee9d-113">Kind</span><span class="sxs-lookup"><span data-stu-id="bee9d-113">Kind</span></span>  <br/> |<span data-ttu-id="bee9d-114">Указывает, является ли целевой объект перехода часового пояса периодом часового пояса или группой переходов часового пояса.</span><span class="sxs-lookup"><span data-stu-id="bee9d-114">Indicates whether the time zone transition target is a time zone period or of a group of time zone transitions.</span></span>  <br/> |
   
#### <a name="kind-attribute-values"></a><span data-ttu-id="bee9d-115">Значения атрибутов Kind</span><span class="sxs-lookup"><span data-stu-id="bee9d-115">Kind attribute values</span></span>

|<span data-ttu-id="bee9d-116">**Значение**</span><span class="sxs-lookup"><span data-stu-id="bee9d-116">**Value**</span></span>|<span data-ttu-id="bee9d-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="bee9d-117">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="bee9d-118">Period</span><span class="sxs-lookup"><span data-stu-id="bee9d-118">Period</span></span>  <br/> |<span data-ttu-id="bee9d-119">Указывает, что целевой объект перехода часового пояса является периодом часового пояса.</span><span class="sxs-lookup"><span data-stu-id="bee9d-119">Specifies that the time zone transition target is a time zone period.</span></span>  <br/> |
|<span data-ttu-id="bee9d-120">Group</span><span class="sxs-lookup"><span data-stu-id="bee9d-120">Group</span></span>  <br/> |<span data-ttu-id="bee9d-121">Указывает, что целевой объект перехода часового пояса является группой переходов часового пояса.</span><span class="sxs-lookup"><span data-stu-id="bee9d-121">Specifies that the time zone transition target is a group of time zone transitions.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="bee9d-122">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="bee9d-122">Child elements</span></span>

<span data-ttu-id="bee9d-123">Нет.</span><span class="sxs-lookup"><span data-stu-id="bee9d-123">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="bee9d-124">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="bee9d-124">Parent elements</span></span>

|<span data-ttu-id="bee9d-125">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="bee9d-125">**Element**</span></span>|<span data-ttu-id="bee9d-126">**Описание**</span><span class="sxs-lookup"><span data-stu-id="bee9d-126">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bee9d-127">абсолутедатетранситион</span><span class="sxs-lookup"><span data-stu-id="bee9d-127">AbsoluteDateTransition</span></span>](absolutedatetransition.md) <br/> |<span data-ttu-id="bee9d-128">Представляет переход часового пояса, который выполняется в определенный день и в определенное время.</span><span class="sxs-lookup"><span data-stu-id="bee9d-128">Represents a time zone transition that occurs on a specific date and at a specific time.</span></span>  <br/> |
|[<span data-ttu-id="bee9d-129">рекуррингдайтранситион</span><span class="sxs-lookup"><span data-stu-id="bee9d-129">RecurringDayTransition</span></span>](recurringdaytransition.md) <br/> |<span data-ttu-id="bee9d-130">Представляет переход часового пояса, который выполняется в один день каждого года.</span><span class="sxs-lookup"><span data-stu-id="bee9d-130">Represents a time zone transition that occurs on the same day each year.</span></span>  <br/> |
|[<span data-ttu-id="bee9d-131">рекуррингдатетранситион</span><span class="sxs-lookup"><span data-stu-id="bee9d-131">RecurringDateTransition</span></span>](recurringdatetransition.md) <br/> |<span data-ttu-id="bee9d-132">Представляет переход часового пояса, который выполняется в указанный день года.</span><span class="sxs-lookup"><span data-stu-id="bee9d-132">Represents a time zone transition that occurs on a specified day of the year.</span></span>  <br/> |
|[<span data-ttu-id="bee9d-133">Ветвление</span><span class="sxs-lookup"><span data-stu-id="bee9d-133">Transition</span></span>](transition.md) <br/> |<span data-ttu-id="bee9d-134">Представляет переход часового пояса.</span><span class="sxs-lookup"><span data-stu-id="bee9d-134">Represents a time zone transition.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="bee9d-135">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="bee9d-135">Text value</span></span>

<span data-ttu-id="bee9d-136">Текстовое значение — это строка, указывающая уникальный идентификатор [периода](period.md) или [транситионсграуп](transitionsgroup.md) , который является целевым объектом перехода часового пояса.</span><span class="sxs-lookup"><span data-stu-id="bee9d-136">The text value is a string that specifies the unique identifier of the [Period](period.md) or [TransitionsGroup](transitionsgroup.md) that is the target of the time zone transition.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="bee9d-137">Примечания</span><span class="sxs-lookup"><span data-stu-id="bee9d-137">Remarks</span></span>

<span data-ttu-id="bee9d-138">Схема, описывающая этот элемент, находится в виртуальном каталоге EWS компьютера, на котором работает сервер Microsoft Exchange с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="bee9d-138">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="bee9d-139">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="bee9d-139">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="bee9d-140">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="bee9d-140">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="bee9d-141">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="bee9d-141">Schema Name</span></span>  <br/> |<span data-ttu-id="bee9d-142">Схема Types</span><span class="sxs-lookup"><span data-stu-id="bee9d-142">Types schema</span></span>  <br/> |
|<span data-ttu-id="bee9d-143">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="bee9d-143">Validation File</span></span>  <br/> |<span data-ttu-id="bee9d-144">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="bee9d-144">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="bee9d-145">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="bee9d-145">Can be Empty</span></span>  <br/> |<span data-ttu-id="bee9d-146">False</span><span class="sxs-lookup"><span data-stu-id="bee9d-146">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="bee9d-147">См. также</span><span class="sxs-lookup"><span data-stu-id="bee9d-147">See also</span></span>



- [<span data-ttu-id="bee9d-148">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="bee9d-148">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

