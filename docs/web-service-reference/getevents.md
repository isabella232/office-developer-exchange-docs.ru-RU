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
description: Элемент GetEvents представляет операцию, используемую клиентами пула для запроса уведомлений с сервера.
ms.openlocfilehash: e7b24207bff579a2f5230676d6520452f96fe0ce
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762762"
---
# <a name="getevents"></a><span data-ttu-id="c6b93-103">GetEvents</span><span class="sxs-lookup"><span data-stu-id="c6b93-103">GetEvents</span></span>

<span data-ttu-id="c6b93-104">Элемент **GetEvents** представляет операцию, используемую клиентами пула для запроса уведомлений с сервера.</span><span class="sxs-lookup"><span data-stu-id="c6b93-104">The **GetEvents** element represents the operation used by pull clients to request notifications from the server.</span></span> 
  
[<span data-ttu-id="c6b93-105">GetEvents</span><span class="sxs-lookup"><span data-stu-id="c6b93-105">GetEvents</span></span>](getevents.md)
  
```xml
<GetEvents>
   <SubscriptionId/>
   <Watermark/>
</GetEvents>
```

 <span data-ttu-id="c6b93-106">**GetEventsType**</span><span class="sxs-lookup"><span data-stu-id="c6b93-106">**GetEventsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c6b93-107">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="c6b93-107">Attributes and elements</span></span>

<span data-ttu-id="c6b93-108">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="c6b93-108">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c6b93-109">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="c6b93-109">Attributes</span></span>

<span data-ttu-id="c6b93-110">Нет.</span><span class="sxs-lookup"><span data-stu-id="c6b93-110">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c6b93-111">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="c6b93-111">Child elements</span></span>

|<span data-ttu-id="c6b93-112">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="c6b93-112">**Element**</span></span>|<span data-ttu-id="c6b93-113">**Описание**</span><span class="sxs-lookup"><span data-stu-id="c6b93-113">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c6b93-114">SubscriptionId (GetEvents)</span><span class="sxs-lookup"><span data-stu-id="c6b93-114">SubscriptionId (GetEvents)</span></span>](subscriptionid-getevents.md) <br/> |<span data-ttu-id="c6b93-115">Представляет идентификатор подписки, который будет опрошен на наличие событий.</span><span class="sxs-lookup"><span data-stu-id="c6b93-115">Represents the identifier for a subscription that is queried for events.</span></span>  <br/> |
|[<span data-ttu-id="c6b93-116">Водяной знак</span><span class="sxs-lookup"><span data-stu-id="c6b93-116">Watermark</span></span>](watermark.md) <br/> |<span data-ttu-id="c6b93-117">Представляет последний водяной знак возвращением клиенту.</span><span class="sxs-lookup"><span data-stu-id="c6b93-117">Represents the last watermark returned to the client.</span></span> <span data-ttu-id="c6b93-118">Если не был вызван GetEvents для данной подписки, клиент использует водяной знак, возвращаемый запросом подписки на.</span><span class="sxs-lookup"><span data-stu-id="c6b93-118">If GetEvents has not been called for this subscription, the client uses the watermark returned from the Subscribe request.</span></span> <span data-ttu-id="c6b93-119">В противном случае используется водяной знак последнего события в ответе последнего GetEvents.</span><span class="sxs-lookup"><span data-stu-id="c6b93-119">Otherwise, the watermark from the last event in the last GetEvents response is used.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="c6b93-120">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="c6b93-120">Parent elements</span></span>

<span data-ttu-id="c6b93-121">Нет.</span><span class="sxs-lookup"><span data-stu-id="c6b93-121">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="c6b93-122">Замечания</span><span class="sxs-lookup"><span data-stu-id="c6b93-122">Remarks</span></span>

<span data-ttu-id="c6b93-123">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="c6b93-123">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c6b93-124">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="c6b93-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c6b93-125">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="c6b93-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="c6b93-126">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="c6b93-126">Schema name</span></span>  <br/> |<span data-ttu-id="c6b93-127">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="c6b93-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="c6b93-128">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="c6b93-128">Validation file</span></span>  <br/> |<span data-ttu-id="c6b93-129">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="c6b93-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="c6b93-130">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="c6b93-130">Can be empty</span></span>  <br/> |<span data-ttu-id="c6b93-131">Нет</span><span class="sxs-lookup"><span data-stu-id="c6b93-131">false</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c6b93-132">См. также</span><span class="sxs-lookup"><span data-stu-id="c6b93-132">See also</span></span>



[<span data-ttu-id="c6b93-133">Операции подписки</span><span class="sxs-lookup"><span data-stu-id="c6b93-133">Subscribe operation</span></span>](subscribe-operation.md)
  
[<span data-ttu-id="c6b93-134">Операция GetEvents</span><span class="sxs-lookup"><span data-stu-id="c6b93-134">GetEvents operation</span></span>](getevents-operation.md)
  
[<span data-ttu-id="c6b93-135">Отписаться операции</span><span class="sxs-lookup"><span data-stu-id="c6b93-135">Unsubscribe operation</span></span>](unsubscribe-operation.md)

