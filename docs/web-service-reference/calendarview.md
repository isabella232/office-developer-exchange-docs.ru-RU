---
title: CalendarView
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CalendarView
api_type:
- schema
ms.assetid: a4a953b8-0710-416c-95ef-59e51eba9982
description: Элемент CalendarView определяет операцию FindItem, возвращая элементы календаря в наборе в том виде, в котором они отображаются в календаре.
ms.openlocfilehash: e547a4b2db5c09ebefd9a072da6cc4733818002e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462264"
---
# <a name="calendarview"></a><span data-ttu-id="74a8f-103">CalendarView</span><span class="sxs-lookup"><span data-stu-id="74a8f-103">CalendarView</span></span>

<span data-ttu-id="74a8f-104">Элемент **CalendarView** определяет [операцию FindItem](finditem-operation.md) , возвращая элементы календаря в наборе в том виде, в котором они отображаются в календаре.</span><span class="sxs-lookup"><span data-stu-id="74a8f-104">The **CalendarView** element defines a [FindItem operation](finditem-operation.md) as returning calendar items in a set as they appear in a calendar.</span></span> 
  
[<span data-ttu-id="74a8f-105">FindItem</span><span class="sxs-lookup"><span data-stu-id="74a8f-105">FindItem</span></span>](finditem.md)
  
[<span data-ttu-id="74a8f-106">CalendarView</span><span class="sxs-lookup"><span data-stu-id="74a8f-106">CalendarView</span></span>](calendarview.md)
  
```XML
<CalendarView MaxEntriesReturned="" StartDate="" EndDate="" />
```

<span data-ttu-id="74a8f-107">**CalendarView**</span><span class="sxs-lookup"><span data-stu-id="74a8f-107">**CalendarView**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="74a8f-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="74a8f-108">Attributes and elements</span></span>

<span data-ttu-id="74a8f-109">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="74a8f-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="74a8f-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="74a8f-110">Attributes</span></span>

|<span data-ttu-id="74a8f-111">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="74a8f-111">**Attribute**</span></span>|<span data-ttu-id="74a8f-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="74a8f-112">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="74a8f-113">**максентриесретурнед**</span><span class="sxs-lookup"><span data-stu-id="74a8f-113">**MaxEntriesReturned**</span></span> <br/> |<span data-ttu-id="74a8f-114">Описывает максимальное число результатов, возвращаемых в ответе FindItem.</span><span class="sxs-lookup"><span data-stu-id="74a8f-114">Describes the maximum number of results to return in the FindItem response.</span></span>  <br/> |
|<span data-ttu-id="74a8f-115">**StartDate**</span><span class="sxs-lookup"><span data-stu-id="74a8f-115">**StartDate**</span></span> <br/> |<span data-ttu-id="74a8f-116">Указывает начало интервала времени, запрашиваемого для элементов календаря.</span><span class="sxs-lookup"><span data-stu-id="74a8f-116">Identifies the start of a time span queried for calendar items.</span></span> <span data-ttu-id="74a8f-117">Все элементы календаря с временем окончания, предшествующим **StartDate** , не будут возвращены.</span><span class="sxs-lookup"><span data-stu-id="74a8f-117">All calendar items that have an end time that is before **StartDate** will not be returned.</span></span> <span data-ttu-id="74a8f-118">Значение **StartDate** может указываться в формате UTC, как в 2006 – 01-02T12:00:00Z или в формате, где указано местное время и смещение часового пояса, как в 2006 – 01-02T04:00:00-08:00.</span><span class="sxs-lookup"><span data-stu-id="74a8f-118">The value of **StartDate** can be specified in coordinated universal time (UTC) format, as in 2006-01-02T12:00:00Z, or in a format where local time and time zone offset is specified, as in 2006-01-02T04:00:00-08:00.</span></span>  <br/><br/><span data-ttu-id="74a8f-119">Этот атрибут является обязательным.</span><span class="sxs-lookup"><span data-stu-id="74a8f-119">This attribute is required.</span></span>  <br/> |
|<span data-ttu-id="74a8f-120">**EndDate**</span><span class="sxs-lookup"><span data-stu-id="74a8f-120">**EndDate**</span></span> <br/> |<span data-ttu-id="74a8f-121">Определяет конец интервала времени, запрашиваемого для элементов календаря.</span><span class="sxs-lookup"><span data-stu-id="74a8f-121">Identifies the end of a time span queried for calendar items.</span></span> <span data-ttu-id="74a8f-122">Все элементы календаря, время начала которых находится в начале или после **даты окончания** , не будут возвращены.</span><span class="sxs-lookup"><span data-stu-id="74a8f-122">All calendar items that have a start time that is on or after **EndDate** will not be returned.</span></span> <span data-ttu-id="74a8f-123">Значение параметра **EndDate** можно указать в формате UTC, как в 2006-02-02T12:00:00Z, или в формате, где указаны местное время и смещение часового пояса, например, в 2006-02-02T04:00:00-08:00.</span><span class="sxs-lookup"><span data-stu-id="74a8f-123">The value of **EndDate** can be specified in UTC format, as in 2006-02-02T12:00:00Z, or in a format where local time and time zone offset is specified, as in 2006-02-02T04:00:00-08:00.</span></span>  <br/><br/><span data-ttu-id="74a8f-124">Значение **EndDate** должно быть больше или равно значению **StartDate**; в противном случае возвращается ошибка.</span><span class="sxs-lookup"><span data-stu-id="74a8f-124">**EndDate** must be greater than or equal to **StartDate**; otherwise an error is returned.</span></span> <span data-ttu-id="74a8f-125">Этот атрибут является обязательным.</span><span class="sxs-lookup"><span data-stu-id="74a8f-125">This attribute is required.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="74a8f-126">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="74a8f-126">Child elements</span></span>

