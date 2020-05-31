---
title: реЦипиенттраккинжевент
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RecipientTrackingEvent
api_type:
- schema
ms.assetid: 2bffdac7-c2f5-4805-ae7e-bd865301acb6
description: Элемент РеЦипиенттраккинжевент содержит сведения об отдельном событии получателя.
ms.openlocfilehash: c5488ba105f9a853a490d6f0f4ff9ff15b537e23
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834989"
---
# <a name="recipienttrackingevent"></a><span data-ttu-id="000fb-103">реЦипиенттраккинжевент</span><span class="sxs-lookup"><span data-stu-id="000fb-103">RecipientTrackingEvent</span></span>

<span data-ttu-id="000fb-104">Элемент **реЦипиенттраккинжевент** содержит сведения об отдельном событии получателя.</span><span class="sxs-lookup"><span data-stu-id="000fb-104">The **RecipientTrackingEvent** element contains information for a single event for a recipient.</span></span> 
  
```XML
<RecipientTrackingEvent>
   <Date/>
   <Recipient/>
   <DeliveryStatus/>
   <EventDescription/>
   <EventData/>
   <Server/>
   <InternalId/>
   <BccRecipient/>
   <HiddenRecipient/>
   <UniquePathId/>
   <RootAddress/>
   <Properties/>
</RecipientTrackingEvent>
```

 <span data-ttu-id="000fb-105">**реЦипиенттраккинжевенттипе**</span><span class="sxs-lookup"><span data-stu-id="000fb-105">**RecipientTrackingEventType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="000fb-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="000fb-106">Attributes and elements</span></span>

<span data-ttu-id="000fb-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="000fb-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="000fb-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="000fb-108">Attributes</span></span>

<span data-ttu-id="000fb-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="000fb-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="000fb-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="000fb-110">Child elements</span></span>

|<span data-ttu-id="000fb-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="000fb-111">**Element**</span></span>|<span data-ttu-id="000fb-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="000fb-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="000fb-113">Дата (MessageTracking)</span><span class="sxs-lookup"><span data-stu-id="000fb-113">Date (MessageTracking)</span></span>](date-messagetracking.md) <br/> |<span data-ttu-id="000fb-114">Этот элемент обязательный.</span><span class="sxs-lookup"><span data-stu-id="000fb-114">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="000fb-115">Получатель</span><span class="sxs-lookup"><span data-stu-id="000fb-115">Recipient</span></span>](recipient.md) <br/> |<span data-ttu-id="000fb-116">Этот элемент обязательный.</span><span class="sxs-lookup"><span data-stu-id="000fb-116">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="000fb-117">деливеристатус</span><span class="sxs-lookup"><span data-stu-id="000fb-117">DeliveryStatus</span></span>](deliverystatus.md) <br/> |<span data-ttu-id="000fb-118">Этот элемент обязательный.</span><span class="sxs-lookup"><span data-stu-id="000fb-118">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="000fb-119">евентдескриптион</span><span class="sxs-lookup"><span data-stu-id="000fb-119">EventDescription</span></span>](eventdescription.md) <br/> |<span data-ttu-id="000fb-120">Этот элемент обязательный.</span><span class="sxs-lookup"><span data-stu-id="000fb-120">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="000fb-121">EventData</span><span class="sxs-lookup"><span data-stu-id="000fb-121">EventData</span></span>](eventdata.md) <br/> |<span data-ttu-id="000fb-122">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="000fb-122">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="000fb-123">Сервер (MessageTracking)</span><span class="sxs-lookup"><span data-stu-id="000fb-123">Server (MessageTracking)</span></span>](server-messagetracking.md) <br/> |<span data-ttu-id="000fb-124">Этот элемент обязательный.</span><span class="sxs-lookup"><span data-stu-id="000fb-124">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="000fb-125">интерналид</span><span class="sxs-lookup"><span data-stu-id="000fb-125">InternalId</span></span>](internalid.md) <br/> |<span data-ttu-id="000fb-126">Этот элемент обязательный.</span><span class="sxs-lookup"><span data-stu-id="000fb-126">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="000fb-127">бккреЦипиент</span><span class="sxs-lookup"><span data-stu-id="000fb-127">BccRecipient</span></span>](bccrecipient.md) <br/> |<span data-ttu-id="000fb-128">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="000fb-128">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="000fb-129">хидденреЦипиент</span><span class="sxs-lookup"><span data-stu-id="000fb-129">HiddenRecipient</span></span>](hiddenrecipient.md) <br/> |<span data-ttu-id="000fb-130">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="000fb-130">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="000fb-131">уникуепасид</span><span class="sxs-lookup"><span data-stu-id="000fb-131">UniquePathId</span></span>](uniquepathid.md) <br/> |<span data-ttu-id="000fb-132">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="000fb-132">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="000fb-133">рутаддресс</span><span class="sxs-lookup"><span data-stu-id="000fb-133">RootAddress</span></span>](rootaddress.md) <br/> |<span data-ttu-id="000fb-134">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="000fb-134">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="000fb-135">Свойства (Аррайофтраккингпропертиестипе)</span><span class="sxs-lookup"><span data-stu-id="000fb-135">Properties (ArrayOfTrackingPropertiesType)</span></span>](properties-arrayoftrackingpropertiestype.md) <br/> |<span data-ttu-id="000fb-136">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="000fb-136">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="000fb-137">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="000fb-137">Parent elements</span></span>

|<span data-ttu-id="000fb-138">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="000fb-138">**Element**</span></span>|<span data-ttu-id="000fb-139">**Описание**</span><span class="sxs-lookup"><span data-stu-id="000fb-139">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="000fb-140">реЦипиенттраккинжевентс</span><span class="sxs-lookup"><span data-stu-id="000fb-140">RecipientTrackingEvents</span></span>](recipienttrackingevents.md) <br/> |<span data-ttu-id="000fb-141">Содержит список одного или нескольких событий отслеживания для получателя.</span><span class="sxs-lookup"><span data-stu-id="000fb-141">Contains a list of one or more tracking events for a recipient.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="000fb-142">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="000fb-142">Text value</span></span>

<span data-ttu-id="000fb-143">Нет.</span><span class="sxs-lookup"><span data-stu-id="000fb-143">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="000fb-144">Примечания</span><span class="sxs-lookup"><span data-stu-id="000fb-144">Remarks</span></span>

<span data-ttu-id="000fb-145">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="000fb-145">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="000fb-146">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="000fb-146">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="000fb-147">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="000fb-147">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="000fb-148">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="000fb-148">Schema Name</span></span>  <br/> |<span data-ttu-id="000fb-149">Схема Types</span><span class="sxs-lookup"><span data-stu-id="000fb-149">Types schema</span></span>  <br/> |
|<span data-ttu-id="000fb-150">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="000fb-150">Validation File</span></span>  <br/> |<span data-ttu-id="000fb-151">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="000fb-151">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="000fb-152">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="000fb-152">Can be Empty</span></span>  <br/> |<span data-ttu-id="000fb-153">False</span><span class="sxs-lookup"><span data-stu-id="000fb-153">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="000fb-154">См. также</span><span class="sxs-lookup"><span data-stu-id="000fb-154">See also</span></span>



[<span data-ttu-id="000fb-155">Операция GetMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="000fb-155">GetMessageTrackingReport operation</span></span>](getmessagetrackingreport-operation.md)


- [<span data-ttu-id="000fb-156">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="000fb-156">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

