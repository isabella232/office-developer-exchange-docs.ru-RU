---
title: TransitionsGroup
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- TransitionsGroup
api_type:
- schema
ms.assetid: 19d56080-546a-4d53-929e-363d56186759
description: Элемент TransitionsGroup представляет массив переходы часового пояса.
ms.openlocfilehash: e5991ad7f73a1694e0d4abadd8d252acc04970e5
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19840238"
---
# <a name="transitionsgroup"></a><span data-ttu-id="6e051-103">TransitionsGroup</span><span class="sxs-lookup"><span data-stu-id="6e051-103">TransitionsGroup</span></span>

<span data-ttu-id="6e051-104">Элемент **TransitionsGroup** представляет массив переходы часового пояса.</span><span class="sxs-lookup"><span data-stu-id="6e051-104">The **TransitionsGroup** element represents an array of time zone transitions.</span></span> 
  
```xml
<TransitionsGroup Id="">
   <AbsoluteDateTransition/>
   <RecurringDayTransition/>
   <RecurringDateTransition/>
</TransitionsGroup>
```

 <span data-ttu-id="6e051-105">**ArrayOfTransitionsType**</span><span class="sxs-lookup"><span data-stu-id="6e051-105">**ArrayOfTransitionsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6e051-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="6e051-106">Attributes and elements</span></span>

<span data-ttu-id="6e051-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="6e051-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6e051-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="6e051-108">Attributes</span></span>

|<span data-ttu-id="6e051-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="6e051-109">**Attribute**</span></span>|<span data-ttu-id="6e051-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="6e051-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="6e051-111">Id</span><span class="sxs-lookup"><span data-stu-id="6e051-111">Id</span></span>  <br/> |<span data-ttu-id="6e051-112">Строковое значение, представляющее уникальный идентификатор группы между слайдами.</span><span class="sxs-lookup"><span data-stu-id="6e051-112">A string value that represents the unique identifier of the transitions group.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="6e051-113">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="6e051-113">Child elements</span></span>

|<span data-ttu-id="6e051-114">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="6e051-114">**Element**</span></span>|<span data-ttu-id="6e051-115">**Описание**</span><span class="sxs-lookup"><span data-stu-id="6e051-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6e051-116">AbsoluteDateTransition</span><span class="sxs-lookup"><span data-stu-id="6e051-116">AbsoluteDateTransition</span></span>](absolutedatetransition.md) <br/> |<span data-ttu-id="6e051-117">Представляет переход часовой пояс, который создается в конкретный день и в определенное время.</span><span class="sxs-lookup"><span data-stu-id="6e051-117">Represents a time zone transition that occurs on a specific date and at a specific time.</span></span>  <br/> |
|[<span data-ttu-id="6e051-118">RecurringDayTransition</span><span class="sxs-lookup"><span data-stu-id="6e051-118">RecurringDayTransition</span></span>](recurringdaytransition.md) <br/> |<span data-ttu-id="6e051-119">Представляет переход часового пояса, что происходит в тот же день каждый год.</span><span class="sxs-lookup"><span data-stu-id="6e051-119">Represents a time zone transition that occurs on the same day each year.</span></span>  <br/> |
|[<span data-ttu-id="6e051-120">RecurringDateTransition</span><span class="sxs-lookup"><span data-stu-id="6e051-120">RecurringDateTransition</span></span>](recurringdatetransition.md) <br/> |<span data-ttu-id="6e051-121">Представляет переход часового пояса, что происходит на указанном дня года.</span><span class="sxs-lookup"><span data-stu-id="6e051-121">Represents a time zone transition that occurs on a specified day of the year.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="6e051-122">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="6e051-122">Parent elements</span></span>

|<span data-ttu-id="6e051-123">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="6e051-123">**Element**</span></span>|<span data-ttu-id="6e051-124">**Описание**</span><span class="sxs-lookup"><span data-stu-id="6e051-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6e051-125">TransitionsGroups</span><span class="sxs-lookup"><span data-stu-id="6e051-125">TransitionsGroups</span></span>](transitionsgroups.md) <br/> |<span data-ttu-id="6e051-126">Представляет массив групп перехода часового пояса.</span><span class="sxs-lookup"><span data-stu-id="6e051-126">Represents an array of time zone transition groups.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="6e051-127">Замечания</span><span class="sxs-lookup"><span data-stu-id="6e051-127">Remarks</span></span>

<span data-ttu-id="6e051-128">Схема, описывающая этот элемент находится в виртуальном каталоге EWS компьютера, на котором выполняется Microsoft Exchange Server с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="6e051-128">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6e051-129">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="6e051-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6e051-130">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="6e051-130">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="6e051-131">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="6e051-131">Schema Name</span></span>  <br/> |<span data-ttu-id="6e051-132">Схема Types</span><span class="sxs-lookup"><span data-stu-id="6e051-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="6e051-133">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="6e051-133">Validation File</span></span>  <br/> |<span data-ttu-id="6e051-134">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="6e051-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="6e051-135">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="6e051-135">Can be Empty</span></span>  <br/> |<span data-ttu-id="6e051-136">False</span><span class="sxs-lookup"><span data-stu-id="6e051-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6e051-137">См. также</span><span class="sxs-lookup"><span data-stu-id="6e051-137">See also</span></span>



- [<span data-ttu-id="6e051-138">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="6e051-138">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

