---
title: VotingInformation
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 351c8dfe-cf8c-45ba-a07d-d764f8189773
description: Элемент VotingInformation указывает голосования сведения на голосования сообщение и утверждения запроса сообщение whereApproveandRejectare параметров голосования.
ms.openlocfilehash: f11c25bb1f3a3c4781cfa6c51e11ff87af40c7f0
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19840478"
---
# <a name="votinginformation"></a><span data-ttu-id="8e40c-103">VotingInformation</span><span class="sxs-lookup"><span data-stu-id="8e40c-103">VotingInformation</span></span>

<span data-ttu-id="8e40c-104">Элемент **VotingInformation** указывает голосования сведения на голосования сообщения и сообщения запроса на утверждение, где «Утверждение» и «Отклонить» имеют параметров голосования.</span><span class="sxs-lookup"><span data-stu-id="8e40c-104">The **VotingInformation** element specifies voting information on a voting message and approval request message where "Approve" and "Reject" are the voting options.</span></span> 
  
```XML
<VotingInformation
   <UserOptions/>
   <VotingResponse/>
</VotingInformation>
```

 <span data-ttu-id="8e40c-105">**VotingInformationType**</span><span class="sxs-lookup"><span data-stu-id="8e40c-105">**VotingInformationType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="8e40c-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="8e40c-106">Attributes and elements</span></span>

<span data-ttu-id="8e40c-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="8e40c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8e40c-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="8e40c-108">Attributes</span></span>

<span data-ttu-id="8e40c-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="8e40c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8e40c-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="8e40c-110">Child elements</span></span>

<span data-ttu-id="8e40c-111">[UserOptions](useroptions.md) | [VotingResponse](votingresponse.md)</span><span class="sxs-lookup"><span data-stu-id="8e40c-111">[UserOptions](useroptions.md) | [VotingResponse](votingresponse.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="8e40c-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="8e40c-112">Parent elements</span></span>

[<span data-ttu-id="8e40c-113">Message</span><span class="sxs-lookup"><span data-stu-id="8e40c-113">Message</span></span>](message-ex15websvcsotherref.md)
  
## <a name="remarks"></a><span data-ttu-id="8e40c-114">Замечания</span><span class="sxs-lookup"><span data-stu-id="8e40c-114">Remarks</span></span>

<span data-ttu-id="8e40c-115">Этот элемент появился в Exchange Server 2013 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="8e40c-115">This element was introduced in Exchange Server 2013 Service Pack 1 (SP1).</span></span>
  
<span data-ttu-id="8e40c-116">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="8e40c-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="8e40c-117">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="8e40c-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8e40c-118">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="8e40c-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="8e40c-119">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="8e40c-119">Schema Name</span></span>  <br/> |<span data-ttu-id="8e40c-120">Схема Types</span><span class="sxs-lookup"><span data-stu-id="8e40c-120">Types schema</span></span>  <br/> |
|<span data-ttu-id="8e40c-121">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="8e40c-121">Validation File</span></span>  <br/> |<span data-ttu-id="8e40c-122">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="8e40c-122">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="8e40c-123">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="8e40c-123">Can be Empty</span></span>  <br/> |<span data-ttu-id="8e40c-124">True</span><span class="sxs-lookup"><span data-stu-id="8e40c-124">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="8e40c-125">См. также</span><span class="sxs-lookup"><span data-stu-id="8e40c-125">See also</span></span>



[<span data-ttu-id="8e40c-126">Message</span><span class="sxs-lookup"><span data-stu-id="8e40c-126">Message</span></span>](message-ex15websvcsotherref.md)


- [<span data-ttu-id="8e40c-127">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="8e40c-127">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

