---
title: Конец
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
description: Элемент End представляет конец длительности.
ms.openlocfilehash: 90eea4fc545fae083e5675225665e517b502ba6f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762342"
---
# <a name="end"></a><span data-ttu-id="c9196-103">Конец</span><span class="sxs-lookup"><span data-stu-id="c9196-103">End</span></span>

<span data-ttu-id="c9196-104">Элемент **End** представляет конец длительности.</span><span class="sxs-lookup"><span data-stu-id="c9196-104">The **End** element represents the end of a duration.</span></span> 
  
```xml
<End/>
```

 <span data-ttu-id="c9196-105">**DateTime**</span><span class="sxs-lookup"><span data-stu-id="c9196-105">**DateTime**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c9196-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="c9196-106">Attributes and elements</span></span>

<span data-ttu-id="c9196-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="c9196-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c9196-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="c9196-108">Attributes</span></span>

<span data-ttu-id="c9196-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="c9196-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c9196-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="c9196-110">Child elements</span></span>

<span data-ttu-id="c9196-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="c9196-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="c9196-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="c9196-112">Parent elements</span></span>

|<span data-ttu-id="c9196-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="c9196-113">**Element**</span></span>|<span data-ttu-id="c9196-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="c9196-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c9196-115">календаритем</span><span class="sxs-lookup"><span data-stu-id="c9196-115">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="c9196-116">Представляет элемент календаря Exchange.</span><span class="sxs-lookup"><span data-stu-id="c9196-116">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="c9196-117">фирстоккурренце</span><span class="sxs-lookup"><span data-stu-id="c9196-117">FirstOccurrence</span></span>](firstoccurrence.md) <br/> |<span data-ttu-id="c9196-118">Представляет первое вхождение повторяющегося элемента календаря.</span><span class="sxs-lookup"><span data-stu-id="c9196-118">Represents the first occurrence of a recurring calendar item.</span></span>  <br/> |
|[<span data-ttu-id="c9196-119">ластоккурренце</span><span class="sxs-lookup"><span data-stu-id="c9196-119">LastOccurrence</span></span>](lastoccurrence.md) <br/> |<span data-ttu-id="c9196-120">Представляет последнее вхождение повторяющегося элемента календаря.</span><span class="sxs-lookup"><span data-stu-id="c9196-120">Represents the last occurrence of a recurring calendar item.</span></span>  <br/> |
|[<span data-ttu-id="c9196-121">Свойство meetingrequest</span><span class="sxs-lookup"><span data-stu-id="c9196-121">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="c9196-122">Представляет приглашение на собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="c9196-122">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="c9196-123">Экземпляр</span><span class="sxs-lookup"><span data-stu-id="c9196-123">Occurrence</span></span>](occurrence.md) <br/> |<span data-ttu-id="c9196-124">Представляет один измененный экземпляр повторяющегося элемента календаря.</span><span class="sxs-lookup"><span data-stu-id="c9196-124">Represents a single modified occurrence of a recurring calendar item.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="c9196-125">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="c9196-125">Text value</span></span>

<span data-ttu-id="c9196-126">Текстовое значение представляет конец длительности.</span><span class="sxs-lookup"><span data-stu-id="c9196-126">The text value represents the end of a duration.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="c9196-127">Примечания</span><span class="sxs-lookup"><span data-stu-id="c9196-127">Remarks</span></span>

<span data-ttu-id="c9196-128">Для операции UpdateItem можно задать время [начала](start.md) и **окончания** для элемента хранилища Exchange.</span><span class="sxs-lookup"><span data-stu-id="c9196-128">The UpdateItem operation can set the [Start](start.md) and **End** time of an Exchange store item.</span></span> <span data-ttu-id="c9196-129">В запросе UpdateItem вы можете задать время [начала](start.md) , не устанавливая и время **окончания** .</span><span class="sxs-lookup"><span data-stu-id="c9196-129">In an UpdateItem request, you can set the [Start](start.md) time without also setting the **End** time.</span></span> <span data-ttu-id="c9196-130">Это может привести к ошибке, если время [начала](start.md) позже времени **окончания** .</span><span class="sxs-lookup"><span data-stu-id="c9196-130">This can cause an error if the [Start](start.md) time is later than the **End** time.</span></span> <span data-ttu-id="c9196-131">Имейте в виду, что клиентские приложения должны выполнить корректировку до времени **окончания** при изменении времени [начала](start.md) , чтобы сохранить длительность.</span><span class="sxs-lookup"><span data-stu-id="c9196-131">Be aware that client applications must perform adjustments to the **End** time when that [Start](start.md) time is changed in order to preserve the duration.</span></span> 
  
 <span data-ttu-id="c9196-132">**Note (Примечание** ) Сведения о смещении часового пояса теряются, если даты [начала](start.md) и **окончания** повторяющегося элемента шаблона не имеют даты, равной первому появлению еженедельного расписания повторения.</span><span class="sxs-lookup"><span data-stu-id="c9196-132">**Note** The time zone offset information is lost if the [Start](start.md) and **End** dates of the recurring master item do not have a date that is equal to the first occurrence of a weekly recurrence pattern.</span></span> 
  
<span data-ttu-id="c9196-133">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="c9196-133">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c9196-134">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="c9196-134">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c9196-135">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="c9196-135">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="c9196-136">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="c9196-136">Schema Name</span></span>  <br/> |<span data-ttu-id="c9196-137">Схема Types</span><span class="sxs-lookup"><span data-stu-id="c9196-137">Types schema</span></span>  <br/> |
|<span data-ttu-id="c9196-138">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="c9196-138">Validation File</span></span>  <br/> |<span data-ttu-id="c9196-139">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="c9196-139">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="c9196-140">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="c9196-140">Can be Empty</span></span>  <br/> |<span data-ttu-id="c9196-141">False</span><span class="sxs-lookup"><span data-stu-id="c9196-141">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c9196-142">См. также</span><span class="sxs-lookup"><span data-stu-id="c9196-142">See also</span></span>



[<span data-ttu-id="c9196-143">виклирекурренце</span><span class="sxs-lookup"><span data-stu-id="c9196-143">WeeklyRecurrence</span></span>](weeklyrecurrence.md)
  
 <span data-ttu-id="c9196-144">**End**</span><span class="sxs-lookup"><span data-stu-id="c9196-144">**End**</span></span>


- [<span data-ttu-id="c9196-145">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="c9196-145">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

