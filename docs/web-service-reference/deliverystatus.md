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
ms.openlocfilehash: ae32202284d3dd272f693fbb7b76070cb6019d28
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461403"
---
# <a name="deliverystatus"></a><span data-ttu-id="25347-103">деливеристатус</span><span class="sxs-lookup"><span data-stu-id="25347-103">DeliveryStatus</span></span>

<span data-ttu-id="25347-104">Элемент **деливеристатус** указывает состояние сообщения.</span><span class="sxs-lookup"><span data-stu-id="25347-104">The **DeliveryStatus** element specifies the status for a message.</span></span> 
  
```XML
<DeliveryStatus>Unsuccessful | Pending | Delivered | Transferred | Read</DeliveryStatus>
```

 <span data-ttu-id="25347-105">**мессажетраккингделиверистатустипе**</span><span class="sxs-lookup"><span data-stu-id="25347-105">**MessageTrackingDeliveryStatusType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="25347-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="25347-106">Attributes and elements</span></span>

<span data-ttu-id="25347-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="25347-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="25347-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="25347-108">Attributes</span></span>

<span data-ttu-id="25347-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="25347-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="25347-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="25347-110">Child elements</span></span>

<span data-ttu-id="25347-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="25347-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="25347-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="25347-112">Parent elements</span></span>

|<span data-ttu-id="25347-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="25347-113">**Element**</span></span>|<span data-ttu-id="25347-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="25347-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="25347-115">реЦипиенттраккинжевент</span><span class="sxs-lookup"><span data-stu-id="25347-115">RecipientTrackingEvent</span></span>](recipienttrackingevent.md) <br/> |<span data-ttu-id="25347-116">Содержит сведения об отдельном событии получателя.</span><span class="sxs-lookup"><span data-stu-id="25347-116">Contains information for a single event for a recipient.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="25347-117">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="25347-117">Text value</span></span>

<span data-ttu-id="25347-118">В следующей таблице приведены возможные текстовые значения для элемента **деливеристатус** .</span><span class="sxs-lookup"><span data-stu-id="25347-118">The following table lists the possible text values for the **DeliveryStatus** element.</span></span> 
  
<span data-ttu-id="25347-119">**Значения элементов Деливеристатус**</span><span class="sxs-lookup"><span data-stu-id="25347-119">**DeliveryStatus element values**</span></span>

|<span data-ttu-id="25347-120">**Значение**</span><span class="sxs-lookup"><span data-stu-id="25347-120">**Value**</span></span>|<span data-ttu-id="25347-121">**Описание**</span><span class="sxs-lookup"><span data-stu-id="25347-121">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="25347-122">Безуспешных</span><span class="sxs-lookup"><span data-stu-id="25347-122">Unsuccessful</span></span>  <br/> |<span data-ttu-id="25347-123">Указывает, что сообщение не было доставлено.</span><span class="sxs-lookup"><span data-stu-id="25347-123">Specifies that a message was not delivered.</span></span>  <br/> |
|<span data-ttu-id="25347-124">Pending</span><span class="sxs-lookup"><span data-stu-id="25347-124">Pending</span></span>  <br/> |<span data-ttu-id="25347-125">Указывает, что сообщение ожидает утверждения модератором.</span><span class="sxs-lookup"><span data-stu-id="25347-125">Specifies that the message is waiting for approval from a moderator.</span></span>  <br/> |
|<span data-ttu-id="25347-126">Отобран</span><span class="sxs-lookup"><span data-stu-id="25347-126">Delivered</span></span>  <br/> |<span data-ttu-id="25347-127">Указывает, что сообщение было доставлено всем указанным получателям.</span><span class="sxs-lookup"><span data-stu-id="25347-127">Specifies that the message was delivered to all of the specified recipients.</span></span>  <br/> |
|<span data-ttu-id="25347-128">Скопирован</span><span class="sxs-lookup"><span data-stu-id="25347-128">Transferred</span></span>  <br/> |<span data-ttu-id="25347-129">Указывает, что сообщение было передано на сервер за пределами области поиска.</span><span class="sxs-lookup"><span data-stu-id="25347-129">Specifies that the message was transferred to a server outside the search scope.</span></span>  <br/> |
|<span data-ttu-id="25347-130">Чтение</span><span class="sxs-lookup"><span data-stu-id="25347-130">Read</span></span>  <br/> |<span data-ttu-id="25347-131">Указывает, что сообщение было доставлено и Прочитано получателями.</span><span class="sxs-lookup"><span data-stu-id="25347-131">Specifies that the message was delivered and read by the recipients.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="25347-132">Примечания</span><span class="sxs-lookup"><span data-stu-id="25347-132">Remarks</span></span>

<span data-ttu-id="25347-133">Элемент **деливеристатус** имел тип **Мессажетраккингделиверистатустипе** в Exchange Server 2010.</span><span class="sxs-lookup"><span data-stu-id="25347-133">The **DeliveryStatus** element was of type **MessageTrackingDeliveryStatusType** in Exchange Server 2010.</span></span> 
  
<span data-ttu-id="25347-134">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="25347-134">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="25347-135">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="25347-135">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="25347-136">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="25347-136">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="25347-137">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="25347-137">Schema Name</span></span>  <br/> |<span data-ttu-id="25347-138">Схема Types</span><span class="sxs-lookup"><span data-stu-id="25347-138">Types schema</span></span>  <br/> |
|<span data-ttu-id="25347-139">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="25347-139">Validation File</span></span>  <br/> |<span data-ttu-id="25347-140">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="25347-140">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="25347-141">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="25347-141">Can be Empty</span></span>  <br/> |<span data-ttu-id="25347-142">False</span><span class="sxs-lookup"><span data-stu-id="25347-142">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="25347-143">См. также</span><span class="sxs-lookup"><span data-stu-id="25347-143">See also</span></span>

- [<span data-ttu-id="25347-144">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="25347-144">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

