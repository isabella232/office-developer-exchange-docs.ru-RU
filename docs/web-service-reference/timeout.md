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
description: Время ожидания элемент представляет продолжительность в минутах, подписки может простаивать без запроса GetEvents от клиента.
ms.openlocfilehash: 0a26002689e131959f09318b01d97ffb73b605f9
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19840186"
---
# <a name="timeout"></a><span data-ttu-id="a824f-103">Timeout</span><span class="sxs-lookup"><span data-stu-id="a824f-103">Timeout</span></span>

<span data-ttu-id="a824f-104">**Время ожидания** элемент представляет продолжительность в минутах, подписки может простаивать без запроса GetEvents от клиента.</span><span class="sxs-lookup"><span data-stu-id="a824f-104">The **Timeout** element represents the duration, in minutes, that the subscription can remain idle without a GetEvents request from the client.</span></span> 
  
```xml
<Timeout/>
```

 <span data-ttu-id="a824f-105">**int**</span><span class="sxs-lookup"><span data-stu-id="a824f-105">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a824f-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="a824f-106">Attributes and elements</span></span>

<span data-ttu-id="a824f-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="a824f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a824f-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="a824f-108">Attributes</span></span>

<span data-ttu-id="a824f-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="a824f-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a824f-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="a824f-110">Child elements</span></span>

<span data-ttu-id="a824f-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="a824f-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="a824f-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="a824f-112">Parent elements</span></span>

|<span data-ttu-id="a824f-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="a824f-113">**Element**</span></span>|<span data-ttu-id="a824f-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="a824f-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a824f-115">PullSubscriptionRequest</span><span class="sxs-lookup"><span data-stu-id="a824f-115">PullSubscriptionRequest</span></span>](pullsubscriptionrequest.md) <br/> |<span data-ttu-id="a824f-116">Представляет подписка на подписку на уведомления о событий на основе репликации по запросу.</span><span class="sxs-lookup"><span data-stu-id="a824f-116">Represents a subscription to a pull-based event notification subscription.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="a824f-117">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="a824f-117">Text value</span></span>

<span data-ttu-id="a824f-118">Текстовое значение, представляющее целое число является обязательным, если данный элемент используется.</span><span class="sxs-lookup"><span data-stu-id="a824f-118">A text value that represents an integer is required if this element is used.</span></span> <span data-ttu-id="a824f-119">Возможные значения для этого элемента: 1 до 1440 включительно.</span><span class="sxs-lookup"><span data-stu-id="a824f-119">The possible values for this element are 1 to 1440, inclusive.</span></span> <span data-ttu-id="a824f-120">Этот элемент обязательный.</span><span class="sxs-lookup"><span data-stu-id="a824f-120">This element is required.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="a824f-121">Замечания</span><span class="sxs-lookup"><span data-stu-id="a824f-121">Remarks</span></span>

<span data-ttu-id="a824f-122">Успешный запрос GetEvents выполнить сброс таймера времени ожидания для подписки.</span><span class="sxs-lookup"><span data-stu-id="a824f-122">The timeout timer for the subscription is reset by a successful GetEvents request.</span></span>
  
<span data-ttu-id="a824f-123">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="a824f-123">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="a824f-124">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="a824f-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a824f-125">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="a824f-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="a824f-126">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="a824f-126">Schema name</span></span>  <br/> |<span data-ttu-id="a824f-127">Схема Types</span><span class="sxs-lookup"><span data-stu-id="a824f-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="a824f-128">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="a824f-128">Validation file</span></span>  <br/> |<span data-ttu-id="a824f-129">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="a824f-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="a824f-130">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="a824f-130">Can be empty</span></span>  <br/> |<span data-ttu-id="a824f-131">False</span><span class="sxs-lookup"><span data-stu-id="a824f-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a824f-132">См. также</span><span class="sxs-lookup"><span data-stu-id="a824f-132">See also</span></span>



[<span data-ttu-id="a824f-133">Операции подписки</span><span class="sxs-lookup"><span data-stu-id="a824f-133">Subscribe operation</span></span>](subscribe-operation.md)
  
[<span data-ttu-id="a824f-134">Операция GetEvents</span><span class="sxs-lookup"><span data-stu-id="a824f-134">GetEvents operation</span></span>](getevents-operation.md)
  
[<span data-ttu-id="a824f-135">Отписаться операции</span><span class="sxs-lookup"><span data-stu-id="a824f-135">Unsubscribe operation</span></span>](unsubscribe-operation.md)

