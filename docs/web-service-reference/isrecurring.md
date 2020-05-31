---
title: IsRecurring
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsRecurring
api_type:
- schema
ms.assetid: f4df6997-8d5b-4893-a4a5-fc7047e0a9c3
description: Элемент IsRecurring указывает, является ли элемент календаря, приглашение на собрание или задача частью повторяющегося элемента. Этот элемент доступен только для чтения.
ms.openlocfilehash: dfb0c28fe225792c7128409a8cf010627c624fe0
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834104"
---
# <a name="isrecurring"></a><span data-ttu-id="d2c70-104">IsRecurring</span><span class="sxs-lookup"><span data-stu-id="d2c70-104">IsRecurring</span></span>

<span data-ttu-id="d2c70-105">Элемент **IsRecurring** указывает, является ли элемент календаря, приглашение на собрание или задача частью повторяющегося элемента.</span><span class="sxs-lookup"><span data-stu-id="d2c70-105">The **IsRecurring** element indicates whether a calendar item, meeting request, or task is part of a recurring item.</span></span> <span data-ttu-id="d2c70-106">Этот элемент доступен только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d2c70-106">This element is read-only.</span></span> 
  
```xml
<IsRecurring/>
```

 <span data-ttu-id="d2c70-107">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="d2c70-107">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d2c70-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="d2c70-108">Attributes and elements</span></span>

<span data-ttu-id="d2c70-109">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="d2c70-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d2c70-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="d2c70-110">Attributes</span></span>

<span data-ttu-id="d2c70-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="d2c70-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d2c70-112">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="d2c70-112">Child elements</span></span>

<span data-ttu-id="d2c70-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="d2c70-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="d2c70-114">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="d2c70-114">Parent elements</span></span>

|<span data-ttu-id="d2c70-115">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="d2c70-115">**Element**</span></span>|<span data-ttu-id="d2c70-116">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d2c70-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d2c70-117">календаритем</span><span class="sxs-lookup"><span data-stu-id="d2c70-117">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="d2c70-118">Представляет элемент календаря Exchange.</span><span class="sxs-lookup"><span data-stu-id="d2c70-118">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="d2c70-119">Свойство meetingrequest</span><span class="sxs-lookup"><span data-stu-id="d2c70-119">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="d2c70-120">Представляет приглашение на собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="d2c70-120">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="d2c70-121">Задача</span><span class="sxs-lookup"><span data-stu-id="d2c70-121">Task</span></span>](task.md) <br/> |<span data-ttu-id="d2c70-122">Представляет задачу в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="d2c70-122">Represents a task in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="d2c70-123">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="d2c70-123">Text value</span></span>

<span data-ttu-id="d2c70-124">Текстовое значение, представляющее логическое значение является обязательным.</span><span class="sxs-lookup"><span data-stu-id="d2c70-124">A text value that represents a Boolean value is required.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="d2c70-125">Примечания</span><span class="sxs-lookup"><span data-stu-id="d2c70-125">Remarks</span></span>

<span data-ttu-id="d2c70-126">В следующей таблице показано, как свойство **IsRecurring** задано для различных типов элементов календаря для организаторов и участников, а также для приглашений на собрания и обновлений.</span><span class="sxs-lookup"><span data-stu-id="d2c70-126">The following table shows how the **IsRecurring** property is set for different calendar item types for organizers and attendees and for meeting requests and updates.</span></span> 
  
|<span data-ttu-id="d2c70-127">**Тип Календаритем**</span><span class="sxs-lookup"><span data-stu-id="d2c70-127">**CalendarItem Type**</span></span>|<span data-ttu-id="d2c70-128">**Органайзер <br/> (IsRecurring)**</span><span class="sxs-lookup"><span data-stu-id="d2c70-128">**Organizer  <br/> (IsRecurring)**</span></span>|<span data-ttu-id="d2c70-129">**Участник <br/> (IsRecurring)**</span><span class="sxs-lookup"><span data-stu-id="d2c70-129">**Attendee  <br/> (IsRecurring)**</span></span>|<span data-ttu-id="d2c70-130">**Приглашение на собрание или <br/> обновление (IsRecurring)**</span><span class="sxs-lookup"><span data-stu-id="d2c70-130">**Meeting request/update  <br/> (IsRecurring)**</span></span>|
|:-----|:-----|:-----|:-----|
|<span data-ttu-id="d2c70-131">Один экземпляр</span><span class="sxs-lookup"><span data-stu-id="d2c70-131">Single Occurrence</span></span>  <br/> |<span data-ttu-id="d2c70-132">**ЗНАЧЕНИЯ**</span><span class="sxs-lookup"><span data-stu-id="d2c70-132">**FALSE**</span></span> <br/> |<span data-ttu-id="d2c70-133">**ЗНАЧЕНИЯ**</span><span class="sxs-lookup"><span data-stu-id="d2c70-133">**FALSE**</span></span> <br/> |<span data-ttu-id="d2c70-134">**ЗНАЧЕНИЯ**</span><span class="sxs-lookup"><span data-stu-id="d2c70-134">**FALSE**</span></span> <br/> |
|<span data-ttu-id="d2c70-135">Повторяющаяся основная реплика</span><span class="sxs-lookup"><span data-stu-id="d2c70-135">Recurring Master</span></span>  <br/> |<span data-ttu-id="d2c70-136">**ЗНАЧЕНИЯ**</span><span class="sxs-lookup"><span data-stu-id="d2c70-136">**FALSE**</span></span> <br/> |<span data-ttu-id="d2c70-137">**ОТНОСИТСЯ**</span><span class="sxs-lookup"><span data-stu-id="d2c70-137">**TRUE**</span></span> <br/> |<span data-ttu-id="d2c70-138">**ОТНОСИТСЯ**</span><span class="sxs-lookup"><span data-stu-id="d2c70-138">**TRUE**</span></span> <br/> |
|<span data-ttu-id="d2c70-139">Повторяющееся исключение</span><span class="sxs-lookup"><span data-stu-id="d2c70-139">Recurring Exception</span></span>  <br/> |<span data-ttu-id="d2c70-140">**ОТНОСИТСЯ**</span><span class="sxs-lookup"><span data-stu-id="d2c70-140">**TRUE**</span></span> <br/> |<span data-ttu-id="d2c70-141">**ОТНОСИТСЯ**</span><span class="sxs-lookup"><span data-stu-id="d2c70-141">**TRUE**</span></span> <br/> |<span data-ttu-id="d2c70-142">**ОТНОСИТСЯ**</span><span class="sxs-lookup"><span data-stu-id="d2c70-142">**TRUE**</span></span> <br/> |
   
