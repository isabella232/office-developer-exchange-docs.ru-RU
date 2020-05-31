---
title: ConnectionTimeout
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ConnectionTimeout
api_type:
- schema
ms.assetid: 14da68a0-bcca-4281-a774-47644baa4ee9
description: Элемент ConnectionTimeout указывает количество минут, в течение которых подключение будет оставаться открытым.
ms.openlocfilehash: 2bb40ba502853c70ef107c4c740fdfe7073abe31
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761717"
---
# <a name="connectiontimeout"></a><span data-ttu-id="12db5-103">ConnectionTimeout</span><span class="sxs-lookup"><span data-stu-id="12db5-103">ConnectionTimeout</span></span>

<span data-ttu-id="12db5-104">Элемент **ConnectionTimeout** указывает количество минут, в течение которых подключение будет оставаться открытым.</span><span class="sxs-lookup"><span data-stu-id="12db5-104">The **ConnectionTimeout** element specifies the number of minutes to keep a connection open.</span></span> 
  
[<span data-ttu-id="12db5-105">Операция GetStreamingEvents</span><span class="sxs-lookup"><span data-stu-id="12db5-105">GetStreamingEvents operation</span></span>](getstreamingevents-operation.md)
  
[<span data-ttu-id="12db5-106">ConnectionTimeout</span><span class="sxs-lookup"><span data-stu-id="12db5-106">ConnectionTimeout</span></span>](connectiontimeout.md)
  
```xml
<ConnectionTimeout/>
```

 <span data-ttu-id="12db5-107">**int**</span><span class="sxs-lookup"><span data-stu-id="12db5-107">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="12db5-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="12db5-108">Attributes and elements</span></span>

<span data-ttu-id="12db5-109">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="12db5-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="12db5-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="12db5-110">Attributes</span></span>

<span data-ttu-id="12db5-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="12db5-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="12db5-112">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="12db5-112">Child elements</span></span>

<span data-ttu-id="12db5-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="12db5-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="12db5-114">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="12db5-114">Parent elements</span></span>

|<span data-ttu-id="12db5-115">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="12db5-115">**Element**</span></span>|<span data-ttu-id="12db5-116">**Описание**</span><span class="sxs-lookup"><span data-stu-id="12db5-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="12db5-117">GetStreamingEvents</span><span class="sxs-lookup"><span data-stu-id="12db5-117">GetStreamingEvents</span></span>](getstreamingevents.md) <br/> |<span data-ttu-id="12db5-118">Определяет запрос на получение уведомлений о событиях из потокового подключения.</span><span class="sxs-lookup"><span data-stu-id="12db5-118">Defines a request to get event notifications from a streaming connection.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="12db5-119">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="12db5-119">Text value</span></span>

<span data-ttu-id="12db5-120">Текстовое значение представляет целое число, которое описывает максимальное число минут, в течение которых будет открыто потоковое подключение.</span><span class="sxs-lookup"><span data-stu-id="12db5-120">The text value represents an integer that describes the maximum number of minutes to keep a streaming connection open.</span></span> <span data-ttu-id="12db5-121">Значение должно находиться в пределах от 1 до 30 включительно.</span><span class="sxs-lookup"><span data-stu-id="12db5-121">The value must be between 1 and 30, inclusive.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="12db5-122">Примечания</span><span class="sxs-lookup"><span data-stu-id="12db5-122">Remarks</span></span>

<span data-ttu-id="12db5-123">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.Этот элемент появился в Exchange Server 2010 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="12db5-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="12db5-124">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="12db5-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="12db5-125">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="12db5-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="12db5-126">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="12db5-126">Schema name</span></span>  <br/> |<span data-ttu-id="12db5-127">Схема Types</span><span class="sxs-lookup"><span data-stu-id="12db5-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="12db5-128">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="12db5-128">Validation file</span></span>  <br/> |<span data-ttu-id="12db5-129">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="12db5-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="12db5-130">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="12db5-130">Can be empty</span></span>  <br/> |<span data-ttu-id="12db5-131">False</span><span class="sxs-lookup"><span data-stu-id="12db5-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="12db5-132">См. также</span><span class="sxs-lookup"><span data-stu-id="12db5-132">See also</span></span>



[<span data-ttu-id="12db5-133">Операция GetStreamingEvents</span><span class="sxs-lookup"><span data-stu-id="12db5-133">GetStreamingEvents operation</span></span>](getstreamingevents-operation.md)


- [<span data-ttu-id="12db5-134">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="12db5-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

