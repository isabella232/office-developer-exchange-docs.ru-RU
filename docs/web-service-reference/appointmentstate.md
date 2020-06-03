---
title: аппоинтментстате
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
description: Элемент Аппоинтментстате указывает состояние встречи.
ms.openlocfilehash: 8b0e827d02e9051f31d43199503dc286c50e2125
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463477"
---
# <a name="appointmentstate"></a><span data-ttu-id="80b7a-103">аппоинтментстате</span><span class="sxs-lookup"><span data-stu-id="80b7a-103">AppointmentState</span></span>

<span data-ttu-id="80b7a-104">Элемент **аппоинтментстате** указывает состояние встречи.</span><span class="sxs-lookup"><span data-stu-id="80b7a-104">The **AppointmentState** element specifies the status of the appointment.</span></span> 
  
```XML
<AppointmentState/>
```

 <span data-ttu-id="80b7a-105">**int**</span><span class="sxs-lookup"><span data-stu-id="80b7a-105">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="80b7a-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="80b7a-106">Attributes and elements</span></span>

<span data-ttu-id="80b7a-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="80b7a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="80b7a-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="80b7a-108">Attributes</span></span>

<span data-ttu-id="80b7a-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="80b7a-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="80b7a-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="80b7a-110">Child elements</span></span>

<span data-ttu-id="80b7a-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="80b7a-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="80b7a-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="80b7a-112">Parent elements</span></span>

|<span data-ttu-id="80b7a-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="80b7a-113">**Element**</span></span>|<span data-ttu-id="80b7a-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="80b7a-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="80b7a-115">календаритем</span><span class="sxs-lookup"><span data-stu-id="80b7a-115">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="80b7a-116">Представляет элемент календаря Exchange.</span><span class="sxs-lookup"><span data-stu-id="80b7a-116">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="80b7a-117">Свойство meetingrequest</span><span class="sxs-lookup"><span data-stu-id="80b7a-117">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="80b7a-118">Представляет собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="80b7a-118">Represents a meeting in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="80b7a-119">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="80b7a-119">Text value</span></span>

<span data-ttu-id="80b7a-120">Этот элемент содержит текстовое значение, представляющее набор битов.</span><span class="sxs-lookup"><span data-stu-id="80b7a-120">This element contains a text value that represents set bits.</span></span> <span data-ttu-id="80b7a-121">Это в виде целого числа.</span><span class="sxs-lookup"><span data-stu-id="80b7a-121">This is in integer form.</span></span> <span data-ttu-id="80b7a-122">Этот элемент доступен только для чтения.</span><span class="sxs-lookup"><span data-stu-id="80b7a-122">This element is read-only.</span></span> <span data-ttu-id="80b7a-123">Он будет возвращен только в ответе.</span><span class="sxs-lookup"><span data-stu-id="80b7a-123">It will only be returned in a response.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="80b7a-124">Примечания</span><span class="sxs-lookup"><span data-stu-id="80b7a-124">Remarks</span></span>

<span data-ttu-id="80b7a-125">Возвращаемое целое значение представляет битовую маску состояния встречи.</span><span class="sxs-lookup"><span data-stu-id="80b7a-125">The integer value that is returned represents the appointment state bitmask.</span></span> <span data-ttu-id="80b7a-126">В приведенной ниже таблице описывается каждый из этих бит.</span><span class="sxs-lookup"><span data-stu-id="80b7a-126">The following table describes each bit.</span></span>
  
|<span data-ttu-id="80b7a-127">**имя**</span><span class="sxs-lookup"><span data-stu-id="80b7a-127">**Name**</span></span>|<span data-ttu-id="80b7a-128">**Битовая**</span><span class="sxs-lookup"><span data-stu-id="80b7a-128">**Bit**</span></span>|<span data-ttu-id="80b7a-129">**Описание**</span><span class="sxs-lookup"><span data-stu-id="80b7a-129">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="80b7a-130">Нет</span><span class="sxs-lookup"><span data-stu-id="80b7a-130">None</span></span>  <br/> |<span data-ttu-id="80b7a-131">0x0000</span><span class="sxs-lookup"><span data-stu-id="80b7a-131">0x0000</span></span>  <br/> |<span data-ttu-id="80b7a-132">Флаги не заданы.</span><span class="sxs-lookup"><span data-stu-id="80b7a-132">No flags have been set.</span></span> <span data-ttu-id="80b7a-133">Используется только для встречи, не включающей участников.</span><span class="sxs-lookup"><span data-stu-id="80b7a-133">This is only used for an appointment that does not include attendees.</span></span>  <br/> |
|<span data-ttu-id="80b7a-134">Назначить</span><span class="sxs-lookup"><span data-stu-id="80b7a-134">Meeting</span></span>  <br/> |<span data-ttu-id="80b7a-135">0x0001</span><span class="sxs-lookup"><span data-stu-id="80b7a-135">0x0001</span></span>  <br/> |<span data-ttu-id="80b7a-136">Эта встреча является собранием.</span><span class="sxs-lookup"><span data-stu-id="80b7a-136">This appointment is a meeting.</span></span>  <br/> |
|<span data-ttu-id="80b7a-137">ПОЛУЧЕНО</span><span class="sxs-lookup"><span data-stu-id="80b7a-137">Received</span></span>  <br/> |<span data-ttu-id="80b7a-138">0x0002</span><span class="sxs-lookup"><span data-stu-id="80b7a-138">0x0002</span></span>  <br/> |<span data-ttu-id="80b7a-139">Эта встреча получена.</span><span class="sxs-lookup"><span data-stu-id="80b7a-139">This appointment has been received.</span></span>  <br/> |
|<span data-ttu-id="80b7a-140">Canceled.</span><span class="sxs-lookup"><span data-stu-id="80b7a-140">Canceled</span></span>  <br/> |<span data-ttu-id="80b7a-141">0x0004</span><span class="sxs-lookup"><span data-stu-id="80b7a-141">0x0004</span></span>  <br/> |<span data-ttu-id="80b7a-142">Эта встреча отменена.</span><span class="sxs-lookup"><span data-stu-id="80b7a-142">This appointment has been canceled.</span></span>  <br/> |
   
<span data-ttu-id="80b7a-143">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="80b7a-143">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="80b7a-144">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="80b7a-144">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="80b7a-145">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="80b7a-145">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="80b7a-146">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="80b7a-146">Schema name</span></span>  <br/> |<span data-ttu-id="80b7a-147">Схема Types</span><span class="sxs-lookup"><span data-stu-id="80b7a-147">Types schema</span></span>  <br/> |
|<span data-ttu-id="80b7a-148">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="80b7a-148">Validation file</span></span>  <br/> |<span data-ttu-id="80b7a-149">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="80b7a-149">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="80b7a-150">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="80b7a-150">Can be empty</span></span>  <br/> |<span data-ttu-id="80b7a-151">False</span><span class="sxs-lookup"><span data-stu-id="80b7a-151">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="80b7a-152">См. также</span><span class="sxs-lookup"><span data-stu-id="80b7a-152">See also</span></span>

- [<span data-ttu-id="80b7a-153">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="80b7a-153">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

