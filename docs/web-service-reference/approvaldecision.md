---
title: ApprovalDecision
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 5e7c5687-cb9e-4f0b-ac8f-b82591914a39
description: Элемент ApprovalDecision указывает принятия решений, созданных в сообщение запроса утверждения.
ms.openlocfilehash: 4ca73813440200e5d2fb9f920d81459d8cd5e4ec
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761479"
---
# <a name="approvaldecision"></a><span data-ttu-id="7581b-103">ApprovalDecision</span><span class="sxs-lookup"><span data-stu-id="7581b-103">ApprovalDecision</span></span>

<span data-ttu-id="7581b-104">Элемент **ApprovalDecision** указывает принятия решений, созданных в сообщение запроса утверждения.</span><span class="sxs-lookup"><span data-stu-id="7581b-104">The **ApprovalDecision** element specifies the decision made on an approval request message.</span></span> 
  
```XML
<ApprovalDecision> 1 | 2 </ApprovalDecision>
```

 <span data-ttu-id="7581b-105">**int**</span><span class="sxs-lookup"><span data-stu-id="7581b-105">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7581b-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="7581b-106">Attributes and elements</span></span>

<span data-ttu-id="7581b-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="7581b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7581b-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="7581b-108">Attributes</span></span>

<span data-ttu-id="7581b-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="7581b-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7581b-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="7581b-110">Child elements</span></span>

<span data-ttu-id="7581b-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="7581b-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="7581b-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="7581b-112">Parent elements</span></span>

[<span data-ttu-id="7581b-113">ApprovalRequestData</span><span class="sxs-lookup"><span data-stu-id="7581b-113">ApprovalRequestData</span></span>](approvalrequestdata.md)
  
## <a name="text-value"></a><span data-ttu-id="7581b-114">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="7581b-114">Text value</span></span>

<span data-ttu-id="7581b-115">Текстовое значение элемента **ApprovalDecision** — 1, если Утверждено и 2, если отклонено.</span><span class="sxs-lookup"><span data-stu-id="7581b-115">The text value of the **ApprovalDecision** element is 1 if approved and 2 if rejected.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="7581b-116">Замечания</span><span class="sxs-lookup"><span data-stu-id="7581b-116">Remarks</span></span>

<span data-ttu-id="7581b-117">Этот элемент появился в Exchange Server 2013 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="7581b-117">This element was introduced in Exchange Server 2013 Service Pack 1 (SP1).</span></span>
  
<span data-ttu-id="7581b-118">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="7581b-118">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7581b-119">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="7581b-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7581b-120">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="7581b-120">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="7581b-121">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="7581b-121">Schema Name</span></span>  <br/> |<span data-ttu-id="7581b-122">Схема Types</span><span class="sxs-lookup"><span data-stu-id="7581b-122">Types schema</span></span>  <br/> |
|<span data-ttu-id="7581b-123">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="7581b-123">Validation File</span></span>  <br/> |<span data-ttu-id="7581b-124">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="7581b-124">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="7581b-125">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="7581b-125">Can be Empty</span></span>  <br/> |<span data-ttu-id="7581b-126">True</span><span class="sxs-lookup"><span data-stu-id="7581b-126">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7581b-127">См. также</span><span class="sxs-lookup"><span data-stu-id="7581b-127">See also</span></span>

- [<span data-ttu-id="7581b-128">ApprovalRequestData</span><span class="sxs-lookup"><span data-stu-id="7581b-128">ApprovalRequestData</span></span>](approvalrequestdata.md)
- [<span data-ttu-id="7581b-129">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="7581b-129">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
