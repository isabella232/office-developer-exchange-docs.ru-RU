---
title: тимеоффсет
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- TimeOffset
api_type:
- schema
ms.assetid: b70bf498-cc3a-4fa6-8236-514acb973b33
description: Элемент Тимеоффсет представляет смещение по времени от времени в формате UTC для смены часового пояса.
ms.openlocfilehash: 8cfd43477f0548227204da9ebc6d7e9307786845
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460290"
---
# <a name="timeoffset"></a><span data-ttu-id="41d7e-103">тимеоффсет</span><span class="sxs-lookup"><span data-stu-id="41d7e-103">TimeOffset</span></span>

<span data-ttu-id="41d7e-104">Элемент **тимеоффсет** представляет смещение по времени от времени в формате UTC для смены часового пояса.</span><span class="sxs-lookup"><span data-stu-id="41d7e-104">The **TimeOffset** element represents the time offset from Coordinated Universal Time (UTC) for the time zone transition.</span></span> 
  
```XML
<TimeOffset/>
```

 <span data-ttu-id="41d7e-105">**duration**</span><span class="sxs-lookup"><span data-stu-id="41d7e-105">**duration**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="41d7e-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="41d7e-106">Attributes and elements</span></span>

<span data-ttu-id="41d7e-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="41d7e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="41d7e-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="41d7e-108">Attributes</span></span>

<span data-ttu-id="41d7e-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="41d7e-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="41d7e-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="41d7e-110">Child elements</span></span>

<span data-ttu-id="41d7e-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="41d7e-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="41d7e-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="41d7e-112">Parent elements</span></span>

|<span data-ttu-id="41d7e-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="41d7e-113">**Element**</span></span>|<span data-ttu-id="41d7e-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="41d7e-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="41d7e-115">рекуррингдатетранситион</span><span class="sxs-lookup"><span data-stu-id="41d7e-115">RecurringDateTransition</span></span>](recurringdatetransition.md) <br/> |<span data-ttu-id="41d7e-116">Представляет переход часового пояса, который выполняется в определенный день каждого года.</span><span class="sxs-lookup"><span data-stu-id="41d7e-116">Represents a time zone transition that occurs on a specific date each year.</span></span>  <br/> |
|[<span data-ttu-id="41d7e-117">рекуррингдайтранситион</span><span class="sxs-lookup"><span data-stu-id="41d7e-117">RecurringDayTransition</span></span>](recurringdaytransition.md) <br/> |<span data-ttu-id="41d7e-118">Представляет переход часового пояса, который выполняется в один день каждого года.</span><span class="sxs-lookup"><span data-stu-id="41d7e-118">Represents a time zone transition that occurs on the same day each year.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="41d7e-119">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="41d7e-119">Text value</span></span>

<span data-ttu-id="41d7e-120">Текстовое значение элемента **тимеоффсет** — это длительность, определяющая смещение времени от времени в формате UTC для смены часового пояса.</span><span class="sxs-lookup"><span data-stu-id="41d7e-120">The text value of the **TimeOffset** element is a duration that specifies the time offset from UTC for the time zone transition.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="41d7e-121">Примечания</span><span class="sxs-lookup"><span data-stu-id="41d7e-121">Remarks</span></span>

<span data-ttu-id="41d7e-122">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="41d7e-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="41d7e-123">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="41d7e-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="41d7e-124">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="41d7e-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="41d7e-125">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="41d7e-125">Schema Name</span></span>  <br/> |<span data-ttu-id="41d7e-126">Схема Types</span><span class="sxs-lookup"><span data-stu-id="41d7e-126">Types schema</span></span>  <br/> |
|<span data-ttu-id="41d7e-127">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="41d7e-127">Validation File</span></span>  <br/> |<span data-ttu-id="41d7e-128">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="41d7e-128">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="41d7e-129">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="41d7e-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="41d7e-130">False</span><span class="sxs-lookup"><span data-stu-id="41d7e-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="41d7e-131">См. также</span><span class="sxs-lookup"><span data-stu-id="41d7e-131">See also</span></span>



- [<span data-ttu-id="41d7e-132">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="41d7e-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

