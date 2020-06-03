---
title: енаблеалвайсделете
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
description: Элемент Енаблеалвайсделете указывает флаг, который позволяет удалять все новые элементы в беседе.
ms.openlocfilehash: 14784d3a6ba52c76b64b81e15c0522d66d125cbf
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44526209"
---
# <a name="enablealwaysdelete"></a><span data-ttu-id="fb396-103">енаблеалвайсделете</span><span class="sxs-lookup"><span data-stu-id="fb396-103">EnableAlwaysDelete</span></span>

<span data-ttu-id="fb396-104">Элемент **енаблеалвайсделете** указывает флаг, который позволяет удалять все новые элементы в беседе.</span><span class="sxs-lookup"><span data-stu-id="fb396-104">The **EnableAlwaysDelete** element specifies a flag that enables deletion for all new items in a conversation.</span></span> 
  
[<span data-ttu-id="fb396-105">ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="fb396-105">ApplyConversationAction</span></span>](applyconversationaction.md)
  
[<span data-ttu-id="fb396-106">конверсатионактионс</span><span class="sxs-lookup"><span data-stu-id="fb396-106">ConversationActions</span></span>](conversationactions.md)
  
[<span data-ttu-id="fb396-107">конверсатионактион</span><span class="sxs-lookup"><span data-stu-id="fb396-107">ConversationAction</span></span>](conversationaction.md)
  
[<span data-ttu-id="fb396-108">енаблеалвайсделете</span><span class="sxs-lookup"><span data-stu-id="fb396-108">EnableAlwaysDelete</span></span>](enablealwaysdelete.md)
  
```XML
<EnableAlwaysDelete/>
```

 <span data-ttu-id="fb396-109">**xs: Boolean**</span><span class="sxs-lookup"><span data-stu-id="fb396-109">**xs:boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="fb396-110">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="fb396-110">Attributes and elements</span></span>

<span data-ttu-id="fb396-111">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="fb396-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="fb396-112">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="fb396-112">Attributes</span></span>

<span data-ttu-id="fb396-113">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="fb396-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="fb396-114">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="fb396-114">Child elements</span></span>

<span data-ttu-id="fb396-115">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="fb396-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="fb396-116">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="fb396-116">Parent elements</span></span>

|<span data-ttu-id="fb396-117">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="fb396-117">**Element**</span></span>|<span data-ttu-id="fb396-118">**Описание**</span><span class="sxs-lookup"><span data-stu-id="fb396-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fb396-119">конверсатионактион</span><span class="sxs-lookup"><span data-stu-id="fb396-119">ConversationAction</span></span>](conversationaction.md) <br/> |<span data-ttu-id="fb396-120">Содержит одно действие, которое будет применено к одной беседе.</span><span class="sxs-lookup"><span data-stu-id="fb396-120">Contains a single action to be applied to a single conversation.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="fb396-121">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="fb396-121">Text value</span></span>

<span data-ttu-id="fb396-122">Текстовое значение элемента **енаблеалвайсделете** равно **true** , чтобы включить удаление всех элементов в беседе; в противном случае — **false**.</span><span class="sxs-lookup"><span data-stu-id="fb396-122">The text value of the **EnableAlwaysDelete** element is **true** to enable the deletion of all items in conversation; otherwise, **false**.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="fb396-123">Примечания</span><span class="sxs-lookup"><span data-stu-id="fb396-123">Remarks</span></span>

<span data-ttu-id="fb396-124">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.Этот элемент появился в Exchange Server 2010 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="fb396-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="fb396-125">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="fb396-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="fb396-126">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="fb396-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="fb396-127">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="fb396-127">Schema Name</span></span>  <br/> |<span data-ttu-id="fb396-128">Схема Types</span><span class="sxs-lookup"><span data-stu-id="fb396-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="fb396-129">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="fb396-129">Validation File</span></span>  <br/> |<span data-ttu-id="fb396-130">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="fb396-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="fb396-131">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="fb396-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="fb396-132">False</span><span class="sxs-lookup"><span data-stu-id="fb396-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="fb396-133">См. также</span><span class="sxs-lookup"><span data-stu-id="fb396-133">See also</span></span>



[<span data-ttu-id="fb396-134">Операция ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="fb396-134">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)

