---
title: UniqueUnreadSenders
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UniqueUnreadSenders
api_type:
- schema
ms.assetid: eb7d1274-ce2e-4ef8-b47f-e911174aab0c
description: Элемент UniqueUnreadSenders содержит список всех людей, отправленные сообщения, которые в настоящее время непрочитанные сообщения в эту беседу в текущую папку. Этот элемент доступен только для чтения.
ms.openlocfilehash: d1f5593f6b86745aa27d86e9d25487f5855cb0cc
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19840287"
---
# <a name="uniqueunreadsenders"></a><span data-ttu-id="ecd47-104">UniqueUnreadSenders</span><span class="sxs-lookup"><span data-stu-id="ecd47-104">UniqueUnreadSenders</span></span>

<span data-ttu-id="ecd47-105">Элемент **UniqueUnreadSenders** содержит список всех людей, отправленные сообщения, которые в настоящее время непрочитанные сообщения в эту беседу в текущую папку.</span><span class="sxs-lookup"><span data-stu-id="ecd47-105">The **UniqueUnreadSenders** element contains a list of all the people who have sent messages that are currently unread in this conversation in the current folder.</span></span> <span data-ttu-id="ecd47-106">Этот элемент доступен только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ecd47-106">This element is read-only.</span></span> 
  
[<span data-ttu-id="ecd47-107">FindConversationResponse</span><span class="sxs-lookup"><span data-stu-id="ecd47-107">FindConversationResponse</span></span>](findconversationresponse.md)
  
[<span data-ttu-id="ecd47-108">Conversations</span><span class="sxs-lookup"><span data-stu-id="ecd47-108">Conversations</span></span>](conversations-ex15websvcsotherref.md)
  
[<span data-ttu-id="ecd47-109">Беседы (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="ecd47-109">Conversation (ConversationType)</span></span>](conversation-conversationtype.md)
  
[<span data-ttu-id="ecd47-110">UniqueUnreadSenders</span><span class="sxs-lookup"><span data-stu-id="ecd47-110">UniqueUnreadSenders</span></span>](uniqueunreadsenders.md)
  
```XML
<UniqueUnreadSenders>
   <String/>
</UniqueUnreadSenders>
```

 <span data-ttu-id="ecd47-111">**ArrayOfStringsType**</span><span class="sxs-lookup"><span data-stu-id="ecd47-111">**ArrayOfStringsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ecd47-112">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="ecd47-112">Attributes and elements</span></span>

<span data-ttu-id="ecd47-113">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="ecd47-113">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ecd47-114">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="ecd47-114">Attributes</span></span>

<span data-ttu-id="ecd47-115">Нет.</span><span class="sxs-lookup"><span data-stu-id="ecd47-115">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ecd47-116">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="ecd47-116">Child elements</span></span>

|<span data-ttu-id="ecd47-117">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="ecd47-117">**Element**</span></span>|<span data-ttu-id="ecd47-118">**Описание**</span><span class="sxs-lookup"><span data-stu-id="ecd47-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ecd47-119">Строка</span><span class="sxs-lookup"><span data-stu-id="ecd47-119">String</span></span>](string.md) <br/> |<span data-ttu-id="ecd47-120">Содержит отправителя разговора.</span><span class="sxs-lookup"><span data-stu-id="ecd47-120">Contains a single conversation sender.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="ecd47-121">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="ecd47-121">Parent elements</span></span>

|<span data-ttu-id="ecd47-122">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="ecd47-122">**Element**</span></span>|<span data-ttu-id="ecd47-123">**Описание**</span><span class="sxs-lookup"><span data-stu-id="ecd47-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ecd47-124">Беседы (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="ecd47-124">Conversation (ConversationType)</span></span>](conversation-conversationtype.md) <br/> |<span data-ttu-id="ecd47-125">Представляет одну беседу.</span><span class="sxs-lookup"><span data-stu-id="ecd47-125">Represents a single conversation.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="ecd47-126">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="ecd47-126">Text value</span></span>

<span data-ttu-id="ecd47-127">Нет.</span><span class="sxs-lookup"><span data-stu-id="ecd47-127">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="ecd47-128">Замечания</span><span class="sxs-lookup"><span data-stu-id="ecd47-128">Remarks</span></span>

<span data-ttu-id="ecd47-129">Этот элемент был представлен в пакете обновления 1 (SP1) для Exchange Server 2010. Схема, описывающая этот элемент находится в виртуальном каталоге IIS, на котором размещается веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="ecd47-129">This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ecd47-130">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="ecd47-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ecd47-131">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="ecd47-131">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="ecd47-132">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="ecd47-132">Schema name</span></span>  <br/> |<span data-ttu-id="ecd47-133">Схема Types</span><span class="sxs-lookup"><span data-stu-id="ecd47-133">Types schema</span></span>  <br/> |
|<span data-ttu-id="ecd47-134">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="ecd47-134">Validation file</span></span>  <br/> |<span data-ttu-id="ecd47-135">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="ecd47-135">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="ecd47-136">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="ecd47-136">Can be empty</span></span>  <br/> |<span data-ttu-id="ecd47-137">False</span><span class="sxs-lookup"><span data-stu-id="ecd47-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ecd47-138">См. также</span><span class="sxs-lookup"><span data-stu-id="ecd47-138">See also</span></span>



[<span data-ttu-id="ecd47-139">FindConversation Operation</span><span class="sxs-lookup"><span data-stu-id="ecd47-139">FindConversation operation</span></span>](findconversation-operation.md)
  
[<span data-ttu-id="ecd47-140">Операция ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="ecd47-140">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)


[<span data-ttu-id="ecd47-141">Conversations in EWS</span><span class="sxs-lookup"><span data-stu-id="ecd47-141">Conversations in EWS</span></span>](http://msdn.microsoft.com/library/91e64629-db6c-4c94-9dcb-d386232e8467%28Office.15%29.aspx)

