---
title: Год
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Year
api_type:
- schema
ms.assetid: 93bf2847-53fa-496c-9a1e-dc9a9ffd0b9f
description: Элемент года используется для определения часового пояса, который изменяется в зависимости от года. Этот элемент является необязательным. Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).
ms.openlocfilehash: 95d75f9c6166fc26e86534346fb07292a7fb3dcd
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19840541"
---
# <a name="year"></a><span data-ttu-id="813d1-105">Год</span><span class="sxs-lookup"><span data-stu-id="813d1-105">Year</span></span>

<span data-ttu-id="813d1-106">Элемент **года** используется для определения часового пояса, который изменяется в зависимости от года.</span><span class="sxs-lookup"><span data-stu-id="813d1-106">The **Year** element is used to define a time zone that changes depending on the year.</span></span> <span data-ttu-id="813d1-107">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="813d1-107">This element is optional.</span></span> <span data-ttu-id="813d1-108">Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="813d1-108">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<Year/>
```

<span data-ttu-id="813d1-109">**string**</span><span class="sxs-lookup"><span data-stu-id="813d1-109">**string**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="813d1-110">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="813d1-110">Attributes and elements</span></span>

<span data-ttu-id="813d1-111">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="813d1-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="813d1-112">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="813d1-112">Attributes</span></span>

<span data-ttu-id="813d1-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="813d1-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="813d1-114">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="813d1-114">Child elements</span></span>

<span data-ttu-id="813d1-115">Нет.</span><span class="sxs-lookup"><span data-stu-id="813d1-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="813d1-116">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="813d1-116">Parent elements</span></span>

|<span data-ttu-id="813d1-117">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="813d1-117">**Element**</span></span>|<span data-ttu-id="813d1-118">**Описание**</span><span class="sxs-lookup"><span data-stu-id="813d1-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="813d1-119">StandardTime</span><span class="sxs-lookup"><span data-stu-id="813d1-119">StandardTime</span></span>](standardtime.md) <br/> |<span data-ttu-id="813d1-120">Представляет смещение от времени относительно времени в формате UTC, представленный в элемент [Bias (UTC)](bias-utc.md) .</span><span class="sxs-lookup"><span data-stu-id="813d1-120">Represents an offset from the time relative to Coordinated Universal Time (UTC) that is represented by the [Bias (UTC)](bias-utc.md) element.</span></span>  <br/> |
|[<span data-ttu-id="813d1-121">DaylightTime</span><span class="sxs-lookup"><span data-stu-id="813d1-121">DaylightTime</span></span>](daylighttime.md) <br/> |<span data-ttu-id="813d1-122">Представляет смещение от времени относительно времени в формате UTC, представленный элемент [Bias (UTC)](bias-utc.md) в области, где наблюдается летнего времени.</span><span class="sxs-lookup"><span data-stu-id="813d1-122">Represents an offset from the time relative to Coordinated Universal Time (UTC) that is represented by the [Bias (UTC)](bias-utc.md) element in regions where daylight saving time is observed.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="813d1-123">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="813d1-123">Text value</span></span>

<span data-ttu-id="813d1-124">Элемент года принимает строку, представляющую года.</span><span class="sxs-lookup"><span data-stu-id="813d1-124">The Year element accepts a string that represents a year.</span></span> <span data-ttu-id="813d1-125">ГГГГ имеет формат года.</span><span class="sxs-lookup"><span data-stu-id="813d1-125">The year format is YYYY.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="813d1-126">Замечания</span><span class="sxs-lookup"><span data-stu-id="813d1-126">Remarks</span></span>

<span data-ttu-id="813d1-127">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="813d1-127">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="813d1-128">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="813d1-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="813d1-129">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="813d1-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="813d1-130">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="813d1-130">Schema Name</span></span>  <br/> |<span data-ttu-id="813d1-131">Схема Types</span><span class="sxs-lookup"><span data-stu-id="813d1-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="813d1-132">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="813d1-132">Validation File</span></span>  <br/> |<span data-ttu-id="813d1-133">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="813d1-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="813d1-134">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="813d1-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="813d1-135">False</span><span class="sxs-lookup"><span data-stu-id="813d1-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="813d1-136">См. также</span><span class="sxs-lookup"><span data-stu-id="813d1-136">See also</span></span>

- [<span data-ttu-id="813d1-137">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="813d1-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

