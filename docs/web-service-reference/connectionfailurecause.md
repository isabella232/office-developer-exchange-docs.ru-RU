---
title: коннектионфаилурекаусе
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ConnectionFailureCause
api_type:
- schema
ms.assetid: d2160c8a-015c-4964-b7f7-93478764a173
description: Элемент Коннектионфаилурекаусе указывает причину отключения от телефонного звонка.
ms.openlocfilehash: 54b4f5b89efdb42ef82dbef8f1af14a39c0ccc6a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761716"
---
# <a name="connectionfailurecause"></a><span data-ttu-id="d433f-103">коннектионфаилурекаусе</span><span class="sxs-lookup"><span data-stu-id="d433f-103">ConnectionFailureCause</span></span>

<span data-ttu-id="d433f-104">Элемент **коннектионфаилурекаусе** указывает причину отключения от телефонного звонка.</span><span class="sxs-lookup"><span data-stu-id="d433f-104">The **ConnectionFailureCause** element specifies the reason for a disconnection from a telephone call.</span></span> 
  
```xml
<ConnectionFailureCause>None or UserBusy or NoAnswer or Unavailable or Other</ConnectionFailureCause>
```

 <span data-ttu-id="d433f-105">**коннектионфаилурекаусетипе**</span><span class="sxs-lookup"><span data-stu-id="d433f-105">**ConnectionFailureCauseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d433f-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="d433f-106">Attributes and elements</span></span>

<span data-ttu-id="d433f-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="d433f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d433f-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="d433f-108">Attributes</span></span>

<span data-ttu-id="d433f-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="d433f-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d433f-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="d433f-110">Child elements</span></span>

<span data-ttu-id="d433f-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="d433f-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="d433f-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="d433f-112">Parent elements</span></span>

|<span data-ttu-id="d433f-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="d433f-113">**Element**</span></span>|<span data-ttu-id="d433f-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d433f-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d433f-115">фонекаллинформатион</span><span class="sxs-lookup"><span data-stu-id="d433f-115">PhoneCallInformation</span></span>](phonecallinformation.md) <br/> |<span data-ttu-id="d433f-116">Задает сведения о состоянии телефонного звонка.</span><span class="sxs-lookup"><span data-stu-id="d433f-116">Specifies the state information for a telephone call.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="d433f-117">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="d433f-117">Text value</span></span>

<span data-ttu-id="d433f-118">В следующей таблице приведены возможные значения для элемента **коннектионфаилурекаусе** .</span><span class="sxs-lookup"><span data-stu-id="d433f-118">The following table lists the possible values for the **ConnectionFailureCause** element.</span></span> 
  
<span data-ttu-id="d433f-119">**Значения элементов Коннектионфаилурекаусе**</span><span class="sxs-lookup"><span data-stu-id="d433f-119">**ConnectionFailureCause element values**</span></span>

|<span data-ttu-id="d433f-120">**Значение**</span><span class="sxs-lookup"><span data-stu-id="d433f-120">**Value**</span></span>|<span data-ttu-id="d433f-121">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d433f-121">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="d433f-122">Нет</span><span class="sxs-lookup"><span data-stu-id="d433f-122">None</span></span>  <br/> |<span data-ttu-id="d433f-123">Состояние вызова не отключено или причина отключения неизвестна.</span><span class="sxs-lookup"><span data-stu-id="d433f-123">Call state is not disconnected or the disconnect reason is not known.</span></span>  <br/> |
|<span data-ttu-id="d433f-124">усербуси</span><span class="sxs-lookup"><span data-stu-id="d433f-124">UserBusy</span></span>  <br/> |<span data-ttu-id="d433f-125">Линия вызываемой стороны занята.</span><span class="sxs-lookup"><span data-stu-id="d433f-125">The called party line was busy.</span></span>  <br/> |
|<span data-ttu-id="d433f-126">Ответ</span><span class="sxs-lookup"><span data-stu-id="d433f-126">NoAnswer</span></span>  <br/> |<span data-ttu-id="d433f-127">Вызываемая сторона не ответила.</span><span class="sxs-lookup"><span data-stu-id="d433f-127">The called party did not answer.</span></span>  <br/> |
|<span data-ttu-id="d433f-128">Выходе</span><span class="sxs-lookup"><span data-stu-id="d433f-128">Unavailable</span></span>  <br/> |<span data-ttu-id="d433f-129">Номер вызываемого абонента был недоступен.</span><span class="sxs-lookup"><span data-stu-id="d433f-129">The called party number was not available.</span></span>  <br/> |
|<span data-ttu-id="d433f-130">Другое</span><span class="sxs-lookup"><span data-stu-id="d433f-130">Other</span></span>  <br/> |<span data-ttu-id="d433f-131">Перехватить все для других причин отключения.</span><span class="sxs-lookup"><span data-stu-id="d433f-131">Catch-all for other disconnect reasons.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="d433f-132">Примечания</span><span class="sxs-lookup"><span data-stu-id="d433f-132">Remarks</span></span>

<span data-ttu-id="d433f-133">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="d433f-133">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d433f-134">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="d433f-134">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d433f-135">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="d433f-135">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d433f-136">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="d433f-136">Schema Name</span></span>  <br/> |<span data-ttu-id="d433f-137">Схема Types</span><span class="sxs-lookup"><span data-stu-id="d433f-137">Types schema</span></span>  <br/> |
|<span data-ttu-id="d433f-138">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="d433f-138">Validation File</span></span>  <br/> |<span data-ttu-id="d433f-139">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="d433f-139">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d433f-140">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="d433f-140">Can be Empty</span></span>  <br/> |<span data-ttu-id="d433f-141">False</span><span class="sxs-lookup"><span data-stu-id="d433f-141">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d433f-142">См. также</span><span class="sxs-lookup"><span data-stu-id="d433f-142">See also</span></span>



- [<span data-ttu-id="d433f-143">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="d433f-143">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

