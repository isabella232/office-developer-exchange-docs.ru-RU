---
title: End
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- End
api_type:
- schema
ms.assetid: 72329821-32ff-495d-b6e5-fdc011003c2e
description: Последний элемент представляет конец длительность.
ms.openlocfilehash: 90eea4fc545fae083e5675225665e517b502ba6f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762342"
---
# <a name="end"></a><span data-ttu-id="6a0da-103">End</span><span class="sxs-lookup"><span data-stu-id="6a0da-103">End</span></span>

<span data-ttu-id="6a0da-104">**Последний** элемент представляет конец длительность.</span><span class="sxs-lookup"><span data-stu-id="6a0da-104">The **End** element represents the end of a duration.</span></span> 
  
```xml
<End/>
```

 <span data-ttu-id="6a0da-105">**DateTime**</span><span class="sxs-lookup"><span data-stu-id="6a0da-105">**DateTime**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6a0da-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="6a0da-106">Attributes and elements</span></span>

<span data-ttu-id="6a0da-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="6a0da-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6a0da-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="6a0da-108">Attributes</span></span>

<span data-ttu-id="6a0da-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="6a0da-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6a0da-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="6a0da-110">Child elements</span></span>

<span data-ttu-id="6a0da-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="6a0da-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="6a0da-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="6a0da-112">Parent elements</span></span>

|<span data-ttu-id="6a0da-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="6a0da-113">**Element**</span></span>|<span data-ttu-id="6a0da-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="6a0da-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6a0da-115">Элемента календаря, имеющего</span><span class="sxs-lookup"><span data-stu-id="6a0da-115">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="6a0da-116">Представляет элемент календаря Exchange.</span><span class="sxs-lookup"><span data-stu-id="6a0da-116">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="6a0da-117">FirstOccurrence</span><span class="sxs-lookup"><span data-stu-id="6a0da-117">FirstOccurrence</span></span>](firstoccurrence.md) <br/> |<span data-ttu-id="6a0da-118">Представляет первого появления повторяющегося элемента календаря.</span><span class="sxs-lookup"><span data-stu-id="6a0da-118">Represents the first occurrence of a recurring calendar item.</span></span>  <br/> |
|[<span data-ttu-id="6a0da-119">LastOccurrence</span><span class="sxs-lookup"><span data-stu-id="6a0da-119">LastOccurrence</span></span>](lastoccurrence.md) <br/> |<span data-ttu-id="6a0da-120">Представляет последнего вхождения повторяющегося элемента календаря.</span><span class="sxs-lookup"><span data-stu-id="6a0da-120">Represents the last occurrence of a recurring calendar item.</span></span>  <br/> |
|[<span data-ttu-id="6a0da-121">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="6a0da-121">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="6a0da-122">Представляет приглашение на собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="6a0da-122">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="6a0da-123">Вхождение</span><span class="sxs-lookup"><span data-stu-id="6a0da-123">Occurrence</span></span>](occurrence.md) <br/> |<span data-ttu-id="6a0da-124">Представляет измененной вхождения повторяющегося элемента календаря.</span><span class="sxs-lookup"><span data-stu-id="6a0da-124">Represents a single modified occurrence of a recurring calendar item.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="6a0da-125">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="6a0da-125">Text value</span></span>

<span data-ttu-id="6a0da-126">Текстовое значение представляет конец длительность.</span><span class="sxs-lookup"><span data-stu-id="6a0da-126">The text value represents the end of a duration.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="6a0da-127">Замечания</span><span class="sxs-lookup"><span data-stu-id="6a0da-127">Remarks</span></span>

<span data-ttu-id="6a0da-128">Операция UpdateItem можно задать время [Start](start.md) и **End** объекта хранилища Exchange.</span><span class="sxs-lookup"><span data-stu-id="6a0da-128">The UpdateItem operation can set the [Start](start.md) and **End** time of an Exchange store item.</span></span> <span data-ttu-id="6a0da-129">В запросе UpdateItem можно задать время [начала](start.md) без предоставления время **окончания** .</span><span class="sxs-lookup"><span data-stu-id="6a0da-129">In an UpdateItem request, you can set the [Start](start.md) time without also setting the **End** time.</span></span> <span data-ttu-id="6a0da-130">Это может вызвать ошибку, если время [начала](start.md) позднее время **окончания** .</span><span class="sxs-lookup"><span data-stu-id="6a0da-130">This can cause an error if the [Start](start.md) time is later than the **End** time.</span></span> <span data-ttu-id="6a0da-131">Обратите внимание, что клиентские приложения должны выполнить настройку время **окончания** , изменения, время [начала](start.md) для сохранения во время выполнения.</span><span class="sxs-lookup"><span data-stu-id="6a0da-131">Be aware that client applications must perform adjustments to the **End** time when that [Start](start.md) time is changed in order to preserve the duration.</span></span> 
  
 <span data-ttu-id="6a0da-132">**Примечание** [Запуск](start.md) и **конечной** дат повторяющегося элемента шаблона, у которых дата, равный первого появления еженедельно повторяющейся информации смещение часового пояса будут потеряны.</span><span class="sxs-lookup"><span data-stu-id="6a0da-132">**Note** The time zone offset information is lost if the [Start](start.md) and **End** dates of the recurring master item do not have a date that is equal to the first occurrence of a weekly recurrence pattern.</span></span> 
  
<span data-ttu-id="6a0da-133">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="6a0da-133">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6a0da-134">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="6a0da-134">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6a0da-135">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="6a0da-135">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="6a0da-136">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="6a0da-136">Schema Name</span></span>  <br/> |<span data-ttu-id="6a0da-137">Схема Types</span><span class="sxs-lookup"><span data-stu-id="6a0da-137">Types schema</span></span>  <br/> |
|<span data-ttu-id="6a0da-138">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="6a0da-138">Validation File</span></span>  <br/> |<span data-ttu-id="6a0da-139">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="6a0da-139">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="6a0da-140">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="6a0da-140">Can be Empty</span></span>  <br/> |<span data-ttu-id="6a0da-141">False</span><span class="sxs-lookup"><span data-stu-id="6a0da-141">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6a0da-142">См. также</span><span class="sxs-lookup"><span data-stu-id="6a0da-142">See also</span></span>



[<span data-ttu-id="6a0da-143">WeeklyRecurrence</span><span class="sxs-lookup"><span data-stu-id="6a0da-143">WeeklyRecurrence</span></span>](weeklyrecurrence.md)
  
 <span data-ttu-id="6a0da-144">**End**</span><span class="sxs-lookup"><span data-stu-id="6a0da-144">**End**</span></span>


- [<span data-ttu-id="6a0da-145">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="6a0da-145">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

