---
title: GetStreamingEvents
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetStreamingEvents
api_type:
- schema
ms.assetid: dbe83857-c4f8-4d98-813f-e03c289697a1
description: Элемент GetStreamingEvents представляет операцию, используемую клиентами для запроса потоковых уведомлений от сервера.
ms.openlocfilehash: b07015541cf9c2fbbbc11ebc9f10421bdb9ee84f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833679"
---
# <a name="getstreamingevents"></a><span data-ttu-id="da563-103">GetStreamingEvents</span><span class="sxs-lookup"><span data-stu-id="da563-103">GetStreamingEvents</span></span>

<span data-ttu-id="da563-104">Элемент **GetStreamingEvents** представляет операцию, используемую клиентами для запроса потоковых уведомлений от сервера.</span><span class="sxs-lookup"><span data-stu-id="da563-104">The **GetStreamingEvents** element represents the operation that is used by clients to request streaming notifications from the server.</span></span> 
  
[<span data-ttu-id="da563-105">GetStreamingEvents</span><span class="sxs-lookup"><span data-stu-id="da563-105">GetStreamingEvents</span></span>](getstreamingevents.md)
  
```XML
<GetStreamingEvents>
   <SubscriptionId/>
   <ConnectionTimeout/>
</GetStreamingEvents>
```

 <span data-ttu-id="da563-106">**жетстреаминжевентстипе**</span><span class="sxs-lookup"><span data-stu-id="da563-106">**GetStreamingEventsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="da563-107">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="da563-107">Attributes and elements</span></span>

<span data-ttu-id="da563-108">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="da563-108">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="da563-109">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="da563-109">Attributes</span></span>

<span data-ttu-id="da563-110">Нет.</span><span class="sxs-lookup"><span data-stu-id="da563-110">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="da563-111">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="da563-111">Child elements</span></span>

|<span data-ttu-id="da563-112">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="da563-112">**Element**</span></span>|<span data-ttu-id="da563-113">**Описание**</span><span class="sxs-lookup"><span data-stu-id="da563-113">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="da563-114">SubscriptionId (GetStreamingEvents)</span><span class="sxs-lookup"><span data-stu-id="da563-114">SubscriptionId (GetStreamingEvents)</span></span>](subscriptionid-getstreamingevents.md) <br/> |<span data-ttu-id="da563-115">Представляет идентификатор подписки, запрашиваемой для событий.</span><span class="sxs-lookup"><span data-stu-id="da563-115">Represents the identifier for a subscription that is queried for events.</span></span>  <br/> |
|[<span data-ttu-id="da563-116">ConnectionTimeout</span><span class="sxs-lookup"><span data-stu-id="da563-116">ConnectionTimeout</span></span>](connectiontimeout.md) <br/> |<span data-ttu-id="da563-117">Представляет количество минут, в течение которых подключение будет оставаться открытым.</span><span class="sxs-lookup"><span data-stu-id="da563-117">Represents the number of minutes to keep a connection open.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="da563-118">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="da563-118">Parent elements</span></span>

<span data-ttu-id="da563-119">Нет.</span><span class="sxs-lookup"><span data-stu-id="da563-119">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="da563-120">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="da563-120">Text value</span></span>

<span data-ttu-id="da563-121">Нет.</span><span class="sxs-lookup"><span data-stu-id="da563-121">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="da563-122">Примечания</span><span class="sxs-lookup"><span data-stu-id="da563-122">Remarks</span></span>

<span data-ttu-id="da563-123">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.Этот элемент появился в Exchange Server 2010 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="da563-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="da563-124">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="da563-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="da563-125">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="da563-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="da563-126">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="da563-126">Schema name</span></span>  <br/> |<span data-ttu-id="da563-127">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="da563-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="da563-128">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="da563-128">Validation file</span></span>  <br/> |<span data-ttu-id="da563-129">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="da563-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="da563-130">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="da563-130">Can be empty</span></span>  <br/> |<span data-ttu-id="da563-131">False</span><span class="sxs-lookup"><span data-stu-id="da563-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="da563-132">См. также</span><span class="sxs-lookup"><span data-stu-id="da563-132">See also</span></span>



[<span data-ttu-id="da563-133">Операции подписки</span><span class="sxs-lookup"><span data-stu-id="da563-133">Subscribe operation</span></span>](subscribe-operation.md)
  
[<span data-ttu-id="da563-134">Операция GetStreamingEvents</span><span class="sxs-lookup"><span data-stu-id="da563-134">GetStreamingEvents operation</span></span>](getstreamingevents-operation.md)
  
[<span data-ttu-id="da563-135">Операция по отмене подписки</span><span class="sxs-lookup"><span data-stu-id="da563-135">Unsubscribe operation</span></span>](unsubscribe-operation.md)


- [<span data-ttu-id="da563-136">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="da563-136">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

