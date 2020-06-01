---
title: фрибусичанжедевент
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
description: Элемент Фрибусичанжедевент представляет событие, в котором изменилось свободное и занятое время элемента.
ms.openlocfilehash: d9ea8bc210ab503c4e9f606bcb66317cefe15de1
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44456481"
---
# <a name="freebusychangedevent"></a><span data-ttu-id="77bcd-103">фрибусичанжедевент</span><span class="sxs-lookup"><span data-stu-id="77bcd-103">FreeBusyChangedEvent</span></span>

<span data-ttu-id="77bcd-104">Элемент **фрибусичанжедевент** представляет событие, в котором изменилось свободное и занятое время элемента.</span><span class="sxs-lookup"><span data-stu-id="77bcd-104">The **FreeBusyChangedEvent** element represents an event in which an item's free/busy time has changed.</span></span> 
  
```xml
<CreatedEvent>
   <Watermark/>
   <TimeStamp/>
   <ItemId/>
   <ParentFolderId/>
</CreatedEvent>
```

 <span data-ttu-id="77bcd-105">**басеобжектчанжедевенттипе**</span><span class="sxs-lookup"><span data-stu-id="77bcd-105">**BaseObjectChangedEventType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="77bcd-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="77bcd-106">Attributes and elements</span></span>

<span data-ttu-id="77bcd-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="77bcd-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="77bcd-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="77bcd-108">Attributes</span></span>

<span data-ttu-id="77bcd-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="77bcd-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="77bcd-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="77bcd-110">Child elements</span></span>

|<span data-ttu-id="77bcd-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="77bcd-111">**Element**</span></span>|<span data-ttu-id="77bcd-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="77bcd-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="77bcd-113">Watermark</span><span class="sxs-lookup"><span data-stu-id="77bcd-113">Watermark</span></span>](watermark.md) <br/> |<span data-ttu-id="77bcd-114">Представляет закладку события в таблице событий почтовых ящиков.</span><span class="sxs-lookup"><span data-stu-id="77bcd-114">Represents an event bookmark in the mailbox events table.</span></span>  <br/> |
|[<span data-ttu-id="77bcd-115">Метка времени</span><span class="sxs-lookup"><span data-stu-id="77bcd-115">TimeStamp</span></span>](timestamp.md) <br/> |<span data-ttu-id="77bcd-116">Представляет метку времени события почтового ящика элемента о занятости.</span><span class="sxs-lookup"><span data-stu-id="77bcd-116">Represents the timestamp of a free/busy item mailbox event.</span></span>  <br/> |
|[<span data-ttu-id="77bcd-117">Идентификатор</span><span class="sxs-lookup"><span data-stu-id="77bcd-117">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="77bcd-118">Представляет идентификатор элемента "сведения о занятости".</span><span class="sxs-lookup"><span data-stu-id="77bcd-118">Represents the identifier of the free/busy item.</span></span>  <br/> |
|[<span data-ttu-id="77bcd-119">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="77bcd-119">ParentFolderId</span></span>](parentfolderid.md) <br/> |<span data-ttu-id="77bcd-120">Представляет идентификатор родительской папки элемента со сведениями о занятости.</span><span class="sxs-lookup"><span data-stu-id="77bcd-120">Represents the identifier of the parent folder of the free/busy item.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="77bcd-121">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="77bcd-121">Parent elements</span></span>

|<span data-ttu-id="77bcd-122">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="77bcd-122">**Element**</span></span>|<span data-ttu-id="77bcd-123">**Описание**</span><span class="sxs-lookup"><span data-stu-id="77bcd-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="77bcd-124">Уведомление</span><span class="sxs-lookup"><span data-stu-id="77bcd-124">Notification</span></span>](notification-ex15websvcsotherref.md) <br/> |<span data-ttu-id="77bcd-125">Содержит сведения о подписке и событиях, произошедших с момента последнего уведомления.</span><span class="sxs-lookup"><span data-stu-id="77bcd-125">Contains information about the subscription and the events that have occurred since the last notification.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="77bcd-126">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="77bcd-126">Text value</span></span>

<span data-ttu-id="77bcd-127">Нет.</span><span class="sxs-lookup"><span data-stu-id="77bcd-127">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="77bcd-128">Примечания</span><span class="sxs-lookup"><span data-stu-id="77bcd-128">Remarks</span></span>

<span data-ttu-id="77bcd-129">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.Этот элемент появился в Exchange Server 2010 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="77bcd-129">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="77bcd-130">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="77bcd-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="77bcd-131">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="77bcd-131">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="77bcd-132">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="77bcd-132">Schema name</span></span>  <br/> |<span data-ttu-id="77bcd-133">Схема Types</span><span class="sxs-lookup"><span data-stu-id="77bcd-133">Types schema</span></span>  <br/> |
|<span data-ttu-id="77bcd-134">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="77bcd-134">Validation file</span></span>  <br/> |<span data-ttu-id="77bcd-135">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="77bcd-135">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="77bcd-136">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="77bcd-136">Can be empty</span></span>  <br/> |<span data-ttu-id="77bcd-137">False</span><span class="sxs-lookup"><span data-stu-id="77bcd-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="77bcd-138">См. также</span><span class="sxs-lookup"><span data-stu-id="77bcd-138">See also</span></span>



[<span data-ttu-id="77bcd-139">Операции подписки</span><span class="sxs-lookup"><span data-stu-id="77bcd-139">Subscribe operation</span></span>](subscribe-operation.md)
  
[<span data-ttu-id="77bcd-140">Операция GetEvents</span><span class="sxs-lookup"><span data-stu-id="77bcd-140">GetEvents operation</span></span>](getevents-operation.md)
  
[<span data-ttu-id="77bcd-141">Операция по отмене подписки</span><span class="sxs-lookup"><span data-stu-id="77bcd-141">Unsubscribe operation</span></span>](unsubscribe-operation.md)


[<span data-ttu-id="77bcd-142">Использование подписок по запросу</span><span class="sxs-lookup"><span data-stu-id="77bcd-142">Using Pull Subscriptions</span></span>](https://msdn.microsoft.com/library/f956bc0e-2b25-4613-966b-54c65456897c%28Office.15%29.aspx)
  
[<span data-ttu-id="77bcd-143">Уведомления о событиях в EWS</span><span class="sxs-lookup"><span data-stu-id="77bcd-143">Event notifications in EWS</span></span>](https://msdn.microsoft.com/library/4fd4b351-d35c-4ccc-9ed9-878932ab9d50%28Office.15%29.aspx)

