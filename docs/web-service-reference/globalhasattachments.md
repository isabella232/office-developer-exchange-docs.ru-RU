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
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833715"
---
# <a name="globalhasattachments"></a><span data-ttu-id="84c13-103">GlobalHasAttachments</span><span class="sxs-lookup"><span data-stu-id="84c13-103">GlobalHasAttachments</span></span>

<span data-ttu-id="84c13-104">Информация, содержащаяся в этом документе, может относиться к функциям и продуктам предварительной версии и может претерпеть значительные изменения до окончательного коммерческого выпуска. Настоящий документ предоставляется "как есть" и служит только для информационных целей. Корпорация Майкрософт не предоставляет никаких гарантий, явных или подразумеваемых, в связи с этим документом Элемент **GlobalHasAttachments** содержит значение, указывающее на наличие по крайней мере один беседы элемента в почтовом ящике вложения.</span><span class="sxs-lookup"><span data-stu-id="84c13-104">The **GlobalHasAttachments** element contains a value that indicates whether at least one conversation item in a mailbox has an attachment.</span></span> 
  
[<span data-ttu-id="84c13-105">FindConversationResponse</span><span class="sxs-lookup"><span data-stu-id="84c13-105">FindConversationResponse</span></span>](findconversationresponse.md)
  
[<span data-ttu-id="84c13-106">Conversations</span><span class="sxs-lookup"><span data-stu-id="84c13-106">Conversations</span></span>](conversations-ex15websvcsotherref.md)
  
[<span data-ttu-id="84c13-107">Беседы (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="84c13-107">Conversation (ConversationType)</span></span>](conversation-conversationtype.md)
  
[<span data-ttu-id="84c13-108">GlobalHasAttachments</span><span class="sxs-lookup"><span data-stu-id="84c13-108">GlobalHasAttachments</span></span>](globalhasattachments.md)
  
```XML
<GlobalHasAttachments/>
```

 <span data-ttu-id="84c13-109">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="84c13-109">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="84c13-110">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="84c13-110">Attributes and elements</span></span>

<span data-ttu-id="84c13-111">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="84c13-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="84c13-112">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="84c13-112">Attributes</span></span>

<span data-ttu-id="84c13-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="84c13-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="84c13-114">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="84c13-114">Child elements</span></span>

<span data-ttu-id="84c13-115">Нет.</span><span class="sxs-lookup"><span data-stu-id="84c13-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="84c13-116">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="84c13-116">Parent elements</span></span>

|<span data-ttu-id="84c13-117">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="84c13-117">**Element**</span></span>|<span data-ttu-id="84c13-118">**Описание**</span><span class="sxs-lookup"><span data-stu-id="84c13-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="84c13-119">Беседы (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="84c13-119">Conversation (ConversationType)</span></span>](conversation-conversationtype.md) <br/> |<span data-ttu-id="84c13-120">Представляет одну беседу.</span><span class="sxs-lookup"><span data-stu-id="84c13-120">Represents a single conversation.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="84c13-121">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="84c13-121">Text value</span></span>

<span data-ttu-id="84c13-p101">Значение элемента **GlobalHasAttachments** указывает, имеет ли хотя бы один беседы элемента в почтовом ящике вложения. Текстовое значение, представляющее логическое значение является обязательным. Значение **true** означает беседы на наличие по крайней мере один видимым вложения. Значение **false** означает, что беседе нет вложений или только скрыты вложения.</span><span class="sxs-lookup"><span data-stu-id="84c13-p101">The value of the **GlobalHasAttachments** element indicates whether at least one conversation item in a mailbox has an attachment. A text value that represents a Boolean value is required. A value of **true** means that the conversation has at least one visible attachment. A value of **false** means that the conversation either has no attachments or has only hidden attachments.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="84c13-126">Замечания</span><span class="sxs-lookup"><span data-stu-id="84c13-126">Remarks</span></span>

<span data-ttu-id="84c13-127">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.Этот элемент появился в Exchange Server 2010 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="84c13-127">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="84c13-128">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="84c13-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="84c13-129">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="84c13-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="84c13-130">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="84c13-130">Schema name</span></span>  <br/> |<span data-ttu-id="84c13-131">Схема Types</span><span class="sxs-lookup"><span data-stu-id="84c13-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="84c13-132">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="84c13-132">Validation file</span></span>  <br/> |<span data-ttu-id="84c13-133">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="84c13-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="84c13-134">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="84c13-134">Can be empty</span></span>  <br/> |<span data-ttu-id="84c13-135">False</span><span class="sxs-lookup"><span data-stu-id="84c13-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="84c13-136">См. также</span><span class="sxs-lookup"><span data-stu-id="84c13-136">See also</span></span>



[<span data-ttu-id="84c13-137">FindConversation Operation</span><span class="sxs-lookup"><span data-stu-id="84c13-137">FindConversation operation</span></span>](findconversation-operation.md)
  
[<span data-ttu-id="84c13-138">Операция ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="84c13-138">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)


[<span data-ttu-id="84c13-139">Conversations in EWS</span><span class="sxs-lookup"><span data-stu-id="84c13-139">Conversations in EWS</span></span>](http://msdn.microsoft.com/library/91e64629-db6c-4c94-9dcb-d386232e8467%28Office.15%29.aspx)

