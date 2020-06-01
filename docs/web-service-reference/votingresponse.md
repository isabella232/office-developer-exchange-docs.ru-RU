---
title: VotingResponse
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 7dae4db5-28d3-4b81-b071-458c814c36b9
description: Элемент Вотингреспонсе указывает отправленный голос. Этот элемент присутствует только в ответах на сообщения запроса на голосование, а не на отклики на утверждения.
ms.openlocfilehash: ed7caff79d1ff2946800630c167350fe866e29dc
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44466467"
---
# <a name="votingresponse"></a><span data-ttu-id="c8422-104">VotingResponse</span><span class="sxs-lookup"><span data-stu-id="c8422-104">VotingResponse</span></span>

<span data-ttu-id="c8422-105">Элемент **вотингреспонсе** указывает отправленный голос.</span><span class="sxs-lookup"><span data-stu-id="c8422-105">The **VotingResponse** element specifies the submitted vote.</span></span> <span data-ttu-id="c8422-106">Этот элемент присутствует только в ответах на сообщения запроса на голосование, а не на отклики на утверждения.</span><span class="sxs-lookup"><span data-stu-id="c8422-106">This element is only present on responses to voting request messages, not on responses to approvals.</span></span> 
  
```XML
<VotingResponse />
```

 <span data-ttu-id="c8422-107">**строка**</span><span class="sxs-lookup"><span data-stu-id="c8422-107">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c8422-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="c8422-108">Attributes and elements</span></span>

<span data-ttu-id="c8422-109">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="c8422-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c8422-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="c8422-110">Attributes</span></span>

<span data-ttu-id="c8422-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="c8422-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c8422-112">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="c8422-112">Child elements</span></span>

<span data-ttu-id="c8422-113">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="c8422-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="c8422-114">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="c8422-114">Parent elements</span></span>

[<span data-ttu-id="c8422-115">вотингинформатион</span><span class="sxs-lookup"><span data-stu-id="c8422-115">VotingInformation</span></span>](votinginformation.md)
  
## <a name="text-value"></a><span data-ttu-id="c8422-116">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="c8422-116">Text value</span></span>

<span data-ttu-id="c8422-117">Текстовое значение элемента **вотингреспонсе** — это отправленный вами голосование.</span><span class="sxs-lookup"><span data-stu-id="c8422-117">The text value of the **VotingResponse** element is the vote submitted.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="c8422-118">Примечания</span><span class="sxs-lookup"><span data-stu-id="c8422-118">Remarks</span></span>

<span data-ttu-id="c8422-119">Этот элемент появился в Exchange Server 2013 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="c8422-119">This element was introduced in Exchange Server 2013 Service Pack 1 (SP1).</span></span>
  
<span data-ttu-id="c8422-120">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="c8422-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c8422-121">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="c8422-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c8422-122">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="c8422-122">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="c8422-123">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="c8422-123">Schema Name</span></span>  <br/> |<span data-ttu-id="c8422-124">Схема Types</span><span class="sxs-lookup"><span data-stu-id="c8422-124">Types schema</span></span>  <br/> |
|<span data-ttu-id="c8422-125">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="c8422-125">Validation File</span></span>  <br/> |<span data-ttu-id="c8422-126">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="c8422-126">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="c8422-127">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="c8422-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="c8422-128">True</span><span class="sxs-lookup"><span data-stu-id="c8422-128">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c8422-129">См. также</span><span class="sxs-lookup"><span data-stu-id="c8422-129">See also</span></span>



[<span data-ttu-id="c8422-130">вотингинформатион</span><span class="sxs-lookup"><span data-stu-id="c8422-130">VotingInformation</span></span>](votinginformation.md)


- [<span data-ttu-id="c8422-131">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="c8422-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

