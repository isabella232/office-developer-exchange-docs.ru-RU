---
title: ConversationAction
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ConversationAction
api_type:
- schema
ms.assetid: 9ecea41a-3860-4569-8e9b-284b451fc4e0
description: Элемент ConversationAction содержит одно действие должен применяться к разговора.
ms.openlocfilehash: 45cd6df3aba94062bd5aa0ddf9367e8cf118dc6b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761811"
---
# <a name="conversationaction"></a><span data-ttu-id="57731-103">ConversationAction</span><span class="sxs-lookup"><span data-stu-id="57731-103">ConversationAction</span></span>

<span data-ttu-id="57731-104">Элемент **ConversationAction** содержит одно действие должен применяться к разговора.</span><span class="sxs-lookup"><span data-stu-id="57731-104">The **ConversationAction** element contains a single action to be applied to a single conversation.</span></span> 
  
[<span data-ttu-id="57731-105">ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="57731-105">ApplyConversationAction</span></span>](applyconversationaction.md)
  
[<span data-ttu-id="57731-106">ConversationActions</span><span class="sxs-lookup"><span data-stu-id="57731-106">ConversationActions</span></span>](conversationactions.md)
  
[<span data-ttu-id="57731-107">ConversationAction</span><span class="sxs-lookup"><span data-stu-id="57731-107">ConversationAction</span></span>](conversationaction.md)
  
```XML
<ConversationAction>
   <Action/>
   <ConversationId/>
   <ContextFolderId/>
   <ConversationLastSyncTime/>
   <ProcessRightAway/>
   <DestinationFolderId/>
   <Categories/>
   <EnableAlwaysDelete/>
   <IsRead/>
   <DeleteType/>
</ConversationAction>
```

 <span data-ttu-id="57731-108">**ConversationActionType**</span><span class="sxs-lookup"><span data-stu-id="57731-108">**ConversationActionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="57731-109">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="57731-109">Attributes and elements</span></span>

<span data-ttu-id="57731-110">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="57731-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="57731-111">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="57731-111">Attributes</span></span>

<span data-ttu-id="57731-112">Нет.</span><span class="sxs-lookup"><span data-stu-id="57731-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="57731-113">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="57731-113">Child elements</span></span>

