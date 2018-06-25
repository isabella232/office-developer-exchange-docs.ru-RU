---
title: FreeBusyChangedEvent
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FreeBusyChangedEvent
api_type:
- schema
ms.assetid: 63abbfc5-c29f-4110-a922-6b1247187f28
description: Элемент FreeBusyChangedEvent представляет событие, в котором был изменен занятости элемента.
ms.openlocfilehash: 7271d375526e7614d0150594c2b988666a59eb8d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762659"
---
# <a name="freebusychangedevent"></a><span data-ttu-id="89952-103">FreeBusyChangedEvent</span><span class="sxs-lookup"><span data-stu-id="89952-103">FreeBusyChangedEvent</span></span>

<span data-ttu-id="89952-104">Элемент **FreeBusyChangedEvent** представляет событие, в котором был изменен занятости элемента.</span><span class="sxs-lookup"><span data-stu-id="89952-104">The **FreeBusyChangedEvent** element represents an event in which an item's free/busy time has changed.</span></span> 
  
```xml
<CreatedEvent>
   <Watermark/>
   <TimeStamp/>
   <ItemId/>
   <ParentFolderId/>
</CreatedEvent>
```

 <span data-ttu-id="89952-105">**BaseObjectChangedEventType**</span><span class="sxs-lookup"><span data-stu-id="89952-105">**BaseObjectChangedEventType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="89952-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="89952-106">Attributes and elements</span></span>

<span data-ttu-id="89952-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="89952-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="89952-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="89952-108">Attributes</span></span>

<span data-ttu-id="89952-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="89952-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="89952-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="89952-110">Child elements</span></span>

|<span data-ttu-id="89952-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="89952-111">**Element**</span></span>|<span data-ttu-id="89952-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="89952-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="89952-113">Водяной знак</span><span class="sxs-lookup"><span data-stu-id="89952-113">Watermark</span></span>](watermark.md) <br/> |<span data-ttu-id="89952-114">Представляет закладку события в таблице событий почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="89952-114">Represents an event bookmark in the mailbox events table.</span></span>  <br/> |
|[<span data-ttu-id="89952-115">Метка времени</span><span class="sxs-lookup"><span data-stu-id="89952-115">TimeStamp</span></span>](timestamp.md) <br/> |<span data-ttu-id="89952-116">Представляет метка времени события почтового ящика занятости элемента.</span><span class="sxs-lookup"><span data-stu-id="89952-116">Represents the timestamp of a free/busy item mailbox event.</span></span>  <br/> |
|[<span data-ttu-id="89952-117">Идентификатор элемента</span><span class="sxs-lookup"><span data-stu-id="89952-117">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="89952-118">Представляет идентификатор элемента сведениям о доступности.</span><span class="sxs-lookup"><span data-stu-id="89952-118">Represents the identifier of the free/busy item.</span></span>  <br/> |
|[<span data-ttu-id="89952-119">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="89952-119">ParentFolderId</span></span>](parentfolderid.md) <br/> |<span data-ttu-id="89952-120">Представляет идентификатор родительской папки элемента сведениям о доступности.</span><span class="sxs-lookup"><span data-stu-id="89952-120">Represents the identifier of the parent folder of the free/busy item.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="89952-121">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="89952-121">Parent elements</span></span>

|<span data-ttu-id="89952-122">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="89952-122">**Element**</span></span>|<span data-ttu-id="89952-123">**Описание**</span><span class="sxs-lookup"><span data-stu-id="89952-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="89952-124">Уведомление</span><span class="sxs-lookup"><span data-stu-id="89952-124">Notification</span></span>](notification-ex15websvcsotherref.md) <br/> |<span data-ttu-id="89952-125">Содержит сведения о подписке и события, произошедшие с момента последнего уведомления.</span><span class="sxs-lookup"><span data-stu-id="89952-125">Contains information about the subscription and the events that have occurred since the last notification.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="89952-126">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="89952-126">Text value</span></span>

<span data-ttu-id="89952-127">Нет.</span><span class="sxs-lookup"><span data-stu-id="89952-127">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="89952-128">Замечания</span><span class="sxs-lookup"><span data-stu-id="89952-128">Remarks</span></span>

<span data-ttu-id="89952-129">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.Этот элемент появился в Exchange Server 2010 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="89952-129">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="89952-130">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="89952-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="89952-131">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="89952-131">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="89952-132">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="89952-132">Schema name</span></span>  <br/> |<span data-ttu-id="89952-133">Схема Types</span><span class="sxs-lookup"><span data-stu-id="89952-133">Types schema</span></span>  <br/> |
|<span data-ttu-id="89952-134">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="89952-134">Validation file</span></span>  <br/> |<span data-ttu-id="89952-135">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="89952-135">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="89952-136">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="89952-136">Can be empty</span></span>  <br/> |<span data-ttu-id="89952-137">False</span><span class="sxs-lookup"><span data-stu-id="89952-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="89952-138">См. также</span><span class="sxs-lookup"><span data-stu-id="89952-138">See also</span></span>



[<span data-ttu-id="89952-139">Операции подписки</span><span class="sxs-lookup"><span data-stu-id="89952-139">Subscribe operation</span></span>](subscribe-operation.md)
  
[<span data-ttu-id="89952-140">Операция GetEvents</span><span class="sxs-lookup"><span data-stu-id="89952-140">GetEvents operation</span></span>](getevents-operation.md)
  
[<span data-ttu-id="89952-141">Отписаться операции</span><span class="sxs-lookup"><span data-stu-id="89952-141">Unsubscribe operation</span></span>](unsubscribe-operation.md)


[<span data-ttu-id="89952-142">С помощью подписки по запросу</span><span class="sxs-lookup"><span data-stu-id="89952-142">Using Pull Subscriptions</span></span>](http://msdn.microsoft.com/library/f956bc0e-2b25-4613-966b-54c65456897c%28Office.15%29.aspx)
  
[<span data-ttu-id="89952-143">Уведомления о событиях в веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="89952-143">Event notifications in EWS</span></span>](http://msdn.microsoft.com/library/4fd4b351-d35c-4ccc-9ed9-878932ab9d50%28Office.15%29.aspx)

