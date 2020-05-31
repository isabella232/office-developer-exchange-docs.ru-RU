---
title: реЦипиенттраккинжевентс
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RecipientTrackingEvents
api_type:
- schema
ms.assetid: c4f729aa-674e-43b2-97f2-bf49740b0a34
description: Элемент РеЦипиенттраккинжевентс представляет коллекцию из одного или нескольких событий для сообщения.
ms.openlocfilehash: 5fa5df422eff533891d021b77d5443b314d36244
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834993"
---
# <a name="recipienttrackingevents"></a><span data-ttu-id="2d7bd-103">реЦипиенттраккинжевентс</span><span class="sxs-lookup"><span data-stu-id="2d7bd-103">RecipientTrackingEvents</span></span>

<span data-ttu-id="2d7bd-104">Элемент **реЦипиенттраккинжевентс** представляет коллекцию из одного или нескольких событий для сообщения.</span><span class="sxs-lookup"><span data-stu-id="2d7bd-104">The **RecipientTrackingEvents** element represents a collection of one or more events for a message.</span></span> 
  
```XML
<RecipientTrackingEvents>
   <RecipientTrackingEvent/>
</RecipientTrackingEvents>
```

 <span data-ttu-id="2d7bd-105">**аррайофреЦипиенттраккинжевенттипе**</span><span class="sxs-lookup"><span data-stu-id="2d7bd-105">**ArrayOfRecipientTrackingEventType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2d7bd-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="2d7bd-106">Attributes and elements</span></span>

<span data-ttu-id="2d7bd-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="2d7bd-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2d7bd-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="2d7bd-108">Attributes</span></span>

<span data-ttu-id="2d7bd-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="2d7bd-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2d7bd-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="2d7bd-110">Child elements</span></span>

|<span data-ttu-id="2d7bd-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="2d7bd-111">**Element**</span></span>|<span data-ttu-id="2d7bd-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="2d7bd-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2d7bd-113">реЦипиенттраккинжевент</span><span class="sxs-lookup"><span data-stu-id="2d7bd-113">RecipientTrackingEvent</span></span>](recipienttrackingevent.md) <br/> |<span data-ttu-id="2d7bd-114">Содержит сведения об определенном событии в отчете об отслеживании.</span><span class="sxs-lookup"><span data-stu-id="2d7bd-114">Contains details for a specific event in the tracking report.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="2d7bd-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="2d7bd-115">Parent elements</span></span>

|<span data-ttu-id="2d7bd-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="2d7bd-116">**Element**</span></span>|<span data-ttu-id="2d7bd-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="2d7bd-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2d7bd-118">MessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="2d7bd-118">MessageTrackingReport</span></span>](messagetrackingreport.md) <br/> |<span data-ttu-id="2d7bd-119">Содержит одно сообщение, которое возвращается в [Операция GetMessageTrackingReport](getmessagetrackingreport-operation.md).</span><span class="sxs-lookup"><span data-stu-id="2d7bd-119">Contains a single message that is returned in a [GetMessageTrackingReport operation](getmessagetrackingreport-operation.md).</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="2d7bd-120">Примечания</span><span class="sxs-lookup"><span data-stu-id="2d7bd-120">Remarks</span></span>

<span data-ttu-id="2d7bd-121">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="2d7bd-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2d7bd-122">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="2d7bd-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2d7bd-123">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="2d7bd-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="2d7bd-124">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="2d7bd-124">Schema Name</span></span>  <br/> |<span data-ttu-id="2d7bd-125">Схема Types</span><span class="sxs-lookup"><span data-stu-id="2d7bd-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="2d7bd-126">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="2d7bd-126">Validation File</span></span>  <br/> |<span data-ttu-id="2d7bd-127">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="2d7bd-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="2d7bd-128">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="2d7bd-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="2d7bd-129">False</span><span class="sxs-lookup"><span data-stu-id="2d7bd-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="2d7bd-130">См. также</span><span class="sxs-lookup"><span data-stu-id="2d7bd-130">See also</span></span>



[<span data-ttu-id="2d7bd-131">Операция GetMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="2d7bd-131">GetMessageTrackingReport operation</span></span>](getmessagetrackingreport-operation.md)


- [<span data-ttu-id="2d7bd-132">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="2d7bd-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