<span data-ttu-id="74a8f-127">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="74a8f-127">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="74a8f-128">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="74a8f-128">Parent elements</span></span>

|<span data-ttu-id="74a8f-129">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="74a8f-129">**Element**</span></span>|<span data-ttu-id="74a8f-130">**Описание**</span><span class="sxs-lookup"><span data-stu-id="74a8f-130">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="74a8f-131">FindItem</span><span class="sxs-lookup"><span data-stu-id="74a8f-131">FindItem</span></span>](finditem.md) <br/> |<span data-ttu-id="74a8f-132">Определяет запрос на поиск элементов в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="74a8f-132">Defines a request to find items in a mailbox.</span></span><br/><br/> <span data-ttu-id="74a8f-133">Ниже приведено выражение XPath для этого элемента:</span><span class="sxs-lookup"><span data-stu-id="74a8f-133">The following is the XPath expression to this element:</span></span>  <br/>  `/FindItem` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="74a8f-134">Примечания</span><span class="sxs-lookup"><span data-stu-id="74a8f-134">Remarks</span></span>

<span data-ttu-id="74a8f-135">Если элемент **CalendarView** указан в запросе FindItem, веб-служба возвращает список одиночных элементов календаря и повторение повторяющихся элементов календаря в диапазоне, заданном в параметрах **StartDate** и **EndDate**.</span><span class="sxs-lookup"><span data-stu-id="74a8f-135">If the **CalendarView** element is specified in a FindItem request, the Web service returns a list of single calendar items and occurrences of recurring calendar items within the range specified by **StartDate** and **EndDate**.</span></span>
  
<span data-ttu-id="74a8f-136">Если элемент **CalendarView** не указан в запросе FindItem, веб-служба возвращает список одиночных элементов календаря и повторяющихся элементов основного календаря.</span><span class="sxs-lookup"><span data-stu-id="74a8f-136">If the **CalendarView** element is not specified in a FindItem request, the Web service returns a list of single calendar items and recurring master calendar items.</span></span> <span data-ttu-id="74a8f-137">Экземпляры повторяющегося элемента календаря не разворачиваются.</span><span class="sxs-lookup"><span data-stu-id="74a8f-137">Calendar occurrences of a recurring calendar item are not expanded.</span></span> 
  
