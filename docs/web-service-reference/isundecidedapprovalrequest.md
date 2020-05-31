---
title: исундеЦидедаппровалрекуест
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 90841617-3b83-4124-8125-0293c9470f4a
description: Элемент ИсундеЦидедаппровалрекуест указывает, включено ли для сообщения запроса утверждения.
ms.openlocfilehash: 82b4624df5b2fe7ca212fdf76248e1ccfa3a081f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834127"
---
# <a name="isundecidedapprovalrequest"></a><span data-ttu-id="a5fe8-103">исундеЦидедаппровалрекуест</span><span class="sxs-lookup"><span data-stu-id="a5fe8-103">IsUndecidedApprovalRequest</span></span>

<span data-ttu-id="a5fe8-104">Элемент **исундеЦидедаппровалрекуест** указывает, включено ли для сообщения запроса утверждения.</span><span class="sxs-lookup"><span data-stu-id="a5fe8-104">The **IsUndecidedApprovalRequest** element specifies whether an approval request message has been acted on.</span></span> 
  
```XML
<IsUndecidedApprovalRequest> true | false </IsUndecidedApprovalRequest>
```

 <span data-ttu-id="a5fe8-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="a5fe8-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a5fe8-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="a5fe8-106">Attributes and elements</span></span>

<span data-ttu-id="a5fe8-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="a5fe8-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a5fe8-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="a5fe8-108">Attributes</span></span>

<span data-ttu-id="a5fe8-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="a5fe8-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a5fe8-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="a5fe8-110">Child elements</span></span>

<span data-ttu-id="a5fe8-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="a5fe8-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="a5fe8-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="a5fe8-112">Parent elements</span></span>

[<span data-ttu-id="a5fe8-113">аппровалрекуестдата</span><span class="sxs-lookup"><span data-stu-id="a5fe8-113">ApprovalRequestData</span></span>](approvalrequestdata.md)
  
## <a name="text-value"></a><span data-ttu-id="a5fe8-114">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="a5fe8-114">Text value</span></span>

<span data-ttu-id="a5fe8-115">Текстовое значение элемента **исундеЦидедаппровалрекуест** имеет значение **true** , если сообщение запроса на утверждение не было обработано.</span><span class="sxs-lookup"><span data-stu-id="a5fe8-115">The text value of the **IsUndecidedApprovalRequest** element is **true** if an approval request message has not been acted on.</span></span> <span data-ttu-id="a5fe8-116">Значение **false** указывает, что запрос на утверждение принят.</span><span class="sxs-lookup"><span data-stu-id="a5fe8-116">A value of **false** indicates that the approval request has been decided.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="a5fe8-117">Примечания</span><span class="sxs-lookup"><span data-stu-id="a5fe8-117">Remarks</span></span>

<span data-ttu-id="a5fe8-118">Этот элемент появился в Exchange Server 2013 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="a5fe8-118">This element was introduced in Exchange Server 2013 Service Pack 1 (SP1).</span></span>
  
<span data-ttu-id="a5fe8-119">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="a5fe8-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a5fe8-120">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="a5fe8-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a5fe8-121">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="a5fe8-121">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="a5fe8-122">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="a5fe8-122">Schema Name</span></span>  <br/> |<span data-ttu-id="a5fe8-123">Схема Types</span><span class="sxs-lookup"><span data-stu-id="a5fe8-123">Types schema</span></span>  <br/> |
|<span data-ttu-id="a5fe8-124">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="a5fe8-124">Validation File</span></span>  <br/> |<span data-ttu-id="a5fe8-125">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="a5fe8-125">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="a5fe8-126">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="a5fe8-126">Can be Empty</span></span>  <br/> |<span data-ttu-id="a5fe8-127">True</span><span class="sxs-lookup"><span data-stu-id="a5fe8-127">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a5fe8-128">См. также</span><span class="sxs-lookup"><span data-stu-id="a5fe8-128">See also</span></span>



[<span data-ttu-id="a5fe8-129">аппровалрекуестдата</span><span class="sxs-lookup"><span data-stu-id="a5fe8-129">ApprovalRequestData</span></span>](approvalrequestdata.md)


- [<span data-ttu-id="a5fe8-130">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="a5fe8-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

