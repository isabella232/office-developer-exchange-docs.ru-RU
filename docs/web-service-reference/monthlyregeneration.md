---
title: MonthlyRegeneration
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MonthlyRegeneration
api_type:
- schema
ms.assetid: 9a52ca97-a663-41fe-b61a-61d8c53833ca
description: Элемент MonthlyRegeneration описывает частота месяца, из которых генерируется задач.
ms.openlocfilehash: 3de8ab5a6a2134ad5c596bf2bcb073d881c89746
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834488"
---
# <a name="monthlyregeneration"></a><span data-ttu-id="f61de-103">MonthlyRegeneration</span><span class="sxs-lookup"><span data-stu-id="f61de-103">MonthlyRegeneration</span></span>

<span data-ttu-id="f61de-104">Элемент **MonthlyRegeneration** описывает частота месяца, из которых генерируется задач.</span><span class="sxs-lookup"><span data-stu-id="f61de-104">The **MonthlyRegeneration** element describes the frequency, in months, of which task is regenerated.</span></span> 
  
```xml
<MonthlyRegeneration>
   <Interval/>
</MonthlyRegeneration>
```

 <span data-ttu-id="f61de-105">**MonthlyRegeneratingPatternType**</span><span class="sxs-lookup"><span data-stu-id="f61de-105">**MonthlyRegeneratingPatternType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f61de-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="f61de-106">Attributes and elements</span></span>

<span data-ttu-id="f61de-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="f61de-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f61de-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="f61de-108">Attributes</span></span>

<span data-ttu-id="f61de-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="f61de-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f61de-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="f61de-110">Child elements</span></span>

|<span data-ttu-id="f61de-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="f61de-111">**Element**</span></span>|<span data-ttu-id="f61de-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="f61de-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f61de-113">Интервал</span><span class="sxs-lookup"><span data-stu-id="f61de-113">Interval</span></span>](interval.md) <br/> |<span data-ttu-id="f61de-114">Задает интервал в месяцев между двумя последовательными повторяющихся элементов.</span><span class="sxs-lookup"><span data-stu-id="f61de-114">Defines the interval, in months, between two consecutive recurring items.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f61de-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="f61de-115">Parent elements</span></span>

|<span data-ttu-id="f61de-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="f61de-116">**Element**</span></span>|<span data-ttu-id="f61de-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="f61de-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f61de-118">Повторение (TaskRecurrenceType)</span><span class="sxs-lookup"><span data-stu-id="f61de-118">Recurrence (TaskRecurrenceType)</span></span>](recurrence-taskrecurrencetype.md) <br/> |<span data-ttu-id="f61de-119">Содержит данные о повторении для повторяющихся задач.</span><span class="sxs-lookup"><span data-stu-id="f61de-119">Contains recurrence information for recurring tasks.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="f61de-120">Замечания</span><span class="sxs-lookup"><span data-stu-id="f61de-120">Remarks</span></span>

<span data-ttu-id="f61de-121">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="f61de-121">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f61de-122">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="f61de-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f61de-123">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="f61de-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="f61de-124">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="f61de-124">Schema name</span></span>  <br/> |<span data-ttu-id="f61de-125">Схема Types</span><span class="sxs-lookup"><span data-stu-id="f61de-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="f61de-126">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="f61de-126">Validation file</span></span>  <br/> |<span data-ttu-id="f61de-127">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="f61de-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="f61de-128">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="f61de-128">Can be empty</span></span>  <br/> |<span data-ttu-id="f61de-129">False</span><span class="sxs-lookup"><span data-stu-id="f61de-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f61de-130">См. также</span><span class="sxs-lookup"><span data-stu-id="f61de-130">See also</span></span>



- [<span data-ttu-id="f61de-131">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="f61de-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

