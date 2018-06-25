---
title: DateTimePrecision
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 822dc5a6-2d57-474b-8a7d-da150898e5b6
description: Элемент DateTimePrecision указывает точность для значений, возвращаемых даты и времени.
ms.openlocfilehash: 4d11598628228b41adf021adbbaa77e6348534bb
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761976"
---
# <a name="datetimeprecision"></a><span data-ttu-id="15e7b-103">DateTimePrecision</span><span class="sxs-lookup"><span data-stu-id="15e7b-103">DateTimePrecision</span></span>

<span data-ttu-id="15e7b-104">Элемент **DateTimePrecision** указывает точность для значений, возвращаемых даты и времени.</span><span class="sxs-lookup"><span data-stu-id="15e7b-104">The **DateTimePrecision** element specifies the precision for returned date/time values.</span></span> 
  
```XML
<DateTimePrecision />
```

<span data-ttu-id="15e7b-105">**DateTimePrecisionType**</span><span class="sxs-lookup"><span data-stu-id="15e7b-105">**DateTimePrecisionType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="15e7b-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="15e7b-106">Attributes and elements</span></span>

<span data-ttu-id="15e7b-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="15e7b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="15e7b-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="15e7b-108">Attributes</span></span>

<span data-ttu-id="15e7b-109">Нет</span><span class="sxs-lookup"><span data-stu-id="15e7b-109">None</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="15e7b-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="15e7b-110">Child elements</span></span>

<span data-ttu-id="15e7b-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="15e7b-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="15e7b-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="15e7b-112">Parent elements</span></span>

<span data-ttu-id="15e7b-113">Элемент **DateTimePrecision** находится в заголовке SOAP.</span><span class="sxs-lookup"><span data-stu-id="15e7b-113">The **DateTimePrecision** element is located in the SOAP header.</span></span> 
  
## <a name="text-value"></a><span data-ttu-id="15e7b-114">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="15e7b-114">Text value</span></span>

<span data-ttu-id="15e7b-115">Текстовое значение является обязательным.</span><span class="sxs-lookup"><span data-stu-id="15e7b-115">A text value is required.</span></span> <span data-ttu-id="15e7b-116">Ниже перечислены возможные значения.</span><span class="sxs-lookup"><span data-stu-id="15e7b-116">The following are the possible values:</span></span>
  
- <span data-ttu-id="15e7b-117">Секунд</span><span class="sxs-lookup"><span data-stu-id="15e7b-117">Seconds</span></span>
    
- <span data-ttu-id="15e7b-118">Мс</span><span class="sxs-lookup"><span data-stu-id="15e7b-118">Milliseconds</span></span>
    
## <a name="remarks"></a><span data-ttu-id="15e7b-119">Замечания</span><span class="sxs-lookup"><span data-stu-id="15e7b-119">Remarks</span></span>

<span data-ttu-id="15e7b-120">Дата и время, когда используется заголовок SOAP с элементом **DateTimePrecision** , задайте значение «Секунд», возвращаемые значения ближайшего секунд (00: 00:00).</span><span class="sxs-lookup"><span data-stu-id="15e7b-120">When a SOAP header with the **DateTimePrecision** element set to "Seconds" is used, date/time values are returned to the nearest seconds (00:00:00).</span></span> <span data-ttu-id="15e7b-121">При использовании «Миллисекундах» Дата/время значения возвращаются до ближайшей миллисекунды (00:00:00.0000).</span><span class="sxs-lookup"><span data-stu-id="15e7b-121">When "Milliseconds" is used, date/time values are returned to the nearest millisecond (00:00:00.0000).</span></span> 
  
<span data-ttu-id="15e7b-122">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="15e7b-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
<span data-ttu-id="15e7b-123">Этот элемент появился в Exchange Server 2010 с пакетом обновления 2 (SP2).</span><span class="sxs-lookup"><span data-stu-id="15e7b-123">This element was introduced in Exchange Server 2010 Service Pack 2 (SP2).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="15e7b-124">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="15e7b-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="15e7b-125">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="15e7b-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="15e7b-126">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="15e7b-126">Schema Name</span></span>  <br/> |<span data-ttu-id="15e7b-127">Схема Types</span><span class="sxs-lookup"><span data-stu-id="15e7b-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="15e7b-128">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="15e7b-128">Validation File</span></span>  <br/> |<span data-ttu-id="15e7b-129">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="15e7b-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="15e7b-130">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="15e7b-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="15e7b-131">False</span><span class="sxs-lookup"><span data-stu-id="15e7b-131">False</span></span>  <br/> |
   

