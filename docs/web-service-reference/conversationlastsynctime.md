---
title: конверсатионластсинктиме
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
description: Элемент Конверсатионластсинктиме содержит дату и время последней синхронизации беседы. Этот элемент должен присутствовать при попытке удалить все элементы в беседе, полученные до указанного времени.
ms.openlocfilehash: f7cc6e205ab9936685d7b8c1f34129b799a53021
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44461431"
---
# <a name="conversationlastsynctime"></a><span data-ttu-id="e4dc4-104">конверсатионластсинктиме</span><span class="sxs-lookup"><span data-stu-id="e4dc4-104">ConversationLastSyncTime</span></span>

<span data-ttu-id="e4dc4-105">Элемент **конверсатионластсинктиме** содержит дату и время последней синхронизации беседы.</span><span class="sxs-lookup"><span data-stu-id="e4dc4-105">The **ConversationLastSyncTime** element contains the date and time that a conversation was last synchronized.</span></span> <span data-ttu-id="e4dc4-106">Этот элемент должен присутствовать при попытке удалить все элементы в беседе, полученные до указанного времени.</span><span class="sxs-lookup"><span data-stu-id="e4dc4-106">This element must be present when trying to delete all items in a conversation that were received up to the specified time.</span></span> 
  
[<span data-ttu-id="e4dc4-107">ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="e4dc4-107">ApplyConversationAction</span></span>](applyconversationaction.md)
  
[<span data-ttu-id="e4dc4-108">конверсатионактионс</span><span class="sxs-lookup"><span data-stu-id="e4dc4-108">ConversationActions</span></span>](conversationactions.md)
  
[<span data-ttu-id="e4dc4-109">конверсатионактион</span><span class="sxs-lookup"><span data-stu-id="e4dc4-109">ConversationAction</span></span>](conversationaction.md)
  
[<span data-ttu-id="e4dc4-110">конверсатионластсинктиме</span><span class="sxs-lookup"><span data-stu-id="e4dc4-110">ConversationLastSyncTime</span></span>](conversationlastsynctime.md)
  
```XML
<ConversationLastSyncTime/>
```

 <span data-ttu-id="e4dc4-111">**xs: dateTime**</span><span class="sxs-lookup"><span data-stu-id="e4dc4-111">**xs:dateTime**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e4dc4-112">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="e4dc4-112">Attributes and elements</span></span>

<span data-ttu-id="e4dc4-113">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="e4dc4-113">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e4dc4-114">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="e4dc4-114">Attributes</span></span>

<span data-ttu-id="e4dc4-115">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="e4dc4-115">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e4dc4-116">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="e4dc4-116">Child elements</span></span>

<span data-ttu-id="e4dc4-117">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="e4dc4-117">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="e4dc4-118">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="e4dc4-118">Parent elements</span></span>

|<span data-ttu-id="e4dc4-119">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="e4dc4-119">**Element**</span></span>|<span data-ttu-id="e4dc4-120">**Описание**</span><span class="sxs-lookup"><span data-stu-id="e4dc4-120">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e4dc4-121">конверсатионактион</span><span class="sxs-lookup"><span data-stu-id="e4dc4-121">ConversationAction</span></span>](conversationaction.md) <br/> |<span data-ttu-id="e4dc4-122">Содержит одно действие, которое будет применено к одной беседе.</span><span class="sxs-lookup"><span data-stu-id="e4dc4-122">Contains a single action to be applied to a single conversation.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="e4dc4-123">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="e4dc4-123">Text value</span></span>

<span data-ttu-id="e4dc4-124">Текстовое значение **конверсатионластсинктиме** указывает время последней синхронизации диалога.</span><span class="sxs-lookup"><span data-stu-id="e4dc4-124">The text value of the **ConversationLastSyncTime** indicates the last time the conversation was synchronized.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="e4dc4-125">Примечания</span><span class="sxs-lookup"><span data-stu-id="e4dc4-125">Remarks</span></span>

<span data-ttu-id="e4dc4-126">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.Этот элемент появился в Exchange Server 2010 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="e4dc4-126">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e4dc4-127">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="e4dc4-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e4dc4-128">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="e4dc4-128">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="e4dc4-129">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="e4dc4-129">Schema Name</span></span>  <br/> |<span data-ttu-id="e4dc4-130">Схема Types</span><span class="sxs-lookup"><span data-stu-id="e4dc4-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="e4dc4-131">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="e4dc4-131">Validation File</span></span>  <br/> |<span data-ttu-id="e4dc4-132">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="e4dc4-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="e4dc4-133">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="e4dc4-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="e4dc4-134">False</span><span class="sxs-lookup"><span data-stu-id="e4dc4-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e4dc4-135">См. также</span><span class="sxs-lookup"><span data-stu-id="e4dc4-135">See also</span></span>



[<span data-ttu-id="e4dc4-136">Операция ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="e4dc4-136">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)


- [<span data-ttu-id="e4dc4-137">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="e4dc4-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

