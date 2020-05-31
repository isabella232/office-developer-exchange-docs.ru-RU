---
title: процессригхтавай
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
description: Элемент Процессригхтавай указывает, отправляется ли ответ сразу после того, как действие начнет обработку на сервере или отправило ли ответ после завершения действия. Этот элемент должен присутствовать, чтобы ответ был асинхронно отправлен в запрошенное действие.
ms.openlocfilehash: 940f8e8fa0a53801ce1c3a45c3aecf1bdb6f519d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834898"
---
# <a name="processrightaway"></a><span data-ttu-id="984cc-104">процессригхтавай</span><span class="sxs-lookup"><span data-stu-id="984cc-104">ProcessRightAway</span></span>

<span data-ttu-id="984cc-105">Элемент **процессригхтавай** указывает, отправляется ли ответ сразу после того, как действие начнет обработку на сервере или отправило ли ответ после завершения действия.</span><span class="sxs-lookup"><span data-stu-id="984cc-105">The **ProcessRightAway** element indicates whether the response is sent as soon as the action starts processing on the server or whether the response is sent after the action has completed.</span></span> <span data-ttu-id="984cc-106">Этот элемент должен присутствовать, чтобы ответ был асинхронно отправлен в запрошенное действие.</span><span class="sxs-lookup"><span data-stu-id="984cc-106">This element must be present for the response to be sent asynchronous to the requested action.</span></span> 
  
[<span data-ttu-id="984cc-107">ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="984cc-107">ApplyConversationAction</span></span>](applyconversationaction.md)
  
[<span data-ttu-id="984cc-108">конверсатионактионс</span><span class="sxs-lookup"><span data-stu-id="984cc-108">ConversationActions</span></span>](conversationactions.md)
  
[<span data-ttu-id="984cc-109">конверсатионактион</span><span class="sxs-lookup"><span data-stu-id="984cc-109">ConversationAction</span></span>](conversationaction.md)
  
[<span data-ttu-id="984cc-110">процессригхтавай</span><span class="sxs-lookup"><span data-stu-id="984cc-110">ProcessRightAway</span></span>](processrightaway.md)
  
```XML
<ProcessRightAway/>
```

 <span data-ttu-id="984cc-111">**xs: Boolean**</span><span class="sxs-lookup"><span data-stu-id="984cc-111">**xs:boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="984cc-112">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="984cc-112">Attributes and elements</span></span>

<span data-ttu-id="984cc-113">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="984cc-113">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="984cc-114">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="984cc-114">Attributes</span></span>

<span data-ttu-id="984cc-115">Нет.</span><span class="sxs-lookup"><span data-stu-id="984cc-115">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="984cc-116">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="984cc-116">Child elements</span></span>

<span data-ttu-id="984cc-117">Нет.</span><span class="sxs-lookup"><span data-stu-id="984cc-117">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="984cc-118">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="984cc-118">Parent elements</span></span>

|<span data-ttu-id="984cc-119">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="984cc-119">**Element**</span></span>|<span data-ttu-id="984cc-120">**Описание**</span><span class="sxs-lookup"><span data-stu-id="984cc-120">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="984cc-121">конверсатионактион</span><span class="sxs-lookup"><span data-stu-id="984cc-121">ConversationAction</span></span>](conversationaction.md) <br/> |<span data-ttu-id="984cc-122">Содержит одно действие, которое будет применено к одной беседе.</span><span class="sxs-lookup"><span data-stu-id="984cc-122">Contains a single action to be applied to a single conversation.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="984cc-123">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="984cc-123">Text value</span></span>

<span data-ttu-id="984cc-124">Текстовое значение **true** указывает на то, что ответ отправляется сразу после того, как действие начнет обработку на сервере.</span><span class="sxs-lookup"><span data-stu-id="984cc-124">A text value of **true** indicates that the response is sent as soon as the action starts processing on the server.</span></span> <span data-ttu-id="984cc-125">Текстовое значение **false** указывает, что ответ отправляется после выполнения действия.</span><span class="sxs-lookup"><span data-stu-id="984cc-125">A text value of **false** indicates that the response is sent after the action has completed.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="984cc-126">Примечания</span><span class="sxs-lookup"><span data-stu-id="984cc-126">Remarks</span></span>

<span data-ttu-id="984cc-127">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.Этот элемент появился в Exchange Server 2010 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="984cc-127">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="984cc-128">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="984cc-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="984cc-129">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="984cc-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="984cc-130">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="984cc-130">Schema Name</span></span>  <br/> |<span data-ttu-id="984cc-131">Схема Types</span><span class="sxs-lookup"><span data-stu-id="984cc-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="984cc-132">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="984cc-132">Validation File</span></span>  <br/> |<span data-ttu-id="984cc-133">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="984cc-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="984cc-134">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="984cc-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="984cc-135">False</span><span class="sxs-lookup"><span data-stu-id="984cc-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="984cc-136">См. также</span><span class="sxs-lookup"><span data-stu-id="984cc-136">See also</span></span>



[<span data-ttu-id="984cc-137">Операция ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="984cc-137">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)


- [<span data-ttu-id="984cc-138">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="984cc-138">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

