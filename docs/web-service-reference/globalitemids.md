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
ms.openlocfilehash: aa656e7f2fb78dafe5bf6013c1f7ad14e2372ba1
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459428"
---
# <a name="globalitemids"></a><span data-ttu-id="68a70-103">глобалитемидс</span><span class="sxs-lookup"><span data-stu-id="68a70-103">GlobalItemIds</span></span>

<span data-ttu-id="68a70-104">Элемент **глобалитемидс** содержит коллекцию идентификаторов элементов для всех элементов бесед в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="68a70-104">The **GlobalItemIds** element contains the collection of item identifiers for all conversation items in a mailbox.</span></span> 
  
[<span data-ttu-id="68a70-105">финдконверсатионреспонсе</span><span class="sxs-lookup"><span data-stu-id="68a70-105">FindConversationResponse</span></span>](findconversationresponse.md)
  
[<span data-ttu-id="68a70-106">Conversations</span><span class="sxs-lookup"><span data-stu-id="68a70-106">Conversations</span></span>](conversations-ex15websvcsotherref.md)
  
[<span data-ttu-id="68a70-107">Беседы (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="68a70-107">Conversation (ConversationType)</span></span>](conversation-conversationtype.md)
  
[<span data-ttu-id="68a70-108">глобалитемидс</span><span class="sxs-lookup"><span data-stu-id="68a70-108">GlobalItemIds</span></span>](globalitemids.md)
  
```XML
<ItemIds>
   <ItemId/>
   <OccurrenceItemId/>
   <RecurringMasterItemId/>
</ItemIds>
```

 <span data-ttu-id="68a70-109">**нонемптяррайофбасеитемидстипе**</span><span class="sxs-lookup"><span data-stu-id="68a70-109">**NonEmptyArrayOfBaseItemIdsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="68a70-110">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="68a70-110">Attributes and elements</span></span>

<span data-ttu-id="68a70-111">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="68a70-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="68a70-112">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="68a70-112">Attributes</span></span>

<span data-ttu-id="68a70-113">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="68a70-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="68a70-114">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="68a70-114">Child elements</span></span>

|<span data-ttu-id="68a70-115">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="68a70-115">**Element**</span></span>|<span data-ttu-id="68a70-116">**Описание**</span><span class="sxs-lookup"><span data-stu-id="68a70-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="68a70-117">Идентификатор</span><span class="sxs-lookup"><span data-stu-id="68a70-117">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="68a70-118">Содержит уникальный идентификатор и ключ изменения элемента в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="68a70-118">Contains the unique identifier and change key of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="68a70-119">оккурренцеитемид</span><span class="sxs-lookup"><span data-stu-id="68a70-119">OccurrenceItemId</span></span>](occurrenceitemid.md) <br/> |<span data-ttu-id="68a70-120">Определяет один экземпляр повторяющегося элемента.</span><span class="sxs-lookup"><span data-stu-id="68a70-120">Identifies a single occurrence of a recurring item.</span></span>  <br/> |
|[<span data-ttu-id="68a70-121">рекуррингмастеритемид</span><span class="sxs-lookup"><span data-stu-id="68a70-121">RecurringMasterItemId</span></span>](recurringmasteritemid.md) <br/> |<span data-ttu-id="68a70-122">Определяет элемент шаблона повторения, определив один из идентификаторов связанных элементов вхождения.</span><span class="sxs-lookup"><span data-stu-id="68a70-122">Identifies a recurrence master item by identifying one of its related occurrence items' identifiers.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="68a70-123">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="68a70-123">Parent elements</span></span>

|<span data-ttu-id="68a70-124">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="68a70-124">**Element**</span></span>|<span data-ttu-id="68a70-125">**Описание**</span><span class="sxs-lookup"><span data-stu-id="68a70-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="68a70-126">Беседы (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="68a70-126">Conversation (ConversationType)</span></span>](conversation-conversationtype.md) <br/> |<span data-ttu-id="68a70-127">Представляет одну беседу.</span><span class="sxs-lookup"><span data-stu-id="68a70-127">Represents a single conversation.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="68a70-128">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="68a70-128">Text value</span></span>

<span data-ttu-id="68a70-129">Нет.</span><span class="sxs-lookup"><span data-stu-id="68a70-129">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="68a70-130">Примечания</span><span class="sxs-lookup"><span data-stu-id="68a70-130">Remarks</span></span>

<span data-ttu-id="68a70-131">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.Этот элемент появился в Exchange Server 2010 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="68a70-131">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="68a70-132">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="68a70-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="68a70-133">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="68a70-133">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="68a70-134">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="68a70-134">Schema name</span></span>  <br/> |<span data-ttu-id="68a70-135">Схема Types</span><span class="sxs-lookup"><span data-stu-id="68a70-135">Types schema</span></span>  <br/> |
|<span data-ttu-id="68a70-136">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="68a70-136">Validation file</span></span>  <br/> |<span data-ttu-id="68a70-137">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="68a70-137">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="68a70-138">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="68a70-138">Can be empty</span></span>  <br/> |<span data-ttu-id="68a70-139">False</span><span class="sxs-lookup"><span data-stu-id="68a70-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="68a70-140">См. также</span><span class="sxs-lookup"><span data-stu-id="68a70-140">See also</span></span>



[<span data-ttu-id="68a70-141">FindConversation Operation</span><span class="sxs-lookup"><span data-stu-id="68a70-141">FindConversation operation</span></span>](findconversation-operation.md)
  
[<span data-ttu-id="68a70-142">Операция ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="68a70-142">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)


[<span data-ttu-id="68a70-143">Conversations in EWS</span><span class="sxs-lookup"><span data-stu-id="68a70-143">Conversations in EWS</span></span>](https://msdn.microsoft.com/library/91e64629-db6c-4c94-9dcb-d386232e8467%28Office.15%29.aspx)

