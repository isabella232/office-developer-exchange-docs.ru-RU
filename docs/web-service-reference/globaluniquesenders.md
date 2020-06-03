---
title: глобалуникуесендерс
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GlobalUniqueSenders
api_type:
- schema
ms.assetid: 6bd9e9cb-19c8-45af-b211-dfb8a6003b1b
description: Элемент Глобалуникуесендер содержит список всех отправителей элементов беседы в почтовом ящике.
ms.openlocfilehash: 0e85e201017e175a9ffc6b923976020d4157d5b7
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459065"
---
# <a name="globaluniquesenders"></a><span data-ttu-id="33aec-103">глобалуникуесендерс</span><span class="sxs-lookup"><span data-stu-id="33aec-103">GlobalUniqueSenders</span></span>

<span data-ttu-id="33aec-104">Элемент **глобалуникуесендер** содержит список всех отправителей элементов беседы в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="33aec-104">The **GlobalUniqueSender** element contains a list of all the senders of conversation items in the mailbox.</span></span> 
  
[<span data-ttu-id="33aec-105">финдконверсатионреспонсе</span><span class="sxs-lookup"><span data-stu-id="33aec-105">FindConversationResponse</span></span>](findconversationresponse.md)
  
[<span data-ttu-id="33aec-106">Conversations</span><span class="sxs-lookup"><span data-stu-id="33aec-106">Conversations</span></span>](conversations-ex15websvcsotherref.md)
  
[<span data-ttu-id="33aec-107">Беседы (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="33aec-107">Conversation (ConversationType)</span></span>](conversation-conversationtype.md)
  
[<span data-ttu-id="33aec-108">глобалуникуесендерс</span><span class="sxs-lookup"><span data-stu-id="33aec-108">GlobalUniqueSenders</span></span>](globaluniquesenders.md)
  
```XML
<GlobalUniqueSender>
   <String/>
</GlobalUniqueSender>
```

 <span data-ttu-id="33aec-109">**аррайофстрингстипе**</span><span class="sxs-lookup"><span data-stu-id="33aec-109">**ArrayOfStringsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="33aec-110">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="33aec-110">Attributes and elements</span></span>

<span data-ttu-id="33aec-111">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="33aec-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="33aec-112">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="33aec-112">Attributes</span></span>

<span data-ttu-id="33aec-113">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="33aec-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="33aec-114">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="33aec-114">Child elements</span></span>

|<span data-ttu-id="33aec-115">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="33aec-115">**Element**</span></span>|<span data-ttu-id="33aec-116">**Описание**</span><span class="sxs-lookup"><span data-stu-id="33aec-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="33aec-117">Строка</span><span class="sxs-lookup"><span data-stu-id="33aec-117">String</span></span>](string.md) <br/> |<span data-ttu-id="33aec-118">Содержит одного отправителя беседы.</span><span class="sxs-lookup"><span data-stu-id="33aec-118">Contains a single conversation sender.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="33aec-119">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="33aec-119">Parent elements</span></span>

|<span data-ttu-id="33aec-120">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="33aec-120">**Element**</span></span>|<span data-ttu-id="33aec-121">**Описание**</span><span class="sxs-lookup"><span data-stu-id="33aec-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="33aec-122">Беседы (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="33aec-122">Conversation (ConversationType)</span></span>](conversation-conversationtype.md) <br/> |<span data-ttu-id="33aec-123">Представляет одну беседу.</span><span class="sxs-lookup"><span data-stu-id="33aec-123">Represents a single conversation.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="33aec-124">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="33aec-124">Text value</span></span>

<span data-ttu-id="33aec-125">Нет.</span><span class="sxs-lookup"><span data-stu-id="33aec-125">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="33aec-126">Примечания</span><span class="sxs-lookup"><span data-stu-id="33aec-126">Remarks</span></span>

<span data-ttu-id="33aec-127">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.Этот элемент появился в Exchange Server 2010 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="33aec-127">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="33aec-128">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="33aec-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="33aec-129">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="33aec-129">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="33aec-130">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="33aec-130">Schema name</span></span>  <br/> |<span data-ttu-id="33aec-131">Схема Types</span><span class="sxs-lookup"><span data-stu-id="33aec-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="33aec-132">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="33aec-132">Validation file</span></span>  <br/> |<span data-ttu-id="33aec-133">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="33aec-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="33aec-134">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="33aec-134">Can be empty</span></span>  <br/> |<span data-ttu-id="33aec-135">False</span><span class="sxs-lookup"><span data-stu-id="33aec-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="33aec-136">См. также</span><span class="sxs-lookup"><span data-stu-id="33aec-136">See also</span></span>



[<span data-ttu-id="33aec-137">FindConversation Operation</span><span class="sxs-lookup"><span data-stu-id="33aec-137">FindConversation operation</span></span>](findconversation-operation.md)
  
[<span data-ttu-id="33aec-138">Операция ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="33aec-138">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)


[<span data-ttu-id="33aec-139">Conversations in EWS</span><span class="sxs-lookup"><span data-stu-id="33aec-139">Conversations in EWS</span></span>](https://msdn.microsoft.com/library/91e64629-db6c-4c94-9dcb-d386232e8467%28Office.15%29.aspx)

