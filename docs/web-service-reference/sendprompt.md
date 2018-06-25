---
title: SendPrompt
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 22cb5a30-75d9-49a8-9d98-255f2e8a722d
description: Элемент SendPrompt указывает тип действий, разрешенных для голосования варианта.
ms.openlocfilehash: f3220d957482ea04c46b014cdf1c67025d5ec21a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835346"
---
# <a name="sendprompt"></a><span data-ttu-id="5e56b-103">SendPrompt</span><span class="sxs-lookup"><span data-stu-id="5e56b-103">SendPrompt</span></span>

<span data-ttu-id="5e56b-104">Элемент **SendPrompt** указывает тип действий, разрешенных для голосования варианта.</span><span class="sxs-lookup"><span data-stu-id="5e56b-104">The **SendPrompt** element specifies the type of action allowed for a voting option.</span></span> 
  
```XML
<SendPrompt> None | Send | VotingOption </SendPrompt>
```

 <span data-ttu-id="5e56b-105">**SendPromptType**</span><span class="sxs-lookup"><span data-stu-id="5e56b-105">**SendPromptType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5e56b-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="5e56b-106">Attributes and elements</span></span>

<span data-ttu-id="5e56b-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="5e56b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5e56b-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="5e56b-108">Attributes</span></span>

<span data-ttu-id="5e56b-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="5e56b-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5e56b-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="5e56b-110">Child elements</span></span>

<span data-ttu-id="5e56b-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="5e56b-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="5e56b-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="5e56b-112">Parent elements</span></span>

[<span data-ttu-id="5e56b-113">VotingOptionData</span><span class="sxs-lookup"><span data-stu-id="5e56b-113">VotingOptionData</span></span>](votingoptiondata.md)
  
## <a name="text-value"></a><span data-ttu-id="5e56b-114">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="5e56b-114">Text value</span></span>

<span data-ttu-id="5e56b-115">Текстовое значение элемента **SendPrompt** является голосования вариант действий.</span><span class="sxs-lookup"><span data-stu-id="5e56b-115">The text value of the **SendPrompt** element is a voting option action.</span></span> <span data-ttu-id="5e56b-116">В таблице ниже перечислены возможные варианты последнего.</span><span class="sxs-lookup"><span data-stu-id="5e56b-116">The following table lists the possible values for this element.</span></span> 
  
****

|<span data-ttu-id="5e56b-117">**Значение**</span><span class="sxs-lookup"><span data-stu-id="5e56b-117">**Value**</span></span>|<span data-ttu-id="5e56b-118">**Описание**</span><span class="sxs-lookup"><span data-stu-id="5e56b-118">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="5e56b-119">Нет</span><span class="sxs-lookup"><span data-stu-id="5e56b-119">None</span></span>  <br/> |<span data-ttu-id="5e56b-120">Никаких действий.</span><span class="sxs-lookup"><span data-stu-id="5e56b-120">No action.</span></span>  <br/> |
|<span data-ttu-id="5e56b-121">Send (отправлено)</span><span class="sxs-lookup"><span data-stu-id="5e56b-121">Send</span></span>  <br/> |<span data-ttu-id="5e56b-122">Ответ немедленно.</span><span class="sxs-lookup"><span data-stu-id="5e56b-122">The response is sent immediately.</span></span>  <br/> |
|<span data-ttu-id="5e56b-123">VotingOption</span><span class="sxs-lookup"><span data-stu-id="5e56b-123">VotingOption</span></span>  <br/> |<span data-ttu-id="5e56b-124">Утверждающий может ввести комментарии при утверждение или отклонение.</span><span class="sxs-lookup"><span data-stu-id="5e56b-124">The approver can enter comments while approving or rejecting.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="5e56b-125">Замечания</span><span class="sxs-lookup"><span data-stu-id="5e56b-125">Remarks</span></span>

<span data-ttu-id="5e56b-126">Этот элемент появился в Exchange Server 2013 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="5e56b-126">This element was introduced in Exchange Server 2013 Service Pack 1 (SP1).</span></span>
  
<span data-ttu-id="5e56b-127">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="5e56b-127">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5e56b-128">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="5e56b-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5e56b-129">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="5e56b-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="5e56b-130">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="5e56b-130">Schema Name</span></span>  <br/> |<span data-ttu-id="5e56b-131">Схема Types</span><span class="sxs-lookup"><span data-stu-id="5e56b-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="5e56b-132">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="5e56b-132">Validation File</span></span>  <br/> |<span data-ttu-id="5e56b-133">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="5e56b-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="5e56b-134">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="5e56b-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="5e56b-135">True</span><span class="sxs-lookup"><span data-stu-id="5e56b-135">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="5e56b-136">См. также</span><span class="sxs-lookup"><span data-stu-id="5e56b-136">See also</span></span>



[<span data-ttu-id="5e56b-137">VotingOptionData</span><span class="sxs-lookup"><span data-stu-id="5e56b-137">VotingOptionData</span></span>](votingoptiondata.md)


- [<span data-ttu-id="5e56b-138">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="5e56b-138">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