|<span data-ttu-id="57731-114">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="57731-114">**Element**</span></span>|<span data-ttu-id="57731-115">**Описание**</span><span class="sxs-lookup"><span data-stu-id="57731-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="57731-116">Действие (ConversationActionTypeType)</span><span class="sxs-lookup"><span data-stu-id="57731-116">Action (ConversationActionTypeType)</span></span>](action-conversationactiontypetype.md) <br/> |<span data-ttu-id="57731-117">Содержит действие, выполняемое в беседу, заданный элементом [ConversationId](conversationid.md) .</span><span class="sxs-lookup"><span data-stu-id="57731-117">Contains the action to perform on the conversation specified by the [ConversationId](conversationid.md) element.</span></span> <span data-ttu-id="57731-118">Этот элемент должен быть указан.</span><span class="sxs-lookup"><span data-stu-id="57731-118">This element must be present.</span></span>  <br/> |
|[<span data-ttu-id="57731-119">ConversationId</span><span class="sxs-lookup"><span data-stu-id="57731-119">ConversationId</span></span>](conversationid.md) <br/> |<span data-ttu-id="57731-120">Содержит идентификатор беседы, в которых будут действием, указанным с помощью элемента [действие (ConversationActionTypeType)](action-conversationactiontypetype.md) , применяется к элементам в беседе.</span><span class="sxs-lookup"><span data-stu-id="57731-120">Contains the identifier of the conversation that will have the action specified by the [Action (ConversationActionTypeType)](action-conversationactiontypetype.md) element applied to items in the conversation.</span></span> <span data-ttu-id="57731-121">Этот элемент должен быть указан.</span><span class="sxs-lookup"><span data-stu-id="57731-121">This element must be present.</span></span>  <br/> |
|[<span data-ttu-id="57731-122">ContextFolderId</span><span class="sxs-lookup"><span data-stu-id="57731-122">ContextFolderId</span></span>](contextfolderid.md) <br/> |<span data-ttu-id="57731-123">Указывает папку, предназначенное для действий, использующих папок.</span><span class="sxs-lookup"><span data-stu-id="57731-123">Indicates the folder that is targeted for actions that use folders.</span></span> <span data-ttu-id="57731-124">Этот элемент должен присутствовать при копирование, удаление, перемещение и настройка состояние чтения элементов беседы в целевой папке.</span><span class="sxs-lookup"><span data-stu-id="57731-124">This element must be present when copying, deleting, moving, and setting read state on conversation items in a target folder.</span></span>  <br/> |
|[<span data-ttu-id="57731-125">ConversationLastSyncTime</span><span class="sxs-lookup"><span data-stu-id="57731-125">ConversationLastSyncTime</span></span>](conversationlastsynctime.md) <br/> |<span data-ttu-id="57731-126">Содержит дату и время последнего синхронизирована беседы.</span><span class="sxs-lookup"><span data-stu-id="57731-126">Contains the date and time that a conversation was last synchronized.</span></span> <span data-ttu-id="57731-127">Этот элемент должен присутствовать при попытке удаления всех элементов в беседе, которые были получены до заданного времени.</span><span class="sxs-lookup"><span data-stu-id="57731-127">This element must be present when trying to delete all items in a conversation that were received up to the specified time.</span></span>  <br/> |
|[<span data-ttu-id="57731-128">ProcessRightAway</span><span class="sxs-lookup"><span data-stu-id="57731-128">ProcessRightAway</span></span>](processrightaway.md) <br/> |<span data-ttu-id="57731-129">Указывает, будет ли ответ сразу после начала действия обработки на сервере или ли ответ после завершения действия.</span><span class="sxs-lookup"><span data-stu-id="57731-129">Indicates whether the response is sent as soon as the action starts processing on the server or whether the response is sent after the action has completed.</span></span> <span data-ttu-id="57731-130">Этот элемент необходим для ответа отправку асинхронных запрошенное действие.</span><span class="sxs-lookup"><span data-stu-id="57731-130">This element must be present for the response to be sent asynchronous to the requested action.</span></span>  <br/> |
|[<span data-ttu-id="57731-131">DestinationFolderId</span><span class="sxs-lookup"><span data-stu-id="57731-131">DestinationFolderId</span></span>](destinationfolderid.md) <br/> |<span data-ttu-id="57731-132">Определяет папку назначения для копирования и перемещения действия.</span><span class="sxs-lookup"><span data-stu-id="57731-132">Indicates the destination folder for copy and move actions.</span></span>  <br/> |
|[<span data-ttu-id="57731-133">Категории</span><span class="sxs-lookup"><span data-stu-id="57731-133">Categories</span></span>](categories-ex15websvcsotherref.md) <br/> |<span data-ttu-id="57731-134">Содержит коллекцию строк, чтобы указать категории, к которым принадлежат элементы в беседе.</span><span class="sxs-lookup"><span data-stu-id="57731-134">Contains a collection of strings that identify the categories to which items in a conversation belong.</span></span>  <br/> |
|[<span data-ttu-id="57731-135">EnableAlwaysDelete</span><span class="sxs-lookup"><span data-stu-id="57731-135">EnableAlwaysDelete</span></span>](enablealwaysdelete.md) <br/> |<span data-ttu-id="57731-136">Задает флаг, который позволяет удалить для всех новых элементов в беседе.</span><span class="sxs-lookup"><span data-stu-id="57731-136">Specifies a flag that enables deletion for all new items in a conversation.</span></span>  <br/> |
|[<span data-ttu-id="57731-137">IsRead</span><span class="sxs-lookup"><span data-stu-id="57731-137">IsRead</span></span>](isread.md) <br/> |<span data-ttu-id="57731-138">Указывает, имеет ли чтение сообщения.</span><span class="sxs-lookup"><span data-stu-id="57731-138">Indicates whether a message has been read.</span></span>  <br/> |
|[<span data-ttu-id="57731-139">DeleteType</span><span class="sxs-lookup"><span data-stu-id="57731-139">DeleteType</span></span>](deletetype.md) <br/> |<span data-ttu-id="57731-140">Показывает, как удалить элементы в беседе.</span><span class="sxs-lookup"><span data-stu-id="57731-140">Indicates how items in a conversation are deleted.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="57731-141">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="57731-141">Parent elements</span></span>

|<span data-ttu-id="57731-142">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="57731-142">**Element**</span></span>|<span data-ttu-id="57731-143">**Описание**</span><span class="sxs-lookup"><span data-stu-id="57731-143">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="57731-144">ConversationActions</span><span class="sxs-lookup"><span data-stu-id="57731-144">ConversationActions</span></span>](conversationactions.md) <br/> |<span data-ttu-id="57731-145">Содержит коллекцию бесед и действий для применения к ним.</span><span class="sxs-lookup"><span data-stu-id="57731-145">Contains a collection of conversations and the actions to apply to them.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="57731-146">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="57731-146">Text value</span></span>

