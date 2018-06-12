---
title: IsUndecidedApprovalRequest
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 90841617-3b83-4124-8125-0293c9470f4a
description: Элемент IsUndecidedApprovalRequest указывает, работает ли на сообщение запроса утверждения.
ms.openlocfilehash: 82b4624df5b2fe7ca212fdf76248e1ccfa3a081f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19834127"
---
# <a name="isundecidedapprovalrequest"></a><span data-ttu-id="1df22-103">IsUndecidedApprovalRequest</span><span class="sxs-lookup"><span data-stu-id="1df22-103">IsUndecidedApprovalRequest</span></span>

<span data-ttu-id="1df22-104">Элемент **IsUndecidedApprovalRequest** указывает, работает ли на сообщение запроса утверждения.</span><span class="sxs-lookup"><span data-stu-id="1df22-104">The **IsUndecidedApprovalRequest** element specifies whether an approval request message has been acted on.</span></span> 
  
```XML
<IsUndecidedApprovalRequest> true | false </IsUndecidedApprovalRequest>
```

 <span data-ttu-id="1df22-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="1df22-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1df22-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="1df22-106">Attributes and elements</span></span>

<span data-ttu-id="1df22-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="1df22-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1df22-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="1df22-108">Attributes</span></span>

<span data-ttu-id="1df22-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="1df22-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1df22-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="1df22-110">Child elements</span></span>

<span data-ttu-id="1df22-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="1df22-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="1df22-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="1df22-112">Parent elements</span></span>

[<span data-ttu-id="1df22-113">ApprovalRequestData</span><span class="sxs-lookup"><span data-stu-id="1df22-113">ApprovalRequestData</span></span>](approvalrequestdata.md)
  
## <a name="text-value"></a><span data-ttu-id="1df22-114">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="1df22-114">Text value</span></span>

<span data-ttu-id="1df22-115">Текстовое значение элемента **IsUndecidedApprovalRequest** равно **true** , если сообщение запроса утверждения не были выполнил.</span><span class="sxs-lookup"><span data-stu-id="1df22-115">The text value of the **IsUndecidedApprovalRequest** element is **true** if an approval request message has not been acted on.</span></span> <span data-ttu-id="1df22-116">Значение **false** указывает, что принятый запроса утверждения.</span><span class="sxs-lookup"><span data-stu-id="1df22-116">A value of **false** indicates that the approval request has been decided.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="1df22-117">Замечания</span><span class="sxs-lookup"><span data-stu-id="1df22-117">Remarks</span></span>

<span data-ttu-id="1df22-118">Этот элемент появился в Exchange Server 2013 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="1df22-118">This element was introduced in Exchange Server 2013 Service Pack 1 (SP1).</span></span>
  
<span data-ttu-id="1df22-119">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="1df22-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1df22-120">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="1df22-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1df22-121">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="1df22-121">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="1df22-122">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="1df22-122">Schema Name</span></span>  <br/> |<span data-ttu-id="1df22-123">Схема Types</span><span class="sxs-lookup"><span data-stu-id="1df22-123">Types schema</span></span>  <br/> |
|<span data-ttu-id="1df22-124">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="1df22-124">Validation File</span></span>  <br/> |<span data-ttu-id="1df22-125">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="1df22-125">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="1df22-126">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="1df22-126">Can be Empty</span></span>  <br/> |<span data-ttu-id="1df22-127">True</span><span class="sxs-lookup"><span data-stu-id="1df22-127">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="1df22-128">См. также</span><span class="sxs-lookup"><span data-stu-id="1df22-128">See also</span></span>



[<span data-ttu-id="1df22-129">ApprovalRequestData</span><span class="sxs-lookup"><span data-stu-id="1df22-129">ApprovalRequestData</span></span>](approvalrequestdata.md)


- [<span data-ttu-id="1df22-130">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="1df22-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

