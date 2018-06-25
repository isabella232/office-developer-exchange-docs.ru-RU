---
title: EnableAlwaysDelete
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- EnableAlwaysDelete
api_type:
- schema
ms.assetid: 7753aec5-3f93-4aeb-a28e-8b9b42ca7f9b
description: Элемент EnableAlwaysDelete указывает флаг, который позволяет удалить для всех новых элементов в беседе.
ms.openlocfilehash: f86765c641604afbf13ac962f4b34fbd8de56200
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762336"
---
# <a name="enablealwaysdelete"></a><span data-ttu-id="591c9-103">EnableAlwaysDelete</span><span class="sxs-lookup"><span data-stu-id="591c9-103">EnableAlwaysDelete</span></span>

<span data-ttu-id="591c9-104">Элемент **EnableAlwaysDelete** указывает флаг, который позволяет удалить для всех новых элементов в беседе.</span><span class="sxs-lookup"><span data-stu-id="591c9-104">The **EnableAlwaysDelete** element specifies a flag that enables deletion for all new items in a conversation.</span></span> 
  
[<span data-ttu-id="591c9-105">ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="591c9-105">ApplyConversationAction</span></span>](applyconversationaction.md)
  
[<span data-ttu-id="591c9-106">ConversationActions</span><span class="sxs-lookup"><span data-stu-id="591c9-106">ConversationActions</span></span>](conversationactions.md)
  
[<span data-ttu-id="591c9-107">ConversationAction</span><span class="sxs-lookup"><span data-stu-id="591c9-107">ConversationAction</span></span>](conversationaction.md)
  
[<span data-ttu-id="591c9-108">EnableAlwaysDelete</span><span class="sxs-lookup"><span data-stu-id="591c9-108">EnableAlwaysDelete</span></span>](enablealwaysdelete.md)
  
```XML
<EnableAlwaysDelete/>
```

 <span data-ttu-id="591c9-109">**xs: Boolean**</span><span class="sxs-lookup"><span data-stu-id="591c9-109">**xs:boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="591c9-110">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="591c9-110">Attributes and elements</span></span>

<span data-ttu-id="591c9-111">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="591c9-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="591c9-112">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="591c9-112">Attributes</span></span>

<span data-ttu-id="591c9-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="591c9-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="591c9-114">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="591c9-114">Child elements</span></span>

<span data-ttu-id="591c9-115">Нет.</span><span class="sxs-lookup"><span data-stu-id="591c9-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="591c9-116">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="591c9-116">Parent elements</span></span>

|<span data-ttu-id="591c9-117">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="591c9-117">**Element**</span></span>|<span data-ttu-id="591c9-118">**Описание**</span><span class="sxs-lookup"><span data-stu-id="591c9-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="591c9-119">ConversationAction</span><span class="sxs-lookup"><span data-stu-id="591c9-119">ConversationAction</span></span>](conversationaction.md) <br/> |<span data-ttu-id="591c9-120">Содержит одно действие должен применяться к разговора.</span><span class="sxs-lookup"><span data-stu-id="591c9-120">Contains a single action to be applied to a single conversation.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="591c9-121">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="591c9-121">Text value</span></span>

<span data-ttu-id="591c9-122">Текстовое значение элемента **EnableAlwaysDelete** имеет **значение true** для включения удаления всех элементов в беседе; в противном случае — **false**.</span><span class="sxs-lookup"><span data-stu-id="591c9-122">The text value of the **EnableAlwaysDelete** element is **true** to enable the deletion of all items in conversation; otherwise, **false**.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="591c9-123">Замечания</span><span class="sxs-lookup"><span data-stu-id="591c9-123">Remarks</span></span>

<span data-ttu-id="591c9-124">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.Этот элемент появился в Exchange Server 2010 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="591c9-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="591c9-125">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="591c9-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="591c9-126">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="591c9-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="591c9-127">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="591c9-127">Schema Name</span></span>  <br/> |<span data-ttu-id="591c9-128">Схема Types</span><span class="sxs-lookup"><span data-stu-id="591c9-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="591c9-129">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="591c9-129">Validation File</span></span>  <br/> |<span data-ttu-id="591c9-130">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="591c9-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="591c9-131">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="591c9-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="591c9-132">False</span><span class="sxs-lookup"><span data-stu-id="591c9-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="591c9-133">См. также</span><span class="sxs-lookup"><span data-stu-id="591c9-133">See also</span></span>



[<span data-ttu-id="591c9-134">Операция ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="591c9-134">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)

