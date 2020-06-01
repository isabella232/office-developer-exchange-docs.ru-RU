---
title: Conversations
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Conversations
api_type:
- schema
ms.assetid: 1d18f98c-6457-45e9-a934-32da20885ac6
description: Элемент conversations содержит массив бесед, которые возвращаются в ответе FindConversation.
ms.openlocfilehash: 8af1023db51dd955c544422520ec5565f09f5372
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463799"
---
# <a name="conversations"></a><span data-ttu-id="f5f37-103">Беседы</span><span class="sxs-lookup"><span data-stu-id="f5f37-103">Conversations</span></span>

<span data-ttu-id="f5f37-104">Элемент conversations содержит **массив бесед,** которые возвращаются в ответе **FindConversation** .</span><span class="sxs-lookup"><span data-stu-id="f5f37-104">The **Conversations** element contains an array of conversations that are returned in the **FindConversation** response.</span></span> 
  
[<span data-ttu-id="f5f37-105">финдконверсатионреспонсе</span><span class="sxs-lookup"><span data-stu-id="f5f37-105">FindConversationResponse</span></span>](findconversationresponse.md)
  
[<span data-ttu-id="f5f37-106">Conversations</span><span class="sxs-lookup"><span data-stu-id="f5f37-106">Conversations</span></span>](conversations-ex15websvcsotherref.md)
  
```xml
<Conversations>
   <Conversation/>
</Conversations>
```

 <span data-ttu-id="f5f37-107">**аррайофконверсатионстипе**</span><span class="sxs-lookup"><span data-stu-id="f5f37-107">**ArrayOfConversationsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f5f37-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="f5f37-108">Attributes and elements</span></span>

<span data-ttu-id="f5f37-109">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="f5f37-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f5f37-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="f5f37-110">Attributes</span></span>

<span data-ttu-id="f5f37-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="f5f37-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f5f37-112">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="f5f37-112">Child elements</span></span>

|<span data-ttu-id="f5f37-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="f5f37-113">**Element**</span></span>|<span data-ttu-id="f5f37-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="f5f37-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f5f37-115">Беседы (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="f5f37-115">Conversation (ConversationType)</span></span>](conversation-conversationtype.md) <br/> |<span data-ttu-id="f5f37-116">Представляет одну беседу.</span><span class="sxs-lookup"><span data-stu-id="f5f37-116">Represents a single conversation.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f5f37-117">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="f5f37-117">Parent elements</span></span>

|<span data-ttu-id="f5f37-118">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="f5f37-118">**Element**</span></span>|<span data-ttu-id="f5f37-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="f5f37-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f5f37-120">финдконверсатионреспонсе</span><span class="sxs-lookup"><span data-stu-id="f5f37-120">FindConversationResponse</span></span>](findconversationresponse.md) <br/> |<span data-ttu-id="f5f37-121">Определяет ответ на запрос **FindConversation** .</span><span class="sxs-lookup"><span data-stu-id="f5f37-121">Defines a response to a **FindConversation** request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="f5f37-122">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="f5f37-122">Text value</span></span>

<span data-ttu-id="f5f37-123">Нет.</span><span class="sxs-lookup"><span data-stu-id="f5f37-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="f5f37-124">Примечания</span><span class="sxs-lookup"><span data-stu-id="f5f37-124">Remarks</span></span>

<span data-ttu-id="f5f37-125">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.Этот элемент появился в Exchange Server 2010 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="f5f37-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f5f37-126">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="f5f37-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f5f37-127">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="f5f37-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="f5f37-128">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="f5f37-128">Schema name</span></span>  <br/> |<span data-ttu-id="f5f37-129">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="f5f37-129">Messages schema</span></span>  <br/> |
|<span data-ttu-id="f5f37-130">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="f5f37-130">Validation file</span></span>  <br/> |<span data-ttu-id="f5f37-131">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="f5f37-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="f5f37-132">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="f5f37-132">Can be empty</span></span>  <br/> |<span data-ttu-id="f5f37-133">False</span><span class="sxs-lookup"><span data-stu-id="f5f37-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f5f37-134">См. также</span><span class="sxs-lookup"><span data-stu-id="f5f37-134">See also</span></span>



[<span data-ttu-id="f5f37-135">Операция FindConversation</span><span class="sxs-lookup"><span data-stu-id="f5f37-135">FindConversation operation</span></span>](findconversation-operation.md)


[<span data-ttu-id="f5f37-136">Conversations in EWS</span><span class="sxs-lookup"><span data-stu-id="f5f37-136">Conversations in EWS</span></span>](https://msdn.microsoft.com/library/91e64629-db6c-4c94-9dcb-d386232e8467%28Office.15%29.aspx)

