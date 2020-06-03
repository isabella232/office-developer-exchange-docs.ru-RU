---
title: ексцептионфиелдури
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
description: Элемент Ексцептионфиелдури определяет определенные ошибки в запросе. Этот элемент используется только в ответ на сообщение об ошибке в узле Мессажексмл.
ms.openlocfilehash: a47d44098f85d8bacb1e7a2c48a33e478e56c7ac
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44454346"
---
# <a name="exceptionfielduri"></a><span data-ttu-id="97459-104">ексцептионфиелдури</span><span class="sxs-lookup"><span data-stu-id="97459-104">ExceptionFieldURI</span></span>

<span data-ttu-id="97459-105">Элемент **ексцептионфиелдури** определяет определенные ошибки в запросе.</span><span class="sxs-lookup"><span data-stu-id="97459-105">The **ExceptionFieldURI** element identifies particular errors in a request.</span></span> <span data-ttu-id="97459-106">Этот элемент используется только в ответ на сообщение об ошибке в узле [мессажексмл](messagexml.md) .</span><span class="sxs-lookup"><span data-stu-id="97459-106">This element is only used as part of an error response in the [MessageXml](messagexml.md) node.</span></span> 
  
```xml
<ExceptionFieldURI FieldURI="" />
```

 <span data-ttu-id="97459-107">**ексцептионпропертюритипе**</span><span class="sxs-lookup"><span data-stu-id="97459-107">**ExceptionPropertyURIType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="97459-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="97459-108">Attributes and elements</span></span>

<span data-ttu-id="97459-109">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="97459-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="97459-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="97459-110">Attributes</span></span>

|<span data-ttu-id="97459-111">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="97459-111">**Attribute**</span></span>|<span data-ttu-id="97459-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="97459-112">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="97459-113">**фиелдури**</span><span class="sxs-lookup"><span data-stu-id="97459-113">**FieldURI**</span></span> <br/> |<span data-ttu-id="97459-114">Определяет свойство вхождения повторяющегося элемента.</span><span class="sxs-lookup"><span data-stu-id="97459-114">Identifies a property of an occurrence of a recurring item.</span></span> <span data-ttu-id="97459-115">Этот атрибут является обязательным.</span><span class="sxs-lookup"><span data-stu-id="97459-115">This attribute is required.</span></span>  <br/> |
   
#### <a name="fielduri-attribute"></a><span data-ttu-id="97459-116">Атрибут Фиелдури</span><span class="sxs-lookup"><span data-stu-id="97459-116">FieldURI Attribute</span></span>

