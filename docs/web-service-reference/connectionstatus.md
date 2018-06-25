---
title: ConnectionStatus
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ConnectionStatus
api_type:
- schema
ms.assetid: 4300f9d6-8bf9-48c2-9f07-d80197864e17
description: Элемент ConnectionStatus с описанием текст состояния потоковой передачи подписки.
ms.openlocfilehash: 567308d79eaccba24230deddf5d78a724b8746af
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761718"
---
# <a name="connectionstatus"></a><span data-ttu-id="4cb10-103">ConnectionStatus</span><span class="sxs-lookup"><span data-stu-id="4cb10-103">ConnectionStatus</span></span>

<span data-ttu-id="4cb10-104">Элемент **ConnectionStatus** с описанием текст состояния потоковой передачи подписки.</span><span class="sxs-lookup"><span data-stu-id="4cb10-104">The **ConnectionStatus** element provides a text description of the status of a streaming subscription.</span></span> 
  
```xml
<ConnectionStatus>OK or Closed</ConnectionStatus>
```

 <span data-ttu-id="4cb10-105">**ConnectionStatusType**</span><span class="sxs-lookup"><span data-stu-id="4cb10-105">**ConnectionStatusType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4cb10-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="4cb10-106">Attributes and elements</span></span>

<span data-ttu-id="4cb10-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="4cb10-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4cb10-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="4cb10-108">Attributes</span></span>

<span data-ttu-id="4cb10-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="4cb10-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4cb10-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="4cb10-110">Child elements</span></span>

<span data-ttu-id="4cb10-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="4cb10-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="4cb10-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="4cb10-112">Parent elements</span></span>

|<span data-ttu-id="4cb10-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="4cb10-113">**Element**</span></span>|<span data-ttu-id="4cb10-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="4cb10-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4cb10-115">GetStreamingEventsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="4cb10-115">GetStreamingEventsResponseMessage</span></span>](getstreamingeventsresponsemessage.md) <br/> |<span data-ttu-id="4cb10-116">Содержит состояние и результат одного запроса [GetStreamingEvents операции](getstreamingevents-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="4cb10-116">Contains the status and result of a single [GetStreamingEvents operation](getstreamingevents-operation.md) request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="4cb10-117">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="4cb10-117">Text value</span></span>

<span data-ttu-id="4cb10-118">Текстовое значение является обязательным.</span><span class="sxs-lookup"><span data-stu-id="4cb10-118">A text value is required.</span></span> <span data-ttu-id="4cb10-119">Ниже приведены возможные значения для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="4cb10-119">The following are the possible text values for this element:</span></span>
  
- <span data-ttu-id="4cb10-120">OK</span><span class="sxs-lookup"><span data-stu-id="4cb10-120">OK</span></span>
    
- <span data-ttu-id="4cb10-121">Закрыт</span><span class="sxs-lookup"><span data-stu-id="4cb10-121">Closed</span></span>
    
## <a name="remarks"></a><span data-ttu-id="4cb10-122">Замечания</span><span class="sxs-lookup"><span data-stu-id="4cb10-122">Remarks</span></span>

<span data-ttu-id="4cb10-123">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.Этот элемент появился в Exchange Server 2010 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="4cb10-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4cb10-124">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="4cb10-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4cb10-125">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="4cb10-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="4cb10-126">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="4cb10-126">Schema Name</span></span>  <br/> |<span data-ttu-id="4cb10-127">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="4cb10-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="4cb10-128">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="4cb10-128">Validation File</span></span>  <br/> |<span data-ttu-id="4cb10-129">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="4cb10-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="4cb10-130">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="4cb10-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="4cb10-131">False</span><span class="sxs-lookup"><span data-stu-id="4cb10-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="4cb10-132">См. также</span><span class="sxs-lookup"><span data-stu-id="4cb10-132">See also</span></span>



[<span data-ttu-id="4cb10-133">Операция GetStreamingEvents</span><span class="sxs-lookup"><span data-stu-id="4cb10-133">GetStreamingEvents operation</span></span>](getstreamingevents-operation.md)


- [<span data-ttu-id="4cb10-134">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="4cb10-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

