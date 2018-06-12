---
title: ApprovalRequestData
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 6c971cf7-5c3a-4e5e-9a7d-048f4ac0aadb
description: Элемент ApprovalRequestData указывает состояние утверждения сообщение запроса утверждения.
ms.openlocfilehash: ed1c1e3db4edd2cf4de032dc61abd73e863d4f1d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761483"
---
# <a name="approvalrequestdata"></a><span data-ttu-id="af638-103">ApprovalRequestData</span><span class="sxs-lookup"><span data-stu-id="af638-103">ApprovalRequestData</span></span>

<span data-ttu-id="af638-104">Элемент **ApprovalRequestData** указывает состояние утверждения сообщение запроса утверждения.</span><span class="sxs-lookup"><span data-stu-id="af638-104">The **ApprovalRequestData** element specifies the approval state of an approval request message.</span></span> 
  
```xml
<ApprovalRequestData>
   <IsUndecidedApprovalRequest/>
   <ApprovalDecision/>
   <ApprovalDecisionMaker/>
   <ApprovalDecisionTime/>
</ApprovalRequestData>
```

 <span data-ttu-id="af638-105">**ApprovalRequestDataType**</span><span class="sxs-lookup"><span data-stu-id="af638-105">**ApprovalRequestDataType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="af638-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="af638-106">Attributes and elements</span></span>

<span data-ttu-id="af638-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="af638-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="af638-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="af638-108">Attributes</span></span>

<span data-ttu-id="af638-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="af638-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="af638-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="af638-110">Child elements</span></span>

<span data-ttu-id="af638-111">[IsUndecidedApprovalRequest](isundecidedapprovalrequest.md) | [ApprovalDecision](approvaldecision.md) | [ApprovalDecisionMaker](approvaldecisionmaker.md) | [ApprovalDecisionTime](approvaldecisiontime.md)</span><span class="sxs-lookup"><span data-stu-id="af638-111">[IsUndecidedApprovalRequest](isundecidedapprovalrequest.md) | [ApprovalDecision](approvaldecision.md) | [ApprovalDecisionMaker](approvaldecisionmaker.md) | [ApprovalDecisionTime](approvaldecisiontime.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="af638-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="af638-112">Parent elements</span></span>

[<span data-ttu-id="af638-113">Message</span><span class="sxs-lookup"><span data-stu-id="af638-113">Message</span></span>](message-ex15websvcsotherref.md)
  
## <a name="remarks"></a><span data-ttu-id="af638-114">Замечания</span><span class="sxs-lookup"><span data-stu-id="af638-114">Remarks</span></span>

<span data-ttu-id="af638-115">Этот элемент появился в Exchange Server 2013 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="af638-115">This element was introduced in Exchange Server 2013 Service Pack 1 (SP1).</span></span>
  
<span data-ttu-id="af638-116">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="af638-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="af638-117">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="af638-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="af638-118">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="af638-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="af638-119">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="af638-119">Schema Name</span></span>  <br/> |<span data-ttu-id="af638-120">Схема Types</span><span class="sxs-lookup"><span data-stu-id="af638-120">Types schema</span></span>  <br/> |
|<span data-ttu-id="af638-121">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="af638-121">Validation File</span></span>  <br/> |<span data-ttu-id="af638-122">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="af638-122">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="af638-123">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="af638-123">Can be Empty</span></span>  <br/> |<span data-ttu-id="af638-124">True</span><span class="sxs-lookup"><span data-stu-id="af638-124">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="af638-125">См. также</span><span class="sxs-lookup"><span data-stu-id="af638-125">See also</span></span>

- [<span data-ttu-id="af638-126">Message</span><span class="sxs-lookup"><span data-stu-id="af638-126">Message</span></span>](message-ex15websvcsotherref.md)
- [<span data-ttu-id="af638-127">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="af638-127">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

