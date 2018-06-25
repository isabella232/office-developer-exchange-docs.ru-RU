---
title: Уведомления
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Notifications
api_type:
- schema
ms.assetid: 153cc420-d2fe-42f1-afb2-9a31ee09a750
description: Элемент уведомления содержит массив сведений о подписке и события, произошедшие с момента последнего уведомления.
ms.openlocfilehash: f576bf579c91b77dcde8646a6af7fdc47145aef7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834550"
---
# <a name="notifications"></a><span data-ttu-id="4c50f-103">Уведомления</span><span class="sxs-lookup"><span data-stu-id="4c50f-103">Notifications</span></span>

<span data-ttu-id="4c50f-104">Элемент **уведомления** содержит массив сведений о подписке и события, произошедшие с момента последнего уведомления.</span><span class="sxs-lookup"><span data-stu-id="4c50f-104">The **Notifications** element contains an array of information about the subscription and the events that have occurred since the last notification.</span></span> 
  
```xml
<Notifications>
   <Notification/>
</Notifications>
```

 <span data-ttu-id="4c50f-105">**NonEmptyArrayOfNotificationsType**</span><span class="sxs-lookup"><span data-stu-id="4c50f-105">**NonEmptyArrayOfNotificationsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4c50f-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="4c50f-106">Attributes and elements</span></span>

<span data-ttu-id="4c50f-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="4c50f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4c50f-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="4c50f-108">Attributes</span></span>

<span data-ttu-id="4c50f-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="4c50f-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4c50f-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="4c50f-110">Child elements</span></span>

|<span data-ttu-id="4c50f-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="4c50f-111">**Element**</span></span>|<span data-ttu-id="4c50f-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="4c50f-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4c50f-113">Уведомление</span><span class="sxs-lookup"><span data-stu-id="4c50f-113">Notification</span></span>](notification-ex15websvcsotherref.md) <br/> |<span data-ttu-id="4c50f-114">Содержит сведения о подписке и события, произошедшие с момента последнего уведомления.</span><span class="sxs-lookup"><span data-stu-id="4c50f-114">Contains information about the subscription and the events that have occurred since the last notification.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="4c50f-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="4c50f-115">Parent elements</span></span>

|<span data-ttu-id="4c50f-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="4c50f-116">**Element**</span></span>|<span data-ttu-id="4c50f-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="4c50f-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4c50f-118">GetStreamingEventsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="4c50f-118">GetStreamingEventsResponseMessage</span></span>](getstreamingeventsresponsemessage.md) <br/> |<span data-ttu-id="4c50f-119">Содержит состояние и результат одного запроса [GetStreamingEvents операции](getstreamingevents-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="4c50f-119">Contains the status and result of a single [GetStreamingEvents operation](getstreamingevents-operation.md) request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="4c50f-120">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="4c50f-120">Text value</span></span>

<span data-ttu-id="4c50f-121">Нет.</span><span class="sxs-lookup"><span data-stu-id="4c50f-121">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="4c50f-122">Замечания</span><span class="sxs-lookup"><span data-stu-id="4c50f-122">Remarks</span></span>

<span data-ttu-id="4c50f-123">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.Этот элемент появился в Exchange Server 2010 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="4c50f-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4c50f-124">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="4c50f-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4c50f-125">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="4c50f-125">Namespace</span></span>  <br/> |<span data-ttu-id="4c50f-126">http://schemas.microsoft.com/exchange/services/2006/messages и http://schemas.microsoft.com/exchange/services/2006/types</span><span class="sxs-lookup"><span data-stu-id="4c50f-126">http://schemas.microsoft.com/exchange/services/2006/messages and http://schemas.microsoft.com/exchange/services/2006/types</span></span>  <br/> |
|<span data-ttu-id="4c50f-127">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="4c50f-127">Schema Name</span></span>  <br/> |<span data-ttu-id="4c50f-128">Схема сообщения; Типы схемы</span><span class="sxs-lookup"><span data-stu-id="4c50f-128">Messages schema; Types schema</span></span>  <br/> |
|<span data-ttu-id="4c50f-129">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="4c50f-129">Validation File</span></span>  <br/> |<span data-ttu-id="4c50f-130">Messages.xsd; Types.xsd</span><span class="sxs-lookup"><span data-stu-id="4c50f-130">Messages.xsd; Types.xsd</span></span>  <br/> |
|<span data-ttu-id="4c50f-131">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="4c50f-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="4c50f-132">False</span><span class="sxs-lookup"><span data-stu-id="4c50f-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="4c50f-133">См. также</span><span class="sxs-lookup"><span data-stu-id="4c50f-133">See also</span></span>



[<span data-ttu-id="4c50f-134">GetFolder Operation</span><span class="sxs-lookup"><span data-stu-id="4c50f-134">GetFolder operation</span></span>](getfolder-operation.md)
  
[<span data-ttu-id="4c50f-135">Операция DeleteFolder</span><span class="sxs-lookup"><span data-stu-id="4c50f-135">DeleteFolder operation</span></span>](deletefolder-operation.md)
  
[<span data-ttu-id="4c50f-136">Операция MoveFolder</span><span class="sxs-lookup"><span data-stu-id="4c50f-136">MoveFolder operation</span></span>](movefolder-operation.md)
  
[<span data-ttu-id="4c50f-137">Операция CopyFolder</span><span class="sxs-lookup"><span data-stu-id="4c50f-137">CopyFolder operation</span></span>](copyfolder-operation.md)
  
[<span data-ttu-id="4c50f-138">Операции подписки</span><span class="sxs-lookup"><span data-stu-id="4c50f-138">Subscribe operation</span></span>](subscribe-operation.md)

