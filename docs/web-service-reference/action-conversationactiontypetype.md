---
title: Действие (ConversationActionTypeType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Action
api_type:
- schema
ms.assetid: 8bbc12f2-76c5-4fda-828f-56b2086a0454
description: Элемент Action содержит действие, выполняемое в беседу, заданный элементом ConversationId.
ms.openlocfilehash: b468eeaf0c2509bfa53cbd83f497f0bae20a7f68
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761323"
---
# <a name="action-conversationactiontypetype"></a><span data-ttu-id="67a81-103">Действие (ConversationActionTypeType)</span><span class="sxs-lookup"><span data-stu-id="67a81-103">Action (ConversationActionTypeType)</span></span>

<span data-ttu-id="67a81-104">Элемент **Action** содержит действие, выполняемое в беседу, заданный элементом [ConversationId](conversationid.md) .</span><span class="sxs-lookup"><span data-stu-id="67a81-104">The **Action** element contains the action to perform on the conversation specified by the [ConversationId](conversationid.md) element.</span></span> 
  
- [<span data-ttu-id="67a81-105">ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="67a81-105">ApplyConversationAction</span></span>](applyconversationaction.md)
  
- [<span data-ttu-id="67a81-106">ConversationActions</span><span class="sxs-lookup"><span data-stu-id="67a81-106">ConversationActions</span></span>](conversationactions.md)
  
- [<span data-ttu-id="67a81-107">ConversationAction</span><span class="sxs-lookup"><span data-stu-id="67a81-107">ConversationAction</span></span>](conversationaction.md)
  
- [<span data-ttu-id="67a81-108">Действие (ConversationActionTypeType)</span><span class="sxs-lookup"><span data-stu-id="67a81-108">Action (ConversationActionTypeType)</span></span>](action-conversationactiontypetype.md)
  
```XML
<Action> AlwaysCategorize | AlwaysDelete | AlwaysMove | Delete | Move | Copy | SetReadState </Action>
```

 <span data-ttu-id="67a81-109">**ConversationActionTypeType**</span><span class="sxs-lookup"><span data-stu-id="67a81-109">**ConversationActionTypeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="67a81-110">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="67a81-110">Attributes and elements</span></span>

<span data-ttu-id="67a81-111">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="67a81-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="67a81-112">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="67a81-112">Attributes</span></span>

<span data-ttu-id="67a81-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="67a81-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="67a81-114">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="67a81-114">Child elements</span></span>

<span data-ttu-id="67a81-115">Нет.</span><span class="sxs-lookup"><span data-stu-id="67a81-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="67a81-116">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="67a81-116">Parent elements</span></span>

|<span data-ttu-id="67a81-117">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="67a81-117">**Element**</span></span>|<span data-ttu-id="67a81-118">**Описание**</span><span class="sxs-lookup"><span data-stu-id="67a81-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="67a81-119">ConversationAction</span><span class="sxs-lookup"><span data-stu-id="67a81-119">ConversationAction</span></span>](conversationaction.md) <br/> |<span data-ttu-id="67a81-120">Содержит одно действие должен применяться к разговора.</span><span class="sxs-lookup"><span data-stu-id="67a81-120">Contains a single action to be applied to a single conversation.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="67a81-121">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="67a81-121">Text value</span></span>

<span data-ttu-id="67a81-122">Текстовое значение элемента **Действие** указывает действие, которое будет выполняться в беседе.</span><span class="sxs-lookup"><span data-stu-id="67a81-122">The text value of the **Action** element indicates which action will be performed on a conversation.</span></span> <span data-ttu-id="67a81-123">Ниже приведены возможные текстовые значения и соответствующие действия.</span><span class="sxs-lookup"><span data-stu-id="67a81-123">The following are the possible text values and the corresponding actions:</span></span> 
  
- <span data-ttu-id="67a81-124">**AlwaysCategorize** - текущих элементов и новых элементов в окне беседы будет автоматически с категориями, обнаруженных в элементе [категорий](categories-ex15websvcsotherref.md) .</span><span class="sxs-lookup"><span data-stu-id="67a81-124">**AlwaysCategorize** - The current items and new items in the conversation will automatically be set with the categories identified in the [Categories](categories-ex15websvcsotherref.md) element.</span></span> 
    
- <span data-ttu-id="67a81-125">Автоматически удалять **AlwaysDelete** - текущих элементов и новые элементы в беседе.</span><span class="sxs-lookup"><span data-stu-id="67a81-125">**AlwaysDelete** - The current items and new items in the conversation will automatically be deleted.</span></span> <span data-ttu-id="67a81-126">Режим удаления задается с помощью элемента [DeleteType](deletetype.md) .</span><span class="sxs-lookup"><span data-stu-id="67a81-126">The deletion mode is set by the [DeleteType](deletetype.md) element.</span></span> 
    
- <span data-ttu-id="67a81-127">**AlwaysMove** - текущих элементов и новые элементы в беседе перемещается автоматически в папку, указанную в элементе [DestinationFolderId](destinationfolderid.md) .</span><span class="sxs-lookup"><span data-stu-id="67a81-127">**AlwaysMove** - The current items and new items in the conversation will automatically be moved to the folder identified by the [DestinationFolderId](destinationfolderid.md) element.</span></span> 
    
- <span data-ttu-id="67a81-128">**Удаление** - текущие элементы в окне беседы будет удалено.</span><span class="sxs-lookup"><span data-stu-id="67a81-128">**Delete** - The current items in the conversation will be deleted.</span></span> <span data-ttu-id="67a81-129">Последующие элементы в беседе, не удаляются.</span><span class="sxs-lookup"><span data-stu-id="67a81-129">Subsequent items in the conversation will not be deleted.</span></span> <span data-ttu-id="67a81-130">Режим удаления задается с помощью элемента [DeleteType](deletetype.md) .</span><span class="sxs-lookup"><span data-stu-id="67a81-130">The deletion mode is set by the [DeleteType](deletetype.md) element.</span></span> 
    
- <span data-ttu-id="67a81-131">**Перемещение** - текущего элементы в беседе будут перемещены в папку, указанную в элементе [DestinationFolderId](destinationfolderid.md) .</span><span class="sxs-lookup"><span data-stu-id="67a81-131">**Move** - The current items in the conversation will be moved to the folder identified by the [DestinationFolderId](destinationfolderid.md) element.</span></span> <span data-ttu-id="67a81-132">Не будут перемещаться последующие элементы в беседе.</span><span class="sxs-lookup"><span data-stu-id="67a81-132">Subsequent items in the conversation will not be moved.</span></span> 
    
- <span data-ttu-id="67a81-133">**Копия** - текущего элементы в беседе предстоит скопировать в папку, указанную в элементе [DestinationFolderId](destinationfolderid.md) .</span><span class="sxs-lookup"><span data-stu-id="67a81-133">**Copy** - The current items in the conversation will be copied to the folder identified by the [DestinationFolderId](destinationfolderid.md) element.</span></span> <span data-ttu-id="67a81-134">Последующие элементы в беседе, не копируются.</span><span class="sxs-lookup"><span data-stu-id="67a81-134">Subsequent items in the conversation will not be copied.</span></span> 
    
- <span data-ttu-id="67a81-135">**SetReadState** - текущие элементы в окне беседы будут иметь их состояние чтения задать.</span><span class="sxs-lookup"><span data-stu-id="67a81-135">**SetReadState** - The current items in the conversation will have their read state set.</span></span> <span data-ttu-id="67a81-136">Состояние чтения задано в элементе [IsRead](isread.md) .</span><span class="sxs-lookup"><span data-stu-id="67a81-136">The read state is set by the [IsRead](isread.md) element.</span></span> 
    
- <span data-ttu-id="67a81-137">**Флаг** - текущие элементы в окне беседы будут иметь флаг, определенный элемент [флаг](flag.md) .</span><span class="sxs-lookup"><span data-stu-id="67a81-137">**Flag** - The current items in the conversation will have a flag set as defined by the [Flag](flag.md) element.</span></span> 
    
## <a name="remarks"></a><span data-ttu-id="67a81-138">Замечания</span><span class="sxs-lookup"><span data-stu-id="67a81-138">Remarks</span></span>

<span data-ttu-id="67a81-139">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.Этот элемент появился в Exchange Server 2010 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="67a81-139">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="67a81-140">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="67a81-140">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="67a81-141">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="67a81-141">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="67a81-142">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="67a81-142">Schema Name</span></span>  <br/> |<span data-ttu-id="67a81-143">Схема Types</span><span class="sxs-lookup"><span data-stu-id="67a81-143">Types schema</span></span>  <br/> |
|<span data-ttu-id="67a81-144">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="67a81-144">Validation File</span></span>  <br/> |<span data-ttu-id="67a81-145">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="67a81-145">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="67a81-146">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="67a81-146">Can be Empty</span></span>  <br/> |<span data-ttu-id="67a81-147">False</span><span class="sxs-lookup"><span data-stu-id="67a81-147">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="67a81-148">См. также</span><span class="sxs-lookup"><span data-stu-id="67a81-148">See also</span></span>

- [<span data-ttu-id="67a81-149">Операция ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="67a81-149">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)
- [<span data-ttu-id="67a81-150">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="67a81-150">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

