---
title: SubscriptionId (Events)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SubscriptionId
api_type:
- schema
ms.assetid: 77c0abab-69e8-428e-8c20-22258e4ef71b
description: Элемент SubscriptionId представляет идентификатор для подписки.
ms.openlocfilehash: 8867b7da7c75cfd9d41f708c0481627d5186cc14
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835622"
---
# <a name="subscriptionid-getevents"></a><span data-ttu-id="f3426-103">SubscriptionId (Events)</span><span class="sxs-lookup"><span data-stu-id="f3426-103">SubscriptionId (GetEvents)</span></span>

<span data-ttu-id="f3426-104">Элемент **SubscriptionId** представляет идентификатор для подписки.</span><span class="sxs-lookup"><span data-stu-id="f3426-104">The **SubscriptionId** element represents the identifier for a subscription.</span></span> 
  
```xml
<SubscriptionId/>
```

 <span data-ttu-id="f3426-105">**субскриптионидтипе**</span><span class="sxs-lookup"><span data-stu-id="f3426-105">**SubscriptionIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f3426-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="f3426-106">Attributes and elements</span></span>

<span data-ttu-id="f3426-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="f3426-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f3426-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="f3426-108">Attributes</span></span>

<span data-ttu-id="f3426-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="f3426-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f3426-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="f3426-110">Child elements</span></span>

<span data-ttu-id="f3426-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="f3426-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="f3426-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="f3426-112">Parent elements</span></span>

|<span data-ttu-id="f3426-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="f3426-113">**Element**</span></span>|<span data-ttu-id="f3426-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="f3426-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f3426-115">GetEvents</span><span class="sxs-lookup"><span data-stu-id="f3426-115">GetEvents</span></span>](getevents.md) <br/> |<span data-ttu-id="f3426-116">Представляет операцию, используемую клиентами опрашивающей репликации для запроса уведомлений с сервера.</span><span class="sxs-lookup"><span data-stu-id="f3426-116">Represents the operation used by pull clients to request notifications from the server.</span></span>  <br/> |
|[<span data-ttu-id="f3426-117">Уведомление</span><span class="sxs-lookup"><span data-stu-id="f3426-117">Notification</span></span>](notification-ex15websvcsotherref.md) <br/> |<span data-ttu-id="f3426-118">Содержит сведения о подписке и событиях, произошедших с момента последнего уведомления.</span><span class="sxs-lookup"><span data-stu-id="f3426-118">Contains information about the subscription and the events that have occurred since the last notification.</span></span>  <br/> |
|[<span data-ttu-id="f3426-119">субскрибереспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="f3426-119">SubscribeResponseMessage</span></span>](subscriberesponsemessage.md) <br/> |<span data-ttu-id="f3426-120">Содержит состояние и результат запроса на подписку.</span><span class="sxs-lookup"><span data-stu-id="f3426-120">Contains the status and result of a Subscribe request.</span></span>  <br/> |
|[<span data-ttu-id="f3426-121">Отмена подписки</span><span class="sxs-lookup"><span data-stu-id="f3426-121">Unsubscribe</span></span>](unsubscribe.md) <br/> |<span data-ttu-id="f3426-122">Содержит свойства, используемые для отмены подписки на подписку.</span><span class="sxs-lookup"><span data-stu-id="f3426-122">Contains the properties used to unsubscribe from a subscription.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="f3426-123">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="f3426-123">Text value</span></span>

<span data-ttu-id="f3426-124">Необходимо указать текстовое значение.</span><span class="sxs-lookup"><span data-stu-id="f3426-124">A text value is required.</span></span> <span data-ttu-id="f3426-125">Текстовое значение — GUID.</span><span class="sxs-lookup"><span data-stu-id="f3426-125">The text value is a GUID.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="f3426-126">Примечания</span><span class="sxs-lookup"><span data-stu-id="f3426-126">Remarks</span></span>

<span data-ttu-id="f3426-127">Идентификатор GUID, представляющий идентификатор подписки, создается сервером клиентского доступа при создании подписки.</span><span class="sxs-lookup"><span data-stu-id="f3426-127">The GUID that represents the subscription identifier is generated by the Client Access server when the subscription is created.</span></span>
  
<span data-ttu-id="f3426-128">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="f3426-128">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f3426-129">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="f3426-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f3426-130">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="f3426-130">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="f3426-131">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="f3426-131">Schema name</span></span>  <br/> |<span data-ttu-id="f3426-132">схема сообщений</span><span class="sxs-lookup"><span data-stu-id="f3426-132">messages schema</span></span>  <br/> |
|<span data-ttu-id="f3426-133">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="f3426-133">Validation file</span></span>  <br/> |<span data-ttu-id="f3426-134">messages. xsd</span><span class="sxs-lookup"><span data-stu-id="f3426-134">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="f3426-135">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="f3426-135">Can be empty</span></span>  <br/> |<span data-ttu-id="f3426-136">False</span><span class="sxs-lookup"><span data-stu-id="f3426-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f3426-137">См. также</span><span class="sxs-lookup"><span data-stu-id="f3426-137">See also</span></span>



[<span data-ttu-id="f3426-138">Операции подписки</span><span class="sxs-lookup"><span data-stu-id="f3426-138">Subscribe operation</span></span>](subscribe-operation.md)
  
[<span data-ttu-id="f3426-139">Операция GetEvents</span><span class="sxs-lookup"><span data-stu-id="f3426-139">GetEvents operation</span></span>](getevents-operation.md)
  
[<span data-ttu-id="f3426-140">Операция по отмене подписки</span><span class="sxs-lookup"><span data-stu-id="f3426-140">Unsubscribe operation</span></span>](unsubscribe-operation.md)

