---
title: YearlyRegeneration
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- YearlyRegeneration
api_type:
- schema
ms.assetid: 23538bca-738e-4319-944e-f459ff8a7eba
description: Элемент YearlyRegeneration описывает частота в годы, в которых генерируется задачи.
ms.openlocfilehash: d034be1ff70e92fd5e96118b9fd1eb3033737f6c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19840537"
---
# <a name="yearlyregeneration"></a><span data-ttu-id="64bd3-103">YearlyRegeneration</span><span class="sxs-lookup"><span data-stu-id="64bd3-103">YearlyRegeneration</span></span>

<span data-ttu-id="64bd3-104">Элемент **YearlyRegeneration** описывает частота в годы, в которых генерируется задачи.</span><span class="sxs-lookup"><span data-stu-id="64bd3-104">The **YearlyRegeneration** element describes the frequency, in years, in which a task is regenerated.</span></span> 
  
```xml
<YearlyRegeneratingPatternType>
   <Interval/>
</YearlyRegeneratingPatternType>
```

<span data-ttu-id="64bd3-105">**YearlyRegeneratingPatternType**</span><span class="sxs-lookup"><span data-stu-id="64bd3-105">**YearlyRegeneratingPatternType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="64bd3-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="64bd3-106">Attributes and elements</span></span>

<span data-ttu-id="64bd3-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="64bd3-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="64bd3-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="64bd3-108">Attributes</span></span>

<span data-ttu-id="64bd3-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="64bd3-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="64bd3-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="64bd3-110">Child elements</span></span>

|<span data-ttu-id="64bd3-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="64bd3-111">**Element**</span></span>|<span data-ttu-id="64bd3-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="64bd3-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="64bd3-113">Интервал</span><span class="sxs-lookup"><span data-stu-id="64bd3-113">Interval</span></span>](interval.md) <br/> |<span data-ttu-id="64bd3-114">Задает интервал в лет, во время которых ключа новой задачи после завершения задачи.</span><span class="sxs-lookup"><span data-stu-id="64bd3-114">Defines the interval, in years, during which a new task is regenerated after the completion of the task.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="64bd3-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="64bd3-115">Parent elements</span></span>

|<span data-ttu-id="64bd3-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="64bd3-116">**Element**</span></span>|<span data-ttu-id="64bd3-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="64bd3-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="64bd3-118">Повторение (TaskRecurrenceType)</span><span class="sxs-lookup"><span data-stu-id="64bd3-118">Recurrence (TaskRecurrenceType)</span></span>](recurrence-taskrecurrencetype.md) <br/> |<span data-ttu-id="64bd3-119">Содержит данные о повторении для повторяющихся задач.</span><span class="sxs-lookup"><span data-stu-id="64bd3-119">Contains recurrence information for recurring tasks.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="64bd3-120">Замечания</span><span class="sxs-lookup"><span data-stu-id="64bd3-120">Remarks</span></span>

<span data-ttu-id="64bd3-121">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="64bd3-121">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="64bd3-122">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="64bd3-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="64bd3-123">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="64bd3-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="64bd3-124">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="64bd3-124">Schema Name</span></span>  <br/> |<span data-ttu-id="64bd3-125">Схема Types</span><span class="sxs-lookup"><span data-stu-id="64bd3-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="64bd3-126">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="64bd3-126">Validation File</span></span>  <br/> |<span data-ttu-id="64bd3-127">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="64bd3-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="64bd3-128">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="64bd3-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="64bd3-129">False</span><span class="sxs-lookup"><span data-stu-id="64bd3-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="64bd3-130">См. также</span><span class="sxs-lookup"><span data-stu-id="64bd3-130">See also</span></span>

- [<span data-ttu-id="64bd3-131">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="64bd3-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

