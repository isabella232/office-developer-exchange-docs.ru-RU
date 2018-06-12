---
title: GetConversationItemsResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 2e930650-7848-4bf2-a975-026309b3ea02
description: Элемент GetConversationItemsResponseMessage указывает сообщение ответа на запрос GetConversationItems.
ms.openlocfilehash: 997319193311ef9267d8f6ff14c70bfe40e2634b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762733"
---
# <a name="getconversationitemsresponsemessage"></a><span data-ttu-id="93102-103">GetConversationItemsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="93102-103">GetConversationItemsResponseMessage</span></span>

<span data-ttu-id="93102-104">Элемент **GetConversationItemsResponseMessage** указывает сообщение ответа на запрос **GetConversationItems** .</span><span class="sxs-lookup"><span data-stu-id="93102-104">The **GetConversationItemsResponseMessage** element specifies the response message for a **GetConversationItems** request.</span></span> 
  
```XML
<GetConversationItemsResponseMessage ResponseClass="Success | Warning | Error">
    <Conversation/>
    <MessageText/>
    <ResponseCode/>
    <DescriptiveLinkKey/>
    <MessageXml/>
</GetConversationItemsResponseMessage>
```

 <span data-ttu-id="93102-105">**GetConversationItemsResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="93102-105">**GetConversationItemsResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="93102-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="93102-106">Attributes and elements</span></span>

<span data-ttu-id="93102-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="93102-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="93102-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="93102-108">Attributes</span></span>

|<span data-ttu-id="93102-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="93102-109">**Attribute**</span></span>|<span data-ttu-id="93102-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="93102-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="93102-111">ResponseClass</span><span class="sxs-lookup"><span data-stu-id="93102-111">ResponseClass</span></span>  <br/> |<span data-ttu-id="93102-112">Указывает класс ответа.</span><span class="sxs-lookup"><span data-stu-id="93102-112">Indicates the class of the response.</span></span>  <br/> |
   
#### <a name="responseclass"></a><span data-ttu-id="93102-113">ResponseClass</span><span class="sxs-lookup"><span data-stu-id="93102-113">ResponseClass</span></span>

|<span data-ttu-id="93102-114">**Значение**</span><span class="sxs-lookup"><span data-stu-id="93102-114">**Value**</span></span>|<span data-ttu-id="93102-115">**Описание**</span><span class="sxs-lookup"><span data-stu-id="93102-115">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="93102-116">Успешное выполнение</span><span class="sxs-lookup"><span data-stu-id="93102-116">Success</span></span>  <br/> |<span data-ttu-id="93102-117">Означает успешное выполнение.</span><span class="sxs-lookup"><span data-stu-id="93102-117">Indicates success.</span></span>  <br/> |
|<span data-ttu-id="93102-118">Предупреждающая</span><span class="sxs-lookup"><span data-stu-id="93102-118">Warning</span></span>  <br/> |<span data-ttu-id="93102-119">Указывает на предупреждение.</span><span class="sxs-lookup"><span data-stu-id="93102-119">Indicates a warning.</span></span>  <br/> |
|<span data-ttu-id="93102-120">Error</span><span class="sxs-lookup"><span data-stu-id="93102-120">Error</span></span>  <br/> |<span data-ttu-id="93102-121">Отображается сообщение об ошибке.</span><span class="sxs-lookup"><span data-stu-id="93102-121">Indicates an error.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="93102-122">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="93102-122">Child elements</span></span>

|<span data-ttu-id="93102-123">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="93102-123">**Element**</span></span>|<span data-ttu-id="93102-124">**Описание**</span><span class="sxs-lookup"><span data-stu-id="93102-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="93102-125">Беседы (ConversationResponseType)</span><span class="sxs-lookup"><span data-stu-id="93102-125">Conversation (ConversationResponseType)</span></span>](conversation-conversationresponsetype.md) <br/> |<span data-ttu-id="93102-126">Представляет один беседы, возвращаемых в ответе **GetConversationItems** .</span><span class="sxs-lookup"><span data-stu-id="93102-126">Represents a single conversation returned in a **GetConversationItems** response.</span></span>  <br/> |
|[<span data-ttu-id="93102-127">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="93102-127">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="93102-128">В настоящее время используется и зарезервировано для будущего использования.</span><span class="sxs-lookup"><span data-stu-id="93102-128">Currently unused and reserved for future use.</span></span>  <br/> |
|[<span data-ttu-id="93102-129">MessageText</span><span class="sxs-lookup"><span data-stu-id="93102-129">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="93102-130">Предоставляет текстовое описание состояния ответа.</span><span class="sxs-lookup"><span data-stu-id="93102-130">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="93102-131">MessageXml</span><span class="sxs-lookup"><span data-stu-id="93102-131">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="93102-132">Предоставляет дополнительные сведения об ошибке ответа.</span><span class="sxs-lookup"><span data-stu-id="93102-132">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="93102-133">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="93102-133">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="93102-134">Предоставляет сведения о состоянии о запросе.</span><span class="sxs-lookup"><span data-stu-id="93102-134">Provides status information about the request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="93102-135">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="93102-135">Parent elements</span></span>

|<span data-ttu-id="93102-136">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="93102-136">**Element**</span></span>|<span data-ttu-id="93102-137">**Описание**</span><span class="sxs-lookup"><span data-stu-id="93102-137">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="93102-138">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="93102-138">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="93102-139">Содержит сообщения ответа на запрос веб-служб Exchange (EWS).</span><span class="sxs-lookup"><span data-stu-id="93102-139">Contains the response messages for an Exchange Web Services (EWS) request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="93102-140">Замечания</span><span class="sxs-lookup"><span data-stu-id="93102-140">Remarks</span></span>

<span data-ttu-id="93102-141">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="93102-141">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="93102-142">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="93102-142">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="93102-143">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="93102-143">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="93102-144">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="93102-144">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="93102-145">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="93102-145">Schema Name</span></span>  <br/> |<span data-ttu-id="93102-146">Схема сообщения</span><span class="sxs-lookup"><span data-stu-id="93102-146">Message schema</span></span>  <br/> |
|<span data-ttu-id="93102-147">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="93102-147">Validation File</span></span>  <br/> |<span data-ttu-id="93102-148">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="93102-148">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="93102-149">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="93102-149">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="93102-150">См. также</span><span class="sxs-lookup"><span data-stu-id="93102-150">See also</span></span>



- [<span data-ttu-id="93102-151">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="93102-151">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