<span data-ttu-id="57731-147">**ConversationAction элемент текстовые значения**</span><span class="sxs-lookup"><span data-stu-id="57731-147">**ConversationAction element text values**</span></span>

|<span data-ttu-id="57731-148">**Значение**</span><span class="sxs-lookup"><span data-stu-id="57731-148">**Value**</span></span>|<span data-ttu-id="57731-149">**Описание**</span><span class="sxs-lookup"><span data-stu-id="57731-149">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="57731-150">AlwaysCategorize</span><span class="sxs-lookup"><span data-stu-id="57731-150">AlwaysCategorize</span></span>  <br/> |<span data-ttu-id="57731-151">Всегда классификации сообщений.</span><span class="sxs-lookup"><span data-stu-id="57731-151">Always categorize the conversation.</span></span>  <br/> |
|<span data-ttu-id="57731-152">AlwaysDelete</span><span class="sxs-lookup"><span data-stu-id="57731-152">AlwaysDelete</span></span>  <br/> |<span data-ttu-id="57731-153">Всегда удаляйте беседу.</span><span class="sxs-lookup"><span data-stu-id="57731-153">Always delete the conversation.</span></span>  <br/> |
|<span data-ttu-id="57731-154">AlwaysMove</span><span class="sxs-lookup"><span data-stu-id="57731-154">AlwaysMove</span></span>  <br/> |<span data-ttu-id="57731-155">Всегда перемещать беседу.</span><span class="sxs-lookup"><span data-stu-id="57731-155">Always move the conversation.</span></span>  <br/> |
|<span data-ttu-id="57731-156">Удаление</span><span class="sxs-lookup"><span data-stu-id="57731-156">Delete</span></span>  <br/> |<span data-ttu-id="57731-157">Удалите беседу.</span><span class="sxs-lookup"><span data-stu-id="57731-157">Delete the conversation.</span></span>  <br/> |
|<span data-ttu-id="57731-158">перемещение.</span><span class="sxs-lookup"><span data-stu-id="57731-158">Move</span></span>  <br/> |<span data-ttu-id="57731-159">Перемещение беседу.</span><span class="sxs-lookup"><span data-stu-id="57731-159">Move the conversation.</span></span>  <br/> |
|<span data-ttu-id="57731-160">Copy</span><span class="sxs-lookup"><span data-stu-id="57731-160">Copy</span></span>  <br/> |<span data-ttu-id="57731-161">Скопируйте беседу.</span><span class="sxs-lookup"><span data-stu-id="57731-161">Copy the conversation.</span></span>  <br/> |
|<span data-ttu-id="57731-162">SetReadState</span><span class="sxs-lookup"><span data-stu-id="57731-162">SetReadState</span></span>  <br/> |<span data-ttu-id="57731-163">Задайте состояние чтения беседы.</span><span class="sxs-lookup"><span data-stu-id="57731-163">Set the read state of the conversation.</span></span>  <br/> |
|<span data-ttu-id="57731-164">SetRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="57731-164">SetRetentionPolicy</span></span>  <br/> |<span data-ttu-id="57731-165">Настройка политики хранения для беседы.</span><span class="sxs-lookup"><span data-stu-id="57731-165">Set the retention policy for the conversation.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="57731-166">Замечания</span><span class="sxs-lookup"><span data-stu-id="57731-166">Remarks</span></span>

<span data-ttu-id="57731-167">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.Этот элемент появился в Exchange Server 2010 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="57731-167">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="57731-168">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="57731-168">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="57731-169">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="57731-169">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="57731-170">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="57731-170">Schema Name</span></span>  <br/> |<span data-ttu-id="57731-171">Схема Types</span><span class="sxs-lookup"><span data-stu-id="57731-171">Types schema</span></span>  <br/> |
|<span data-ttu-id="57731-172">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="57731-172">Validation File</span></span>  <br/> |<span data-ttu-id="57731-173">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="57731-173">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="57731-174">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="57731-174">Can be Empty</span></span>  <br/> |<span data-ttu-id="57731-175">False</span><span class="sxs-lookup"><span data-stu-id="57731-175">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="57731-176">См. также</span><span class="sxs-lookup"><span data-stu-id="57731-176">See also</span></span>



[<span data-ttu-id="57731-177">Операция ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="57731-177">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)


- [<span data-ttu-id="57731-178">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="57731-178">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

