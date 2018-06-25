---
title: Месяц (часовой пояс переходов)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Month
api_type:
- schema
ms.assetid: 5e6aac75-366d-43d0-8ccb-956285474662
description: Элемент Month представляет месяц, в котором осуществляется часового пояса.
ms.openlocfilehash: 887bd750b9cad1e28e6f7603c7b3289da8f8dc07
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834483"
---
# <a name="month-time-zone-transition"></a><span data-ttu-id="5b86a-103">Месяц (часовой пояс переходов)</span><span class="sxs-lookup"><span data-stu-id="5b86a-103">Month (Time Zone Transition)</span></span>

<span data-ttu-id="5b86a-104">Элемент **Month** представляет месяц, в котором осуществляется часового пояса.</span><span class="sxs-lookup"><span data-stu-id="5b86a-104">The **Month** element represents the month in which the time zone transition occurs.</span></span> 
  
```xml
<Month/>
```

 <span data-ttu-id="5b86a-105">**int**</span><span class="sxs-lookup"><span data-stu-id="5b86a-105">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5b86a-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="5b86a-106">Attributes and elements</span></span>

<span data-ttu-id="5b86a-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="5b86a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5b86a-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="5b86a-108">Attributes</span></span>

<span data-ttu-id="5b86a-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="5b86a-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5b86a-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="5b86a-110">Child elements</span></span>

<span data-ttu-id="5b86a-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="5b86a-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="5b86a-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="5b86a-112">Parent elements</span></span>

|<span data-ttu-id="5b86a-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="5b86a-113">**Element**</span></span>|<span data-ttu-id="5b86a-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="5b86a-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5b86a-115">RecurringDateTransition</span><span class="sxs-lookup"><span data-stu-id="5b86a-115">RecurringDateTransition</span></span>](recurringdatetransition.md) <br/> |<span data-ttu-id="5b86a-116">Представляет переход часового пояса, что происходит в конкретный день каждый год.</span><span class="sxs-lookup"><span data-stu-id="5b86a-116">Represents a time zone transition that occurs on a specific date each year.</span></span>  <br/> |
|[<span data-ttu-id="5b86a-117">RecurringDayTransition</span><span class="sxs-lookup"><span data-stu-id="5b86a-117">RecurringDayTransition</span></span>](recurringdaytransition.md) <br/> |<span data-ttu-id="5b86a-118">Представляет переход часового пояса, что происходит в тот же день каждый год.</span><span class="sxs-lookup"><span data-stu-id="5b86a-118">Represents a time zone transition that occurs on the same day each year.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="5b86a-119">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="5b86a-119">Text value</span></span>

<span data-ttu-id="5b86a-120">Текстовое значение представляет собой целое число, представляющее месяц, в котором осуществляется часового пояса.</span><span class="sxs-lookup"><span data-stu-id="5b86a-120">The text value is an integer that represents the month in which the time zone transition occurs.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="5b86a-121">Замечания</span><span class="sxs-lookup"><span data-stu-id="5b86a-121">Remarks</span></span>

<span data-ttu-id="5b86a-122">Схема, описывающая этот элемент находится в виртуальном каталоге EWS компьютера, на котором выполняется Microsoft Exchange Server с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="5b86a-122">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5b86a-123">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="5b86a-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5b86a-124">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="5b86a-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="5b86a-125">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="5b86a-125">Schema Name</span></span>  <br/> |<span data-ttu-id="5b86a-126">Схема Types</span><span class="sxs-lookup"><span data-stu-id="5b86a-126">Types schema</span></span>  <br/> |
|<span data-ttu-id="5b86a-127">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="5b86a-127">Validation File</span></span>  <br/> |<span data-ttu-id="5b86a-128">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="5b86a-128">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="5b86a-129">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="5b86a-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="5b86a-130">False</span><span class="sxs-lookup"><span data-stu-id="5b86a-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="5b86a-131">См. также</span><span class="sxs-lookup"><span data-stu-id="5b86a-131">See also</span></span>



- [<span data-ttu-id="5b86a-132">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="5b86a-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

