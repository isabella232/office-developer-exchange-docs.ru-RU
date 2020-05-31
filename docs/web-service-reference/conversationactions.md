---
title: конверсатионактионс
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ConversationActions
api_type:
- schema
ms.assetid: 3d6c663d-4bd9-4eec-b95a-cd683f592672
description: Элемент Конверсатионактионс содержит коллекцию бесед и действия, которые необходимо применить к ним.
ms.openlocfilehash: 3dff7ff66f758f1cd2eb3cd7b8126294d2799fc0
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761815"
---
# <a name="conversationactions"></a><span data-ttu-id="d00c8-103">конверсатионактионс</span><span class="sxs-lookup"><span data-stu-id="d00c8-103">ConversationActions</span></span>

<span data-ttu-id="d00c8-104">Элемент **конверсатионактионс** содержит коллекцию бесед и действия, которые необходимо применить к ним.</span><span class="sxs-lookup"><span data-stu-id="d00c8-104">The **ConversationActions** element contains a collection of conversations and the actions to apply to them.</span></span> 
  
[<span data-ttu-id="d00c8-105">ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="d00c8-105">ApplyConversationAction</span></span>](applyconversationaction.md)
  
[<span data-ttu-id="d00c8-106">конверсатионактионс</span><span class="sxs-lookup"><span data-stu-id="d00c8-106">ConversationActions</span></span>](conversationactions.md)
  
```XML
<ConversationActions>
   <ConversationAction/>
</ConversationActions>
```

 <span data-ttu-id="d00c8-107">**нонемптяррайофаппликонверсатионактионтипе**</span><span class="sxs-lookup"><span data-stu-id="d00c8-107">**NonEmptyArrayOfApplyConversationActionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d00c8-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="d00c8-108">Attributes and elements</span></span>

<span data-ttu-id="d00c8-109">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="d00c8-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d00c8-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="d00c8-110">Attributes</span></span>

<span data-ttu-id="d00c8-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="d00c8-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d00c8-112">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="d00c8-112">Child elements</span></span>

|<span data-ttu-id="d00c8-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="d00c8-113">**Element**</span></span>|<span data-ttu-id="d00c8-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d00c8-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d00c8-115">конверсатионактион</span><span class="sxs-lookup"><span data-stu-id="d00c8-115">ConversationAction</span></span>](conversationaction.md) <br/> |<span data-ttu-id="d00c8-116">Содержит одно действие, которое будет применено к одной беседе.</span><span class="sxs-lookup"><span data-stu-id="d00c8-116">Contains a single action to be applied to a single conversation.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d00c8-117">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="d00c8-117">Parent elements</span></span>

|<span data-ttu-id="d00c8-118">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="d00c8-118">**Element**</span></span>|<span data-ttu-id="d00c8-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d00c8-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d00c8-120">ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="d00c8-120">ApplyConversationAction</span></span>](applyconversationaction.md) <br/> |<span data-ttu-id="d00c8-121">Определяет запрос на применение действий к элементам в беседе.</span><span class="sxs-lookup"><span data-stu-id="d00c8-121">Defines a request to apply actions to items in a conversation.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="d00c8-122">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="d00c8-122">Text value</span></span>

<span data-ttu-id="d00c8-123">Нет.</span><span class="sxs-lookup"><span data-stu-id="d00c8-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="d00c8-124">Примечания</span><span class="sxs-lookup"><span data-stu-id="d00c8-124">Remarks</span></span>

<span data-ttu-id="d00c8-125">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.Этот элемент появился в Exchange Server 2010 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="d00c8-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d00c8-126">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="d00c8-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d00c8-127">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="d00c8-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="d00c8-128">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="d00c8-128">Schema Name</span></span>  <br/> |<span data-ttu-id="d00c8-129">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="d00c8-129">Messages schema</span></span>  <br/> |
|<span data-ttu-id="d00c8-130">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="d00c8-130">Validation File</span></span>  <br/> |<span data-ttu-id="d00c8-131">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="d00c8-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="d00c8-132">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="d00c8-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="d00c8-133">False</span><span class="sxs-lookup"><span data-stu-id="d00c8-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d00c8-134">См. также</span><span class="sxs-lookup"><span data-stu-id="d00c8-134">See also</span></span>



[<span data-ttu-id="d00c8-135">Операция ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="d00c8-135">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)

