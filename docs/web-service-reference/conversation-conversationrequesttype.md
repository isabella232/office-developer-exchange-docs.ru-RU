---
title: Беседы (ConversationRequestType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 0308b71c-d4ff-44a8-b9ca-d5965291ee1d
description: Элемент Conversation представляет разговора, возвращаемых в ответе GetConversationItems.
ms.openlocfilehash: ef56e26fda7d2bf6556069355918aa576ce14cb6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761804"
---
# <a name="conversation-conversationrequesttype"></a><span data-ttu-id="b5b9d-103">Беседы (ConversationRequestType)</span><span class="sxs-lookup"><span data-stu-id="b5b9d-103">Conversation (ConversationRequestType)</span></span>

<span data-ttu-id="b5b9d-104">Элемент **Conversation** представляет разговора, возвращаемых в ответе **GetConversationItems** .</span><span class="sxs-lookup"><span data-stu-id="b5b9d-104">The **Conversation** element represents a single conversation returned in a **GetConversationItems** response.</span></span> 
  
```XML
<Conversation>
   <ConversationId/>
   <SyncState/>
</Conversation>
```

 ****
## <a name="attributes-and-elements"></a><span data-ttu-id="b5b9d-105">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="b5b9d-105">Attributes and elements</span></span>

<span data-ttu-id="b5b9d-106">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="b5b9d-106">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b5b9d-107">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="b5b9d-107">Attributes</span></span>

<span data-ttu-id="b5b9d-108">Нет.</span><span class="sxs-lookup"><span data-stu-id="b5b9d-108">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b5b9d-109">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="b5b9d-109">Child elements</span></span>

<span data-ttu-id="b5b9d-110">[ConversationId](conversationid.md) | [состояние (base64Binary)](syncstate-base64binary.md)</span><span class="sxs-lookup"><span data-stu-id="b5b9d-110">[ConversationId](conversationid.md) | [SyncState (base64Binary)](syncstate-base64binary.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="b5b9d-111">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="b5b9d-111">Parent elements</span></span>

[<span data-ttu-id="b5b9d-112">Conversations</span><span class="sxs-lookup"><span data-stu-id="b5b9d-112">Conversations</span></span>](conversations-ex15websvcsotherref.md)
  
## <a name="remarks"></a><span data-ttu-id="b5b9d-113">Замечания</span><span class="sxs-lookup"><span data-stu-id="b5b9d-113">Remarks</span></span>

<span data-ttu-id="b5b9d-114">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="b5b9d-114">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="b5b9d-115">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="b5b9d-115">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b5b9d-116">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="b5b9d-116">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b5b9d-117">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="b5b9d-117">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="b5b9d-118">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="b5b9d-118">Schema name</span></span>  <br/> |<span data-ttu-id="b5b9d-119">Схема Types</span><span class="sxs-lookup"><span data-stu-id="b5b9d-119">Types schema</span></span>  <br/> |
|<span data-ttu-id="b5b9d-120">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="b5b9d-120">Validation file</span></span>  <br/> |<span data-ttu-id="b5b9d-121">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="b5b9d-121">types.xsd</span></span>  <br/> |
|<span data-ttu-id="b5b9d-122">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="b5b9d-122">Can be empty</span></span>  <br/> |<span data-ttu-id="b5b9d-123">Нет</span><span class="sxs-lookup"><span data-stu-id="b5b9d-123">false</span></span>  <br/> |
   

