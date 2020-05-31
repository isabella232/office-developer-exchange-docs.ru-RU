---
title: конверсатионактион
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
description: Элемент Конверсатионактион содержит одно действие, которое будет применено к одной беседе.
ms.openlocfilehash: 45cd6df3aba94062bd5aa0ddf9367e8cf118dc6b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761811"
---
# <a name="conversationaction"></a><span data-ttu-id="d886f-103">конверсатионактион</span><span class="sxs-lookup"><span data-stu-id="d886f-103">ConversationAction</span></span>

<span data-ttu-id="d886f-104">Элемент **конверсатионактион** содержит одно действие, которое будет применено к одной беседе.</span><span class="sxs-lookup"><span data-stu-id="d886f-104">The **ConversationAction** element contains a single action to be applied to a single conversation.</span></span> 
  
[<span data-ttu-id="d886f-105">ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="d886f-105">ApplyConversationAction</span></span>](applyconversationaction.md)
  
[<span data-ttu-id="d886f-106">конверсатионактионс</span><span class="sxs-lookup"><span data-stu-id="d886f-106">ConversationActions</span></span>](conversationactions.md)
  
[<span data-ttu-id="d886f-107">конверсатионактион</span><span class="sxs-lookup"><span data-stu-id="d886f-107">ConversationAction</span></span>](conversationaction.md)
  
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

 <span data-ttu-id="d886f-108">**конверсатионактионтипе**</span><span class="sxs-lookup"><span data-stu-id="d886f-108">**ConversationActionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d886f-109">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="d886f-109">Attributes and elements</span></span>

<span data-ttu-id="d886f-110">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="d886f-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d886f-111">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="d886f-111">Attributes</span></span>

<span data-ttu-id="d886f-112">Нет.</span><span class="sxs-lookup"><span data-stu-id="d886f-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d886f-113">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="d886f-113">Child elements</span></span>