<span data-ttu-id="74a8f-138">В запросах CalendarView следует использовать только следующие свойства, так как они поддерживают более быстрые запросы в календаре.</span><span class="sxs-lookup"><span data-stu-id="74a8f-138">CalendarView queries should only make use of the following properties since they support faster calendar queries.</span></span>
  
### <a name="recurrence-blob-properties"></a><span data-ttu-id="74a8f-139">Свойства больших двоичных объектов повторения</span><span class="sxs-lookup"><span data-stu-id="74a8f-139">Recurrence blob properties</span></span>
  
- <span data-ttu-id="74a8f-140">мапистарттиме</span><span class="sxs-lookup"><span data-stu-id="74a8f-140">MapiStartTime</span></span>
    
- <span data-ttu-id="74a8f-141">мапиендтиме</span><span class="sxs-lookup"><span data-stu-id="74a8f-141">MapiEndTime</span></span>
    
- <span data-ttu-id="74a8f-142">субжектпрефиксинтернал</span><span class="sxs-lookup"><span data-stu-id="74a8f-142">SubjectPrefixInternal</span></span>
    
- <span data-ttu-id="74a8f-143">нормализедсубжектинтернал</span><span class="sxs-lookup"><span data-stu-id="74a8f-143">NormalizedSubjectInternal</span></span>
    
- <span data-ttu-id="74a8f-144">маписубжект</span><span class="sxs-lookup"><span data-stu-id="74a8f-144">MapiSubject</span></span>
    
- <span data-ttu-id="74a8f-145">Расположение</span><span class="sxs-lookup"><span data-stu-id="74a8f-145">Location</span></span>
    
- <span data-ttu-id="74a8f-146">аппоинтментколор</span><span class="sxs-lookup"><span data-stu-id="74a8f-146">AppointmentColor</span></span>
    
- <span data-ttu-id="74a8f-147">мапиисаллдайевент</span><span class="sxs-lookup"><span data-stu-id="74a8f-147">MapiIsAllDayEvent</span></span>
    
- <span data-ttu-id="74a8f-148">мапихасаттачмент</span><span class="sxs-lookup"><span data-stu-id="74a8f-148">MapiHasAttachment</span></span>
    
- <span data-ttu-id="74a8f-149">фрибусистатус</span><span class="sxs-lookup"><span data-stu-id="74a8f-149">FreeBusyStatus</span></span>
    
- <span data-ttu-id="74a8f-150">реминдериссетинтернал</span><span class="sxs-lookup"><span data-stu-id="74a8f-150">ReminderIsSetInternal</span></span>
    
- <span data-ttu-id="74a8f-151">реминдерминутесбефорестартинтернал</span><span class="sxs-lookup"><span data-stu-id="74a8f-151">ReminderMinutesBeforeStartInternal</span></span>
    
- <span data-ttu-id="74a8f-152">аппоинтментстате</span><span class="sxs-lookup"><span data-stu-id="74a8f-152">AppointmentState</span></span>
    
- <span data-ttu-id="74a8f-153">AllAttachmentsHidden</span><span class="sxs-lookup"><span data-stu-id="74a8f-153">AllAttachmentsHidden</span></span>
    
- <span data-ttu-id="74a8f-154">чанжехигхлигхт</span><span class="sxs-lookup"><span data-stu-id="74a8f-154">ChangeHighlight</span></span>
    
### <a name="calculated-from-the-primary-recurrence-blob-or-master"></a><span data-ttu-id="74a8f-155">Рассчитывается на основе основного объекта BLOB или основного объекта повторения</span><span class="sxs-lookup"><span data-stu-id="74a8f-155">Calculated from the primary recurrence blob or master</span></span>
  
- <span data-ttu-id="74a8f-156">Идентификатор</span><span class="sxs-lookup"><span data-stu-id="74a8f-156">ItemId</span></span>
    
- <span data-ttu-id="74a8f-157">IsRecurring</span><span class="sxs-lookup"><span data-stu-id="74a8f-157">IsRecurring</span></span>
    
- <span data-ttu-id="74a8f-158">Исключение</span><span class="sxs-lookup"><span data-stu-id="74a8f-158">IsException</span></span>
    
