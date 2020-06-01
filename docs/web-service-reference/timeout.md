---
title: Timeout
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Timeout
api_type:
- schema
ms.assetid: c2e1ca5a-6667-4f6f-aac4-89de33bddc54
description: Элемент timeout представляет продолжительность в минутах, в течение которого подписка может быть бездействовать без запроса на получение событий от клиента.
ms.openlocfilehash: 6f3228cd480bf0eaf259c4f321bc74d0845b9bba
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459898"
---
# <a name="timeout"></a><span data-ttu-id="2323b-103">Timeout</span><span class="sxs-lookup"><span data-stu-id="2323b-103">Timeout</span></span>

<span data-ttu-id="2323b-104">Элемент **timeout** представляет продолжительность в минутах, в течение которого подписка может быть бездействовать без запроса на получение событий от клиента.</span><span class="sxs-lookup"><span data-stu-id="2323b-104">The **Timeout** element represents the duration, in minutes, that the subscription can remain idle without a GetEvents request from the client.</span></span> 
  
```xml
<Timeout/>
```

 <span data-ttu-id="2323b-105">**int**</span><span class="sxs-lookup"><span data-stu-id="2323b-105">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2323b-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="2323b-106">Attributes and elements</span></span>

<span data-ttu-id="2323b-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="2323b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2323b-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="2323b-108">Attributes</span></span>

<span data-ttu-id="2323b-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="2323b-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2323b-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="2323b-110">Child elements</span></span>

<span data-ttu-id="2323b-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="2323b-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="2323b-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="2323b-112">Parent elements</span></span>

|<span data-ttu-id="2323b-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="2323b-113">**Element**</span></span>|<span data-ttu-id="2323b-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="2323b-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2323b-115">пуллсубскриптионрекуест</span><span class="sxs-lookup"><span data-stu-id="2323b-115">PullSubscriptionRequest</span></span>](pullsubscriptionrequest.md) <br/> |<span data-ttu-id="2323b-116">Представляет подписку на подписку на уведомления о событиях по запросу.</span><span class="sxs-lookup"><span data-stu-id="2323b-116">Represents a subscription to a pull-based event notification subscription.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="2323b-117">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="2323b-117">Text value</span></span>

<span data-ttu-id="2323b-118">При использовании этого элемента необходимо указать текстовое значение, представляющее целое число.</span><span class="sxs-lookup"><span data-stu-id="2323b-118">A text value that represents an integer is required if this element is used.</span></span> <span data-ttu-id="2323b-119">Возможные значения для этого элемента — от 1 до 1440 включительно.</span><span class="sxs-lookup"><span data-stu-id="2323b-119">The possible values for this element are 1 to 1440, inclusive.</span></span> <span data-ttu-id="2323b-120">Этот элемент обязательный.</span><span class="sxs-lookup"><span data-stu-id="2323b-120">This element is required.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="2323b-121">Примечания</span><span class="sxs-lookup"><span data-stu-id="2323b-121">Remarks</span></span>

<span data-ttu-id="2323b-122">Таймер времени ожидания для подписки сбрасывается из-за успешных запросов на получение событий.</span><span class="sxs-lookup"><span data-stu-id="2323b-122">The timeout timer for the subscription is reset by a successful GetEvents request.</span></span>
  
<span data-ttu-id="2323b-123">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="2323b-123">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="2323b-124">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="2323b-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2323b-125">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="2323b-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="2323b-126">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="2323b-126">Schema name</span></span>  <br/> |<span data-ttu-id="2323b-127">Схема Types</span><span class="sxs-lookup"><span data-stu-id="2323b-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="2323b-128">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="2323b-128">Validation file</span></span>  <br/> |<span data-ttu-id="2323b-129">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="2323b-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="2323b-130">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="2323b-130">Can be empty</span></span>  <br/> |<span data-ttu-id="2323b-131">False</span><span class="sxs-lookup"><span data-stu-id="2323b-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="2323b-132">См. также</span><span class="sxs-lookup"><span data-stu-id="2323b-132">See also</span></span>



[<span data-ttu-id="2323b-133">Операции подписки</span><span class="sxs-lookup"><span data-stu-id="2323b-133">Subscribe operation</span></span>](subscribe-operation.md)
  
[<span data-ttu-id="2323b-134">Операция GetEvents</span><span class="sxs-lookup"><span data-stu-id="2323b-134">GetEvents operation</span></span>](getevents-operation.md)
  
[<span data-ttu-id="2323b-135">Операция по отмене подписки</span><span class="sxs-lookup"><span data-stu-id="2323b-135">Unsubscribe operation</span></span>](unsubscribe-operation.md)

