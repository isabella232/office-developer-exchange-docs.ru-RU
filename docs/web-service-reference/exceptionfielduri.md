---
title: ExceptionFieldURI
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ExceptionFieldURI
api_type:
- schema
ms.assetid: 7afda93a-0f8c-4c9e-8e09-f1b0bfc928bf
description: Элемент ExceptionFieldURI идентифицирует определенные ошибки в запросе. Этот элемент используется только как часть ответа об ошибке в узле MessageXml.
ms.openlocfilehash: 79909405179cec0d0b86ad12bf52031e1daeb790
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762408"
---
# <a name="exceptionfielduri"></a><span data-ttu-id="71e37-104">ExceptionFieldURI</span><span class="sxs-lookup"><span data-stu-id="71e37-104">ExceptionFieldURI</span></span>

<span data-ttu-id="71e37-105">Элемент **ExceptionFieldURI** идентифицирует определенные ошибки в запросе.</span><span class="sxs-lookup"><span data-stu-id="71e37-105">The **ExceptionFieldURI** element identifies particular errors in a request.</span></span> <span data-ttu-id="71e37-106">Этот элемент используется только как часть ответа об ошибке в узле [MessageXml](messagexml.md) .</span><span class="sxs-lookup"><span data-stu-id="71e37-106">This element is only used as part of an error response in the [MessageXml](messagexml.md) node.</span></span> 
  
```xml
<ExceptionFieldURI FieldURI="" />
```

 <span data-ttu-id="71e37-107">**ExceptionPropertyURIType**</span><span class="sxs-lookup"><span data-stu-id="71e37-107">**ExceptionPropertyURIType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="71e37-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="71e37-108">Attributes and elements</span></span>

<span data-ttu-id="71e37-109">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="71e37-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="71e37-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="71e37-110">Attributes</span></span>

|<span data-ttu-id="71e37-111">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="71e37-111">**Attribute**</span></span>|<span data-ttu-id="71e37-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="71e37-112">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="71e37-113">**FieldURI**</span><span class="sxs-lookup"><span data-stu-id="71e37-113">**FieldURI**</span></span> <br/> |<span data-ttu-id="71e37-114">Определяет свойство вхождения повторяющегося элемента.</span><span class="sxs-lookup"><span data-stu-id="71e37-114">Identifies a property of an occurrence of a recurring item.</span></span> <span data-ttu-id="71e37-115">Этот атрибут является обязательным.</span><span class="sxs-lookup"><span data-stu-id="71e37-115">This attribute is required.</span></span>  <br/> |
   
#### <a name="fielduri-attribute"></a><span data-ttu-id="71e37-116">Атрибут FieldURI</span><span class="sxs-lookup"><span data-stu-id="71e37-116">FieldURI Attribute</span></span>

