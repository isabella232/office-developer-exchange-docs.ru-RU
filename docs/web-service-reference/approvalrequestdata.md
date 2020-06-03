---
title: аппровалрекуестдата
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 6c971cf7-5c3a-4e5e-9a7d-048f4ac0aadb
description: Элемент Аппровалрекуестдата указывает состояние утверждения сообщения с запросом на утверждение.
ms.openlocfilehash: decbd4d646a56b9810387adcdb6a9049da89bc38
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462306"
---
# <a name="approvalrequestdata"></a><span data-ttu-id="96b5c-103">аппровалрекуестдата</span><span class="sxs-lookup"><span data-stu-id="96b5c-103">ApprovalRequestData</span></span>

<span data-ttu-id="96b5c-104">Элемент **аппровалрекуестдата** указывает состояние утверждения сообщения с запросом на утверждение.</span><span class="sxs-lookup"><span data-stu-id="96b5c-104">The **ApprovalRequestData** element specifies the approval state of an approval request message.</span></span> 
  
```xml
<ApprovalRequestData>
   <IsUndecidedApprovalRequest/>
   <ApprovalDecision/>
   <ApprovalDecisionMaker/>
   <ApprovalDecisionTime/>
</ApprovalRequestData>
```

 <span data-ttu-id="96b5c-105">**аппровалрекуестдататипе**</span><span class="sxs-lookup"><span data-stu-id="96b5c-105">**ApprovalRequestDataType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="96b5c-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="96b5c-106">Attributes and elements</span></span>

<span data-ttu-id="96b5c-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="96b5c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="96b5c-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="96b5c-108">Attributes</span></span>

<span data-ttu-id="96b5c-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="96b5c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="96b5c-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="96b5c-110">Child elements</span></span>

<span data-ttu-id="96b5c-111">[ИсундеЦидедаппровалрекуест](isundecidedapprovalrequest.md)  |  [АппровалдеЦисион](approvaldecision.md)  |  [АппровалдеЦисионмакер](approvaldecisionmaker.md)  |  [АппровалдеЦисионтиме](approvaldecisiontime.md)</span><span class="sxs-lookup"><span data-stu-id="96b5c-111">[IsUndecidedApprovalRequest](isundecidedapprovalrequest.md) | [ApprovalDecision](approvaldecision.md) | [ApprovalDecisionMaker](approvaldecisionmaker.md) | [ApprovalDecisionTime](approvaldecisiontime.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="96b5c-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="96b5c-112">Parent elements</span></span>

[<span data-ttu-id="96b5c-113">Сообщение</span><span class="sxs-lookup"><span data-stu-id="96b5c-113">Message</span></span>](message-ex15websvcsotherref.md)
  
## <a name="remarks"></a><span data-ttu-id="96b5c-114">Примечания</span><span class="sxs-lookup"><span data-stu-id="96b5c-114">Remarks</span></span>

<span data-ttu-id="96b5c-115">Этот элемент появился в Exchange Server 2013 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="96b5c-115">This element was introduced in Exchange Server 2013 Service Pack 1 (SP1).</span></span>
  
<span data-ttu-id="96b5c-116">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="96b5c-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="96b5c-117">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="96b5c-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="96b5c-118">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="96b5c-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="96b5c-119">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="96b5c-119">Schema Name</span></span>  <br/> |<span data-ttu-id="96b5c-120">Схема Types</span><span class="sxs-lookup"><span data-stu-id="96b5c-120">Types schema</span></span>  <br/> |
|<span data-ttu-id="96b5c-121">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="96b5c-121">Validation File</span></span>  <br/> |<span data-ttu-id="96b5c-122">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="96b5c-122">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="96b5c-123">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="96b5c-123">Can be Empty</span></span>  <br/> |<span data-ttu-id="96b5c-124">True</span><span class="sxs-lookup"><span data-stu-id="96b5c-124">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="96b5c-125">См. также</span><span class="sxs-lookup"><span data-stu-id="96b5c-125">See also</span></span>

- [<span data-ttu-id="96b5c-126">Сообщение</span><span class="sxs-lookup"><span data-stu-id="96b5c-126">Message</span></span>](message-ex15websvcsotherref.md)
- [<span data-ttu-id="96b5c-127">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="96b5c-127">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