|<span data-ttu-id="d886f-114">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="d886f-114">**Element**</span></span>|<span data-ttu-id="d886f-115">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d886f-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d886f-116">Action (Конверсатионактионтипетипе)</span><span class="sxs-lookup"><span data-stu-id="d886f-116">Action (ConversationActionTypeType)</span></span>](action-conversationactiontypetype.md) <br/> |<span data-ttu-id="d886f-117">Содержит действие, которое необходимо выполнить для диалога, указанного с помощью элемента [ConversationId](conversationid.md) .</span><span class="sxs-lookup"><span data-stu-id="d886f-117">Contains the action to perform on the conversation specified by the [ConversationId](conversationid.md) element.</span></span> <span data-ttu-id="d886f-118">Этот элемент должен присутствовать.</span><span class="sxs-lookup"><span data-stu-id="d886f-118">This element must be present.</span></span>  <br/> |
|[<span data-ttu-id="d886f-119">ConversationId</span><span class="sxs-lookup"><span data-stu-id="d886f-119">ConversationId</span></span>](conversationid.md) <br/> |<span data-ttu-id="d886f-120">Содержит идентификатор диалога, который будет иметь действие, указанное элементом [Action (конверсатионактионтипетипе)](action-conversationactiontypetype.md) , примененным к элементам в беседе.</span><span class="sxs-lookup"><span data-stu-id="d886f-120">Contains the identifier of the conversation that will have the action specified by the [Action (ConversationActionTypeType)](action-conversationactiontypetype.md) element applied to items in the conversation.</span></span> <span data-ttu-id="d886f-121">Этот элемент должен присутствовать.</span><span class="sxs-lookup"><span data-stu-id="d886f-121">This element must be present.</span></span>  <br/> |
|[<span data-ttu-id="d886f-122">контекстфолдерид</span><span class="sxs-lookup"><span data-stu-id="d886f-122">ContextFolderId</span></span>](contextfolderid.md) <br/> |<span data-ttu-id="d886f-123">Указывает папку, предназначенную для действий, в которых используются папки.</span><span class="sxs-lookup"><span data-stu-id="d886f-123">Indicates the folder that is targeted for actions that use folders.</span></span> <span data-ttu-id="d886f-124">Этот элемент должен присутствовать при копировании, удалении, перемещении и установке состояния чтения элементов беседы в целевой папке.</span><span class="sxs-lookup"><span data-stu-id="d886f-124">This element must be present when copying, deleting, moving, and setting read state on conversation items in a target folder.</span></span>  <br/> |
|[<span data-ttu-id="d886f-125">конверсатионластсинктиме</span><span class="sxs-lookup"><span data-stu-id="d886f-125">ConversationLastSyncTime</span></span>](conversationlastsynctime.md) <br/> |<span data-ttu-id="d886f-126">Содержит дату и время последней синхронизации беседы.</span><span class="sxs-lookup"><span data-stu-id="d886f-126">Contains the date and time that a conversation was last synchronized.</span></span> <span data-ttu-id="d886f-127">Этот элемент должен присутствовать при попытке удалить все элементы в беседе, полученные до указанного времени.</span><span class="sxs-lookup"><span data-stu-id="d886f-127">This element must be present when trying to delete all items in a conversation that were received up to the specified time.</span></span>  <br/> |
|[<span data-ttu-id="d886f-128">процессригхтавай</span><span class="sxs-lookup"><span data-stu-id="d886f-128">ProcessRightAway</span></span>](processrightaway.md) <br/> |<span data-ttu-id="d886f-129">Указывает, отправляется ли ответ сразу после того, как действие начнет обработку на сервере или отправило ли ответ после завершения действия.</span><span class="sxs-lookup"><span data-stu-id="d886f-129">Indicates whether the response is sent as soon as the action starts processing on the server or whether the response is sent after the action has completed.</span></span> <span data-ttu-id="d886f-130">Этот элемент должен присутствовать, чтобы ответ был асинхронно отправлен в запрошенное действие.</span><span class="sxs-lookup"><span data-stu-id="d886f-130">This element must be present for the response to be sent asynchronous to the requested action.</span></span>  <br/> |
|[<span data-ttu-id="d886f-131">дестинатионфолдерид</span><span class="sxs-lookup"><span data-stu-id="d886f-131">DestinationFolderId</span></span>](destinationfolderid.md) <br/> |<span data-ttu-id="d886f-132">Указывает целевую папку для действий по копированию и перемещению.</span><span class="sxs-lookup"><span data-stu-id="d886f-132">Indicates the destination folder for copy and move actions.</span></span>  <br/> |
|[<span data-ttu-id="d886f-133">Категории</span><span class="sxs-lookup"><span data-stu-id="d886f-133">Categories</span></span>](categories-ex15websvcsotherref.md) <br/> |<span data-ttu-id="d886f-134">Содержит коллекцию строк, определяющих категории, к которым относятся элементы в беседе.</span><span class="sxs-lookup"><span data-stu-id="d886f-134">Contains a collection of strings that identify the categories to which items in a conversation belong.</span></span>  <br/> |
|[<span data-ttu-id="d886f-135">енаблеалвайсделете</span><span class="sxs-lookup"><span data-stu-id="d886f-135">EnableAlwaysDelete</span></span>](enablealwaysdelete.md) <br/> |<span data-ttu-id="d886f-136">Указывает флаг, который включает удаление для всех новых элементов в беседе.</span><span class="sxs-lookup"><span data-stu-id="d886f-136">Specifies a flag that enables deletion for all new items in a conversation.</span></span>  <br/> |
|[<span data-ttu-id="d886f-137">IsRead</span><span class="sxs-lookup"><span data-stu-id="d886f-137">IsRead</span></span>](isread.md) <br/> |<span data-ttu-id="d886f-138">Указывает, было ли Прочитано сообщение.</span><span class="sxs-lookup"><span data-stu-id="d886f-138">Indicates whether a message has been read.</span></span>  <br/> |
|[<span data-ttu-id="d886f-139">делететипе</span><span class="sxs-lookup"><span data-stu-id="d886f-139">DeleteType</span></span>](deletetype.md) <br/> |<span data-ttu-id="d886f-140">Указывает, как удаляются элементы в беседе.</span><span class="sxs-lookup"><span data-stu-id="d886f-140">Indicates how items in a conversation are deleted.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d886f-141">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="d886f-141">Parent elements</span></span>

|<span data-ttu-id="d886f-142">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="d886f-142">**Element**</span></span>|<span data-ttu-id="d886f-143">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d886f-143">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d886f-144">конверсатионактионс</span><span class="sxs-lookup"><span data-stu-id="d886f-144">ConversationActions</span></span>](conversationactions.md) <br/> |<span data-ttu-id="d886f-145">Содержит коллекцию бесед и действий, которые необходимо применить к ним.</span><span class="sxs-lookup"><span data-stu-id="d886f-145">Contains a collection of conversations and the actions to apply to them.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="d886f-146">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="d886f-146">Text value</span></span>

