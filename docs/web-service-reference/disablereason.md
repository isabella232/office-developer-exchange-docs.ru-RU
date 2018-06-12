---
title: DisableReason
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f41b5be6-9b79-4e83-8cdb-aa779e13cb3f
description: Элемент DisableReason указывает причины для отключения приложения.
ms.openlocfilehash: f900bd1b98b294900f767c778b9c5f87f74042ca
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762127"
---
# <a name="disablereason"></a><span data-ttu-id="d6193-103">DisableReason</span><span class="sxs-lookup"><span data-stu-id="d6193-103">DisableReason</span></span>

<span data-ttu-id="d6193-104">Элемент **DisableReason** указывает причины для отключения приложения.</span><span class="sxs-lookup"><span data-stu-id="d6193-104">The **DisableReason** element specifies the reason for disabling an app.</span></span> 
  
```XML
<DisableReason> NoReason | OutlookClientPerformance | OWAClientPerformance | MobileClientPerformance </DisableReason>
```

 <span data-ttu-id="d6193-105">**DisableReasonType**</span><span class="sxs-lookup"><span data-stu-id="d6193-105">**DisableReasonType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d6193-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="d6193-106">Attributes and elements</span></span>

<span data-ttu-id="d6193-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="d6193-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d6193-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="d6193-108">Attributes</span></span>

<span data-ttu-id="d6193-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="d6193-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d6193-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="d6193-110">Child elements</span></span>

<span data-ttu-id="d6193-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="d6193-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="d6193-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="d6193-112">Parent elements</span></span>

|<span data-ttu-id="d6193-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="d6193-113">**Element**</span></span>|<span data-ttu-id="d6193-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d6193-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d6193-115">DisableApp</span><span class="sxs-lookup"><span data-stu-id="d6193-115">DisableApp</span></span>](disableapp.md) <br/> |<span data-ttu-id="d6193-116">Определяет запрос, чтобы отключить приложение.</span><span class="sxs-lookup"><span data-stu-id="d6193-116">Specifies a request to disable an app.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="d6193-117">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="d6193-117">Text value</span></span>

<span data-ttu-id="d6193-118">**Текстовое значение элемента DisableReason**</span><span class="sxs-lookup"><span data-stu-id="d6193-118">**DisableReason element text value**</span></span>

|<span data-ttu-id="d6193-119">**Значение**</span><span class="sxs-lookup"><span data-stu-id="d6193-119">**Value**</span></span>|<span data-ttu-id="d6193-120">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d6193-120">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="d6193-121">NoReason</span><span class="sxs-lookup"><span data-stu-id="d6193-121">NoReason</span></span>  <br/> |<span data-ttu-id="d6193-122">Причина не указана</span><span class="sxs-lookup"><span data-stu-id="d6193-122">No reason given</span></span>  <br/> |
|<span data-ttu-id="d6193-123">OutlookClientPerformance</span><span class="sxs-lookup"><span data-stu-id="d6193-123">OutlookClientPerformance</span></span>  <br/> |<span data-ttu-id="d6193-124">Для повышения производительности клиента электронной почты.</span><span class="sxs-lookup"><span data-stu-id="d6193-124">To improve email client performance.</span></span>  <br/> |
|<span data-ttu-id="d6193-125">OWAClientPerformance</span><span class="sxs-lookup"><span data-stu-id="d6193-125">OWAClientPerformance</span></span>  <br/> |<span data-ttu-id="d6193-126">Для повышения производительности клиента Web app.</span><span class="sxs-lookup"><span data-stu-id="d6193-126">To improve Web app client performance.</span></span>  <br/> |
|<span data-ttu-id="d6193-127">MobileClientPerformance</span><span class="sxs-lookup"><span data-stu-id="d6193-127">MobileClientPerformance</span></span>  <br/> |<span data-ttu-id="d6193-128">Для повышения производительности мобильного клиента.</span><span class="sxs-lookup"><span data-stu-id="d6193-128">To improve mobile client performance.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="d6193-129">Замечания</span><span class="sxs-lookup"><span data-stu-id="d6193-129">Remarks</span></span>

<span data-ttu-id="d6193-130">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="d6193-130">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="d6193-131">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="d6193-131">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d6193-132">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="d6193-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d6193-133">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="d6193-133">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d6193-134">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="d6193-134">Schema Name</span></span>  <br/> |<span data-ttu-id="d6193-135">Схема типа</span><span class="sxs-lookup"><span data-stu-id="d6193-135">Type schema</span></span>  <br/> |
|<span data-ttu-id="d6193-136">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="d6193-136">Validation File</span></span>  <br/> |<span data-ttu-id="d6193-137">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="d6193-137">types.xsd</span></span>  <br/> |
|<span data-ttu-id="d6193-138">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="d6193-138">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="d6193-139">См. также</span><span class="sxs-lookup"><span data-stu-id="d6193-139">See also</span></span>

- [<span data-ttu-id="d6193-140">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="d6193-140">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