- <span data-ttu-id="74a8f-159">аппоинтментрекурринг</span><span class="sxs-lookup"><span data-stu-id="74a8f-159">AppointmentRecurring</span></span>
    
- <span data-ttu-id="74a8f-160">мапистарттиме</span><span class="sxs-lookup"><span data-stu-id="74a8f-160">MapiStartTime</span></span>
    
- <span data-ttu-id="74a8f-161">мапипрстартдате</span><span class="sxs-lookup"><span data-stu-id="74a8f-161">MapiPRStartDate</span></span>
    
- <span data-ttu-id="74a8f-162">мапиендтиме</span><span class="sxs-lookup"><span data-stu-id="74a8f-162">MapiEndTime</span></span>
    
- <span data-ttu-id="74a8f-163">мапипренддате</span><span class="sxs-lookup"><span data-stu-id="74a8f-163">MapiPREndDate</span></span>
    
- <span data-ttu-id="74a8f-164">календаритемтипе</span><span class="sxs-lookup"><span data-stu-id="74a8f-164">CalendarItemType</span></span>
    
- <span data-ttu-id="74a8f-165">глобалобжектид</span><span class="sxs-lookup"><span data-stu-id="74a8f-165">GlobalObjectId</span></span>
    
- <span data-ttu-id="74a8f-166">тимезонедефинитионстарт</span><span class="sxs-lookup"><span data-stu-id="74a8f-166">TimeZoneDefinitionStart</span></span>
    
- <span data-ttu-id="74a8f-167">тимезонедефинитионенд</span><span class="sxs-lookup"><span data-stu-id="74a8f-167">TimeZoneDefinitionEnd</span></span>
    
### <a name="master-calendar-item-properties"></a><span data-ttu-id="74a8f-168">Свойства элемента главного календаря</span><span class="sxs-lookup"><span data-stu-id="74a8f-168">Master calendar item properties</span></span>
  
- <span data-ttu-id="74a8f-169">Код</span><span class="sxs-lookup"><span data-stu-id="74a8f-169">EntryId</span></span>
    
- <span data-ttu-id="74a8f-170">чанжекэй</span><span class="sxs-lookup"><span data-stu-id="74a8f-170">ChangeKey</span></span>
    
- <span data-ttu-id="74a8f-171">ItemClass</span><span class="sxs-lookup"><span data-stu-id="74a8f-171">ItemClass</span></span>
    
- <span data-ttu-id="74a8f-172">сентрепресентинжемаиладдресс</span><span class="sxs-lookup"><span data-stu-id="74a8f-172">SentRepresentingEmailAddress</span></span>
    
- <span data-ttu-id="74a8f-173">сентрепресентингдисплайнаме</span><span class="sxs-lookup"><span data-stu-id="74a8f-173">SentRepresentingDisplayName</span></span>
    
- <span data-ttu-id="74a8f-174">сентрепресентинжентрид</span><span class="sxs-lookup"><span data-stu-id="74a8f-174">SentRepresentingEntryId</span></span>
    
- <span data-ttu-id="74a8f-175">аппоинтментрекурренцеблоб</span><span class="sxs-lookup"><span data-stu-id="74a8f-175">AppointmentRecurrenceBlob</span></span>
    
- <span data-ttu-id="74a8f-176">TimeZone</span><span class="sxs-lookup"><span data-stu-id="74a8f-176">TimeZone</span></span>
    
- <span data-ttu-id="74a8f-177">тимезонеблоб</span><span class="sxs-lookup"><span data-stu-id="74a8f-177">TimeZoneBlob</span></span>
    
- <span data-ttu-id="74a8f-178">тимезонедефинитионрекурринг</span><span class="sxs-lookup"><span data-stu-id="74a8f-178">TimeZoneDefinitionRecurring</span></span>
    
- <span data-ttu-id="74a8f-179">клеанглобалобжектид</span><span class="sxs-lookup"><span data-stu-id="74a8f-179">CleanGlobalObjectId</span></span>
    
- <span data-ttu-id="74a8f-180">аппоинтментрекурринг</span><span class="sxs-lookup"><span data-stu-id="74a8f-180">AppointmentRecurring</span></span>
    
