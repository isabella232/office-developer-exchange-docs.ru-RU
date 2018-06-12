---
title: VotingResponse
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 7dae4db5-28d3-4b81-b071-458c814c36b9
description: Элемент VotingResponse указывает отправляемого голос. Этот элемент должен быть установлен, ответов на сообщения запроса на голосования, а не ответов на утверждение.
ms.openlocfilehash: 865b24a4f7ec1cc7b53d4928b04f071cddf5fbfc
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19840484"
---
# <a name="votingresponse"></a><span data-ttu-id="34b8d-104">VotingResponse</span><span class="sxs-lookup"><span data-stu-id="34b8d-104">VotingResponse</span></span>

<span data-ttu-id="34b8d-105">Элемент **VotingResponse** указывает отправляемого голос.</span><span class="sxs-lookup"><span data-stu-id="34b8d-105">The **VotingResponse** element specifies the submitted vote.</span></span> <span data-ttu-id="34b8d-106">Этот элемент должен быть установлен, ответов на сообщения запроса на голосования, а не ответов на утверждение.</span><span class="sxs-lookup"><span data-stu-id="34b8d-106">This element is only present on responses to voting request messages, not on responses to approvals.</span></span> 
  
```XML
<VotingResponse />
```

 <span data-ttu-id="34b8d-107">**string**</span><span class="sxs-lookup"><span data-stu-id="34b8d-107">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="34b8d-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="34b8d-108">Attributes and elements</span></span>

<span data-ttu-id="34b8d-109">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="34b8d-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="34b8d-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="34b8d-110">Attributes</span></span>

<span data-ttu-id="34b8d-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="34b8d-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="34b8d-112">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="34b8d-112">Child elements</span></span>

<span data-ttu-id="34b8d-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="34b8d-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="34b8d-114">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="34b8d-114">Parent elements</span></span>

[<span data-ttu-id="34b8d-115">VotingInformation</span><span class="sxs-lookup"><span data-stu-id="34b8d-115">VotingInformation</span></span>](votinginformation.md)
  
## <a name="text-value"></a><span data-ttu-id="34b8d-116">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="34b8d-116">Text value</span></span>

<span data-ttu-id="34b8d-117">Текстовое значение элемента **VotingResponse** является голосования отправке.</span><span class="sxs-lookup"><span data-stu-id="34b8d-117">The text value of the **VotingResponse** element is the vote submitted.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="34b8d-118">Замечания</span><span class="sxs-lookup"><span data-stu-id="34b8d-118">Remarks</span></span>

<span data-ttu-id="34b8d-119">Этот элемент появился в Exchange Server 2013 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="34b8d-119">This element was introduced in Exchange Server 2013 Service Pack 1 (SP1).</span></span>
  
<span data-ttu-id="34b8d-120">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="34b8d-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="34b8d-121">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="34b8d-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="34b8d-122">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="34b8d-122">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="34b8d-123">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="34b8d-123">Schema Name</span></span>  <br/> |<span data-ttu-id="34b8d-124">Схема Types</span><span class="sxs-lookup"><span data-stu-id="34b8d-124">Types schema</span></span>  <br/> |
|<span data-ttu-id="34b8d-125">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="34b8d-125">Validation File</span></span>  <br/> |<span data-ttu-id="34b8d-126">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="34b8d-126">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="34b8d-127">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="34b8d-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="34b8d-128">True</span><span class="sxs-lookup"><span data-stu-id="34b8d-128">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="34b8d-129">См. также</span><span class="sxs-lookup"><span data-stu-id="34b8d-129">See also</span></span>



[<span data-ttu-id="34b8d-130">VotingInformation</span><span class="sxs-lookup"><span data-stu-id="34b8d-130">VotingInformation</span></span>](votinginformation.md)


- [<span data-ttu-id="34b8d-131">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="34b8d-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

