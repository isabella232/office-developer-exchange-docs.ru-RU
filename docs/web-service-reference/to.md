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
ms.openlocfilehash: 8cce700eedd64035f2e21be4db6b517f3f85d98d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44468798"
---
# <a name="to"></a><span data-ttu-id="619cc-104">To</span><span class="sxs-lookup"><span data-stu-id="619cc-104">To</span></span>

<span data-ttu-id="619cc-105">Элемент **to** указывает целевой объект перехода часового пояса.</span><span class="sxs-lookup"><span data-stu-id="619cc-105">The **To** element specifies the target of the time zone transition.</span></span> <span data-ttu-id="619cc-106">Целевой объект — это период времени часового пояса или группа переходов часового пояса.</span><span class="sxs-lookup"><span data-stu-id="619cc-106">The target is either a time zone period or a group of time zone transitions.</span></span> 
  
```xml
<To Kind=""/>
```

 <span data-ttu-id="619cc-107">**транситионтаржеттипе**</span><span class="sxs-lookup"><span data-stu-id="619cc-107">**TransitionTargetType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="619cc-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="619cc-108">Attributes and elements</span></span>

<span data-ttu-id="619cc-109">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="619cc-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="619cc-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="619cc-110">Attributes</span></span>

|<span data-ttu-id="619cc-111">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="619cc-111">**Attribute**</span></span>|<span data-ttu-id="619cc-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="619cc-112">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="619cc-113">Kind</span><span class="sxs-lookup"><span data-stu-id="619cc-113">Kind</span></span>  <br/> |<span data-ttu-id="619cc-114">Указывает, является ли целевой объект перехода часового пояса периодом часового пояса или группой переходов часового пояса.</span><span class="sxs-lookup"><span data-stu-id="619cc-114">Indicates whether the time zone transition target is a time zone period or of a group of time zone transitions.</span></span>  <br/> |
   
#### <a name="kind-attribute-values"></a><span data-ttu-id="619cc-115">Значения атрибутов Kind</span><span class="sxs-lookup"><span data-stu-id="619cc-115">Kind attribute values</span></span>

|<span data-ttu-id="619cc-116">**Значение**</span><span class="sxs-lookup"><span data-stu-id="619cc-116">**Value**</span></span>|<span data-ttu-id="619cc-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="619cc-117">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="619cc-118">Period</span><span class="sxs-lookup"><span data-stu-id="619cc-118">Period</span></span>  <br/> |<span data-ttu-id="619cc-119">Указывает, что целевой объект перехода часового пояса является периодом часового пояса.</span><span class="sxs-lookup"><span data-stu-id="619cc-119">Specifies that the time zone transition target is a time zone period.</span></span>  <br/> |
|<span data-ttu-id="619cc-120">Group</span><span class="sxs-lookup"><span data-stu-id="619cc-120">Group</span></span>  <br/> |<span data-ttu-id="619cc-121">Указывает, что целевой объект перехода часового пояса является группой переходов часового пояса.</span><span class="sxs-lookup"><span data-stu-id="619cc-121">Specifies that the time zone transition target is a group of time zone transitions.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="619cc-122">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="619cc-122">Child elements</span></span>

<span data-ttu-id="619cc-123">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="619cc-123">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="619cc-124">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="619cc-124">Parent elements</span></span>

|<span data-ttu-id="619cc-125">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="619cc-125">**Element**</span></span>|<span data-ttu-id="619cc-126">**Описание**</span><span class="sxs-lookup"><span data-stu-id="619cc-126">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="619cc-127">абсолутедатетранситион</span><span class="sxs-lookup"><span data-stu-id="619cc-127">AbsoluteDateTransition</span></span>](absolutedatetransition.md) <br/> |<span data-ttu-id="619cc-128">Представляет переход часового пояса, который выполняется в определенный день и в определенное время.</span><span class="sxs-lookup"><span data-stu-id="619cc-128">Represents a time zone transition that occurs on a specific date and at a specific time.</span></span>  <br/> |
|[<span data-ttu-id="619cc-129">рекуррингдайтранситион</span><span class="sxs-lookup"><span data-stu-id="619cc-129">RecurringDayTransition</span></span>](recurringdaytransition.md) <br/> |<span data-ttu-id="619cc-130">Представляет переход часового пояса, который выполняется в один день каждого года.</span><span class="sxs-lookup"><span data-stu-id="619cc-130">Represents a time zone transition that occurs on the same day each year.</span></span>  <br/> |
|[<span data-ttu-id="619cc-131">рекуррингдатетранситион</span><span class="sxs-lookup"><span data-stu-id="619cc-131">RecurringDateTransition</span></span>](recurringdatetransition.md) <br/> |<span data-ttu-id="619cc-132">Представляет переход часового пояса, который выполняется в указанный день года.</span><span class="sxs-lookup"><span data-stu-id="619cc-132">Represents a time zone transition that occurs on a specified day of the year.</span></span>  <br/> |
|[<span data-ttu-id="619cc-133">Ветвление</span><span class="sxs-lookup"><span data-stu-id="619cc-133">Transition</span></span>](transition.md) <br/> |<span data-ttu-id="619cc-134">Представляет переход часового пояса.</span><span class="sxs-lookup"><span data-stu-id="619cc-134">Represents a time zone transition.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="619cc-135">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="619cc-135">Text value</span></span>

<span data-ttu-id="619cc-136">Текстовое значение — это строка, указывающая уникальный идентификатор [периода](period.md) или [транситионсграуп](transitionsgroup.md) , который является целевым объектом перехода часового пояса.</span><span class="sxs-lookup"><span data-stu-id="619cc-136">The text value is a string that specifies the unique identifier of the [Period](period.md) or [TransitionsGroup](transitionsgroup.md) that is the target of the time zone transition.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="619cc-137">Примечания</span><span class="sxs-lookup"><span data-stu-id="619cc-137">Remarks</span></span>

<span data-ttu-id="619cc-138">Схема, описывающая этот элемент, находится в виртуальном каталоге EWS компьютера, на котором работает сервер Microsoft Exchange с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="619cc-138">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="619cc-139">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="619cc-139">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="619cc-140">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="619cc-140">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="619cc-141">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="619cc-141">Schema Name</span></span>  <br/> |<span data-ttu-id="619cc-142">Схема Types</span><span class="sxs-lookup"><span data-stu-id="619cc-142">Types schema</span></span>  <br/> |
|<span data-ttu-id="619cc-143">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="619cc-143">Validation File</span></span>  <br/> |<span data-ttu-id="619cc-144">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="619cc-144">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="619cc-145">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="619cc-145">Can be Empty</span></span>  <br/> |<span data-ttu-id="619cc-146">False</span><span class="sxs-lookup"><span data-stu-id="619cc-146">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="619cc-147">См. также</span><span class="sxs-lookup"><span data-stu-id="619cc-147">See also</span></span>



- [<span data-ttu-id="619cc-148">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="619cc-148">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

