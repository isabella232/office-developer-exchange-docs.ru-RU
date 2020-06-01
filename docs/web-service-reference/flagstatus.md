---
title: FlagStatus
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FlagStatus
api_type:
- schema
ms.assetid: d5907ec5-3a60-4d83-bf85-406c54f95eb7
description: Элемент Флагстатус содержит сводный статус флага для элементов беседы в текущей папке.
ms.openlocfilehash: e65849c4909292c07450f8578fe7a7065c98ab44
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44466215"
---
# <a name="flagstatus"></a><span data-ttu-id="7d460-103">FlagStatus</span><span class="sxs-lookup"><span data-stu-id="7d460-103">FlagStatus</span></span>

<span data-ttu-id="7d460-104">Элемент **флагстатус** содержит сводный статус флага для элементов беседы в текущей папке.</span><span class="sxs-lookup"><span data-stu-id="7d460-104">The **FlagStatus** element contains the aggregated flag status for conversation items in the current folder.</span></span> 
  
[<span data-ttu-id="7d460-105">финдконверсатионреспонсе</span><span class="sxs-lookup"><span data-stu-id="7d460-105">FindConversationResponse</span></span>](findconversationresponse.md)
  
[<span data-ttu-id="7d460-106">Conversations</span><span class="sxs-lookup"><span data-stu-id="7d460-106">Conversations</span></span>](conversations-ex15websvcsotherref.md)
  
[<span data-ttu-id="7d460-107">Беседы (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="7d460-107">Conversation (ConversationType)</span></span>](conversation-conversationtype.md)
  
[<span data-ttu-id="7d460-108">FlagStatus</span><span class="sxs-lookup"><span data-stu-id="7d460-108">FlagStatus</span></span>](flagstatus.md)
  
```XML
<FlagStatus> NotFlagged | Flagged | Complete </FlagStatus>
```

 <span data-ttu-id="7d460-109">**флагстатустипе**</span><span class="sxs-lookup"><span data-stu-id="7d460-109">**FlagStatusType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7d460-110">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="7d460-110">Attributes and elements</span></span>

<span data-ttu-id="7d460-111">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="7d460-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7d460-112">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="7d460-112">Attributes</span></span>

<span data-ttu-id="7d460-113">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="7d460-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7d460-114">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="7d460-114">Child elements</span></span>

<span data-ttu-id="7d460-115">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="7d460-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="7d460-116">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="7d460-116">Parent elements</span></span>

|<span data-ttu-id="7d460-117">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="7d460-117">**Element**</span></span>|<span data-ttu-id="7d460-118">**Описание**</span><span class="sxs-lookup"><span data-stu-id="7d460-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7d460-119">Беседы (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="7d460-119">Conversation (ConversationType)</span></span>](conversation-conversationtype.md) <br/> |<span data-ttu-id="7d460-120">Представляет одну беседу.</span><span class="sxs-lookup"><span data-stu-id="7d460-120">Represents a single conversation.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="7d460-121">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="7d460-121">Text value</span></span>

<span data-ttu-id="7d460-122">Текстовое значение элемента **флагстатус** — это сводный статус флага для элементов беседы в текущей папке.</span><span class="sxs-lookup"><span data-stu-id="7d460-122">The text value of the **FlagStatus** element is the aggregated flag status for conversation items in the current folder.</span></span> <span data-ttu-id="7d460-123">Ниже приведены возможные текстовые значения.</span><span class="sxs-lookup"><span data-stu-id="7d460-123">The following are the possible text values:</span></span> 
  
- <span data-ttu-id="7d460-124">**Нотфлагжед** — указывает состояние "без отметки".</span><span class="sxs-lookup"><span data-stu-id="7d460-124">**NotFlagged** - Indicates the not-flagged status.</span></span> 
    
- <span data-ttu-id="7d460-125">**Отмечено** — указывает на состояние помечено.</span><span class="sxs-lookup"><span data-stu-id="7d460-125">**Flagged** - Indicates the flagged status.</span></span> 
    
- <span data-ttu-id="7d460-126">**Complete** — полный статус флага.</span><span class="sxs-lookup"><span data-stu-id="7d460-126">**Complete** - Indicates the complete flag status.</span></span> 
    
## <a name="remarks"></a><span data-ttu-id="7d460-127">Примечания</span><span class="sxs-lookup"><span data-stu-id="7d460-127">Remarks</span></span>

<span data-ttu-id="7d460-128">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.Этот элемент появился в Exchange Server 2010 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="7d460-128">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7d460-129">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="7d460-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7d460-130">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="7d460-130">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="7d460-131">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="7d460-131">Schema name</span></span>  <br/> |<span data-ttu-id="7d460-132">Схема Types</span><span class="sxs-lookup"><span data-stu-id="7d460-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="7d460-133">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="7d460-133">Validation file</span></span>  <br/> |<span data-ttu-id="7d460-134">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="7d460-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="7d460-135">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="7d460-135">Can be empty</span></span>  <br/> |<span data-ttu-id="7d460-136">False</span><span class="sxs-lookup"><span data-stu-id="7d460-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7d460-137">См. также</span><span class="sxs-lookup"><span data-stu-id="7d460-137">See also</span></span>



[<span data-ttu-id="7d460-138">FindConversation Operation</span><span class="sxs-lookup"><span data-stu-id="7d460-138">FindConversation operation</span></span>](findconversation-operation.md)
  
[<span data-ttu-id="7d460-139">Операция ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="7d460-139">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)


[<span data-ttu-id="7d460-140">Conversations in EWS</span><span class="sxs-lookup"><span data-stu-id="7d460-140">Conversations in EWS</span></span>](https://msdn.microsoft.com/library/91e64629-db6c-4c94-9dcb-d386232e8467%28Office.15%29.aspx)

