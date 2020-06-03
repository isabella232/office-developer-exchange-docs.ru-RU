---
title: даилиреженератион
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
description: Элемент Даилиреженератион описывает частоту повторного создания задачи (в днях).
ms.openlocfilehash: 518e4666031131f4a5fc80cc72c28a2110b468c5
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462166"
---
# <a name="dailyregeneration"></a><span data-ttu-id="16e02-103">даилиреженератион</span><span class="sxs-lookup"><span data-stu-id="16e02-103">DailyRegeneration</span></span>

<span data-ttu-id="16e02-104">Элемент **даилиреженератион** описывает частоту повторного создания задачи (в днях).</span><span class="sxs-lookup"><span data-stu-id="16e02-104">The **DailyRegeneration** element describes the frequency, in days, in which a task is regenerated.</span></span> 
  
```xml
<DailyRegeneration>
   <Interval/>
</DailyRegeneration>
```

<span data-ttu-id="16e02-105">**даилиреженератингпаттернтипе**</span><span class="sxs-lookup"><span data-stu-id="16e02-105">**DailyRegeneratingPatternType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="16e02-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="16e02-106">Attributes and elements</span></span>

<span data-ttu-id="16e02-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="16e02-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="16e02-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="16e02-108">Attributes</span></span>

<span data-ttu-id="16e02-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="16e02-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="16e02-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="16e02-110">Child elements</span></span>

|<span data-ttu-id="16e02-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="16e02-111">**Element**</span></span>|<span data-ttu-id="16e02-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="16e02-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="16e02-113">Interval</span><span class="sxs-lookup"><span data-stu-id="16e02-113">Interval</span></span>](interval.md) <br/> |<span data-ttu-id="16e02-114">Определяет интервал (в днях) между двумя последовательными повторяющимися элементами.</span><span class="sxs-lookup"><span data-stu-id="16e02-114">Defines the interval, in days, between two consecutive recurring items.</span></span> <span data-ttu-id="16e02-115">Значение должно находиться в диапазоне от 1 до 999.</span><span class="sxs-lookup"><span data-stu-id="16e02-115">The value must be in the range of 1 to 999.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="16e02-116">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="16e02-116">Parent elements</span></span>

|<span data-ttu-id="16e02-117">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="16e02-117">**Element**</span></span>|<span data-ttu-id="16e02-118">**Описание**</span><span class="sxs-lookup"><span data-stu-id="16e02-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="16e02-119">Повторение (Таскрекурренцетипе)</span><span class="sxs-lookup"><span data-stu-id="16e02-119">Recurrence (TaskRecurrenceType)</span></span>](recurrence-taskrecurrencetype.md) <br/> |<span data-ttu-id="16e02-120">Содержит сведения о повторении для повторяющихся задач.</span><span class="sxs-lookup"><span data-stu-id="16e02-120">Contains recurrence information for recurring tasks.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="16e02-121">Примечания</span><span class="sxs-lookup"><span data-stu-id="16e02-121">Remarks</span></span>

<span data-ttu-id="16e02-122">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="16e02-122">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="16e02-123">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="16e02-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="16e02-124">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="16e02-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="16e02-125">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="16e02-125">Schema name</span></span>  <br/> |<span data-ttu-id="16e02-126">Схема Types</span><span class="sxs-lookup"><span data-stu-id="16e02-126">Types schema</span></span>  <br/> |
|<span data-ttu-id="16e02-127">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="16e02-127">Validation file</span></span>  <br/> |<span data-ttu-id="16e02-128">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="16e02-128">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="16e02-129">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="16e02-129">Can be empty</span></span>  <br/> |<span data-ttu-id="16e02-130">False</span><span class="sxs-lookup"><span data-stu-id="16e02-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="16e02-131">См. также</span><span class="sxs-lookup"><span data-stu-id="16e02-131">See also</span></span>

- [<span data-ttu-id="16e02-132">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="16e02-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