|<span data-ttu-id="71e37-117">**Значение**</span><span class="sxs-lookup"><span data-stu-id="71e37-117">**Value**</span></span>|<span data-ttu-id="71e37-118">**Описание**</span><span class="sxs-lookup"><span data-stu-id="71e37-118">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="71e37-119">Имя: вложения</span><span class="sxs-lookup"><span data-stu-id="71e37-119">attachment:Name</span></span>  <br/> |<span data-ttu-id="71e37-120">Определяет имя вложения, содержащий ошибку.</span><span class="sxs-lookup"><span data-stu-id="71e37-120">Identifies the attachment name as containing an error.</span></span>  <br/> |
|<span data-ttu-id="71e37-121">вложения: ContentType</span><span class="sxs-lookup"><span data-stu-id="71e37-121">attachment:ContentType</span></span>  <br/> |<span data-ttu-id="71e37-122">Идентифицирует тип контента как содержащий ошибки.</span><span class="sxs-lookup"><span data-stu-id="71e37-122">Identifies the content type as containing an error.</span></span>  <br/> |
|<span data-ttu-id="71e37-123">Содержимое вложения:</span><span class="sxs-lookup"><span data-stu-id="71e37-123">attachment:Content</span></span>  <br/> |<span data-ttu-id="71e37-124">Задает содержимое, как содержащий ошибки.</span><span class="sxs-lookup"><span data-stu-id="71e37-124">Identifies the content as containing an error.</span></span>  <br/> |
|<span data-ttu-id="71e37-125">Повторение: месяц</span><span class="sxs-lookup"><span data-stu-id="71e37-125">recurrence:Month</span></span>  <br/> |<span data-ttu-id="71e37-126">Определяет поле месяц как содержащий ошибки.</span><span class="sxs-lookup"><span data-stu-id="71e37-126">Identifies the month field as containing an error.</span></span>  <br/> |
|<span data-ttu-id="71e37-127">Повторение: DayOfWeekIndex</span><span class="sxs-lookup"><span data-stu-id="71e37-127">recurrence:DayOfWeekIndex</span></span>  <br/> |<span data-ttu-id="71e37-128">Определяет день недели индекса, содержащее ошибку.</span><span class="sxs-lookup"><span data-stu-id="71e37-128">Identifies the day of week index as containing an error.</span></span>  <br/> |
|<span data-ttu-id="71e37-129">Повторение: DaysOfWeek</span><span class="sxs-lookup"><span data-stu-id="71e37-129">recurrence:DaysOfWeek</span></span>  <br/> |<span data-ttu-id="71e37-130">Определяет свойство DaysOfWeek как содержащий ошибки.</span><span class="sxs-lookup"><span data-stu-id="71e37-130">Identifies the DaysOfWeek property as containing an error.</span></span>  <br/> |
|<span data-ttu-id="71e37-131">Повторение: день месяца</span><span class="sxs-lookup"><span data-stu-id="71e37-131">recurrence:DayOfMonth</span></span>  <br/> |<span data-ttu-id="71e37-132">Определяет день месяца, содержащее ошибку.</span><span class="sxs-lookup"><span data-stu-id="71e37-132">Identifies the DayOfMonth as containing an error.</span></span>  <br/> |
|<span data-ttu-id="71e37-133">Интервал повторения:</span><span class="sxs-lookup"><span data-stu-id="71e37-133">recurrence:Interval</span></span>  <br/> |<span data-ttu-id="71e37-134">Задает интервал, содержащее ошибку.</span><span class="sxs-lookup"><span data-stu-id="71e37-134">Identifies the interval as containing an error.</span></span>  <br/> |
|<span data-ttu-id="71e37-135">Повторение: NumberOfOccurrences</span><span class="sxs-lookup"><span data-stu-id="71e37-135">recurrence:NumberOfOccurrences</span></span>  <br/> |<span data-ttu-id="71e37-136">Определяет число вхождений как содержащий ошибки.</span><span class="sxs-lookup"><span data-stu-id="71e37-136">Identifies the number of occurrences as containing an error.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="71e37-137">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="71e37-137">Child elements</span></span>

<span data-ttu-id="71e37-138">Нет.</span><span class="sxs-lookup"><span data-stu-id="71e37-138">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="71e37-139">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="71e37-139">Parent elements</span></span>

|<span data-ttu-id="71e37-140">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="71e37-140">**Element**</span></span>|<span data-ttu-id="71e37-141">**Описание**</span><span class="sxs-lookup"><span data-stu-id="71e37-141">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="71e37-142">MessageXml</span><span class="sxs-lookup"><span data-stu-id="71e37-142">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="71e37-143">Предоставляет дополнительные сведения об ошибке ответа.</span><span class="sxs-lookup"><span data-stu-id="71e37-143">Provides additional error response information.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="71e37-144">Замечания</span><span class="sxs-lookup"><span data-stu-id="71e37-144">Remarks</span></span>

<span data-ttu-id="71e37-145">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="71e37-145">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="71e37-146">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="71e37-146">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="71e37-147">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="71e37-147">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="71e37-148">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="71e37-148">Schema Name</span></span>  <br/> |<span data-ttu-id="71e37-149">Схема Types</span><span class="sxs-lookup"><span data-stu-id="71e37-149">Types schema</span></span>  <br/> |
|<span data-ttu-id="71e37-150">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="71e37-150">Validation File</span></span>  <br/> |<span data-ttu-id="71e37-151">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="71e37-151">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="71e37-152">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="71e37-152">Can be Empty</span></span>  <br/> |<span data-ttu-id="71e37-153">False</span><span class="sxs-lookup"><span data-stu-id="71e37-153">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="71e37-154">См. также</span><span class="sxs-lookup"><span data-stu-id="71e37-154">See also</span></span>



- [<span data-ttu-id="71e37-155">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="71e37-155">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

