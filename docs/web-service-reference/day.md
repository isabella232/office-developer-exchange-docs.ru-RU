---
title: Day
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Day
api_type:
- schema
ms.assetid: d3b2dc66-486a-41d1-bff3-606f0bf92715
description: Элемент Day представляет день месяца, в который происходит переход часового пояса.
ms.openlocfilehash: 8ee5ed2e996a6a4b84648df41faf2718784b9d30
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457482"
---
# <a name="day"></a><span data-ttu-id="29866-103">Day</span><span class="sxs-lookup"><span data-stu-id="29866-103">Day</span></span>

<span data-ttu-id="29866-104">Элемент **Day** представляет день месяца, в который происходит переход часового пояса.</span><span class="sxs-lookup"><span data-stu-id="29866-104">The **Day** element represents the day of the month on which the time zone transition occurs.</span></span> 
  
```xml
<Day/>
```

<span data-ttu-id="29866-105">**int**</span><span class="sxs-lookup"><span data-stu-id="29866-105">**int**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="29866-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="29866-106">Attributes and elements</span></span>

<span data-ttu-id="29866-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="29866-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="29866-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="29866-108">Attributes</span></span>

<span data-ttu-id="29866-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="29866-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="29866-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="29866-110">Child elements</span></span>

<span data-ttu-id="29866-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="29866-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="29866-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="29866-112">Parent elements</span></span>

|<span data-ttu-id="29866-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="29866-113">**Element**</span></span>|<span data-ttu-id="29866-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="29866-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="29866-115">рекуррингдатетранситион</span><span class="sxs-lookup"><span data-stu-id="29866-115">RecurringDateTransition</span></span>](recurringdatetransition.md) <br/> |<span data-ttu-id="29866-116">Представляет переход часового пояса, который выполняется в определенный день каждого года.</span><span class="sxs-lookup"><span data-stu-id="29866-116">Represents a time zone transition that occurs on a specific date each year.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="29866-117">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="29866-117">Text value</span></span>

<span data-ttu-id="29866-118">Текстовое значение элемента **Day** — это целое число, представляющее день месяца, в который происходит переход часового пояса.</span><span class="sxs-lookup"><span data-stu-id="29866-118">The text value of the **Day** element is an integer that represents the day of the month on which the time zone transition occurs.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="29866-119">Примечания</span><span class="sxs-lookup"><span data-stu-id="29866-119">Remarks</span></span>

<span data-ttu-id="29866-120">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="29866-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="29866-121">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="29866-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="29866-122">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="29866-122">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="29866-123">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="29866-123">Schema Name</span></span>  <br/> |<span data-ttu-id="29866-124">Схема Types</span><span class="sxs-lookup"><span data-stu-id="29866-124">Types schema</span></span>  <br/> |
|<span data-ttu-id="29866-125">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="29866-125">Validation File</span></span>  <br/> |<span data-ttu-id="29866-126">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="29866-126">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="29866-127">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="29866-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="29866-128">False</span><span class="sxs-lookup"><span data-stu-id="29866-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="29866-129">См. также</span><span class="sxs-lookup"><span data-stu-id="29866-129">See also</span></span>

- [<span data-ttu-id="29866-130">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="29866-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

