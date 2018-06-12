---
title: GlobalHasAttachments
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GlobalHasAttachments
api_type:
- schema
ms.assetid: 3d075e93-14bc-479d-957f-9b7873d1db39
description: Элемент GlobalHasAttachments содержит значение, указывающее на наличие по крайней мере один беседы элемента в почтовом ящике вложения.
ms.openlocfilehash: 85443c45f611a2f4bff392ffecb26029564d7558
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833715"
---
# <a name="globalhasattachments"></a><span data-ttu-id="94745-103">GlobalHasAttachments</span><span class="sxs-lookup"><span data-stu-id="94745-103">GlobalHasAttachments</span></span>

<span data-ttu-id="94745-104">Информация, содержащаяся в этом документе, может относиться к функциям и продуктам предварительной версии и может претерпеть значительные изменения до окончательного коммерческого выпуска. Настоящий документ предоставляется "как есть" и служит только для информационных целей. Корпорация Майкрософт не предоставляет никаких гарантий, явных или подразумеваемых, в связи с этим документом Элемент **GlobalHasAttachments** содержит значение, указывающее на наличие по крайней мере один беседы элемента в почтовом ящике вложения.</span><span class="sxs-lookup"><span data-stu-id="94745-104">The **GlobalHasAttachments** element contains a value that indicates whether at least one conversation item in a mailbox has an attachment.</span></span> 
  
[<span data-ttu-id="94745-105">FindConversationResponse</span><span class="sxs-lookup"><span data-stu-id="94745-105">FindConversationResponse</span></span>](findconversationresponse.md)
  
[<span data-ttu-id="94745-106">Conversations</span><span class="sxs-lookup"><span data-stu-id="94745-106">Conversations</span></span>](conversations-ex15websvcsotherref.md)
  
[<span data-ttu-id="94745-107">Беседы (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="94745-107">Conversation (ConversationType)</span></span>](conversation-conversationtype.md)
  
[<span data-ttu-id="94745-108">GlobalHasAttachments</span><span class="sxs-lookup"><span data-stu-id="94745-108">GlobalHasAttachments</span></span>](globalhasattachments.md)
  
```XML
<GlobalHasAttachments/>
```

 <span data-ttu-id="94745-109">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="94745-109">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="94745-110">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="94745-110">Attributes and elements</span></span>

<span data-ttu-id="94745-111">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="94745-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="94745-112">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="94745-112">Attributes</span></span>

<span data-ttu-id="94745-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="94745-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="94745-114">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="94745-114">Child elements</span></span>

<span data-ttu-id="94745-115">Нет.</span><span class="sxs-lookup"><span data-stu-id="94745-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="94745-116">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="94745-116">Parent elements</span></span>

|<span data-ttu-id="94745-117">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="94745-117">**Element**</span></span>|<span data-ttu-id="94745-118">**Описание**</span><span class="sxs-lookup"><span data-stu-id="94745-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="94745-119">Беседы (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="94745-119">Conversation (ConversationType)</span></span>](conversation-conversationtype.md) <br/> |<span data-ttu-id="94745-120">Представляет одну беседу.</span><span class="sxs-lookup"><span data-stu-id="94745-120">Represents a single conversation.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="94745-121">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="94745-121">Text value</span></span>

<span data-ttu-id="94745-p101">Значение элемента **GlobalHasAttachments** указывает, имеет ли хотя бы один беседы элемента в почтовом ящике вложения. Текстовое значение, представляющее логическое значение является обязательным. Значение **true** означает беседы на наличие по крайней мере один видимым вложения. Значение **false** означает, что беседе нет вложений или только скрыты вложения.</span><span class="sxs-lookup"><span data-stu-id="94745-p101">The value of the **GlobalHasAttachments** element indicates whether at least one conversation item in a mailbox has an attachment. A text value that represents a Boolean value is required. A value of **true** means that the conversation has at least one visible attachment. A value of **false** means that the conversation either has no attachments or has only hidden attachments.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="94745-126">Замечания</span><span class="sxs-lookup"><span data-stu-id="94745-126">Remarks</span></span>

<span data-ttu-id="94745-127">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.Этот элемент появился в Exchange Server 2010 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="94745-127">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="94745-128">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="94745-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="94745-129">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="94745-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="94745-130">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="94745-130">Schema name</span></span>  <br/> |<span data-ttu-id="94745-131">Схема Types</span><span class="sxs-lookup"><span data-stu-id="94745-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="94745-132">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="94745-132">Validation file</span></span>  <br/> |<span data-ttu-id="94745-133">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="94745-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="94745-134">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="94745-134">Can be empty</span></span>  <br/> |<span data-ttu-id="94745-135">False</span><span class="sxs-lookup"><span data-stu-id="94745-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="94745-136">См. также</span><span class="sxs-lookup"><span data-stu-id="94745-136">See also</span></span>



[<span data-ttu-id="94745-137">FindConversation Operation</span><span class="sxs-lookup"><span data-stu-id="94745-137">FindConversation operation</span></span>](findconversation-operation.md)
  
[<span data-ttu-id="94745-138">Операция ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="94745-138">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)


[<span data-ttu-id="94745-139">Conversations in EWS</span><span class="sxs-lookup"><span data-stu-id="94745-139">Conversations in EWS</span></span>](http://msdn.microsoft.com/library/91e64629-db6c-4c94-9dcb-d386232e8467%28Office.15%29.aspx)

