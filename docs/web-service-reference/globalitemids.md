---
title: глобалитемидс
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GlobalItemIds
api_type:
- schema
ms.assetid: b0f03ce0-a4c3-47de-9360-a880a3606e42
description: Элемент Глобалитемидс содержит коллекцию идентификаторов элементов для всех элементов бесед в почтовом ящике.
ms.openlocfilehash: 064ebc4c612aaf569eafa56e57a27cf7153f2130
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833737"
---
# <a name="globalitemids"></a><span data-ttu-id="3e6d0-103">глобалитемидс</span><span class="sxs-lookup"><span data-stu-id="3e6d0-103">GlobalItemIds</span></span>

<span data-ttu-id="3e6d0-104">Элемент **глобалитемидс** содержит коллекцию идентификаторов элементов для всех элементов бесед в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="3e6d0-104">The **GlobalItemIds** element contains the collection of item identifiers for all conversation items in a mailbox.</span></span> 
  
[<span data-ttu-id="3e6d0-105">финдконверсатионреспонсе</span><span class="sxs-lookup"><span data-stu-id="3e6d0-105">FindConversationResponse</span></span>](findconversationresponse.md)
  
[<span data-ttu-id="3e6d0-106">Conversations</span><span class="sxs-lookup"><span data-stu-id="3e6d0-106">Conversations</span></span>](conversations-ex15websvcsotherref.md)
  
[<span data-ttu-id="3e6d0-107">Беседы (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="3e6d0-107">Conversation (ConversationType)</span></span>](conversation-conversationtype.md)
  
[<span data-ttu-id="3e6d0-108">глобалитемидс</span><span class="sxs-lookup"><span data-stu-id="3e6d0-108">GlobalItemIds</span></span>](globalitemids.md)
  
```XML
<ItemIds>
   <ItemId/>
   <OccurrenceItemId/>
   <RecurringMasterItemId/>
</ItemIds>
```

 <span data-ttu-id="3e6d0-109">**нонемптяррайофбасеитемидстипе**</span><span class="sxs-lookup"><span data-stu-id="3e6d0-109">**NonEmptyArrayOfBaseItemIdsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3e6d0-110">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="3e6d0-110">Attributes and elements</span></span>

<span data-ttu-id="3e6d0-111">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="3e6d0-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3e6d0-112">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="3e6d0-112">Attributes</span></span>

<span data-ttu-id="3e6d0-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="3e6d0-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3e6d0-114">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="3e6d0-114">Child elements</span></span>

|<span data-ttu-id="3e6d0-115">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="3e6d0-115">**Element**</span></span>|<span data-ttu-id="3e6d0-116">**Описание**</span><span class="sxs-lookup"><span data-stu-id="3e6d0-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3e6d0-117">Идентификатор</span><span class="sxs-lookup"><span data-stu-id="3e6d0-117">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="3e6d0-118">Содержит уникальный идентификатор и ключ изменения элемента в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="3e6d0-118">Contains the unique identifier and change key of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="3e6d0-119">оккурренцеитемид</span><span class="sxs-lookup"><span data-stu-id="3e6d0-119">OccurrenceItemId</span></span>](occurrenceitemid.md) <br/> |<span data-ttu-id="3e6d0-120">Определяет один экземпляр повторяющегося элемента.</span><span class="sxs-lookup"><span data-stu-id="3e6d0-120">Identifies a single occurrence of a recurring item.</span></span>  <br/> |
|[<span data-ttu-id="3e6d0-121">рекуррингмастеритемид</span><span class="sxs-lookup"><span data-stu-id="3e6d0-121">RecurringMasterItemId</span></span>](recurringmasteritemid.md) <br/> |<span data-ttu-id="3e6d0-122">Определяет элемент шаблона повторения, определив один из идентификаторов связанных элементов вхождения.</span><span class="sxs-lookup"><span data-stu-id="3e6d0-122">Identifies a recurrence master item by identifying one of its related occurrence items' identifiers.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="3e6d0-123">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="3e6d0-123">Parent elements</span></span>

|<span data-ttu-id="3e6d0-124">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="3e6d0-124">**Element**</span></span>|<span data-ttu-id="3e6d0-125">**Описание**</span><span class="sxs-lookup"><span data-stu-id="3e6d0-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3e6d0-126">Беседы (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="3e6d0-126">Conversation (ConversationType)</span></span>](conversation-conversationtype.md) <br/> |<span data-ttu-id="3e6d0-127">Представляет одну беседу.</span><span class="sxs-lookup"><span data-stu-id="3e6d0-127">Represents a single conversation.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="3e6d0-128">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="3e6d0-128">Text value</span></span>

<span data-ttu-id="3e6d0-129">Нет.</span><span class="sxs-lookup"><span data-stu-id="3e6d0-129">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="3e6d0-130">Примечания</span><span class="sxs-lookup"><span data-stu-id="3e6d0-130">Remarks</span></span>

<span data-ttu-id="3e6d0-131">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.Этот элемент появился в Exchange Server 2010 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="3e6d0-131">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3e6d0-132">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="3e6d0-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3e6d0-133">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="3e6d0-133">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="3e6d0-134">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="3e6d0-134">Schema name</span></span>  <br/> |<span data-ttu-id="3e6d0-135">Схема Types</span><span class="sxs-lookup"><span data-stu-id="3e6d0-135">Types schema</span></span>  <br/> |
|<span data-ttu-id="3e6d0-136">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="3e6d0-136">Validation file</span></span>  <br/> |<span data-ttu-id="3e6d0-137">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="3e6d0-137">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="3e6d0-138">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="3e6d0-138">Can be empty</span></span>  <br/> |<span data-ttu-id="3e6d0-139">False</span><span class="sxs-lookup"><span data-stu-id="3e6d0-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3e6d0-140">См. также</span><span class="sxs-lookup"><span data-stu-id="3e6d0-140">See also</span></span>



[<span data-ttu-id="3e6d0-141">FindConversation Operation</span><span class="sxs-lookup"><span data-stu-id="3e6d0-141">FindConversation operation</span></span>](findconversation-operation.md)
  
[<span data-ttu-id="3e6d0-142">Операция ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="3e6d0-142">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)


[<span data-ttu-id="3e6d0-143">Conversations in EWS</span><span class="sxs-lookup"><span data-stu-id="3e6d0-143">Conversations in EWS</span></span>](http://msdn.microsoft.com/library/91e64629-db6c-4c94-9dcb-d386232e8467%28Office.15%29.aspx)

