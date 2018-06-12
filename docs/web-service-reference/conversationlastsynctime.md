---
title: ConversationLastSyncTime
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ConversationLastSyncTime
api_type:
- schema
ms.assetid: 90f8f9e3-5fc6-4a6a-bdfb-fc91fa51f8a2
description: Элемент ConversationLastSyncTime содержит дату и время последнего синхронизирована беседы. Этот элемент должен присутствовать при попытке удаления всех элементов в беседе, которые были получены до заданного времени.
ms.openlocfilehash: 3b086d69ac0ef307059df4902e65f796c63733d1
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761819"
---
# <a name="conversationlastsynctime"></a><span data-ttu-id="f268b-104">ConversationLastSyncTime</span><span class="sxs-lookup"><span data-stu-id="f268b-104">ConversationLastSyncTime</span></span>

<span data-ttu-id="f268b-105">Элемент **ConversationLastSyncTime** содержит дату и время последнего синхронизирована беседы.</span><span class="sxs-lookup"><span data-stu-id="f268b-105">The **ConversationLastSyncTime** element contains the date and time that a conversation was last synchronized.</span></span> <span data-ttu-id="f268b-106">Этот элемент должен присутствовать при попытке удаления всех элементов в беседе, которые были получены до заданного времени.</span><span class="sxs-lookup"><span data-stu-id="f268b-106">This element must be present when trying to delete all items in a conversation that were received up to the specified time.</span></span> 
  
[<span data-ttu-id="f268b-107">ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="f268b-107">ApplyConversationAction</span></span>](applyconversationaction.md)
  
[<span data-ttu-id="f268b-108">ConversationActions</span><span class="sxs-lookup"><span data-stu-id="f268b-108">ConversationActions</span></span>](conversationactions.md)
  
[<span data-ttu-id="f268b-109">ConversationAction</span><span class="sxs-lookup"><span data-stu-id="f268b-109">ConversationAction</span></span>](conversationaction.md)
  
[<span data-ttu-id="f268b-110">ConversationLastSyncTime</span><span class="sxs-lookup"><span data-stu-id="f268b-110">ConversationLastSyncTime</span></span>](conversationlastsynctime.md)
  
```XML
<ConversationLastSyncTime/>
```

 <span data-ttu-id="f268b-111">**xs: DateTime**</span><span class="sxs-lookup"><span data-stu-id="f268b-111">**xs:dateTime**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f268b-112">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="f268b-112">Attributes and elements</span></span>

<span data-ttu-id="f268b-113">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="f268b-113">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f268b-114">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="f268b-114">Attributes</span></span>

<span data-ttu-id="f268b-115">Нет.</span><span class="sxs-lookup"><span data-stu-id="f268b-115">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f268b-116">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="f268b-116">Child elements</span></span>

<span data-ttu-id="f268b-117">Нет.</span><span class="sxs-lookup"><span data-stu-id="f268b-117">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="f268b-118">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="f268b-118">Parent elements</span></span>

|<span data-ttu-id="f268b-119">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="f268b-119">**Element**</span></span>|<span data-ttu-id="f268b-120">**Описание**</span><span class="sxs-lookup"><span data-stu-id="f268b-120">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f268b-121">ConversationAction</span><span class="sxs-lookup"><span data-stu-id="f268b-121">ConversationAction</span></span>](conversationaction.md) <br/> |<span data-ttu-id="f268b-122">Содержит одно действие должен применяться к разговора.</span><span class="sxs-lookup"><span data-stu-id="f268b-122">Contains a single action to be applied to a single conversation.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="f268b-123">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="f268b-123">Text value</span></span>

<span data-ttu-id="f268b-124">Текстовое значение **ConversationLastSyncTime** указывает время последнего синхронизации беседу.</span><span class="sxs-lookup"><span data-stu-id="f268b-124">The text value of the **ConversationLastSyncTime** indicates the last time the conversation was synchronized.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="f268b-125">Замечания</span><span class="sxs-lookup"><span data-stu-id="f268b-125">Remarks</span></span>

<span data-ttu-id="f268b-126">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.Этот элемент появился в Exchange Server 2010 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="f268b-126">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f268b-127">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="f268b-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f268b-128">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="f268b-128">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="f268b-129">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="f268b-129">Schema Name</span></span>  <br/> |<span data-ttu-id="f268b-130">Схема Types</span><span class="sxs-lookup"><span data-stu-id="f268b-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="f268b-131">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="f268b-131">Validation File</span></span>  <br/> |<span data-ttu-id="f268b-132">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="f268b-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="f268b-133">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="f268b-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="f268b-134">False</span><span class="sxs-lookup"><span data-stu-id="f268b-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f268b-135">См. также</span><span class="sxs-lookup"><span data-stu-id="f268b-135">See also</span></span>



[<span data-ttu-id="f268b-136">Операция ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="f268b-136">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)


- [<span data-ttu-id="f268b-137">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="f268b-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

