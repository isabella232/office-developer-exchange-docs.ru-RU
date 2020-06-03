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
ms.openlocfilehash: 1406d69647bde5389dc9bb61adf7537a57d5adfc
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463673"
---
# <a name="disablereason"></a><span data-ttu-id="c0124-103">дисаблереасон</span><span class="sxs-lookup"><span data-stu-id="c0124-103">DisableReason</span></span>

<span data-ttu-id="c0124-104">Элемент **дисаблереасон** указывает причину отключения приложения.</span><span class="sxs-lookup"><span data-stu-id="c0124-104">The **DisableReason** element specifies the reason for disabling an app.</span></span> 
  
```XML
<DisableReason> NoReason | OutlookClientPerformance | OWAClientPerformance | MobileClientPerformance </DisableReason>
```

 <span data-ttu-id="c0124-105">**дисаблереасонтипе**</span><span class="sxs-lookup"><span data-stu-id="c0124-105">**DisableReasonType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c0124-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="c0124-106">Attributes and elements</span></span>

<span data-ttu-id="c0124-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="c0124-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c0124-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="c0124-108">Attributes</span></span>

<span data-ttu-id="c0124-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="c0124-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c0124-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="c0124-110">Child elements</span></span>

<span data-ttu-id="c0124-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="c0124-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="c0124-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="c0124-112">Parent elements</span></span>

|<span data-ttu-id="c0124-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="c0124-113">**Element**</span></span>|<span data-ttu-id="c0124-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="c0124-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c0124-115">DisableApp</span><span class="sxs-lookup"><span data-stu-id="c0124-115">DisableApp</span></span>](disableapp.md) <br/> |<span data-ttu-id="c0124-116">Указывает запрос на отключение приложения.</span><span class="sxs-lookup"><span data-stu-id="c0124-116">Specifies a request to disable an app.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="c0124-117">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="c0124-117">Text value</span></span>

<span data-ttu-id="c0124-118">**Текстовое значение элемента Дисаблереасон**</span><span class="sxs-lookup"><span data-stu-id="c0124-118">**DisableReason element text value**</span></span>

|<span data-ttu-id="c0124-119">**Значение**</span><span class="sxs-lookup"><span data-stu-id="c0124-119">**Value**</span></span>|<span data-ttu-id="c0124-120">**Описание**</span><span class="sxs-lookup"><span data-stu-id="c0124-120">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="c0124-121">Причина</span><span class="sxs-lookup"><span data-stu-id="c0124-121">NoReason</span></span>  <br/> |<span data-ttu-id="c0124-122">Причина не задана</span><span class="sxs-lookup"><span data-stu-id="c0124-122">No reason given</span></span>  <br/> |
|<span data-ttu-id="c0124-123">аутлукклиентперформанце</span><span class="sxs-lookup"><span data-stu-id="c0124-123">OutlookClientPerformance</span></span>  <br/> |<span data-ttu-id="c0124-124">Для повышения производительности почтового клиента.</span><span class="sxs-lookup"><span data-stu-id="c0124-124">To improve email client performance.</span></span>  <br/> |
|<span data-ttu-id="c0124-125">оваклиентперформанце</span><span class="sxs-lookup"><span data-stu-id="c0124-125">OWAClientPerformance</span></span>  <br/> |<span data-ttu-id="c0124-126">Для повышения производительности клиента веб-приложения.</span><span class="sxs-lookup"><span data-stu-id="c0124-126">To improve Web app client performance.</span></span>  <br/> |
|<span data-ttu-id="c0124-127">мобилеклиентперформанце</span><span class="sxs-lookup"><span data-stu-id="c0124-127">MobileClientPerformance</span></span>  <br/> |<span data-ttu-id="c0124-128">Для повышения производительности мобильных клиентов.</span><span class="sxs-lookup"><span data-stu-id="c0124-128">To improve mobile client performance.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="c0124-129">Примечания</span><span class="sxs-lookup"><span data-stu-id="c0124-129">Remarks</span></span>

<span data-ttu-id="c0124-130">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="c0124-130">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="c0124-131">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="c0124-131">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c0124-132">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="c0124-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c0124-133">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="c0124-133">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="c0124-134">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="c0124-134">Schema Name</span></span>  <br/> |<span data-ttu-id="c0124-135">Схема типа</span><span class="sxs-lookup"><span data-stu-id="c0124-135">Type schema</span></span>  <br/> |
|<span data-ttu-id="c0124-136">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="c0124-136">Validation File</span></span>  <br/> |<span data-ttu-id="c0124-137">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="c0124-137">types.xsd</span></span>  <br/> |
|<span data-ttu-id="c0124-138">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="c0124-138">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="c0124-139">См. также</span><span class="sxs-lookup"><span data-stu-id="c0124-139">See also</span></span>

- [<span data-ttu-id="c0124-140">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="c0124-140">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

