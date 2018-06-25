---
title: ConnectionFailureCause
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ConnectionFailureCause
api_type:
- schema
ms.assetid: d2160c8a-015c-4964-b7f7-93478764a173
description: Элемент ConnectionFailureCause указывает причину отключение от телефонный звонок.
ms.openlocfilehash: 54b4f5b89efdb42ef82dbef8f1af14a39c0ccc6a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761716"
---
# <a name="connectionfailurecause"></a><span data-ttu-id="34125-103">ConnectionFailureCause</span><span class="sxs-lookup"><span data-stu-id="34125-103">ConnectionFailureCause</span></span>

<span data-ttu-id="34125-104">Элемент **ConnectionFailureCause** указывает причину отключение от телефонный звонок.</span><span class="sxs-lookup"><span data-stu-id="34125-104">The **ConnectionFailureCause** element specifies the reason for a disconnection from a telephone call.</span></span> 
  
```xml
<ConnectionFailureCause>None or UserBusy or NoAnswer or Unavailable or Other</ConnectionFailureCause>
```

 <span data-ttu-id="34125-105">**ConnectionFailureCauseType**</span><span class="sxs-lookup"><span data-stu-id="34125-105">**ConnectionFailureCauseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="34125-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="34125-106">Attributes and elements</span></span>

<span data-ttu-id="34125-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="34125-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="34125-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="34125-108">Attributes</span></span>

<span data-ttu-id="34125-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="34125-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="34125-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="34125-110">Child elements</span></span>

<span data-ttu-id="34125-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="34125-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="34125-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="34125-112">Parent elements</span></span>

|<span data-ttu-id="34125-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="34125-113">**Element**</span></span>|<span data-ttu-id="34125-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="34125-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="34125-115">PhoneCallInformation</span><span class="sxs-lookup"><span data-stu-id="34125-115">PhoneCallInformation</span></span>](phonecallinformation.md) <br/> |<span data-ttu-id="34125-116">Задает сведения о состоянии для телефонные звонки.</span><span class="sxs-lookup"><span data-stu-id="34125-116">Specifies the state information for a telephone call.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="34125-117">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="34125-117">Text value</span></span>

<span data-ttu-id="34125-118">В следующей таблице приведены возможные значения для элемента **ConnectionFailureCause** .</span><span class="sxs-lookup"><span data-stu-id="34125-118">The following table lists the possible values for the **ConnectionFailureCause** element.</span></span> 
  
<span data-ttu-id="34125-119">**Значения элементов ConnectionFailureCause**</span><span class="sxs-lookup"><span data-stu-id="34125-119">**ConnectionFailureCause element values**</span></span>

|<span data-ttu-id="34125-120">**Значение**</span><span class="sxs-lookup"><span data-stu-id="34125-120">**Value**</span></span>|<span data-ttu-id="34125-121">**Описание**</span><span class="sxs-lookup"><span data-stu-id="34125-121">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="34125-122">Нет</span><span class="sxs-lookup"><span data-stu-id="34125-122">None</span></span>  <br/> |<span data-ttu-id="34125-123">Состоянии вызова не отключены или отключить причине не известен.</span><span class="sxs-lookup"><span data-stu-id="34125-123">Call state is not disconnected or the disconnect reason is not known.</span></span>  <br/> |
|<span data-ttu-id="34125-124">UserBusy</span><span class="sxs-lookup"><span data-stu-id="34125-124">UserBusy</span></span>  <br/> |<span data-ttu-id="34125-125">Строке вызываемой стороны была занята.</span><span class="sxs-lookup"><span data-stu-id="34125-125">The called party line was busy.</span></span>  <br/> |
|<span data-ttu-id="34125-126">NoAnswer</span><span class="sxs-lookup"><span data-stu-id="34125-126">NoAnswer</span></span>  <br/> |<span data-ttu-id="34125-127">Вызываемый абонент не отвечает.</span><span class="sxs-lookup"><span data-stu-id="34125-127">The called party did not answer.</span></span>  <br/> |
|<span data-ttu-id="34125-128">Недоступен</span><span class="sxs-lookup"><span data-stu-id="34125-128">Unavailable</span></span>  <br/> |<span data-ttu-id="34125-129">Количество вызываемый абонент не доступен.</span><span class="sxs-lookup"><span data-stu-id="34125-129">The called party number was not available.</span></span>  <br/> |
|<span data-ttu-id="34125-130">Other (другие)</span><span class="sxs-lookup"><span data-stu-id="34125-130">Other</span></span>  <br/> |<span data-ttu-id="34125-131">Универсальными по другим причинам disconnect.</span><span class="sxs-lookup"><span data-stu-id="34125-131">Catch-all for other disconnect reasons.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="34125-132">Замечания</span><span class="sxs-lookup"><span data-stu-id="34125-132">Remarks</span></span>

<span data-ttu-id="34125-133">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="34125-133">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="34125-134">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="34125-134">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="34125-135">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="34125-135">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="34125-136">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="34125-136">Schema Name</span></span>  <br/> |<span data-ttu-id="34125-137">Схема Types</span><span class="sxs-lookup"><span data-stu-id="34125-137">Types schema</span></span>  <br/> |
|<span data-ttu-id="34125-138">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="34125-138">Validation File</span></span>  <br/> |<span data-ttu-id="34125-139">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="34125-139">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="34125-140">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="34125-140">Can be Empty</span></span>  <br/> |<span data-ttu-id="34125-141">False</span><span class="sxs-lookup"><span data-stu-id="34125-141">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="34125-142">См. также</span><span class="sxs-lookup"><span data-stu-id="34125-142">See also</span></span>



- [<span data-ttu-id="34125-143">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="34125-143">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