|<span data-ttu-id="97459-117">**Значение**</span><span class="sxs-lookup"><span data-stu-id="97459-117">**Value**</span></span>|<span data-ttu-id="97459-118">**Описание**</span><span class="sxs-lookup"><span data-stu-id="97459-118">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="97459-119">вложение: имя</span><span class="sxs-lookup"><span data-stu-id="97459-119">attachment:Name</span></span>  <br/> |<span data-ttu-id="97459-120">Определяет имя вложения, содержащее ошибку.</span><span class="sxs-lookup"><span data-stu-id="97459-120">Identifies the attachment name as containing an error.</span></span>  <br/> |
|<span data-ttu-id="97459-121">вложение: ContentType</span><span class="sxs-lookup"><span data-stu-id="97459-121">attachment:ContentType</span></span>  <br/> |<span data-ttu-id="97459-122">Определяет тип контента, который содержит ошибку.</span><span class="sxs-lookup"><span data-stu-id="97459-122">Identifies the content type as containing an error.</span></span>  <br/> |
|<span data-ttu-id="97459-123">вложение: контент</span><span class="sxs-lookup"><span data-stu-id="97459-123">attachment:Content</span></span>  <br/> |<span data-ttu-id="97459-124">Определяет содержимое, содержащее ошибку.</span><span class="sxs-lookup"><span data-stu-id="97459-124">Identifies the content as containing an error.</span></span>  <br/> |
|<span data-ttu-id="97459-125">повторение: месяц</span><span class="sxs-lookup"><span data-stu-id="97459-125">recurrence:Month</span></span>  <br/> |<span data-ttu-id="97459-126">Определяет поле месяца, содержащее ошибку.</span><span class="sxs-lookup"><span data-stu-id="97459-126">Identifies the month field as containing an error.</span></span>  <br/> |
|<span data-ttu-id="97459-127">повторение: Дайофвикиндекс</span><span class="sxs-lookup"><span data-stu-id="97459-127">recurrence:DayOfWeekIndex</span></span>  <br/> |<span data-ttu-id="97459-128">Указывает индекс дня недели, содержащий ошибку.</span><span class="sxs-lookup"><span data-stu-id="97459-128">Identifies the day of week index as containing an error.</span></span>  <br/> |
|<span data-ttu-id="97459-129">повторение: DaysOfWeek</span><span class="sxs-lookup"><span data-stu-id="97459-129">recurrence:DaysOfWeek</span></span>  <br/> |<span data-ttu-id="97459-130">Определяет свойство DaysOfWeek, содержащее ошибку.</span><span class="sxs-lookup"><span data-stu-id="97459-130">Identifies the DaysOfWeek property as containing an error.</span></span>  <br/> |
|<span data-ttu-id="97459-131">повторение: DayOfMonth</span><span class="sxs-lookup"><span data-stu-id="97459-131">recurrence:DayOfMonth</span></span>  <br/> |<span data-ttu-id="97459-132">Определяет DayOfMonth как содержащий ошибку.</span><span class="sxs-lookup"><span data-stu-id="97459-132">Identifies the DayOfMonth as containing an error.</span></span>  <br/> |
|<span data-ttu-id="97459-133">повторение: интервал</span><span class="sxs-lookup"><span data-stu-id="97459-133">recurrence:Interval</span></span>  <br/> |<span data-ttu-id="97459-134">Определяет интервал, содержащий ошибку.</span><span class="sxs-lookup"><span data-stu-id="97459-134">Identifies the interval as containing an error.</span></span>  <br/> |
|<span data-ttu-id="97459-135">повторение: Нумберофоккурренцес</span><span class="sxs-lookup"><span data-stu-id="97459-135">recurrence:NumberOfOccurrences</span></span>  <br/> |<span data-ttu-id="97459-136">Определяет количество вхождений, содержащих ошибку.</span><span class="sxs-lookup"><span data-stu-id="97459-136">Identifies the number of occurrences as containing an error.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="97459-137">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="97459-137">Child elements</span></span>

<span data-ttu-id="97459-138">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="97459-138">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="97459-139">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="97459-139">Parent elements</span></span>

|<span data-ttu-id="97459-140">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="97459-140">**Element**</span></span>|<span data-ttu-id="97459-141">**Описание**</span><span class="sxs-lookup"><span data-stu-id="97459-141">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="97459-142">мессажексмл</span><span class="sxs-lookup"><span data-stu-id="97459-142">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="97459-143">Предоставляет дополнительные сведения об ошибке.</span><span class="sxs-lookup"><span data-stu-id="97459-143">Provides additional error response information.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="97459-144">Примечания</span><span class="sxs-lookup"><span data-stu-id="97459-144">Remarks</span></span>

<span data-ttu-id="97459-145">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="97459-145">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="97459-146">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="97459-146">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="97459-147">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="97459-147">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="97459-148">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="97459-148">Schema Name</span></span>  <br/> |<span data-ttu-id="97459-149">Схема Types</span><span class="sxs-lookup"><span data-stu-id="97459-149">Types schema</span></span>  <br/> |
|<span data-ttu-id="97459-150">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="97459-150">Validation File</span></span>  <br/> |<span data-ttu-id="97459-151">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="97459-151">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="97459-152">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="97459-152">Can be Empty</span></span>  <br/> |<span data-ttu-id="97459-153">False</span><span class="sxs-lookup"><span data-stu-id="97459-153">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="97459-154">См. также</span><span class="sxs-lookup"><span data-stu-id="97459-154">See also</span></span>



- [<span data-ttu-id="97459-155">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="97459-155">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

