---
title: UniqueRecipients
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UniqueRecipients
api_type:
- schema
ms.assetid: 9f46ed05-5370-46ee-80f5-83f97224c76e
description: Элемент UniqueRecipients содержит список бесед в определенной папке. Этот элемент доступен только для чтения.
ms.openlocfilehash: 710559e599c6cec1db371165f01187f8960024f6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19840294"
---
# <a name="uniquerecipients"></a><span data-ttu-id="0b7a3-104">UniqueRecipients</span><span class="sxs-lookup"><span data-stu-id="0b7a3-104">UniqueRecipients</span></span>

<span data-ttu-id="0b7a3-p102">Информация, содержащаяся в этом документе, может относиться к функциям и продуктам предварительной версии и может претерпеть значительные изменения до окончательного коммерческого выпуска. Настоящий документ предоставляется "как есть" и служит только для информационных целей. Корпорация Майкрософт не предоставляет никаких гарантий, явных или подразумеваемых, в связи с этим документом Элемент **UniqueRecipients** содержит список бесед в определенной папке. Этот элемент доступен только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0b7a3-p102">The **UniqueRecipients** element contains the recipient list of a conversation in a particular folder. This element is read-only.</span></span> 
  
[<span data-ttu-id="0b7a3-107">FindConversationResponse</span><span class="sxs-lookup"><span data-stu-id="0b7a3-107">FindConversationResponse</span></span>](findconversationresponse.md)
  
[<span data-ttu-id="0b7a3-108">Conversations</span><span class="sxs-lookup"><span data-stu-id="0b7a3-108">Conversations</span></span>](conversations-ex15websvcsotherref.md)
  
[<span data-ttu-id="0b7a3-109">Беседы (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="0b7a3-109">Conversation (ConversationType)</span></span>](conversation-conversationtype.md)
  
[<span data-ttu-id="0b7a3-110">UniqueRecipients</span><span class="sxs-lookup"><span data-stu-id="0b7a3-110">UniqueRecipients</span></span>](uniquerecipients.md)
  
```XML
<UniqueRecpients>
   <String/>
</UniqueRecpients>
```

 <span data-ttu-id="0b7a3-111">**ArrayOfStringsType**</span><span class="sxs-lookup"><span data-stu-id="0b7a3-111">**ArrayOfStringsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0b7a3-112">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="0b7a3-112">Attributes and elements</span></span>

<span data-ttu-id="0b7a3-113">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="0b7a3-113">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0b7a3-114">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="0b7a3-114">Attributes</span></span>

<span data-ttu-id="0b7a3-115">Нет.</span><span class="sxs-lookup"><span data-stu-id="0b7a3-115">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0b7a3-116">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="0b7a3-116">Child elements</span></span>

|<span data-ttu-id="0b7a3-117">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="0b7a3-117">**Element**</span></span>|<span data-ttu-id="0b7a3-118">**Описание**</span><span class="sxs-lookup"><span data-stu-id="0b7a3-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0b7a3-119">Строка</span><span class="sxs-lookup"><span data-stu-id="0b7a3-119">String</span></span>](string.md) <br/> |<span data-ttu-id="0b7a3-p103">Представляет уникальное получателя беседы. Этот элемент доступен только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0b7a3-p103">Represents a unique recipient of a conversation. This element is read-only.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="0b7a3-122">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="0b7a3-122">Parent elements</span></span>

|<span data-ttu-id="0b7a3-123">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="0b7a3-123">**Element**</span></span>|<span data-ttu-id="0b7a3-124">**Описание**</span><span class="sxs-lookup"><span data-stu-id="0b7a3-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0b7a3-125">Беседы (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="0b7a3-125">Conversation (ConversationType)</span></span>](conversation-conversationtype.md) <br/> |<span data-ttu-id="0b7a3-126">Представляет одну беседу.</span><span class="sxs-lookup"><span data-stu-id="0b7a3-126">Represents a single conversation.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="0b7a3-127">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="0b7a3-127">Text value</span></span>

<span data-ttu-id="0b7a3-128">Нет.</span><span class="sxs-lookup"><span data-stu-id="0b7a3-128">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="0b7a3-129">Замечания</span><span class="sxs-lookup"><span data-stu-id="0b7a3-129">Remarks</span></span>

<span data-ttu-id="0b7a3-130">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.Этот элемент появился в Exchange Server 2010 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="0b7a3-130">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0b7a3-131">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="0b7a3-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0b7a3-132">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="0b7a3-132">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="0b7a3-133">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="0b7a3-133">Schema name</span></span>  <br/> |<span data-ttu-id="0b7a3-134">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="0b7a3-134">Messages schema</span></span>  <br/> |
|<span data-ttu-id="0b7a3-135">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="0b7a3-135">Validation file</span></span>  <br/> |<span data-ttu-id="0b7a3-136">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="0b7a3-136">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="0b7a3-137">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="0b7a3-137">Can be empty</span></span>  <br/> |<span data-ttu-id="0b7a3-138">False</span><span class="sxs-lookup"><span data-stu-id="0b7a3-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0b7a3-139">См. также</span><span class="sxs-lookup"><span data-stu-id="0b7a3-139">See also</span></span>



[<span data-ttu-id="0b7a3-140">FindConversation Operation</span><span class="sxs-lookup"><span data-stu-id="0b7a3-140">FindConversation operation</span></span>](findconversation-operation.md)


[<span data-ttu-id="0b7a3-141">Conversations in EWS</span><span class="sxs-lookup"><span data-stu-id="0b7a3-141">Conversations in EWS</span></span>](http://msdn.microsoft.com/library/91e64629-db6c-4c94-9dcb-d386232e8467%28Office.15%29.aspx)

