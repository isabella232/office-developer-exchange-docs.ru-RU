---
title: GlobalUniqueRecipients
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GlobalUniqueRecipients
api_type:
- schema
ms.assetid: 67379c1c-85d9-4b11-8f17-ad9d24904788
description: Элемент GlobalUniqueRecipients содержит список получателей беседы сводный в почтовый ящик.
ms.openlocfilehash: 5eb6e60d3ece8d8369f4603e36ffaaf72a3e459d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833742"
---
# <a name="globaluniquerecipients"></a><span data-ttu-id="edc5e-103">GlobalUniqueRecipients</span><span class="sxs-lookup"><span data-stu-id="edc5e-103">GlobalUniqueRecipients</span></span>

<span data-ttu-id="edc5e-104">Информация, содержащаяся в этом документе, может относиться к функциям и продуктам предварительной версии и может претерпеть значительные изменения до окончательного коммерческого выпуска. Настоящий документ предоставляется "как есть" и служит только для информационных целей. Корпорация Майкрософт не предоставляет никаких гарантий, явных или подразумеваемых, в связи с этим документом Элемент **GlobalUniqueRecipients** содержит список получателей беседы сводный в почтовый ящик.</span><span class="sxs-lookup"><span data-stu-id="edc5e-104">The **GlobalUniqueRecipients** element contains the recipient list of a conversation aggregated across a mailbox.</span></span> 
  
[<span data-ttu-id="edc5e-105">FindConversationResponse</span><span class="sxs-lookup"><span data-stu-id="edc5e-105">FindConversationResponse</span></span>](findconversationresponse.md)
  
[<span data-ttu-id="edc5e-106">Conversations</span><span class="sxs-lookup"><span data-stu-id="edc5e-106">Conversations</span></span>](conversations-ex15websvcsotherref.md)
  
[<span data-ttu-id="edc5e-107">Беседы (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="edc5e-107">Conversation (ConversationType)</span></span>](conversation-conversationtype.md)
  
[<span data-ttu-id="edc5e-108">GlobalUniqueRecipients</span><span class="sxs-lookup"><span data-stu-id="edc5e-108">GlobalUniqueRecipients</span></span>](globaluniquerecipients.md)
  
```XML
<GlobalUniqueRecipients>
   <String/>
</GlobalUniqueRecipients>
```

 <span data-ttu-id="edc5e-109">**ArrayOfStringsType**</span><span class="sxs-lookup"><span data-stu-id="edc5e-109">**ArrayOfStringsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="edc5e-110">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="edc5e-110">Attributes and elements</span></span>

<span data-ttu-id="edc5e-111">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="edc5e-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="edc5e-112">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="edc5e-112">Attributes</span></span>

<span data-ttu-id="edc5e-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="edc5e-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="edc5e-114">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="edc5e-114">Child elements</span></span>

|<span data-ttu-id="edc5e-115">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="edc5e-115">**Element**</span></span>|<span data-ttu-id="edc5e-116">**Описание**</span><span class="sxs-lookup"><span data-stu-id="edc5e-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="edc5e-117">Строка</span><span class="sxs-lookup"><span data-stu-id="edc5e-117">String</span></span>](string.md) <br/> |<span data-ttu-id="edc5e-118">Содержит получателя разговора.</span><span class="sxs-lookup"><span data-stu-id="edc5e-118">Contains a single conversation recipient.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="edc5e-119">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="edc5e-119">Parent elements</span></span>

|<span data-ttu-id="edc5e-120">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="edc5e-120">**Element**</span></span>|<span data-ttu-id="edc5e-121">**Описание**</span><span class="sxs-lookup"><span data-stu-id="edc5e-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="edc5e-122">Беседы (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="edc5e-122">Conversation (ConversationType)</span></span>](conversation-conversationtype.md) <br/> |<span data-ttu-id="edc5e-123">Представляет одну беседу.</span><span class="sxs-lookup"><span data-stu-id="edc5e-123">Represents a single conversation.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="edc5e-124">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="edc5e-124">Text value</span></span>

<span data-ttu-id="edc5e-125">Нет.</span><span class="sxs-lookup"><span data-stu-id="edc5e-125">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="edc5e-126">Замечания</span><span class="sxs-lookup"><span data-stu-id="edc5e-126">Remarks</span></span>

<span data-ttu-id="edc5e-127">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.Этот элемент появился в Exchange Server 2010 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="edc5e-127">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="edc5e-128">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="edc5e-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="edc5e-129">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="edc5e-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="edc5e-130">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="edc5e-130">Schema name</span></span>  <br/> |<span data-ttu-id="edc5e-131">Схема Types</span><span class="sxs-lookup"><span data-stu-id="edc5e-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="edc5e-132">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="edc5e-132">Validation file</span></span>  <br/> |<span data-ttu-id="edc5e-133">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="edc5e-133">types.xsd</span></span>  <br/> |
|<span data-ttu-id="edc5e-134">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="edc5e-134">Can be empty</span></span>  <br/> |<span data-ttu-id="edc5e-135">False</span><span class="sxs-lookup"><span data-stu-id="edc5e-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="edc5e-136">См. также</span><span class="sxs-lookup"><span data-stu-id="edc5e-136">See also</span></span>



[<span data-ttu-id="edc5e-137">FindConversation Operation</span><span class="sxs-lookup"><span data-stu-id="edc5e-137">FindConversation operation</span></span>](findconversation-operation.md)
  
[<span data-ttu-id="edc5e-138">Операция ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="edc5e-138">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)


[<span data-ttu-id="edc5e-139">Conversations in EWS</span><span class="sxs-lookup"><span data-stu-id="edc5e-139">Conversations in EWS</span></span>](http://msdn.microsoft.com/library/91e64629-db6c-4c94-9dcb-d386232e8467%28Office.15%29.aspx)

