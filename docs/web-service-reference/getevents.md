---
title: GetEvents
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetEvents
api_type:
- schema
ms.assetid: 22d4da6b-d8a8-484f-82c4-3e4b8f5431cd
description: Элемент Events представляет операцию, используемую клиентами, запрашивающими уведомления от сервера.
ms.openlocfilehash: 004f782ccd32b3c5e501080bfc59419a6e7d9ce4
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462502"
---
# <a name="getevents"></a><span data-ttu-id="c8e13-103">GetEvents</span><span class="sxs-lookup"><span data-stu-id="c8e13-103">GetEvents</span></span>

<span data-ttu-id="c8e13-104">Элемент **Events** представляет операцию, используемую клиентами, запрашивающими уведомления от сервера.</span><span class="sxs-lookup"><span data-stu-id="c8e13-104">The **GetEvents** element represents the operation used by pull clients to request notifications from the server.</span></span> 
  
[<span data-ttu-id="c8e13-105">GetEvents</span><span class="sxs-lookup"><span data-stu-id="c8e13-105">GetEvents</span></span>](getevents.md)
  
```xml
<GetEvents>
   <SubscriptionId/>
   <Watermark/>
</GetEvents>
```

 <span data-ttu-id="c8e13-106">**жетевентстипе**</span><span class="sxs-lookup"><span data-stu-id="c8e13-106">**GetEventsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c8e13-107">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="c8e13-107">Attributes and elements</span></span>

<span data-ttu-id="c8e13-108">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="c8e13-108">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c8e13-109">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="c8e13-109">Attributes</span></span>

<span data-ttu-id="c8e13-110">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="c8e13-110">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c8e13-111">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="c8e13-111">Child elements</span></span>

|<span data-ttu-id="c8e13-112">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="c8e13-112">**Element**</span></span>|<span data-ttu-id="c8e13-113">**Описание**</span><span class="sxs-lookup"><span data-stu-id="c8e13-113">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c8e13-114">SubscriptionId (Events)</span><span class="sxs-lookup"><span data-stu-id="c8e13-114">SubscriptionId (GetEvents)</span></span>](subscriptionid-getevents.md) <br/> |<span data-ttu-id="c8e13-115">Представляет идентификатор подписки, запрашиваемой для событий.</span><span class="sxs-lookup"><span data-stu-id="c8e13-115">Represents the identifier for a subscription that is queried for events.</span></span>  <br/> |
|[<span data-ttu-id="c8e13-116">Watermark</span><span class="sxs-lookup"><span data-stu-id="c8e13-116">Watermark</span></span>](watermark.md) <br/> |<span data-ttu-id="c8e13-117">Представляет последний водяной знак, возвращенный клиенту.</span><span class="sxs-lookup"><span data-stu-id="c8e13-117">Represents the last watermark returned to the client.</span></span> <span data-ttu-id="c8e13-118">Если для этой подписки не вызывались события для этой подписки, клиент использует водяной знак, возвращенный из запроса Subscribe.</span><span class="sxs-lookup"><span data-stu-id="c8e13-118">If GetEvents has not been called for this subscription, the client uses the watermark returned from the Subscribe request.</span></span> <span data-ttu-id="c8e13-119">В противном случае используется водяной знак из последнего события в последнем ответе на событие.</span><span class="sxs-lookup"><span data-stu-id="c8e13-119">Otherwise, the watermark from the last event in the last GetEvents response is used.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="c8e13-120">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="c8e13-120">Parent elements</span></span>

<span data-ttu-id="c8e13-121">Нет.</span><span class="sxs-lookup"><span data-stu-id="c8e13-121">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="c8e13-122">Примечания</span><span class="sxs-lookup"><span data-stu-id="c8e13-122">Remarks</span></span>

<span data-ttu-id="c8e13-123">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="c8e13-123">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c8e13-124">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="c8e13-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c8e13-125">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="c8e13-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="c8e13-126">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="c8e13-126">Schema name</span></span>  <br/> |<span data-ttu-id="c8e13-127">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="c8e13-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="c8e13-128">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="c8e13-128">Validation file</span></span>  <br/> |<span data-ttu-id="c8e13-129">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="c8e13-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="c8e13-130">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="c8e13-130">Can be empty</span></span>  <br/> |<span data-ttu-id="c8e13-131">false</span><span class="sxs-lookup"><span data-stu-id="c8e13-131">false</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c8e13-132">См. также</span><span class="sxs-lookup"><span data-stu-id="c8e13-132">See also</span></span>



[<span data-ttu-id="c8e13-133">Операции подписки</span><span class="sxs-lookup"><span data-stu-id="c8e13-133">Subscribe operation</span></span>](subscribe-operation.md)
  
[<span data-ttu-id="c8e13-134">Операция GetEvents</span><span class="sxs-lookup"><span data-stu-id="c8e13-134">GetEvents operation</span></span>](getevents-operation.md)
  
[<span data-ttu-id="c8e13-135">Операция по отмене подписки</span><span class="sxs-lookup"><span data-stu-id="c8e13-135">Unsubscribe operation</span></span>](unsubscribe-operation.md)

