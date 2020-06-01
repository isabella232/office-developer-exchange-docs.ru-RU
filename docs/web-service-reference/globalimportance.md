---
title: глобалимпортанце
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GlobalImportance
api_type:
- schema
ms.assetid: 8bcec699-e771-4f38-b7d9-61f324af1b4e
description: Элемент Глобалимпортанце содержит совокупную важность для всех элементов бесед в почтовом ящике.
ms.openlocfilehash: c760168afa3edac20ca0ae7bc677610d8456d178
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459449"
---
# <a name="globalimportance"></a><span data-ttu-id="429f7-103">глобалимпортанце</span><span class="sxs-lookup"><span data-stu-id="429f7-103">GlobalImportance</span></span>

<span data-ttu-id="429f7-104">Элемент **глобалимпортанце** содержит совокупную важность для всех элементов бесед в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="429f7-104">The **GlobalImportance** element contains the aggregated importance for all conversation items in a mailbox.</span></span> 
  
[<span data-ttu-id="429f7-105">финдконверсатионреспонсе</span><span class="sxs-lookup"><span data-stu-id="429f7-105">FindConversationResponse</span></span>](findconversationresponse.md)
  
[<span data-ttu-id="429f7-106">Conversations</span><span class="sxs-lookup"><span data-stu-id="429f7-106">Conversations</span></span>](conversations-ex15websvcsotherref.md)
  
[<span data-ttu-id="429f7-107">Беседы (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="429f7-107">Conversation (ConversationType)</span></span>](conversation-conversationtype.md)
  
[<span data-ttu-id="429f7-108">глобалимпортанце</span><span class="sxs-lookup"><span data-stu-id="429f7-108">GlobalImportance</span></span>](globalimportance.md)
  
```XML
<GlobalImportance> Low | Normal | High </GlobalImportance>
```

 <span data-ttu-id="429f7-109">**импортанцечоицестипе**</span><span class="sxs-lookup"><span data-stu-id="429f7-109">**ImportanceChoicesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="429f7-110">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="429f7-110">Attributes and elements</span></span>

<span data-ttu-id="429f7-111">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="429f7-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="429f7-112">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="429f7-112">Attributes</span></span>

<span data-ttu-id="429f7-113">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="429f7-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="429f7-114">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="429f7-114">Child elements</span></span>

<span data-ttu-id="429f7-115">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="429f7-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="429f7-116">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="429f7-116">Parent elements</span></span>

|<span data-ttu-id="429f7-117">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="429f7-117">**Element**</span></span>|<span data-ttu-id="429f7-118">**Описание**</span><span class="sxs-lookup"><span data-stu-id="429f7-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="429f7-119">Беседы (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="429f7-119">Conversation (ConversationType)</span></span>](conversation-conversationtype.md) <br/> |<span data-ttu-id="429f7-120">Представляет одну беседу.</span><span class="sxs-lookup"><span data-stu-id="429f7-120">Represents a single conversation.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="429f7-121">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="429f7-121">Text value</span></span>

<span data-ttu-id="429f7-122">Необходимо указать текстовое значение.</span><span class="sxs-lookup"><span data-stu-id="429f7-122">A text value is required.</span></span> <span data-ttu-id="429f7-123">Ниже приведены возможные значения для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="429f7-123">The following are the possible values for this element:</span></span>
  
- <span data-ttu-id="429f7-124">Низкий</span><span class="sxs-lookup"><span data-stu-id="429f7-124">Low</span></span>
    
- <span data-ttu-id="429f7-125">Normal</span><span class="sxs-lookup"><span data-stu-id="429f7-125">Normal</span></span>
    
- <span data-ttu-id="429f7-126">Высокая</span><span class="sxs-lookup"><span data-stu-id="429f7-126">High</span></span>
    
## <a name="remarks"></a><span data-ttu-id="429f7-127">Примечания</span><span class="sxs-lookup"><span data-stu-id="429f7-127">Remarks</span></span>

<span data-ttu-id="429f7-128">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.Этот элемент появился в Exchange Server 2010 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="429f7-128">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="429f7-129">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="429f7-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="429f7-130">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="429f7-130">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="429f7-131">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="429f7-131">Schema name</span></span>  <br/> |<span data-ttu-id="429f7-132">Схема Types</span><span class="sxs-lookup"><span data-stu-id="429f7-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="429f7-133">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="429f7-133">Validation file</span></span>  <br/> |<span data-ttu-id="429f7-134">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="429f7-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="429f7-135">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="429f7-135">Can be empty</span></span>  <br/> |<span data-ttu-id="429f7-136">False</span><span class="sxs-lookup"><span data-stu-id="429f7-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="429f7-137">См. также</span><span class="sxs-lookup"><span data-stu-id="429f7-137">See also</span></span>



[<span data-ttu-id="429f7-138">FindConversation Operation</span><span class="sxs-lookup"><span data-stu-id="429f7-138">FindConversation operation</span></span>](findconversation-operation.md)
  
[<span data-ttu-id="429f7-139">Операция ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="429f7-139">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)


[<span data-ttu-id="429f7-140">Conversations in EWS</span><span class="sxs-lookup"><span data-stu-id="429f7-140">Conversations in EWS</span></span>](https://msdn.microsoft.com/library/91e64629-db6c-4c94-9dcb-d386232e8467%28Office.15%29.aspx)

