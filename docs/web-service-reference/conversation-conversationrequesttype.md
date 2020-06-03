---
title: Беседа (Конверсатионрекуесттипе)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 0308b71c-d4ff-44a8-b9ca-d5965291ee1d
description: Элемент CONVERSATION представляет один диалог, возвращенный в ответе GetConversationItems.
ms.openlocfilehash: 925fd6fce83cad36f4a0e95bb6228ba65e4e9c43
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44466782"
---
# <a name="conversation-conversationrequesttype"></a><span data-ttu-id="dcb3f-103">Беседа (Конверсатионрекуесттипе)</span><span class="sxs-lookup"><span data-stu-id="dcb3f-103">Conversation (ConversationRequestType)</span></span>

<span data-ttu-id="dcb3f-104">Элемент **CONVERSATION** представляет один диалог, возвращенный в ответе **GetConversationItems** .</span><span class="sxs-lookup"><span data-stu-id="dcb3f-104">The **Conversation** element represents a single conversation returned in a **GetConversationItems** response.</span></span> 
  
```XML
<Conversation>
   <ConversationId/>
   <SyncState/>
</Conversation>
```

 ****
## <a name="attributes-and-elements"></a><span data-ttu-id="dcb3f-105">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="dcb3f-105">Attributes and elements</span></span>

<span data-ttu-id="dcb3f-106">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="dcb3f-106">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="dcb3f-107">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="dcb3f-107">Attributes</span></span>

<span data-ttu-id="dcb3f-108">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="dcb3f-108">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="dcb3f-109">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="dcb3f-109">Child elements</span></span>

<span data-ttu-id="dcb3f-110">[ConversationId](conversationid.md)  |  [Синкстате (base64Binary)](syncstate-base64binary.md)</span><span class="sxs-lookup"><span data-stu-id="dcb3f-110">[ConversationId](conversationid.md) | [SyncState (base64Binary)](syncstate-base64binary.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="dcb3f-111">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="dcb3f-111">Parent elements</span></span>

[<span data-ttu-id="dcb3f-112">Беседы</span><span class="sxs-lookup"><span data-stu-id="dcb3f-112">Conversations</span></span>](conversations-ex15websvcsotherref.md)
  
## <a name="remarks"></a><span data-ttu-id="dcb3f-113">Примечания</span><span class="sxs-lookup"><span data-stu-id="dcb3f-113">Remarks</span></span>

<span data-ttu-id="dcb3f-114">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="dcb3f-114">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="dcb3f-115">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="dcb3f-115">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="dcb3f-116">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="dcb3f-116">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="dcb3f-117">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="dcb3f-117">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="dcb3f-118">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="dcb3f-118">Schema name</span></span>  <br/> |<span data-ttu-id="dcb3f-119">Схема Types</span><span class="sxs-lookup"><span data-stu-id="dcb3f-119">Types schema</span></span>  <br/> |
|<span data-ttu-id="dcb3f-120">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="dcb3f-120">Validation file</span></span>  <br/> |<span data-ttu-id="dcb3f-121">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="dcb3f-121">types.xsd</span></span>  <br/> |
|<span data-ttu-id="dcb3f-122">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="dcb3f-122">Can be empty</span></span>  <br/> |<span data-ttu-id="dcb3f-123">false</span><span class="sxs-lookup"><span data-stu-id="dcb3f-123">false</span></span>  <br/> |
   

