---
title: глобалимпортанце
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GlobalImportance
api_type:
- schema
ms.assetid: 8bcec699-e771-4f38-b7d9-61f324af1b4e
description: Элемент Глобалимпортанце содержит совокупную важность для всех элементов бесед в почтовом ящике.
ms.openlocfilehash: c9cdcf20fd3e6eca9ab501cbc747544a4d7b7ded
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833731"
---
# <a name="globalimportance"></a><span data-ttu-id="163d2-103">глобалимпортанце</span><span class="sxs-lookup"><span data-stu-id="163d2-103">GlobalImportance</span></span>

<span data-ttu-id="163d2-104">Элемент **глобалимпортанце** содержит совокупную важность для всех элементов бесед в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="163d2-104">The **GlobalImportance** element contains the aggregated importance for all conversation items in a mailbox.</span></span> 
  
[<span data-ttu-id="163d2-105">финдконверсатионреспонсе</span><span class="sxs-lookup"><span data-stu-id="163d2-105">FindConversationResponse</span></span>](findconversationresponse.md)
  
[<span data-ttu-id="163d2-106">Conversations</span><span class="sxs-lookup"><span data-stu-id="163d2-106">Conversations</span></span>](conversations-ex15websvcsotherref.md)
  
[<span data-ttu-id="163d2-107">Беседы (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="163d2-107">Conversation (ConversationType)</span></span>](conversation-conversationtype.md)
  
[<span data-ttu-id="163d2-108">глобалимпортанце</span><span class="sxs-lookup"><span data-stu-id="163d2-108">GlobalImportance</span></span>](globalimportance.md)
  
```XML
<GlobalImportance> Low | Normal | High </GlobalImportance>
```

 <span data-ttu-id="163d2-109">**импортанцечоицестипе**</span><span class="sxs-lookup"><span data-stu-id="163d2-109">**ImportanceChoicesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="163d2-110">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="163d2-110">Attributes and elements</span></span>

<span data-ttu-id="163d2-111">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="163d2-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="163d2-112">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="163d2-112">Attributes</span></span>

<span data-ttu-id="163d2-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="163d2-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="163d2-114">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="163d2-114">Child elements</span></span>

<span data-ttu-id="163d2-115">Нет.</span><span class="sxs-lookup"><span data-stu-id="163d2-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="163d2-116">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="163d2-116">Parent elements</span></span>

|<span data-ttu-id="163d2-117">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="163d2-117">**Element**</span></span>|<span data-ttu-id="163d2-118">**Описание**</span><span class="sxs-lookup"><span data-stu-id="163d2-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="163d2-119">Беседы (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="163d2-119">Conversation (ConversationType)</span></span>](conversation-conversationtype.md) <br/> |<span data-ttu-id="163d2-120">Представляет одну беседу.</span><span class="sxs-lookup"><span data-stu-id="163d2-120">Represents a single conversation.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="163d2-121">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="163d2-121">Text value</span></span>

<span data-ttu-id="163d2-122">Необходимо указать текстовое значение.</span><span class="sxs-lookup"><span data-stu-id="163d2-122">A text value is required.</span></span> <span data-ttu-id="163d2-123">Ниже приведены возможные значения для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="163d2-123">The following are the possible values for this element:</span></span>
  
- <span data-ttu-id="163d2-124">Низкий</span><span class="sxs-lookup"><span data-stu-id="163d2-124">Low</span></span>
    
- <span data-ttu-id="163d2-125">Normal</span><span class="sxs-lookup"><span data-stu-id="163d2-125">Normal</span></span>
    
- <span data-ttu-id="163d2-126">Высокий</span><span class="sxs-lookup"><span data-stu-id="163d2-126">High</span></span>
    
## <a name="remarks"></a><span data-ttu-id="163d2-127">Примечания</span><span class="sxs-lookup"><span data-stu-id="163d2-127">Remarks</span></span>

<span data-ttu-id="163d2-128">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.Этот элемент появился в Exchange Server 2010 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="163d2-128">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="163d2-129">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="163d2-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="163d2-130">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="163d2-130">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="163d2-131">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="163d2-131">Schema name</span></span>  <br/> |<span data-ttu-id="163d2-132">Схема Types</span><span class="sxs-lookup"><span data-stu-id="163d2-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="163d2-133">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="163d2-133">Validation file</span></span>  <br/> |<span data-ttu-id="163d2-134">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="163d2-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="163d2-135">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="163d2-135">Can be empty</span></span>  <br/> |<span data-ttu-id="163d2-136">False</span><span class="sxs-lookup"><span data-stu-id="163d2-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="163d2-137">См. также</span><span class="sxs-lookup"><span data-stu-id="163d2-137">See also</span></span>



[<span data-ttu-id="163d2-138">FindConversation Operation</span><span class="sxs-lookup"><span data-stu-id="163d2-138">FindConversation operation</span></span>](findconversation-operation.md)
  
[<span data-ttu-id="163d2-139">Операция ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="163d2-139">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)


[<span data-ttu-id="163d2-140">Conversations in EWS</span><span class="sxs-lookup"><span data-stu-id="163d2-140">Conversations in EWS</span></span>](http://msdn.microsoft.com/library/91e64629-db6c-4c94-9dcb-d386232e8467%28Office.15%29.aspx)

