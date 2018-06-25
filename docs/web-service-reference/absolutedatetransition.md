---
title: AbsoluteDateTransition
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AbsoluteDateTransition
api_type:
- schema
ms.assetid: 8f5731eb-bed0-45bf-ba89-4aaf20c34a39
description: Элемент AbsoluteDateTransition представляет перехода часовой пояс, который создается в конкретный день и в определенное время.
ms.openlocfilehash: 1e9e5f3f2269814a82b827efe46c71a172e21348
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761324"
---
# <a name="absolutedatetransition"></a><span data-ttu-id="25dd7-103">AbsoluteDateTransition</span><span class="sxs-lookup"><span data-stu-id="25dd7-103">AbsoluteDateTransition</span></span>

<span data-ttu-id="25dd7-104">Элемент **AbsoluteDateTransition** представляет перехода часовой пояс, который создается в конкретный день и в определенное время.</span><span class="sxs-lookup"><span data-stu-id="25dd7-104">The **AbsoluteDateTransition** element represents a time zone transition that occurs on a specific date and at a specific time.</span></span> 
  
```xml
<AbsoluteDateTransition>
   <To/>
   <DateTime/>
</AbsoluteDateTransition>
```

<span data-ttu-id="25dd7-105">**AbsoluteDateTransitionType**</span><span class="sxs-lookup"><span data-stu-id="25dd7-105">**AbsoluteDateTransitionType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="25dd7-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="25dd7-106">Attributes and elements</span></span>

<span data-ttu-id="25dd7-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="25dd7-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="25dd7-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="25dd7-108">Attributes</span></span>

<span data-ttu-id="25dd7-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="25dd7-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="25dd7-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="25dd7-110">Child elements</span></span>

|<span data-ttu-id="25dd7-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="25dd7-111">**Element**</span></span>|<span data-ttu-id="25dd7-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="25dd7-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="25dd7-113">Задача</span><span class="sxs-lookup"><span data-stu-id="25dd7-113">To</span></span>](to.md) <br/> |<span data-ttu-id="25dd7-114">Задает [период](period.md) или [TransitionsGroup](transitionsgroup.md) , который является целевым для перехода часового пояса.</span><span class="sxs-lookup"><span data-stu-id="25dd7-114">Specifies the [Period](period.md) or [TransitionsGroup](transitionsgroup.md) that is the target of the time zone transition.</span></span>  <br/> |
|[<span data-ttu-id="25dd7-115">DateTime</span><span class="sxs-lookup"><span data-stu-id="25dd7-115">DateTime</span></span>](datetime.md) <br/> |<span data-ttu-id="25dd7-116">Представляет дату и время, когда происходит переход часового пояса.</span><span class="sxs-lookup"><span data-stu-id="25dd7-116">Represents the date and time at which the time zone transition occurs.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="25dd7-117">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="25dd7-117">Parent elements</span></span>

|<span data-ttu-id="25dd7-118">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="25dd7-118">**Element**</span></span>|<span data-ttu-id="25dd7-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="25dd7-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="25dd7-120">Переходы между</span><span class="sxs-lookup"><span data-stu-id="25dd7-120">Transitions</span></span>](transitions.md) <br/> |<span data-ttu-id="25dd7-121">Представляет коллекцию переходы часового пояса.</span><span class="sxs-lookup"><span data-stu-id="25dd7-121">Represents a collection of time zone transitions.</span></span>  <br/> |
|[<span data-ttu-id="25dd7-122">TransitionsGroup</span><span class="sxs-lookup"><span data-stu-id="25dd7-122">TransitionsGroup</span></span>](transitionsgroup.md) <br/> |<span data-ttu-id="25dd7-123">Представляет коллекцию переходы часового пояса.</span><span class="sxs-lookup"><span data-stu-id="25dd7-123">Represents a collection of time zone transitions.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="25dd7-124">Замечания</span><span class="sxs-lookup"><span data-stu-id="25dd7-124">Remarks</span></span>

<span data-ttu-id="25dd7-125">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="25dd7-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="25dd7-126">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="25dd7-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="25dd7-127">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="25dd7-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="25dd7-128">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="25dd7-128">Schema Name</span></span>  <br/> |<span data-ttu-id="25dd7-129">Схема Types</span><span class="sxs-lookup"><span data-stu-id="25dd7-129">Types schema</span></span>  <br/> |
|<span data-ttu-id="25dd7-130">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="25dd7-130">Validation File</span></span>  <br/> |<span data-ttu-id="25dd7-131">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="25dd7-131">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="25dd7-132">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="25dd7-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="25dd7-133">False</span><span class="sxs-lookup"><span data-stu-id="25dd7-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="25dd7-134">См. также</span><span class="sxs-lookup"><span data-stu-id="25dd7-134">See also</span></span>

- [<span data-ttu-id="25dd7-135">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="25dd7-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

