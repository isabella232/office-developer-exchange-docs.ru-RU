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
ms.openlocfilehash: d608328f8adae56e140affdb36b38605d6f89486
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530122"
---
# <a name="globalcategories"></a><span data-ttu-id="97db1-103">глобалкатегориес</span><span class="sxs-lookup"><span data-stu-id="97db1-103">GlobalCategories</span></span>

<span data-ttu-id="97db1-104">Элемент **глобалкатегориес** содержит список категорий для всех элементов бесед в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="97db1-104">The **GlobalCategories** element contains the category list for all conversation items in a mailbox.</span></span> 
  
[<span data-ttu-id="97db1-105">финдконверсатионреспонсе</span><span class="sxs-lookup"><span data-stu-id="97db1-105">FindConversationResponse</span></span>](findconversationresponse.md)
  
[<span data-ttu-id="97db1-106">Conversations</span><span class="sxs-lookup"><span data-stu-id="97db1-106">Conversations</span></span>](conversations-ex15websvcsotherref.md)
  
[<span data-ttu-id="97db1-107">Беседы (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="97db1-107">Conversation (ConversationType)</span></span>](conversation-conversationtype.md)
  
[<span data-ttu-id="97db1-108">глобалкатегориес</span><span class="sxs-lookup"><span data-stu-id="97db1-108">GlobalCategories</span></span>](globalcategories.md)
  
```XML
<GlobalCategories>
   <String/>
</GlobalCategories>
```

 <span data-ttu-id="97db1-109">**аррайофстрингстипе**</span><span class="sxs-lookup"><span data-stu-id="97db1-109">**ArrayOfStringsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="97db1-110">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="97db1-110">Attributes and elements</span></span>

<span data-ttu-id="97db1-111">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="97db1-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="97db1-112">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="97db1-112">Attributes</span></span>

<span data-ttu-id="97db1-113">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="97db1-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="97db1-114">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="97db1-114">Child elements</span></span>

|<span data-ttu-id="97db1-115">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="97db1-115">**Element**</span></span>|<span data-ttu-id="97db1-116">**Описание**</span><span class="sxs-lookup"><span data-stu-id="97db1-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="97db1-117">Строка</span><span class="sxs-lookup"><span data-stu-id="97db1-117">String</span></span>](string.md) <br/> |<span data-ttu-id="97db1-118">Содержит одну категорию.</span><span class="sxs-lookup"><span data-stu-id="97db1-118">Contains a single category.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="97db1-119">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="97db1-119">Parent elements</span></span>

|<span data-ttu-id="97db1-120">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="97db1-120">**Element**</span></span>|<span data-ttu-id="97db1-121">**Описание**</span><span class="sxs-lookup"><span data-stu-id="97db1-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="97db1-122">Беседы (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="97db1-122">Conversation (ConversationType)</span></span>](conversation-conversationtype.md) <br/> |<span data-ttu-id="97db1-123">Представляет одну беседу.</span><span class="sxs-lookup"><span data-stu-id="97db1-123">Represents a single conversation.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="97db1-124">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="97db1-124">Text value</span></span>

<span data-ttu-id="97db1-125">Нет.</span><span class="sxs-lookup"><span data-stu-id="97db1-125">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="97db1-126">Примечания</span><span class="sxs-lookup"><span data-stu-id="97db1-126">Remarks</span></span>

<span data-ttu-id="97db1-127">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.Этот элемент появился в Exchange Server 2010 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="97db1-127">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="97db1-128">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="97db1-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="97db1-129">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="97db1-129">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="97db1-130">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="97db1-130">Schema name</span></span>  <br/> |<span data-ttu-id="97db1-131">Схема Types</span><span class="sxs-lookup"><span data-stu-id="97db1-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="97db1-132">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="97db1-132">Validation file</span></span>  <br/> |<span data-ttu-id="97db1-133">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="97db1-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="97db1-134">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="97db1-134">Can be empty</span></span>  <br/> |<span data-ttu-id="97db1-135">False</span><span class="sxs-lookup"><span data-stu-id="97db1-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="97db1-136">См. также</span><span class="sxs-lookup"><span data-stu-id="97db1-136">See also</span></span>



[<span data-ttu-id="97db1-137">FindConversation Operation</span><span class="sxs-lookup"><span data-stu-id="97db1-137">FindConversation operation</span></span>](findconversation-operation.md)
  
[<span data-ttu-id="97db1-138">Операция ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="97db1-138">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)


[<span data-ttu-id="97db1-139">Conversations in EWS</span><span class="sxs-lookup"><span data-stu-id="97db1-139">Conversations in EWS</span></span>](https://msdn.microsoft.com/library/91e64629-db6c-4c94-9dcb-d386232e8467%28Office.15%29.aspx)

