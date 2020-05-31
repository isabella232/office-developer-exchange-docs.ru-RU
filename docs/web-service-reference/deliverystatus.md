---
title: деливеристатус
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DeliveryStatus
api_type:
- schema
ms.assetid: eab55db3-affb-42be-a586-5caa04052433
description: Элемент Деливеристатус указывает состояние сообщения.
ms.openlocfilehash: 4e6f31e8ef4f98d8e838ba91167c7dd5d6ab2590
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762064"
---
# <a name="deliverystatus"></a><span data-ttu-id="dbc5a-103">деливеристатус</span><span class="sxs-lookup"><span data-stu-id="dbc5a-103">DeliveryStatus</span></span>

<span data-ttu-id="dbc5a-104">Элемент **деливеристатус** указывает состояние сообщения.</span><span class="sxs-lookup"><span data-stu-id="dbc5a-104">The **DeliveryStatus** element specifies the status for a message.</span></span> 
  
```XML
<DeliveryStatus>Unsuccessful | Pending | Delivered | Transferred | Read</DeliveryStatus>
```

 <span data-ttu-id="dbc5a-105">**мессажетраккингделиверистатустипе**</span><span class="sxs-lookup"><span data-stu-id="dbc5a-105">**MessageTrackingDeliveryStatusType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="dbc5a-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="dbc5a-106">Attributes and elements</span></span>

<span data-ttu-id="dbc5a-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="dbc5a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="dbc5a-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="dbc5a-108">Attributes</span></span>

<span data-ttu-id="dbc5a-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="dbc5a-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="dbc5a-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="dbc5a-110">Child elements</span></span>

<span data-ttu-id="dbc5a-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="dbc5a-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="dbc5a-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="dbc5a-112">Parent elements</span></span>

|<span data-ttu-id="dbc5a-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="dbc5a-113">**Element**</span></span>|<span data-ttu-id="dbc5a-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="dbc5a-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="dbc5a-115">реЦипиенттраккинжевент</span><span class="sxs-lookup"><span data-stu-id="dbc5a-115">RecipientTrackingEvent</span></span>](recipienttrackingevent.md) <br/> |<span data-ttu-id="dbc5a-116">Содержит сведения об отдельном событии получателя.</span><span class="sxs-lookup"><span data-stu-id="dbc5a-116">Contains information for a single event for a recipient.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="dbc5a-117">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="dbc5a-117">Text value</span></span>

<span data-ttu-id="dbc5a-118">В следующей таблице приведены возможные текстовые значения для элемента **деливеристатус** .</span><span class="sxs-lookup"><span data-stu-id="dbc5a-118">The following table lists the possible text values for the **DeliveryStatus** element.</span></span> 
  
<span data-ttu-id="dbc5a-119">**Значения элементов Деливеристатус**</span><span class="sxs-lookup"><span data-stu-id="dbc5a-119">**DeliveryStatus element values**</span></span>

|<span data-ttu-id="dbc5a-120">**Значение**</span><span class="sxs-lookup"><span data-stu-id="dbc5a-120">**Value**</span></span>|<span data-ttu-id="dbc5a-121">**Описание**</span><span class="sxs-lookup"><span data-stu-id="dbc5a-121">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="dbc5a-122">Безуспешных</span><span class="sxs-lookup"><span data-stu-id="dbc5a-122">Unsuccessful</span></span>  <br/> |<span data-ttu-id="dbc5a-123">Указывает, что сообщение не было доставлено.</span><span class="sxs-lookup"><span data-stu-id="dbc5a-123">Specifies that a message was not delivered.</span></span>  <br/> |
|<span data-ttu-id="dbc5a-124">Pending</span><span class="sxs-lookup"><span data-stu-id="dbc5a-124">Pending</span></span>  <br/> |<span data-ttu-id="dbc5a-125">Указывает, что сообщение ожидает утверждения модератором.</span><span class="sxs-lookup"><span data-stu-id="dbc5a-125">Specifies that the message is waiting for approval from a moderator.</span></span>  <br/> |
|<span data-ttu-id="dbc5a-126">Отобран</span><span class="sxs-lookup"><span data-stu-id="dbc5a-126">Delivered</span></span>  <br/> |<span data-ttu-id="dbc5a-127">Указывает, что сообщение было доставлено всем указанным получателям.</span><span class="sxs-lookup"><span data-stu-id="dbc5a-127">Specifies that the message was delivered to all of the specified recipients.</span></span>  <br/> |
|<span data-ttu-id="dbc5a-128">Скопирован</span><span class="sxs-lookup"><span data-stu-id="dbc5a-128">Transferred</span></span>  <br/> |<span data-ttu-id="dbc5a-129">Указывает, что сообщение было передано на сервер за пределами области поиска.</span><span class="sxs-lookup"><span data-stu-id="dbc5a-129">Specifies that the message was transferred to a server outside the search scope.</span></span>  <br/> |
|<span data-ttu-id="dbc5a-130">Чтение</span><span class="sxs-lookup"><span data-stu-id="dbc5a-130">Read</span></span>  <br/> |<span data-ttu-id="dbc5a-131">Указывает, что сообщение было доставлено и Прочитано получателями.</span><span class="sxs-lookup"><span data-stu-id="dbc5a-131">Specifies that the message was delivered and read by the recipients.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="dbc5a-132">Примечания</span><span class="sxs-lookup"><span data-stu-id="dbc5a-132">Remarks</span></span>

<span data-ttu-id="dbc5a-133">Элемент **деливеристатус** имел тип **Мессажетраккингделиверистатустипе** в Exchange Server 2010.</span><span class="sxs-lookup"><span data-stu-id="dbc5a-133">The **DeliveryStatus** element was of type **MessageTrackingDeliveryStatusType** in Exchange Server 2010.</span></span> 
  
<span data-ttu-id="dbc5a-134">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="dbc5a-134">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="dbc5a-135">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="dbc5a-135">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="dbc5a-136">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="dbc5a-136">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="dbc5a-137">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="dbc5a-137">Schema Name</span></span>  <br/> |<span data-ttu-id="dbc5a-138">Схема Types</span><span class="sxs-lookup"><span data-stu-id="dbc5a-138">Types schema</span></span>  <br/> |
|<span data-ttu-id="dbc5a-139">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="dbc5a-139">Validation File</span></span>  <br/> |<span data-ttu-id="dbc5a-140">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="dbc5a-140">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="dbc5a-141">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="dbc5a-141">Can be Empty</span></span>  <br/> |<span data-ttu-id="dbc5a-142">False</span><span class="sxs-lookup"><span data-stu-id="dbc5a-142">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="dbc5a-143">См. также</span><span class="sxs-lookup"><span data-stu-id="dbc5a-143">See also</span></span>

- [<span data-ttu-id="dbc5a-144">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="dbc5a-144">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