<span data-ttu-id="d886f-147">**Текстовые значения элементов Конверсатионактион**</span><span class="sxs-lookup"><span data-stu-id="d886f-147">**ConversationAction element text values**</span></span>

|<span data-ttu-id="d886f-148">**Значение**</span><span class="sxs-lookup"><span data-stu-id="d886f-148">**Value**</span></span>|<span data-ttu-id="d886f-149">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d886f-149">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="d886f-150">алвайскатегоризе</span><span class="sxs-lookup"><span data-stu-id="d886f-150">AlwaysCategorize</span></span>  <br/> |<span data-ttu-id="d886f-151">Всегда классифицировать беседу.</span><span class="sxs-lookup"><span data-stu-id="d886f-151">Always categorize the conversation.</span></span>  <br/> |
|<span data-ttu-id="d886f-152">алвайсделете</span><span class="sxs-lookup"><span data-stu-id="d886f-152">AlwaysDelete</span></span>  <br/> |<span data-ttu-id="d886f-153">Всегда удаляйте беседу.</span><span class="sxs-lookup"><span data-stu-id="d886f-153">Always delete the conversation.</span></span>  <br/> |
|<span data-ttu-id="d886f-154">алвайсмове</span><span class="sxs-lookup"><span data-stu-id="d886f-154">AlwaysMove</span></span>  <br/> |<span data-ttu-id="d886f-155">Всегда перемещайте беседу.</span><span class="sxs-lookup"><span data-stu-id="d886f-155">Always move the conversation.</span></span>  <br/> |
|<span data-ttu-id="d886f-156">Удаление</span><span class="sxs-lookup"><span data-stu-id="d886f-156">Delete</span></span>  <br/> |<span data-ttu-id="d886f-157">Удаление беседы.</span><span class="sxs-lookup"><span data-stu-id="d886f-157">Delete the conversation.</span></span>  <br/> |
|<span data-ttu-id="d886f-158">Move</span><span class="sxs-lookup"><span data-stu-id="d886f-158">Move</span></span>  <br/> |<span data-ttu-id="d886f-159">Перемещение беседы.</span><span class="sxs-lookup"><span data-stu-id="d886f-159">Move the conversation.</span></span>  <br/> |
|<span data-ttu-id="d886f-160">Copy</span><span class="sxs-lookup"><span data-stu-id="d886f-160">Copy</span></span>  <br/> |<span data-ttu-id="d886f-161">Скопируйте беседу.</span><span class="sxs-lookup"><span data-stu-id="d886f-161">Copy the conversation.</span></span>  <br/> |
|<span data-ttu-id="d886f-162">сетреадстате</span><span class="sxs-lookup"><span data-stu-id="d886f-162">SetReadState</span></span>  <br/> |<span data-ttu-id="d886f-163">Задание состояния чтения беседы.</span><span class="sxs-lookup"><span data-stu-id="d886f-163">Set the read state of the conversation.</span></span>  <br/> |
|<span data-ttu-id="d886f-164">сетретентионполици</span><span class="sxs-lookup"><span data-stu-id="d886f-164">SetRetentionPolicy</span></span>  <br/> |<span data-ttu-id="d886f-165">Задайте политику хранения для беседы.</span><span class="sxs-lookup"><span data-stu-id="d886f-165">Set the retention policy for the conversation.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="d886f-166">Примечания</span><span class="sxs-lookup"><span data-stu-id="d886f-166">Remarks</span></span>

<span data-ttu-id="d886f-167">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.Этот элемент появился в Exchange Server 2010 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="d886f-167">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d886f-168">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="d886f-168">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d886f-169">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="d886f-169">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d886f-170">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="d886f-170">Schema Name</span></span>  <br/> |<span data-ttu-id="d886f-171">Схема Types</span><span class="sxs-lookup"><span data-stu-id="d886f-171">Types schema</span></span>  <br/> |
|<span data-ttu-id="d886f-172">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="d886f-172">Validation File</span></span>  <br/> |<span data-ttu-id="d886f-173">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="d886f-173">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d886f-174">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="d886f-174">Can be Empty</span></span>  <br/> |<span data-ttu-id="d886f-175">False</span><span class="sxs-lookup"><span data-stu-id="d886f-175">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d886f-176">См. также</span><span class="sxs-lookup"><span data-stu-id="d886f-176">See also</span></span>



[<span data-ttu-id="d886f-177">Операция ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="d886f-177">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)


- [<span data-ttu-id="d886f-178">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="d886f-178">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

