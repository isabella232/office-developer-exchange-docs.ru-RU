---
title: MoreEvents
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MoreEvents
api_type:
- schema
ms.assetid: 76a7ea58-a44f-49b8-baba-d21302d742ad
description: Элемент MoreEvents определяет, есть ли дополнительные события в очереди доставки для клиента.
ms.openlocfilehash: cc3f7ed3b4b5f5ce27a9d45d508506bfa62e5086
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834489"
---
# <a name="moreevents"></a><span data-ttu-id="ea569-103">MoreEvents</span><span class="sxs-lookup"><span data-stu-id="ea569-103">MoreEvents</span></span>

<span data-ttu-id="ea569-104">Элемент **MoreEvents** определяет, есть ли дополнительные события в очереди доставки для клиента.</span><span class="sxs-lookup"><span data-stu-id="ea569-104">The **MoreEvents** element indicates whether there are more events in the queue to be delivered to the client.</span></span> 
  
```xml
<MoreEvents/>
```

 <span data-ttu-id="ea569-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="ea569-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ea569-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="ea569-106">Attributes and elements</span></span>

<span data-ttu-id="ea569-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="ea569-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ea569-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="ea569-108">Attributes</span></span>

<span data-ttu-id="ea569-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="ea569-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ea569-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="ea569-110">Child elements</span></span>

<span data-ttu-id="ea569-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="ea569-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="ea569-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="ea569-112">Parent elements</span></span>

|<span data-ttu-id="ea569-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="ea569-113">**Element**</span></span>|<span data-ttu-id="ea569-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="ea569-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ea569-115">Уведомление</span><span class="sxs-lookup"><span data-stu-id="ea569-115">Notification</span></span>](notification-ex15websvcsotherref.md) <br/> |<span data-ttu-id="ea569-116">Содержит сведения о подписке и события, произошедшие с момента последнего уведомления.</span><span class="sxs-lookup"><span data-stu-id="ea569-116">Contains information about the subscription and the events that have occurred since the last notification.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="ea569-117">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="ea569-117">Text value</span></span>

<span data-ttu-id="ea569-118">Текстовое значение представляет значение типа Boolean.</span><span class="sxs-lookup"><span data-stu-id="ea569-118">The text value represents a Boolean value.</span></span> <span data-ttu-id="ea569-119">Значение **true** указывает, что другие события в очереди.</span><span class="sxs-lookup"><span data-stu-id="ea569-119">A value of **true** indicates that more events are in the queue.</span></span> <span data-ttu-id="ea569-120">Значение **false** указывает, что не другие события в очереди.</span><span class="sxs-lookup"><span data-stu-id="ea569-120">A value of **false** indicates that no more events are in the queue.</span></span> <span data-ttu-id="ea569-121">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ea569-121">This property is read-only.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="ea569-122">Замечания</span><span class="sxs-lookup"><span data-stu-id="ea569-122">Remarks</span></span>

<span data-ttu-id="ea569-123">В случае оповещения о репликации по запросу значение **true** в этот элемент указывает клиенту, что другой запрос GetEvents должно быть выдано для получения оставшихся событий.</span><span class="sxs-lookup"><span data-stu-id="ea569-123">In the case of Pull notifications, a **true** value in this element indicates to the client that another GetEvents request should be issued to get the remaining events.</span></span> <span data-ttu-id="ea569-124">При условии, что спецификации клиента требуют минимальные задержки уведомлений о событиях, пока не будет возвращено **значение false,** **MoreEvents** значение GetEvents запросы должны продолжать в непрерывной последовательности.</span><span class="sxs-lookup"><span data-stu-id="ea569-124">Assuming that the client specifications require minimum latency for event notifications, GetEvents requests should continue in a continuous succession until a **false** **MoreEvents** value is returned.</span></span> 
  
<span data-ttu-id="ea569-125">В случае Push-уведомлений значение **true** для **MoreEvents** указывает клиенту, что другой запрос уведомления будут отправляться клиенту для доставки оставшихся событий.</span><span class="sxs-lookup"><span data-stu-id="ea569-125">In the case of Push notifications, a **true** value for **MoreEvents** indicates to the client that another notification request will be sent to the client to deliver the remaining events.</span></span> <span data-ttu-id="ea569-126">Как и уведомления по запросу, эти запросы по обработке результатов будет продолжаться в непрерывной последовательности до пуст очередь событий на сервере клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="ea569-126">Similar to Pull notifications, these follow-up requests will continue in continuous succession until the event queue on the Client Access server is empty.</span></span> 
  
<span data-ttu-id="ea569-127">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="ea569-127">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ea569-128">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="ea569-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ea569-129">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="ea569-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="ea569-130">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="ea569-130">Schema Name</span></span>  <br/> |<span data-ttu-id="ea569-131">Схема Types</span><span class="sxs-lookup"><span data-stu-id="ea569-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="ea569-132">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="ea569-132">Validation File</span></span>  <br/> |<span data-ttu-id="ea569-133">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="ea569-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="ea569-134">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="ea569-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="ea569-135">False</span><span class="sxs-lookup"><span data-stu-id="ea569-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ea569-136">См. также</span><span class="sxs-lookup"><span data-stu-id="ea569-136">See also</span></span>



[<span data-ttu-id="ea569-137">Операции подписки</span><span class="sxs-lookup"><span data-stu-id="ea569-137">Subscribe operation</span></span>](subscribe-operation.md)
  
[<span data-ttu-id="ea569-138">Операция GetEvents</span><span class="sxs-lookup"><span data-stu-id="ea569-138">GetEvents operation</span></span>](getevents-operation.md)
  
[<span data-ttu-id="ea569-139">Отписаться операции</span><span class="sxs-lookup"><span data-stu-id="ea569-139">Unsubscribe operation</span></span>](unsubscribe-operation.md)

