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
ms.openlocfilehash: 46b1b2c8eec9bae871b4dafe43036e9d725075ae
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19840165"
---
# <a name="timeoffset"></a><span data-ttu-id="da040-103">тимеоффсет</span><span class="sxs-lookup"><span data-stu-id="da040-103">TimeOffset</span></span>

<span data-ttu-id="da040-104">Элемент **тимеоффсет** представляет смещение по времени от времени в формате UTC для смены часового пояса.</span><span class="sxs-lookup"><span data-stu-id="da040-104">The **TimeOffset** element represents the time offset from Coordinated Universal Time (UTC) for the time zone transition.</span></span> 
  
```XML
<TimeOffset/>
```

 <span data-ttu-id="da040-105">**duration**</span><span class="sxs-lookup"><span data-stu-id="da040-105">**duration**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="da040-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="da040-106">Attributes and elements</span></span>

<span data-ttu-id="da040-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="da040-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="da040-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="da040-108">Attributes</span></span>

<span data-ttu-id="da040-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="da040-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="da040-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="da040-110">Child elements</span></span>

<span data-ttu-id="da040-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="da040-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="da040-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="da040-112">Parent elements</span></span>

|<span data-ttu-id="da040-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="da040-113">**Element**</span></span>|<span data-ttu-id="da040-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="da040-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="da040-115">рекуррингдатетранситион</span><span class="sxs-lookup"><span data-stu-id="da040-115">RecurringDateTransition</span></span>](recurringdatetransition.md) <br/> |<span data-ttu-id="da040-116">Представляет переход часового пояса, который выполняется в определенный день каждого года.</span><span class="sxs-lookup"><span data-stu-id="da040-116">Represents a time zone transition that occurs on a specific date each year.</span></span>  <br/> |
|[<span data-ttu-id="da040-117">рекуррингдайтранситион</span><span class="sxs-lookup"><span data-stu-id="da040-117">RecurringDayTransition</span></span>](recurringdaytransition.md) <br/> |<span data-ttu-id="da040-118">Представляет переход часового пояса, который выполняется в один день каждого года.</span><span class="sxs-lookup"><span data-stu-id="da040-118">Represents a time zone transition that occurs on the same day each year.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="da040-119">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="da040-119">Text value</span></span>

<span data-ttu-id="da040-120">Текстовое значение элемента **тимеоффсет** — это длительность, определяющая смещение времени от времени в формате UTC для смены часового пояса.</span><span class="sxs-lookup"><span data-stu-id="da040-120">The text value of the **TimeOffset** element is a duration that specifies the time offset from UTC for the time zone transition.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="da040-121">Примечания</span><span class="sxs-lookup"><span data-stu-id="da040-121">Remarks</span></span>

<span data-ttu-id="da040-122">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="da040-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="da040-123">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="da040-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="da040-124">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="da040-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="da040-125">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="da040-125">Schema Name</span></span>  <br/> |<span data-ttu-id="da040-126">Схема Types</span><span class="sxs-lookup"><span data-stu-id="da040-126">Types schema</span></span>  <br/> |
|<span data-ttu-id="da040-127">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="da040-127">Validation File</span></span>  <br/> |<span data-ttu-id="da040-128">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="da040-128">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="da040-129">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="da040-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="da040-130">False</span><span class="sxs-lookup"><span data-stu-id="da040-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="da040-131">См. также</span><span class="sxs-lookup"><span data-stu-id="da040-131">See also</span></span>



- [<span data-ttu-id="da040-132">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="da040-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

