---
title: DailyRegeneration
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DailyRegeneration
api_type:
- schema
ms.assetid: cafb57e4-c518-45e0-b565-2babd0dab1df
description: Элемент DailyRegeneration описывает период в днях, в которых генерируется задачи.
ms.openlocfilehash: 356f7fd2672b2ad87d17e597c52e9f12273ce3c6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761962"
---
# <a name="dailyregeneration"></a><span data-ttu-id="46088-103">DailyRegeneration</span><span class="sxs-lookup"><span data-stu-id="46088-103">DailyRegeneration</span></span>

<span data-ttu-id="46088-104">Элемент **DailyRegeneration** описывает период в днях, в которых генерируется задачи.</span><span class="sxs-lookup"><span data-stu-id="46088-104">The **DailyRegeneration** element describes the frequency, in days, in which a task is regenerated.</span></span> 
  
```xml
<DailyRegeneration>
   <Interval/>
</DailyRegeneration>
```

<span data-ttu-id="46088-105">**DailyRegeneratingPatternType**</span><span class="sxs-lookup"><span data-stu-id="46088-105">**DailyRegeneratingPatternType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="46088-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="46088-106">Attributes and elements</span></span>

<span data-ttu-id="46088-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="46088-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="46088-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="46088-108">Attributes</span></span>

<span data-ttu-id="46088-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="46088-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="46088-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="46088-110">Child elements</span></span>

|<span data-ttu-id="46088-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="46088-111">**Element**</span></span>|<span data-ttu-id="46088-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="46088-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="46088-113">Интервал</span><span class="sxs-lookup"><span data-stu-id="46088-113">Interval</span></span>](interval.md) <br/> |<span data-ttu-id="46088-114">Задает интервал в днях между двумя последовательными повторяющихся элементов.</span><span class="sxs-lookup"><span data-stu-id="46088-114">Defines the interval, in days, between two consecutive recurring items.</span></span> <span data-ttu-id="46088-115">Значение должно быть в диапазоне от 1 до 999.</span><span class="sxs-lookup"><span data-stu-id="46088-115">The value must be in the range of 1 to 999.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="46088-116">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="46088-116">Parent elements</span></span>

|<span data-ttu-id="46088-117">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="46088-117">**Element**</span></span>|<span data-ttu-id="46088-118">**Описание**</span><span class="sxs-lookup"><span data-stu-id="46088-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="46088-119">Повторение (TaskRecurrenceType)</span><span class="sxs-lookup"><span data-stu-id="46088-119">Recurrence (TaskRecurrenceType)</span></span>](recurrence-taskrecurrencetype.md) <br/> |<span data-ttu-id="46088-120">Содержит данные о повторении для повторяющихся задач.</span><span class="sxs-lookup"><span data-stu-id="46088-120">Contains recurrence information for recurring tasks.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="46088-121">Замечания</span><span class="sxs-lookup"><span data-stu-id="46088-121">Remarks</span></span>

<span data-ttu-id="46088-122">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="46088-122">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="46088-123">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="46088-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="46088-124">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="46088-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="46088-125">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="46088-125">Schema name</span></span>  <br/> |<span data-ttu-id="46088-126">Схема Types</span><span class="sxs-lookup"><span data-stu-id="46088-126">Types schema</span></span>  <br/> |
|<span data-ttu-id="46088-127">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="46088-127">Validation file</span></span>  <br/> |<span data-ttu-id="46088-128">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="46088-128">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="46088-129">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="46088-129">Can be empty</span></span>  <br/> |<span data-ttu-id="46088-130">False</span><span class="sxs-lookup"><span data-stu-id="46088-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="46088-131">См. также</span><span class="sxs-lookup"><span data-stu-id="46088-131">See also</span></span>

- [<span data-ttu-id="46088-132">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="46088-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

