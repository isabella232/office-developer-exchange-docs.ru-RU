---
title: AppointmentState
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AppointmentState
api_type:
- schema
ms.assetid: ab3f5d04-ace1-4a15-9107-cefa6c41abc7
description: Элемент AppointmentState указывает состояние встречи.
ms.openlocfilehash: 05e92a3fea10a84518b0680c425011a91bc43d93
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761480"
---
# <a name="appointmentstate"></a><span data-ttu-id="0d1f5-103">AppointmentState</span><span class="sxs-lookup"><span data-stu-id="0d1f5-103">AppointmentState</span></span>

<span data-ttu-id="0d1f5-104">Элемент **AppointmentState** указывает состояние встречи.</span><span class="sxs-lookup"><span data-stu-id="0d1f5-104">The **AppointmentState** element specifies the status of the appointment.</span></span> 
  
```XML
<AppointmentState/>
```

 <span data-ttu-id="0d1f5-105">**int**</span><span class="sxs-lookup"><span data-stu-id="0d1f5-105">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0d1f5-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="0d1f5-106">Attributes and elements</span></span>

<span data-ttu-id="0d1f5-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="0d1f5-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0d1f5-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="0d1f5-108">Attributes</span></span>

<span data-ttu-id="0d1f5-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="0d1f5-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0d1f5-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="0d1f5-110">Child elements</span></span>

<span data-ttu-id="0d1f5-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="0d1f5-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="0d1f5-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="0d1f5-112">Parent elements</span></span>

|<span data-ttu-id="0d1f5-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="0d1f5-113">**Element**</span></span>|<span data-ttu-id="0d1f5-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="0d1f5-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0d1f5-115">Элемента календаря, имеющего</span><span class="sxs-lookup"><span data-stu-id="0d1f5-115">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="0d1f5-116">Представляет элемент календаря Exchange.</span><span class="sxs-lookup"><span data-stu-id="0d1f5-116">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="0d1f5-117">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="0d1f5-117">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="0d1f5-118">Представляет собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="0d1f5-118">Represents a meeting in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="0d1f5-119">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="0d1f5-119">Text value</span></span>

<span data-ttu-id="0d1f5-120">Этот элемент содержит значение текста, что представляет значение бит.</span><span class="sxs-lookup"><span data-stu-id="0d1f5-120">This element contains a text value that represents set bits.</span></span> <span data-ttu-id="0d1f5-121">Это в форме целое число.</span><span class="sxs-lookup"><span data-stu-id="0d1f5-121">This is in integer form.</span></span> <span data-ttu-id="0d1f5-122">Этот элемент доступен только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0d1f5-122">This element is read-only.</span></span> <span data-ttu-id="0d1f5-123">Он только будет возвращен в ответе.</span><span class="sxs-lookup"><span data-stu-id="0d1f5-123">It will only be returned in a response.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="0d1f5-124">Замечания</span><span class="sxs-lookup"><span data-stu-id="0d1f5-124">Remarks</span></span>

<span data-ttu-id="0d1f5-125">Целое значение, которое возвращается представляет битовую маску состояние встречи.</span><span class="sxs-lookup"><span data-stu-id="0d1f5-125">The integer value that is returned represents the appointment state bitmask.</span></span> <span data-ttu-id="0d1f5-126">В следующей таблице описываются каждый бит.</span><span class="sxs-lookup"><span data-stu-id="0d1f5-126">The following table describes each bit.</span></span>
  
|<span data-ttu-id="0d1f5-127">**Имя**</span><span class="sxs-lookup"><span data-stu-id="0d1f5-127">**Name**</span></span>|<span data-ttu-id="0d1f5-128">**Бит**</span><span class="sxs-lookup"><span data-stu-id="0d1f5-128">**Bit**</span></span>|<span data-ttu-id="0d1f5-129">**Описание**</span><span class="sxs-lookup"><span data-stu-id="0d1f5-129">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="0d1f5-130">Нет</span><span class="sxs-lookup"><span data-stu-id="0d1f5-130">None</span></span>  <br/> |<span data-ttu-id="0d1f5-131">0x0000</span><span class="sxs-lookup"><span data-stu-id="0d1f5-131">0x0000</span></span>  <br/> |<span data-ttu-id="0d1f5-132">Флаги не были установлены.</span><span class="sxs-lookup"><span data-stu-id="0d1f5-132">No flags have been set.</span></span> <span data-ttu-id="0d1f5-133">Используется только для встречи, которая не включает участников.</span><span class="sxs-lookup"><span data-stu-id="0d1f5-133">This is only used for an appointment that does not include attendees.</span></span>  <br/> |
|<span data-ttu-id="0d1f5-134">Собрание</span><span class="sxs-lookup"><span data-stu-id="0d1f5-134">Meeting</span></span>  <br/> |<span data-ttu-id="0d1f5-135">0x0001</span><span class="sxs-lookup"><span data-stu-id="0d1f5-135">0x0001</span></span>  <br/> |<span data-ttu-id="0d1f5-136">В этом встреча является собранием.</span><span class="sxs-lookup"><span data-stu-id="0d1f5-136">This appointment is a meeting.</span></span>  <br/> |
|<span data-ttu-id="0d1f5-137">Получено</span><span class="sxs-lookup"><span data-stu-id="0d1f5-137">Received</span></span>  <br/> |<span data-ttu-id="0d1f5-138">0x0002</span><span class="sxs-lookup"><span data-stu-id="0d1f5-138">0x0002</span></span>  <br/> |<span data-ttu-id="0d1f5-139">В этом встречи был получен.</span><span class="sxs-lookup"><span data-stu-id="0d1f5-139">This appointment has been received.</span></span>  <br/> |
|<span data-ttu-id="0d1f5-140">Canceled.</span><span class="sxs-lookup"><span data-stu-id="0d1f5-140">Canceled</span></span>  <br/> |<span data-ttu-id="0d1f5-141">0x0004</span><span class="sxs-lookup"><span data-stu-id="0d1f5-141">0x0004</span></span>  <br/> |<span data-ttu-id="0d1f5-142">В этом встречи было отменено.</span><span class="sxs-lookup"><span data-stu-id="0d1f5-142">This appointment has been canceled.</span></span>  <br/> |
   
<span data-ttu-id="0d1f5-143">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="0d1f5-143">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0d1f5-144">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="0d1f5-144">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0d1f5-145">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="0d1f5-145">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="0d1f5-146">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="0d1f5-146">Schema name</span></span>  <br/> |<span data-ttu-id="0d1f5-147">Схема Types</span><span class="sxs-lookup"><span data-stu-id="0d1f5-147">Types schema</span></span>  <br/> |
|<span data-ttu-id="0d1f5-148">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="0d1f5-148">Validation file</span></span>  <br/> |<span data-ttu-id="0d1f5-149">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="0d1f5-149">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="0d1f5-150">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="0d1f5-150">Can be empty</span></span>  <br/> |<span data-ttu-id="0d1f5-151">False</span><span class="sxs-lookup"><span data-stu-id="0d1f5-151">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0d1f5-152">См. также</span><span class="sxs-lookup"><span data-stu-id="0d1f5-152">See also</span></span>

- [<span data-ttu-id="0d1f5-153">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="0d1f5-153">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
