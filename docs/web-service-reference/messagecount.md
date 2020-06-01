---
title: MessageCount
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MessageCount
api_type:
- schema
ms.assetid: 5efc5903-fcb3-44cf-aabb-b6912268df8e
description: Элемент MessageCount содержит общее число элементов беседы в текущей папке.
ms.openlocfilehash: f0b6ffce370ccf8195a9132146e062f0660163c8
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/01/2020
ms.locfileid: "44468707"
---
# <a name="messagecount"></a><span data-ttu-id="56f08-103">MessageCount</span><span class="sxs-lookup"><span data-stu-id="56f08-103">MessageCount</span></span>

<span data-ttu-id="56f08-104">Элемент **MessageCount** содержит общее число элементов беседы в текущей папке.</span><span class="sxs-lookup"><span data-stu-id="56f08-104">The **MessageCount** element contains the total number of conversation items in the current folder.</span></span> 
  
[<span data-ttu-id="56f08-105">финдконверсатионреспонсе</span><span class="sxs-lookup"><span data-stu-id="56f08-105">FindConversationResponse</span></span>](findconversationresponse.md)
  
[<span data-ttu-id="56f08-106">Conversations</span><span class="sxs-lookup"><span data-stu-id="56f08-106">Conversations</span></span>](conversations-ex15websvcsotherref.md)
  
[<span data-ttu-id="56f08-107">Беседы (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="56f08-107">Conversation (ConversationType)</span></span>](conversation-conversationtype.md)
  
[<span data-ttu-id="56f08-108">MessageCount</span><span class="sxs-lookup"><span data-stu-id="56f08-108">MessageCount</span></span>](messagecount.md)
  
```XML
<MessageCount/>
```

 <span data-ttu-id="56f08-109">**xs: int**</span><span class="sxs-lookup"><span data-stu-id="56f08-109">**xs:int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="56f08-110">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="56f08-110">Attributes and elements</span></span>

<span data-ttu-id="56f08-111">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="56f08-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="56f08-112">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="56f08-112">Attributes</span></span>

<span data-ttu-id="56f08-113">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="56f08-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="56f08-114">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="56f08-114">Child elements</span></span>

<span data-ttu-id="56f08-115">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="56f08-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="56f08-116">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="56f08-116">Parent elements</span></span>

|<span data-ttu-id="56f08-117">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="56f08-117">**Element**</span></span>|<span data-ttu-id="56f08-118">**Описание**</span><span class="sxs-lookup"><span data-stu-id="56f08-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="56f08-119">Беседы (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="56f08-119">Conversation (ConversationType)</span></span>](conversation-conversationtype.md) <br/> |<span data-ttu-id="56f08-120">Представляет одну беседу.</span><span class="sxs-lookup"><span data-stu-id="56f08-120">Represents a single conversation.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="56f08-121">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="56f08-121">Text value</span></span>

<span data-ttu-id="56f08-122">Текстовое значение элемента **MessageCount** — это общее количество элементов бесед в папке.</span><span class="sxs-lookup"><span data-stu-id="56f08-122">The text value of the **MessageCount** element is the total number of conversation items in a folder.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="56f08-123">Примечания</span><span class="sxs-lookup"><span data-stu-id="56f08-123">Remarks</span></span>

<span data-ttu-id="56f08-124">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.Этот элемент появился в Exchange Server 2010 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="56f08-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="56f08-125">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="56f08-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="56f08-126">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="56f08-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="56f08-127">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="56f08-127">Schema name</span></span>  <br/> |<span data-ttu-id="56f08-128">Схема Types</span><span class="sxs-lookup"><span data-stu-id="56f08-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="56f08-129">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="56f08-129">Validation file</span></span>  <br/> |<span data-ttu-id="56f08-130">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="56f08-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="56f08-131">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="56f08-131">Can be empty</span></span>  <br/> |<span data-ttu-id="56f08-132">False</span><span class="sxs-lookup"><span data-stu-id="56f08-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="56f08-133">См. также</span><span class="sxs-lookup"><span data-stu-id="56f08-133">See also</span></span>



[<span data-ttu-id="56f08-134">FindConversation Operation</span><span class="sxs-lookup"><span data-stu-id="56f08-134">FindConversation operation</span></span>](findconversation-operation.md)
  
[<span data-ttu-id="56f08-135">Операция ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="56f08-135">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)


- [<span data-ttu-id="56f08-136">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="56f08-136">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="56f08-137">Conversations in EWS</span><span class="sxs-lookup"><span data-stu-id="56f08-137">Conversations in EWS</span></span>](https://msdn.microsoft.com/library/91e64629-db6c-4c94-9dcb-d386232e8467%28Office.15%29.aspx)

