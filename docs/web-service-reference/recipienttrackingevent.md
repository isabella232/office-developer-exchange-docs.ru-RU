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
ms.openlocfilehash: e9a014cdfac122f112205cfa5032535a770f9d82
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465487"
---
# <a name="recipienttrackingevent"></a><span data-ttu-id="8276f-103">реЦипиенттраккинжевент</span><span class="sxs-lookup"><span data-stu-id="8276f-103">RecipientTrackingEvent</span></span>

<span data-ttu-id="8276f-104">Элемент **реЦипиенттраккинжевент** содержит сведения об отдельном событии получателя.</span><span class="sxs-lookup"><span data-stu-id="8276f-104">The **RecipientTrackingEvent** element contains information for a single event for a recipient.</span></span> 
  
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

 <span data-ttu-id="8276f-105">**реЦипиенттраккинжевенттипе**</span><span class="sxs-lookup"><span data-stu-id="8276f-105">**RecipientTrackingEventType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="8276f-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="8276f-106">Attributes and elements</span></span>

<span data-ttu-id="8276f-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="8276f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8276f-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="8276f-108">Attributes</span></span>

<span data-ttu-id="8276f-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="8276f-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8276f-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="8276f-110">Child elements</span></span>

|<span data-ttu-id="8276f-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="8276f-111">**Element**</span></span>|<span data-ttu-id="8276f-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="8276f-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8276f-113">Дата (MessageTracking)</span><span class="sxs-lookup"><span data-stu-id="8276f-113">Date (MessageTracking)</span></span>](date-messagetracking.md) <br/> |<span data-ttu-id="8276f-114">Этот элемент обязательный.</span><span class="sxs-lookup"><span data-stu-id="8276f-114">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="8276f-115">Получатель</span><span class="sxs-lookup"><span data-stu-id="8276f-115">Recipient</span></span>](recipient.md) <br/> |<span data-ttu-id="8276f-116">Этот элемент обязательный.</span><span class="sxs-lookup"><span data-stu-id="8276f-116">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="8276f-117">деливеристатус</span><span class="sxs-lookup"><span data-stu-id="8276f-117">DeliveryStatus</span></span>](deliverystatus.md) <br/> |<span data-ttu-id="8276f-118">Этот элемент обязательный.</span><span class="sxs-lookup"><span data-stu-id="8276f-118">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="8276f-119">евентдескриптион</span><span class="sxs-lookup"><span data-stu-id="8276f-119">EventDescription</span></span>](eventdescription.md) <br/> |<span data-ttu-id="8276f-120">Этот элемент обязательный.</span><span class="sxs-lookup"><span data-stu-id="8276f-120">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="8276f-121">EventData</span><span class="sxs-lookup"><span data-stu-id="8276f-121">EventData</span></span>](eventdata.md) <br/> |<span data-ttu-id="8276f-122">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="8276f-122">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="8276f-123">Сервер (MessageTracking)</span><span class="sxs-lookup"><span data-stu-id="8276f-123">Server (MessageTracking)</span></span>](server-messagetracking.md) <br/> |<span data-ttu-id="8276f-124">Этот элемент обязательный.</span><span class="sxs-lookup"><span data-stu-id="8276f-124">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="8276f-125">интерналид</span><span class="sxs-lookup"><span data-stu-id="8276f-125">InternalId</span></span>](internalid.md) <br/> |<span data-ttu-id="8276f-126">Этот элемент обязательный.</span><span class="sxs-lookup"><span data-stu-id="8276f-126">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="8276f-127">бккреЦипиент</span><span class="sxs-lookup"><span data-stu-id="8276f-127">BccRecipient</span></span>](bccrecipient.md) <br/> |<span data-ttu-id="8276f-128">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="8276f-128">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="8276f-129">хидденреЦипиент</span><span class="sxs-lookup"><span data-stu-id="8276f-129">HiddenRecipient</span></span>](hiddenrecipient.md) <br/> |<span data-ttu-id="8276f-130">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="8276f-130">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="8276f-131">уникуепасид</span><span class="sxs-lookup"><span data-stu-id="8276f-131">UniquePathId</span></span>](uniquepathid.md) <br/> |<span data-ttu-id="8276f-132">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="8276f-132">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="8276f-133">рутаддресс</span><span class="sxs-lookup"><span data-stu-id="8276f-133">RootAddress</span></span>](rootaddress.md) <br/> |<span data-ttu-id="8276f-134">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="8276f-134">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="8276f-135">Свойства (Аррайофтраккингпропертиестипе)</span><span class="sxs-lookup"><span data-stu-id="8276f-135">Properties (ArrayOfTrackingPropertiesType)</span></span>](properties-arrayoftrackingpropertiestype.md) <br/> |<span data-ttu-id="8276f-136">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="8276f-136">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="8276f-137">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="8276f-137">Parent elements</span></span>

|<span data-ttu-id="8276f-138">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="8276f-138">**Element**</span></span>|<span data-ttu-id="8276f-139">**Описание**</span><span class="sxs-lookup"><span data-stu-id="8276f-139">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8276f-140">реЦипиенттраккинжевентс</span><span class="sxs-lookup"><span data-stu-id="8276f-140">RecipientTrackingEvents</span></span>](recipienttrackingevents.md) <br/> |<span data-ttu-id="8276f-141">Содержит список одного или нескольких событий отслеживания для получателя.</span><span class="sxs-lookup"><span data-stu-id="8276f-141">Contains a list of one or more tracking events for a recipient.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="8276f-142">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="8276f-142">Text value</span></span>

<span data-ttu-id="8276f-143">Нет.</span><span class="sxs-lookup"><span data-stu-id="8276f-143">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="8276f-144">Примечания</span><span class="sxs-lookup"><span data-stu-id="8276f-144">Remarks</span></span>

<span data-ttu-id="8276f-145">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="8276f-145">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="8276f-146">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="8276f-146">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8276f-147">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="8276f-147">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="8276f-148">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="8276f-148">Schema Name</span></span>  <br/> |<span data-ttu-id="8276f-149">Схема Types</span><span class="sxs-lookup"><span data-stu-id="8276f-149">Types schema</span></span>  <br/> |
|<span data-ttu-id="8276f-150">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="8276f-150">Validation File</span></span>  <br/> |<span data-ttu-id="8276f-151">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="8276f-151">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="8276f-152">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="8276f-152">Can be Empty</span></span>  <br/> |<span data-ttu-id="8276f-153">False</span><span class="sxs-lookup"><span data-stu-id="8276f-153">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="8276f-154">См. также</span><span class="sxs-lookup"><span data-stu-id="8276f-154">See also</span></span>



[<span data-ttu-id="8276f-155">Операция GetMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="8276f-155">GetMessageTrackingReport operation</span></span>](getmessagetrackingreport-operation.md)


- [<span data-ttu-id="8276f-156">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="8276f-156">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