<span data-ttu-id="d2c70-143">Значение свойства **IsRecurring** , заданное для повторяющихся элементов основного календаря для организатора, является неправильным; Это значение должно быть равно **true**.</span><span class="sxs-lookup"><span data-stu-id="d2c70-143">The **IsRecurring** property value that is set for recurring master calendar items for the organizer is incorrect; this value should be set to **TRUE**.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="d2c70-144">Операция GetUserAvailability также содержит элемент [IsRecurring (календаревентдетаилс)](isrecurring-calendareventdetails.md) .</span><span class="sxs-lookup"><span data-stu-id="d2c70-144">The GetUserAvailability operation also has an [IsRecurring (CalendarEventDetails)](isrecurring-calendareventdetails.md) element.</span></span> 
  
<span data-ttu-id="d2c70-145">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="d2c70-145">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d2c70-146">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="d2c70-146">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d2c70-147">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="d2c70-147">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d2c70-148">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="d2c70-148">Schema name</span></span>  <br/> |<span data-ttu-id="d2c70-149">Схема Types</span><span class="sxs-lookup"><span data-stu-id="d2c70-149">Types schema</span></span>  <br/> |
|<span data-ttu-id="d2c70-150">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="d2c70-150">Validation file</span></span>  <br/> |<span data-ttu-id="d2c70-151">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="d2c70-151">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d2c70-152">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="d2c70-152">Can be empty</span></span>  <br/> |<span data-ttu-id="d2c70-153">False</span><span class="sxs-lookup"><span data-stu-id="d2c70-153">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d2c70-154">См. также</span><span class="sxs-lookup"><span data-stu-id="d2c70-154">See also</span></span>



[<span data-ttu-id="d2c70-155">Тасктипе. IsRecurring</span><span class="sxs-lookup"><span data-stu-id="d2c70-155">TaskType.IsRecurring</span></span>](https://msdn.microsoft.com/library/ExchangeWebServices.TaskType.IsRecurring.aspx)
  
[<span data-ttu-id="d2c70-156">Календаревентдетаилс. IsRecurring</span><span class="sxs-lookup"><span data-stu-id="d2c70-156">CalendarEventDetails.IsRecurring</span></span>](https://msdn.microsoft.com/library/ExchangeWebServices.CalendarEventDetails.IsRecurring.aspx)
  
[<span data-ttu-id="d2c70-157">Календаритемтипе. IsRecurring</span><span class="sxs-lookup"><span data-stu-id="d2c70-157">CalendarItemType.IsRecurring</span></span>](https://msdn.microsoft.com/library/ExchangeWebServices.CalendarItemType.IsRecurring.aspx)
  
[<span data-ttu-id="d2c70-158">Митингрекуестмессажетипе. IsRecurring</span><span class="sxs-lookup"><span data-stu-id="d2c70-158">MeetingRequestMessageType.IsRecurring</span></span>](https://msdn.microsoft.com/library/ExchangeWebServices.MeetingRequestMessageType.IsRecurring.aspx)
  
[<span data-ttu-id="d2c70-159">Календаритемтипе. ИсрекуррингспеЦифиед</span><span class="sxs-lookup"><span data-stu-id="d2c70-159">CalendarItemType.IsRecurringSpecified</span></span>](https://msdn.microsoft.com/library/ExchangeWebServices.CalendarItemType.IsRecurringSpecified.aspx)
  
[<span data-ttu-id="d2c70-160">Митингрекуестмессажетипе. ИсрекуррингспеЦифиед</span><span class="sxs-lookup"><span data-stu-id="d2c70-160">MeetingRequestMessageType.IsRecurringSpecified</span></span>](https://msdn.microsoft.com/library/ExchangeWebServices.MeetingRequestMessageType.IsRecurringSpecified.aspx)
  
[<span data-ttu-id="d2c70-161">Тасктипе. ИсрекуррингспеЦифиед</span><span class="sxs-lookup"><span data-stu-id="d2c70-161">TaskType.IsRecurringSpecified</span></span>](https://msdn.microsoft.com/library/ExchangeWebServices.TaskType.IsRecurringSpecified.aspx)


- [<span data-ttu-id="d2c70-162">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="d2c70-162">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

