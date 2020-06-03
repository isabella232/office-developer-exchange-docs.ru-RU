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
ms.openlocfilehash: 0949cf64b8583c4b3fa5a1700475f01cc480f69f
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458175"
---
# <a name="isundecidedapprovalrequest"></a><span data-ttu-id="659a7-103">исундеЦидедаппровалрекуест</span><span class="sxs-lookup"><span data-stu-id="659a7-103">IsUndecidedApprovalRequest</span></span>

<span data-ttu-id="659a7-104">Элемент **исундеЦидедаппровалрекуест** указывает, включено ли для сообщения запроса утверждения.</span><span class="sxs-lookup"><span data-stu-id="659a7-104">The **IsUndecidedApprovalRequest** element specifies whether an approval request message has been acted on.</span></span> 
  
```XML
<IsUndecidedApprovalRequest> true | false </IsUndecidedApprovalRequest>
```

 <span data-ttu-id="659a7-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="659a7-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="659a7-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="659a7-106">Attributes and elements</span></span>

<span data-ttu-id="659a7-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="659a7-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="659a7-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="659a7-108">Attributes</span></span>

<span data-ttu-id="659a7-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="659a7-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="659a7-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="659a7-110">Child elements</span></span>

<span data-ttu-id="659a7-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="659a7-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="659a7-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="659a7-112">Parent elements</span></span>

[<span data-ttu-id="659a7-113">аппровалрекуестдата</span><span class="sxs-lookup"><span data-stu-id="659a7-113">ApprovalRequestData</span></span>](approvalrequestdata.md)
  
## <a name="text-value"></a><span data-ttu-id="659a7-114">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="659a7-114">Text value</span></span>

<span data-ttu-id="659a7-115">Текстовое значение элемента **исундеЦидедаппровалрекуест** имеет значение **true** , если сообщение запроса на утверждение не было обработано.</span><span class="sxs-lookup"><span data-stu-id="659a7-115">The text value of the **IsUndecidedApprovalRequest** element is **true** if an approval request message has not been acted on.</span></span> <span data-ttu-id="659a7-116">Значение **false** указывает, что запрос на утверждение принят.</span><span class="sxs-lookup"><span data-stu-id="659a7-116">A value of **false** indicates that the approval request has been decided.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="659a7-117">Примечания</span><span class="sxs-lookup"><span data-stu-id="659a7-117">Remarks</span></span>

<span data-ttu-id="659a7-118">Этот элемент появился в Exchange Server 2013 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="659a7-118">This element was introduced in Exchange Server 2013 Service Pack 1 (SP1).</span></span>
  
<span data-ttu-id="659a7-119">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="659a7-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="659a7-120">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="659a7-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="659a7-121">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="659a7-121">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="659a7-122">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="659a7-122">Schema Name</span></span>  <br/> |<span data-ttu-id="659a7-123">Схема Types</span><span class="sxs-lookup"><span data-stu-id="659a7-123">Types schema</span></span>  <br/> |
|<span data-ttu-id="659a7-124">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="659a7-124">Validation File</span></span>  <br/> |<span data-ttu-id="659a7-125">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="659a7-125">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="659a7-126">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="659a7-126">Can be Empty</span></span>  <br/> |<span data-ttu-id="659a7-127">True</span><span class="sxs-lookup"><span data-stu-id="659a7-127">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="659a7-128">См. также</span><span class="sxs-lookup"><span data-stu-id="659a7-128">See also</span></span>



[<span data-ttu-id="659a7-129">аппровалрекуестдата</span><span class="sxs-lookup"><span data-stu-id="659a7-129">ApprovalRequestData</span></span>](approvalrequestdata.md)


- [<span data-ttu-id="659a7-130">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="659a7-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

