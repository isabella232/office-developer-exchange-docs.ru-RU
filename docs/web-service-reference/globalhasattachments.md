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
ms.openlocfilehash: e314e8e5c06ca7d7820b910c05b381765e88911f
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459478"
---
# <a name="globalhasattachments"></a><span data-ttu-id="88161-103">GlobalHasAttachments</span><span class="sxs-lookup"><span data-stu-id="88161-103">GlobalHasAttachments</span></span>

<span data-ttu-id="88161-104">Информация, содержащаяся в этом документе, может относиться к функциям и продуктам предварительной версии и может претерпеть значительные изменения до окончательного коммерческого выпуска. Настоящий документ предоставляется "как есть" и служит только для информационных целей. Корпорация Майкрософт не предоставляет никаких гарантий, явных или подразумеваемых, в связи с этим документом Элемент **GlobalHasAttachments** содержит значение, указывающее на наличие по крайней мере один беседы элемента в почтовом ящике вложения.</span><span class="sxs-lookup"><span data-stu-id="88161-104">The **GlobalHasAttachments** element contains a value that indicates whether at least one conversation item in a mailbox has an attachment.</span></span> 
  
[<span data-ttu-id="88161-105">финдконверсатионреспонсе</span><span class="sxs-lookup"><span data-stu-id="88161-105">FindConversationResponse</span></span>](findconversationresponse.md)
  
[<span data-ttu-id="88161-106">Conversations</span><span class="sxs-lookup"><span data-stu-id="88161-106">Conversations</span></span>](conversations-ex15websvcsotherref.md)
  
[<span data-ttu-id="88161-107">Беседы (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="88161-107">Conversation (ConversationType)</span></span>](conversation-conversationtype.md)
  
[<span data-ttu-id="88161-108">GlobalHasAttachments</span><span class="sxs-lookup"><span data-stu-id="88161-108">GlobalHasAttachments</span></span>](globalhasattachments.md)
  
```XML
<GlobalHasAttachments/>
```

 <span data-ttu-id="88161-109">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="88161-109">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="88161-110">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="88161-110">Attributes and elements</span></span>

<span data-ttu-id="88161-111">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="88161-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="88161-112">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="88161-112">Attributes</span></span>

<span data-ttu-id="88161-113">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="88161-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="88161-114">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="88161-114">Child elements</span></span>

<span data-ttu-id="88161-115">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="88161-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="88161-116">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="88161-116">Parent elements</span></span>

|<span data-ttu-id="88161-117">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="88161-117">**Element**</span></span>|<span data-ttu-id="88161-118">**Описание**</span><span class="sxs-lookup"><span data-stu-id="88161-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="88161-119">Беседы (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="88161-119">Conversation (ConversationType)</span></span>](conversation-conversationtype.md) <br/> |<span data-ttu-id="88161-120">Представляет одну беседу.</span><span class="sxs-lookup"><span data-stu-id="88161-120">Represents a single conversation.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="88161-121">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="88161-121">Text value</span></span>

<span data-ttu-id="88161-p101">Значение элемента **GlobalHasAttachments** указывает, имеет ли хотя бы один беседы элемента в почтовом ящике вложения. Текстовое значение, представляющее логическое значение является обязательным. Значение **true** означает беседы на наличие по крайней мере один видимым вложения. Значение **false** означает, что беседе нет вложений или только скрыты вложения.</span><span class="sxs-lookup"><span data-stu-id="88161-p101">The value of the **GlobalHasAttachments** element indicates whether at least one conversation item in a mailbox has an attachment. A text value that represents a Boolean value is required. A value of **true** means that the conversation has at least one visible attachment. A value of **false** means that the conversation either has no attachments or has only hidden attachments.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="88161-126">Примечания</span><span class="sxs-lookup"><span data-stu-id="88161-126">Remarks</span></span>

<span data-ttu-id="88161-127">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.Этот элемент появился в Exchange Server 2010 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="88161-127">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="88161-128">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="88161-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="88161-129">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="88161-129">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="88161-130">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="88161-130">Schema name</span></span>  <br/> |<span data-ttu-id="88161-131">Схема Types</span><span class="sxs-lookup"><span data-stu-id="88161-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="88161-132">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="88161-132">Validation file</span></span>  <br/> |<span data-ttu-id="88161-133">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="88161-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="88161-134">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="88161-134">Can be empty</span></span>  <br/> |<span data-ttu-id="88161-135">False</span><span class="sxs-lookup"><span data-stu-id="88161-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="88161-136">См. также</span><span class="sxs-lookup"><span data-stu-id="88161-136">See also</span></span>



[<span data-ttu-id="88161-137">FindConversation Operation</span><span class="sxs-lookup"><span data-stu-id="88161-137">FindConversation operation</span></span>](findconversation-operation.md)
  
[<span data-ttu-id="88161-138">Операция ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="88161-138">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)


[<span data-ttu-id="88161-139">Conversations in EWS</span><span class="sxs-lookup"><span data-stu-id="88161-139">Conversations in EWS</span></span>](https://msdn.microsoft.com/library/91e64629-db6c-4c94-9dcb-d386232e8467%28Office.15%29.aspx)

