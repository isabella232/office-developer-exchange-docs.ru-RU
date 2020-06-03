---
title: конверсатионнодес
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 5c8a35b8-a940-4b3e-8768-9ba95766fd79
description: Элемент Конверсатионнодес указывает коллекцию узлов беседы.
ms.openlocfilehash: 39ffb97f1004535e2fc70b58f8d56afe129e8ee2
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461396"
---
# <a name="conversationnodes"></a><span data-ttu-id="a7704-103">конверсатионнодес</span><span class="sxs-lookup"><span data-stu-id="a7704-103">ConversationNodes</span></span>

<span data-ttu-id="a7704-104">Элемент **конверсатионнодес** указывает коллекцию узлов беседы.</span><span class="sxs-lookup"><span data-stu-id="a7704-104">The **ConversationNodes** element specifies a collection of conversation nodes.</span></span> 
  
```XML
<ConversationNodes>
    <ConversationNode></ConversationNode>
</ConversationNodes>
```

 <span data-ttu-id="a7704-105">**аррайофконверсатионнодестипе**</span><span class="sxs-lookup"><span data-stu-id="a7704-105">**ArrayOfConversationNodesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a7704-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="a7704-106">Attributes and elements</span></span>

<span data-ttu-id="a7704-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="a7704-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a7704-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="a7704-108">Attributes</span></span>

<span data-ttu-id="a7704-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="a7704-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a7704-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="a7704-110">Child elements</span></span>

|<span data-ttu-id="a7704-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="a7704-111">**Element**</span></span>|<span data-ttu-id="a7704-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="a7704-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a7704-113">конверсатионноде</span><span class="sxs-lookup"><span data-stu-id="a7704-113">ConversationNode</span></span>](conversationnode.md) <br/> |<span data-ttu-id="a7704-114">Указывает узел в беседе.</span><span class="sxs-lookup"><span data-stu-id="a7704-114">Specifies a node in a conversation.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="a7704-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="a7704-115">Parent elements</span></span>

|<span data-ttu-id="a7704-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="a7704-116">**Element**</span></span>|<span data-ttu-id="a7704-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="a7704-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a7704-118">Беседа (Конверсатионреспонсетипе)</span><span class="sxs-lookup"><span data-stu-id="a7704-118">Conversation (ConversationResponseType)</span></span>](conversation-conversationresponsetype.md) <br/> |<span data-ttu-id="a7704-119">Представляет один диалог, возвращенный в ответе **GetConversationItems** .</span><span class="sxs-lookup"><span data-stu-id="a7704-119">Represents a single conversation returned in a **GetConversationItems** response.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="a7704-120">Примечания</span><span class="sxs-lookup"><span data-stu-id="a7704-120">Remarks</span></span>

<span data-ttu-id="a7704-121">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="a7704-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="a7704-122">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="a7704-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a7704-123">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="a7704-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a7704-124">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="a7704-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="a7704-125">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="a7704-125">Schema Name</span></span>  <br/> |<span data-ttu-id="a7704-126">Схема типа</span><span class="sxs-lookup"><span data-stu-id="a7704-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="a7704-127">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="a7704-127">Validation File</span></span>  <br/> |<span data-ttu-id="a7704-128">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="a7704-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="a7704-129">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="a7704-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="a7704-130">См. также</span><span class="sxs-lookup"><span data-stu-id="a7704-130">See also</span></span>



- [<span data-ttu-id="a7704-131">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="a7704-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

