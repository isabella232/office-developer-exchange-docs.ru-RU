---
title: WeeklyRegeneration
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- WeeklyRegeneration
api_type:
- schema
ms.assetid: f128fdaa-ca3d-4614-8e55-f25e76a67b6c
description: Элемент WeeklyRegeneration описывает частоту, недель, в которых генерируется задачи.
ms.openlocfilehash: 36cd3cc5c180f2b2cf53708e7787d0595f518def
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19840511"
---
# <a name="weeklyregeneration"></a><span data-ttu-id="8090a-103">WeeklyRegeneration</span><span class="sxs-lookup"><span data-stu-id="8090a-103">WeeklyRegeneration</span></span>

<span data-ttu-id="8090a-104">Элемент **WeeklyRegeneration** описывает частоту, недель, в которых генерируется задачи.</span><span class="sxs-lookup"><span data-stu-id="8090a-104">The **WeeklyRegeneration** element describes the frequency, in weeks, in which a task is regenerated.</span></span> 
  
```xml
<WeeklyRegeneration>
   <Interval/>
</WeeklyRegeneration>
```

 <span data-ttu-id="8090a-105">**WeeklyRegeneratingPatternType**</span><span class="sxs-lookup"><span data-stu-id="8090a-105">**WeeklyRegeneratingPatternType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="8090a-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="8090a-106">Attributes and elements</span></span>

<span data-ttu-id="8090a-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="8090a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8090a-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="8090a-108">Attributes</span></span>

<span data-ttu-id="8090a-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="8090a-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8090a-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="8090a-110">Child elements</span></span>

|<span data-ttu-id="8090a-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="8090a-111">**Element**</span></span>|<span data-ttu-id="8090a-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="8090a-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8090a-113">Интервал</span><span class="sxs-lookup"><span data-stu-id="8090a-113">Interval</span></span>](interval.md) <br/> |<span data-ttu-id="8090a-114">Задает интервал в недель, с момента завершения задачи, после которого генерируется новую задачу.</span><span class="sxs-lookup"><span data-stu-id="8090a-114">Defines the interval, in weeks, since the task was completed, after which a new task is regenerated.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="8090a-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="8090a-115">Parent elements</span></span>

|<span data-ttu-id="8090a-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="8090a-116">**Element**</span></span>|<span data-ttu-id="8090a-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="8090a-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8090a-118">Повторение (TaskRecurrenceType)</span><span class="sxs-lookup"><span data-stu-id="8090a-118">Recurrence (TaskRecurrenceType)</span></span>](recurrence-taskrecurrencetype.md) <br/> |<span data-ttu-id="8090a-119">Содержит данные о повторении для повторяющихся задач.</span><span class="sxs-lookup"><span data-stu-id="8090a-119">Contains recurrence information for recurring tasks.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="8090a-120">Замечания</span><span class="sxs-lookup"><span data-stu-id="8090a-120">Remarks</span></span>

<span data-ttu-id="8090a-121">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="8090a-121">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="8090a-122">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="8090a-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8090a-123">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="8090a-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="8090a-124">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="8090a-124">Schema Name</span></span>  <br/> |<span data-ttu-id="8090a-125">Схема Types</span><span class="sxs-lookup"><span data-stu-id="8090a-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="8090a-126">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="8090a-126">Validation File</span></span>  <br/> |<span data-ttu-id="8090a-127">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="8090a-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="8090a-128">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="8090a-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="8090a-129">False</span><span class="sxs-lookup"><span data-stu-id="8090a-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="8090a-130">См. также</span><span class="sxs-lookup"><span data-stu-id="8090a-130">See also</span></span>



- [<span data-ttu-id="8090a-131">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="8090a-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

