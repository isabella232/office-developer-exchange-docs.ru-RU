---
title: дисаблереасон
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f41b5be6-9b79-4e83-8cdb-aa779e13cb3f
description: Элемент Дисаблереасон указывает причину отключения приложения.
ms.openlocfilehash: f900bd1b98b294900f767c778b9c5f87f74042ca
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762127"
---
# <a name="disablereason"></a><span data-ttu-id="4700f-103">дисаблереасон</span><span class="sxs-lookup"><span data-stu-id="4700f-103">DisableReason</span></span>

<span data-ttu-id="4700f-104">Элемент **дисаблереасон** указывает причину отключения приложения.</span><span class="sxs-lookup"><span data-stu-id="4700f-104">The **DisableReason** element specifies the reason for disabling an app.</span></span> 
  
```XML
<DisableReason> NoReason | OutlookClientPerformance | OWAClientPerformance | MobileClientPerformance </DisableReason>
```

 <span data-ttu-id="4700f-105">**дисаблереасонтипе**</span><span class="sxs-lookup"><span data-stu-id="4700f-105">**DisableReasonType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4700f-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="4700f-106">Attributes and elements</span></span>

<span data-ttu-id="4700f-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="4700f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4700f-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="4700f-108">Attributes</span></span>

<span data-ttu-id="4700f-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="4700f-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4700f-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="4700f-110">Child elements</span></span>

<span data-ttu-id="4700f-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="4700f-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="4700f-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="4700f-112">Parent elements</span></span>

|<span data-ttu-id="4700f-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="4700f-113">**Element**</span></span>|<span data-ttu-id="4700f-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="4700f-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4700f-115">DisableApp</span><span class="sxs-lookup"><span data-stu-id="4700f-115">DisableApp</span></span>](disableapp.md) <br/> |<span data-ttu-id="4700f-116">Указывает запрос на отключение приложения.</span><span class="sxs-lookup"><span data-stu-id="4700f-116">Specifies a request to disable an app.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="4700f-117">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="4700f-117">Text value</span></span>

<span data-ttu-id="4700f-118">**Текстовое значение элемента Дисаблереасон**</span><span class="sxs-lookup"><span data-stu-id="4700f-118">**DisableReason element text value**</span></span>

|<span data-ttu-id="4700f-119">**Значение**</span><span class="sxs-lookup"><span data-stu-id="4700f-119">**Value**</span></span>|<span data-ttu-id="4700f-120">**Описание**</span><span class="sxs-lookup"><span data-stu-id="4700f-120">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="4700f-121">Причина</span><span class="sxs-lookup"><span data-stu-id="4700f-121">NoReason</span></span>  <br/> |<span data-ttu-id="4700f-122">Причина не задана</span><span class="sxs-lookup"><span data-stu-id="4700f-122">No reason given</span></span>  <br/> |
|<span data-ttu-id="4700f-123">аутлукклиентперформанце</span><span class="sxs-lookup"><span data-stu-id="4700f-123">OutlookClientPerformance</span></span>  <br/> |<span data-ttu-id="4700f-124">Для повышения производительности почтового клиента.</span><span class="sxs-lookup"><span data-stu-id="4700f-124">To improve email client performance.</span></span>  <br/> |
|<span data-ttu-id="4700f-125">оваклиентперформанце</span><span class="sxs-lookup"><span data-stu-id="4700f-125">OWAClientPerformance</span></span>  <br/> |<span data-ttu-id="4700f-126">Для повышения производительности клиента веб-приложения.</span><span class="sxs-lookup"><span data-stu-id="4700f-126">To improve Web app client performance.</span></span>  <br/> |
|<span data-ttu-id="4700f-127">мобилеклиентперформанце</span><span class="sxs-lookup"><span data-stu-id="4700f-127">MobileClientPerformance</span></span>  <br/> |<span data-ttu-id="4700f-128">Для повышения производительности мобильных клиентов.</span><span class="sxs-lookup"><span data-stu-id="4700f-128">To improve mobile client performance.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="4700f-129">Примечания</span><span class="sxs-lookup"><span data-stu-id="4700f-129">Remarks</span></span>

<span data-ttu-id="4700f-130">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="4700f-130">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="4700f-131">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="4700f-131">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4700f-132">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="4700f-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4700f-133">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="4700f-133">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="4700f-134">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="4700f-134">Schema Name</span></span>  <br/> |<span data-ttu-id="4700f-135">Схема типа</span><span class="sxs-lookup"><span data-stu-id="4700f-135">Type schema</span></span>  <br/> |
|<span data-ttu-id="4700f-136">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="4700f-136">Validation File</span></span>  <br/> |<span data-ttu-id="4700f-137">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="4700f-137">types.xsd</span></span>  <br/> |
|<span data-ttu-id="4700f-138">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="4700f-138">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="4700f-139">См. также</span><span class="sxs-lookup"><span data-stu-id="4700f-139">See also</span></span>

- [<span data-ttu-id="4700f-140">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="4700f-140">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

