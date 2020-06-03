---
title: виклиреженератион
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
description: Элемент Виклиреженератион описывает частоту повторного создания задачи в неделях.
ms.openlocfilehash: dc333e051fd2213942e629a3f2764c72abfaeba5
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459751"
---
# <a name="weeklyregeneration"></a><span data-ttu-id="c5360-103">виклиреженератион</span><span class="sxs-lookup"><span data-stu-id="c5360-103">WeeklyRegeneration</span></span>

<span data-ttu-id="c5360-104">Элемент **виклиреженератион** описывает частоту повторного создания задачи в неделях.</span><span class="sxs-lookup"><span data-stu-id="c5360-104">The **WeeklyRegeneration** element describes the frequency, in weeks, in which a task is regenerated.</span></span> 
  
```xml
<WeeklyRegeneration>
   <Interval/>
</WeeklyRegeneration>
```

 <span data-ttu-id="c5360-105">**виклиреженератингпаттернтипе**</span><span class="sxs-lookup"><span data-stu-id="c5360-105">**WeeklyRegeneratingPatternType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c5360-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="c5360-106">Attributes and elements</span></span>

<span data-ttu-id="c5360-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="c5360-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c5360-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="c5360-108">Attributes</span></span>

<span data-ttu-id="c5360-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="c5360-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c5360-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="c5360-110">Child elements</span></span>

|<span data-ttu-id="c5360-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="c5360-111">**Element**</span></span>|<span data-ttu-id="c5360-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="c5360-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c5360-113">Interval</span><span class="sxs-lookup"><span data-stu-id="c5360-113">Interval</span></span>](interval.md) <br/> |<span data-ttu-id="c5360-114">Определяет интервал (в неделях) с момента завершения задачи, после которого новая задача создается повторно.</span><span class="sxs-lookup"><span data-stu-id="c5360-114">Defines the interval, in weeks, since the task was completed, after which a new task is regenerated.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="c5360-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="c5360-115">Parent elements</span></span>

|<span data-ttu-id="c5360-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="c5360-116">**Element**</span></span>|<span data-ttu-id="c5360-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="c5360-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c5360-118">Повторение (Таскрекурренцетипе)</span><span class="sxs-lookup"><span data-stu-id="c5360-118">Recurrence (TaskRecurrenceType)</span></span>](recurrence-taskrecurrencetype.md) <br/> |<span data-ttu-id="c5360-119">Содержит сведения о повторении для повторяющихся задач.</span><span class="sxs-lookup"><span data-stu-id="c5360-119">Contains recurrence information for recurring tasks.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="c5360-120">Примечания</span><span class="sxs-lookup"><span data-stu-id="c5360-120">Remarks</span></span>

<span data-ttu-id="c5360-121">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="c5360-121">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c5360-122">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="c5360-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c5360-123">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="c5360-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="c5360-124">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="c5360-124">Schema Name</span></span>  <br/> |<span data-ttu-id="c5360-125">Схема Types</span><span class="sxs-lookup"><span data-stu-id="c5360-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="c5360-126">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="c5360-126">Validation File</span></span>  <br/> |<span data-ttu-id="c5360-127">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="c5360-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="c5360-128">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="c5360-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="c5360-129">False</span><span class="sxs-lookup"><span data-stu-id="c5360-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c5360-130">См. также</span><span class="sxs-lookup"><span data-stu-id="c5360-130">See also</span></span>



- [<span data-ttu-id="c5360-131">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="c5360-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

