---
title: ProcessRightAway
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ProcessRightAway
api_type:
- schema
ms.assetid: f6bba68b-ae4f-41c1-b3e7-c8a31cdb1b0c
description: Элемент ProcessRightAway указывает, будет ли ответ сразу после начала действия обработки на сервере или ли ответ после завершения действия. Этот элемент необходим для ответа отправку асинхронных запрошенное действие.
ms.openlocfilehash: 940f8e8fa0a53801ce1c3a45c3aecf1bdb6f519d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19834898"
---
# <a name="processrightaway"></a><span data-ttu-id="ffcde-104">ProcessRightAway</span><span class="sxs-lookup"><span data-stu-id="ffcde-104">ProcessRightAway</span></span>

<span data-ttu-id="ffcde-105">Элемент **ProcessRightAway** указывает, будет ли ответ сразу после начала действия обработки на сервере или ли ответ после завершения действия.</span><span class="sxs-lookup"><span data-stu-id="ffcde-105">The **ProcessRightAway** element indicates whether the response is sent as soon as the action starts processing on the server or whether the response is sent after the action has completed.</span></span> <span data-ttu-id="ffcde-106">Этот элемент необходим для ответа отправку асинхронных запрошенное действие.</span><span class="sxs-lookup"><span data-stu-id="ffcde-106">This element must be present for the response to be sent asynchronous to the requested action.</span></span> 
  
[<span data-ttu-id="ffcde-107">ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="ffcde-107">ApplyConversationAction</span></span>](applyconversationaction.md)
  
[<span data-ttu-id="ffcde-108">ConversationActions</span><span class="sxs-lookup"><span data-stu-id="ffcde-108">ConversationActions</span></span>](conversationactions.md)
  
[<span data-ttu-id="ffcde-109">ConversationAction</span><span class="sxs-lookup"><span data-stu-id="ffcde-109">ConversationAction</span></span>](conversationaction.md)
  
[<span data-ttu-id="ffcde-110">ProcessRightAway</span><span class="sxs-lookup"><span data-stu-id="ffcde-110">ProcessRightAway</span></span>](processrightaway.md)
  
```XML
<ProcessRightAway/>
```

 <span data-ttu-id="ffcde-111">**xs: Boolean**</span><span class="sxs-lookup"><span data-stu-id="ffcde-111">**xs:boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ffcde-112">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="ffcde-112">Attributes and elements</span></span>

<span data-ttu-id="ffcde-113">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="ffcde-113">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ffcde-114">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="ffcde-114">Attributes</span></span>

<span data-ttu-id="ffcde-115">Нет.</span><span class="sxs-lookup"><span data-stu-id="ffcde-115">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ffcde-116">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="ffcde-116">Child elements</span></span>

<span data-ttu-id="ffcde-117">Нет.</span><span class="sxs-lookup"><span data-stu-id="ffcde-117">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="ffcde-118">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="ffcde-118">Parent elements</span></span>

|<span data-ttu-id="ffcde-119">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="ffcde-119">**Element**</span></span>|<span data-ttu-id="ffcde-120">**Описание**</span><span class="sxs-lookup"><span data-stu-id="ffcde-120">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ffcde-121">ConversationAction</span><span class="sxs-lookup"><span data-stu-id="ffcde-121">ConversationAction</span></span>](conversationaction.md) <br/> |<span data-ttu-id="ffcde-122">Содержит одно действие должен применяться к разговора.</span><span class="sxs-lookup"><span data-stu-id="ffcde-122">Contains a single action to be applied to a single conversation.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="ffcde-123">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="ffcde-123">Text value</span></span>

<span data-ttu-id="ffcde-124">Текстовое значение **true,** указывает, что ответ сразу после начала действия обработки на сервере.</span><span class="sxs-lookup"><span data-stu-id="ffcde-124">A text value of **true** indicates that the response is sent as soon as the action starts processing on the server.</span></span> <span data-ttu-id="ffcde-125">Текстовое значение **false** указывает, что ответ после завершения действия.</span><span class="sxs-lookup"><span data-stu-id="ffcde-125">A text value of **false** indicates that the response is sent after the action has completed.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="ffcde-126">Замечания</span><span class="sxs-lookup"><span data-stu-id="ffcde-126">Remarks</span></span>

<span data-ttu-id="ffcde-127">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.Этот элемент появился в Exchange Server 2010 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="ffcde-127">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ffcde-128">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="ffcde-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ffcde-129">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="ffcde-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="ffcde-130">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="ffcde-130">Schema Name</span></span>  <br/> |<span data-ttu-id="ffcde-131">Схема Types</span><span class="sxs-lookup"><span data-stu-id="ffcde-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="ffcde-132">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="ffcde-132">Validation File</span></span>  <br/> |<span data-ttu-id="ffcde-133">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="ffcde-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="ffcde-134">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="ffcde-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="ffcde-135">False</span><span class="sxs-lookup"><span data-stu-id="ffcde-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ffcde-136">См. также</span><span class="sxs-lookup"><span data-stu-id="ffcde-136">See also</span></span>



[<span data-ttu-id="ffcde-137">Операция ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="ffcde-137">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)


- [<span data-ttu-id="ffcde-138">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="ffcde-138">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

