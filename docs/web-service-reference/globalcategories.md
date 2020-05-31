---
title: глобалкатегориес
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GlobalCategories
api_type:
- schema
ms.assetid: 7a1d3f04-4ada-4a31-845e-f1f1ff6e136f
description: Элемент Глобалкатегориес содержит список категорий для всех элементов бесед в почтовом ящике.
ms.openlocfilehash: 5cedea821b14264f15026c2d297c3017534ca354
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833711"
---
# <a name="globalcategories"></a><span data-ttu-id="f41e1-103">глобалкатегориес</span><span class="sxs-lookup"><span data-stu-id="f41e1-103">GlobalCategories</span></span>

<span data-ttu-id="f41e1-104">Элемент **глобалкатегориес** содержит список категорий для всех элементов бесед в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="f41e1-104">The **GlobalCategories** element contains the category list for all conversation items in a mailbox.</span></span> 
  
[<span data-ttu-id="f41e1-105">финдконверсатионреспонсе</span><span class="sxs-lookup"><span data-stu-id="f41e1-105">FindConversationResponse</span></span>](findconversationresponse.md)
  
[<span data-ttu-id="f41e1-106">Conversations</span><span class="sxs-lookup"><span data-stu-id="f41e1-106">Conversations</span></span>](conversations-ex15websvcsotherref.md)
  
[<span data-ttu-id="f41e1-107">Беседы (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="f41e1-107">Conversation (ConversationType)</span></span>](conversation-conversationtype.md)
  
[<span data-ttu-id="f41e1-108">глобалкатегориес</span><span class="sxs-lookup"><span data-stu-id="f41e1-108">GlobalCategories</span></span>](globalcategories.md)
  
```XML
<GlobalCategories>
   <String/>
</GlobalCategories>
```

 <span data-ttu-id="f41e1-109">**аррайофстрингстипе**</span><span class="sxs-lookup"><span data-stu-id="f41e1-109">**ArrayOfStringsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f41e1-110">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="f41e1-110">Attributes and elements</span></span>

<span data-ttu-id="f41e1-111">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="f41e1-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f41e1-112">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="f41e1-112">Attributes</span></span>

<span data-ttu-id="f41e1-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="f41e1-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f41e1-114">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="f41e1-114">Child elements</span></span>

|<span data-ttu-id="f41e1-115">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="f41e1-115">**Element**</span></span>|<span data-ttu-id="f41e1-116">**Описание**</span><span class="sxs-lookup"><span data-stu-id="f41e1-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f41e1-117">Строка</span><span class="sxs-lookup"><span data-stu-id="f41e1-117">String</span></span>](string.md) <br/> |<span data-ttu-id="f41e1-118">Содержит одну категорию.</span><span class="sxs-lookup"><span data-stu-id="f41e1-118">Contains a single category.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f41e1-119">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="f41e1-119">Parent elements</span></span>

|<span data-ttu-id="f41e1-120">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="f41e1-120">**Element**</span></span>|<span data-ttu-id="f41e1-121">**Описание**</span><span class="sxs-lookup"><span data-stu-id="f41e1-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f41e1-122">Беседы (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="f41e1-122">Conversation (ConversationType)</span></span>](conversation-conversationtype.md) <br/> |<span data-ttu-id="f41e1-123">Представляет одну беседу.</span><span class="sxs-lookup"><span data-stu-id="f41e1-123">Represents a single conversation.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="f41e1-124">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="f41e1-124">Text value</span></span>

<span data-ttu-id="f41e1-125">Нет.</span><span class="sxs-lookup"><span data-stu-id="f41e1-125">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="f41e1-126">Примечания</span><span class="sxs-lookup"><span data-stu-id="f41e1-126">Remarks</span></span>

<span data-ttu-id="f41e1-127">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.Этот элемент появился в Exchange Server 2010 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="f41e1-127">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f41e1-128">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="f41e1-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f41e1-129">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="f41e1-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="f41e1-130">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="f41e1-130">Schema name</span></span>  <br/> |<span data-ttu-id="f41e1-131">Схема Types</span><span class="sxs-lookup"><span data-stu-id="f41e1-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="f41e1-132">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="f41e1-132">Validation file</span></span>  <br/> |<span data-ttu-id="f41e1-133">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="f41e1-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="f41e1-134">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="f41e1-134">Can be empty</span></span>  <br/> |<span data-ttu-id="f41e1-135">False</span><span class="sxs-lookup"><span data-stu-id="f41e1-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f41e1-136">См. также</span><span class="sxs-lookup"><span data-stu-id="f41e1-136">See also</span></span>



[<span data-ttu-id="f41e1-137">FindConversation Operation</span><span class="sxs-lookup"><span data-stu-id="f41e1-137">FindConversation operation</span></span>](findconversation-operation.md)
  
[<span data-ttu-id="f41e1-138">Операция ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="f41e1-138">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)


[<span data-ttu-id="f41e1-139">Conversations in EWS</span><span class="sxs-lookup"><span data-stu-id="f41e1-139">Conversations in EWS</span></span>](http://msdn.microsoft.com/library/91e64629-db6c-4c94-9dcb-d386232e8467%28Office.15%29.aspx)

