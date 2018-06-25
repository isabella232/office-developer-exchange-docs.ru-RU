---
title: UniqueSenders
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UniqueSenders
api_type:
- schema
ms.assetid: 1f55f2fe-b2f2-4169-83c1-fa5c752bd695
description: Элемент UniqueSenders содержит список всех отправителей элементов беседы в текущую папку. Этот элемент доступен только для чтения.
ms.openlocfilehash: b75846534141e23e6d8158bc36f0ef60bcb1d7ad
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19840289"
---
# <a name="uniquesenders"></a><span data-ttu-id="86005-104">UniqueSenders</span><span class="sxs-lookup"><span data-stu-id="86005-104">UniqueSenders</span></span>

<span data-ttu-id="86005-105">Элемент **UniqueSenders** содержит список всех отправителей элементов беседы в текущую папку.</span><span class="sxs-lookup"><span data-stu-id="86005-105">The **UniqueSenders** element contains a list of all the senders of conversation items in the current folder.</span></span> <span data-ttu-id="86005-106">Этот элемент доступен только для чтения.</span><span class="sxs-lookup"><span data-stu-id="86005-106">This element is read-only.</span></span> 
  
[<span data-ttu-id="86005-107">FindConversationResponse</span><span class="sxs-lookup"><span data-stu-id="86005-107">FindConversationResponse</span></span>](findconversationresponse.md)
  
[<span data-ttu-id="86005-108">Conversations</span><span class="sxs-lookup"><span data-stu-id="86005-108">Conversations</span></span>](conversations-ex15websvcsotherref.md)
  
[<span data-ttu-id="86005-109">Беседы (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="86005-109">Conversation (ConversationType)</span></span>](conversation-conversationtype.md)
  
[<span data-ttu-id="86005-110">UniqueSenders</span><span class="sxs-lookup"><span data-stu-id="86005-110">UniqueSenders</span></span>](uniquesenders.md)
  
```XML
<UniqueSenders>
   <String/>
</UniqueSenders>
```

 <span data-ttu-id="86005-111">**ArrayOfStringsType**</span><span class="sxs-lookup"><span data-stu-id="86005-111">**ArrayOfStringsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="86005-112">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="86005-112">Attributes and elements</span></span>

<span data-ttu-id="86005-113">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="86005-113">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="86005-114">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="86005-114">Attributes</span></span>

<span data-ttu-id="86005-115">Нет.</span><span class="sxs-lookup"><span data-stu-id="86005-115">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="86005-116">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="86005-116">Child elements</span></span>

|<span data-ttu-id="86005-117">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="86005-117">**Element**</span></span>|<span data-ttu-id="86005-118">**Описание**</span><span class="sxs-lookup"><span data-stu-id="86005-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="86005-119">Строка</span><span class="sxs-lookup"><span data-stu-id="86005-119">String</span></span>](string.md) <br/> |<span data-ttu-id="86005-120">Содержит отправителя разговора.</span><span class="sxs-lookup"><span data-stu-id="86005-120">Contains a single conversation sender.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="86005-121">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="86005-121">Parent elements</span></span>

|<span data-ttu-id="86005-122">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="86005-122">**Element**</span></span>|<span data-ttu-id="86005-123">**Описание**</span><span class="sxs-lookup"><span data-stu-id="86005-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="86005-124">Беседы (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="86005-124">Conversation (ConversationType)</span></span>](conversation-conversationtype.md) <br/> |<span data-ttu-id="86005-125">Представляет одну беседу.</span><span class="sxs-lookup"><span data-stu-id="86005-125">Represents a single conversation.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="86005-126">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="86005-126">Text value</span></span>

<span data-ttu-id="86005-127">Нет.</span><span class="sxs-lookup"><span data-stu-id="86005-127">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="86005-128">Замечания</span><span class="sxs-lookup"><span data-stu-id="86005-128">Remarks</span></span>

<span data-ttu-id="86005-129">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.Этот элемент появился в Exchange Server 2010 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="86005-129">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="86005-130">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="86005-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="86005-131">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="86005-131">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="86005-132">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="86005-132">Schema name</span></span>  <br/> |<span data-ttu-id="86005-133">Схема Types</span><span class="sxs-lookup"><span data-stu-id="86005-133">Types schema</span></span>  <br/> |
|<span data-ttu-id="86005-134">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="86005-134">Validation file</span></span>  <br/> |<span data-ttu-id="86005-135">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="86005-135">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="86005-136">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="86005-136">Can be empty</span></span>  <br/> |<span data-ttu-id="86005-137">False</span><span class="sxs-lookup"><span data-stu-id="86005-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="86005-138">См. также</span><span class="sxs-lookup"><span data-stu-id="86005-138">See also</span></span>



[<span data-ttu-id="86005-139">FindConversation Operation</span><span class="sxs-lookup"><span data-stu-id="86005-139">FindConversation operation</span></span>](findconversation-operation.md)
  
[<span data-ttu-id="86005-140">Операция ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="86005-140">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)


[<span data-ttu-id="86005-141">Conversations in EWS</span><span class="sxs-lookup"><span data-stu-id="86005-141">Conversations in EWS</span></span>](http://msdn.microsoft.com/library/91e64629-db6c-4c94-9dcb-d386232e8467%28Office.15%29.aspx)

