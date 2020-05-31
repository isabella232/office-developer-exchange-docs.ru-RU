---
title: EventType
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- EventType
api_type:
- schema
ms.assetid: 04b70f9e-c226-4130-958e-0db0275cf58b
description: Элемент EventType используется для создания подписки и определяет тип события, который должен быть указан в уведомлении.
ms.openlocfilehash: fb54c9e042f105d10e68cb0e9b48feae7ed8bf7b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762394"
---
# <a name="eventtype"></a><span data-ttu-id="dda97-103">EventType</span><span class="sxs-lookup"><span data-stu-id="dda97-103">EventType</span></span>

<span data-ttu-id="dda97-104">Элемент **EventType** используется для создания подписки и определяет тип события, который должен быть указан в уведомлении.</span><span class="sxs-lookup"><span data-stu-id="dda97-104">The **EventType** element is used to create a subscription and identifies an event type to be reported in a notification.</span></span> 
  
```xml
<EventType/>
```

 <span data-ttu-id="dda97-105">**нотификатионевенттипетипе**</span><span class="sxs-lookup"><span data-stu-id="dda97-105">**NotificationEventTypeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="dda97-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="dda97-106">Attributes and elements</span></span>

<span data-ttu-id="dda97-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="dda97-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="dda97-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="dda97-108">Attributes</span></span>

<span data-ttu-id="dda97-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="dda97-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="dda97-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="dda97-110">Child elements</span></span>

<span data-ttu-id="dda97-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="dda97-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="dda97-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="dda97-112">Parent elements</span></span>

|<span data-ttu-id="dda97-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="dda97-113">**Element**</span></span>|<span data-ttu-id="dda97-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="dda97-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="dda97-115">евенттипес</span><span class="sxs-lookup"><span data-stu-id="dda97-115">EventTypes</span></span>](eventtypes.md) <br/> |<span data-ttu-id="dda97-116">Содержит коллекцию типов событий уведомления о событиях, которые используются для создания подписки.</span><span class="sxs-lookup"><span data-stu-id="dda97-116">Contains a collection of event notification event types that are used to create a subscription.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="dda97-117">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="dda97-117">Text value</span></span>

<span data-ttu-id="dda97-118">Необходимо указать текстовое значение.</span><span class="sxs-lookup"><span data-stu-id="dda97-118">A text value is required.</span></span> <span data-ttu-id="dda97-119">Ниже перечислены возможные значения.</span><span class="sxs-lookup"><span data-stu-id="dda97-119">The following are the possible values:</span></span>
  
- <span data-ttu-id="dda97-120">копиедевент</span><span class="sxs-lookup"><span data-stu-id="dda97-120">CopiedEvent</span></span>
    
- <span data-ttu-id="dda97-121">креатедевент</span><span class="sxs-lookup"><span data-stu-id="dda97-121">CreatedEvent</span></span>
    
- <span data-ttu-id="dda97-122">делетедевент</span><span class="sxs-lookup"><span data-stu-id="dda97-122">DeletedEvent</span></span>
    
- <span data-ttu-id="dda97-123">модифиедевент</span><span class="sxs-lookup"><span data-stu-id="dda97-123">ModifiedEvent</span></span>
    
- <span data-ttu-id="dda97-124">моведевент</span><span class="sxs-lookup"><span data-stu-id="dda97-124">MovedEvent</span></span>
    
- <span data-ttu-id="dda97-125">невмаилевент</span><span class="sxs-lookup"><span data-stu-id="dda97-125">NewMailEvent</span></span>
    
- <span data-ttu-id="dda97-126">фрибусичанжедевент</span><span class="sxs-lookup"><span data-stu-id="dda97-126">FreeBusyChangedEvent</span></span>
    
## <a name="remarks"></a><span data-ttu-id="dda97-127">Примечания</span><span class="sxs-lookup"><span data-stu-id="dda97-127">Remarks</span></span>

<span data-ttu-id="dda97-128">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.Этот элемент появился в Exchange Server 2010 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="dda97-128">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="dda97-129">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="dda97-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="dda97-130">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="dda97-130">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="dda97-131">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="dda97-131">Schema Name</span></span>  <br/> |<span data-ttu-id="dda97-132">Схема Types</span><span class="sxs-lookup"><span data-stu-id="dda97-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="dda97-133">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="dda97-133">Validation File</span></span>  <br/> |<span data-ttu-id="dda97-134">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="dda97-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="dda97-135">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="dda97-135">Can be Empty</span></span>  <br/> |<span data-ttu-id="dda97-136">False</span><span class="sxs-lookup"><span data-stu-id="dda97-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="dda97-137">См. также</span><span class="sxs-lookup"><span data-stu-id="dda97-137">See also</span></span>



[<span data-ttu-id="dda97-138">Операции подписки</span><span class="sxs-lookup"><span data-stu-id="dda97-138">Subscribe operation</span></span>](subscribe-operation.md)
  
[<span data-ttu-id="dda97-139">Операция GetEvents</span><span class="sxs-lookup"><span data-stu-id="dda97-139">GetEvents operation</span></span>](getevents-operation.md)
  
[<span data-ttu-id="dda97-140">Операция по отмене подписки</span><span class="sxs-lookup"><span data-stu-id="dda97-140">Unsubscribe operation</span></span>](unsubscribe-operation.md)