- <span data-ttu-id="74a8f-181">Исключение</span><span class="sxs-lookup"><span data-stu-id="74a8f-181">IsException</span></span>
    
- <span data-ttu-id="74a8f-182">IsRecurring</span><span class="sxs-lookup"><span data-stu-id="74a8f-182">IsRecurring</span></span>
    
- <span data-ttu-id="74a8f-183">маписенситивити</span><span class="sxs-lookup"><span data-stu-id="74a8f-183">MapiSensitivity</span></span>
    
- <span data-ttu-id="74a8f-184">контаинеркласс</span><span class="sxs-lookup"><span data-stu-id="74a8f-184">ContainerClass</span></span>
    
- <span data-ttu-id="74a8f-185">мапипрстартдате</span><span class="sxs-lookup"><span data-stu-id="74a8f-185">MapiPRStartDate</span></span>
    
- <span data-ttu-id="74a8f-186">мапипренддате</span><span class="sxs-lookup"><span data-stu-id="74a8f-186">MapiPREndDate</span></span>
    
- <span data-ttu-id="74a8f-187">Категории</span><span class="sxs-lookup"><span data-stu-id="74a8f-187">Categories</span></span>
    
<span data-ttu-id="74a8f-188">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="74a8f-188">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="example"></a><span data-ttu-id="74a8f-189">Пример</span><span class="sxs-lookup"><span data-stu-id="74a8f-189">Example</span></span>

<span data-ttu-id="74a8f-190">В приведенном ниже примере показан запрос FindItem.</span><span class="sxs-lookup"><span data-stu-id="74a8f-190">The following example shows a FindItem request.</span></span> <span data-ttu-id="74a8f-191">Успешный запрос возвращает ответ, включающий элементы календаря, запущенные в 2006 г. 05 – 18T00:00:00 – 08:00 или позже и заканчиваются до 2006 г. 05 – 19T00:00:00:00.</span><span class="sxs-lookup"><span data-stu-id="74a8f-191">A successful request returns a response that includes calendar items that started at 2006-05-18T00:00:00-08:00 or after and ended before 2006-05-19T00:00:00-08:00.</span></span>
  
```xml
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <FindItem Traversal="Shallow" xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <ItemShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:FieldURI FieldURI="calendar:Start"/>
          <t:FieldURI FieldURI="calendar:End"/>
          <t:FieldURI FieldURI="item:Subject"/>
        </t:AdditionalProperties>
      </ItemShape>
      <CalendarView MaxEntriesReturned="2" StartDate="2006-05-18T00:00:00-08:00" EndDate="2006-05-19T00:00:00-08:00"/>
      <ParentFolderIds>
        <t:DistinguishedFolderId Id="calendar"/>
      </ParentFolderIds>
    </FindItem>
  </soap:Body>
</soap:Envelope>
```

## <a name="element-information"></a><span data-ttu-id="74a8f-192">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="74a8f-192">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="74a8f-193">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="74a8f-193">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="74a8f-194">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="74a8f-194">Schema Name</span></span>  <br/> |<span data-ttu-id="74a8f-195">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="74a8f-195">Messages schema</span></span>  <br/> |
|<span data-ttu-id="74a8f-196">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="74a8f-196">Validation File</span></span>  <br/> |<span data-ttu-id="74a8f-197">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="74a8f-197">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="74a8f-198">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="74a8f-198">Can be Empty</span></span>  <br/> |<span data-ttu-id="74a8f-199">False</span><span class="sxs-lookup"><span data-stu-id="74a8f-199">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="74a8f-200">См. также</span><span class="sxs-lookup"><span data-stu-id="74a8f-200">See also</span></span>

- [<span data-ttu-id="74a8f-201">Операция FindItem</span><span class="sxs-lookup"><span data-stu-id="74a8f-201">FindItem operation</span></span>](finditem-operation.md)
- [<span data-ttu-id="74a8f-202">Поиск элементов</span><span class="sxs-lookup"><span data-stu-id="74a8f-202">Finding Items</span></span>](https://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)

