---
title: Отметка
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 7b47bc74-a60d-4308-8674-5d52444a1753
description: Элемент флаг указывает флаг для элемента почтового ящика.
ms.openlocfilehash: f30f435e8f064d7165ae52de737bbd75b0546206
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762607"
---
# <a name="flag"></a><span data-ttu-id="49292-103">Отметка</span><span class="sxs-lookup"><span data-stu-id="49292-103">Flag</span></span>

<span data-ttu-id="49292-104">Элемент **флаг** указывает флаг для элемента почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="49292-104">The **Flag** element specifies a flag on a mailbox item.</span></span> 
  
```XML
<Flag>
    <FlagStatus/>
    <StartDate/>
    <DueDate/>
    <CompleteDate/>
</Flag>
```

 <span data-ttu-id="49292-105">**FlagType**</span><span class="sxs-lookup"><span data-stu-id="49292-105">**FlagType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="49292-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="49292-106">Attributes and elements</span></span>

<span data-ttu-id="49292-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="49292-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="49292-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="49292-108">Attributes</span></span>

<span data-ttu-id="49292-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="49292-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="49292-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="49292-110">Child elements</span></span>

|<span data-ttu-id="49292-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="49292-111">**Element**</span></span>|<span data-ttu-id="49292-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="49292-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="49292-113">FlagStatus</span><span class="sxs-lookup"><span data-stu-id="49292-113">FlagStatus</span></span>](flagstatus.md) <br/> |<span data-ttu-id="49292-114">Содержит объединенные флаг состояния для элементов в текущей папке.</span><span class="sxs-lookup"><span data-stu-id="49292-114">Contains the aggregated flag status for items in the current folder.</span></span>  <br/> |
|[<span data-ttu-id="49292-115">Дата начала</span><span class="sxs-lookup"><span data-stu-id="49292-115">StartDate</span></span>](startdate.md) <br/> |<span data-ttu-id="49292-116">Представляет дату начала элемента.</span><span class="sxs-lookup"><span data-stu-id="49292-116">Represents the start date of an item.</span></span>  <br/> |
|[<span data-ttu-id="49292-117">DueDate</span><span class="sxs-lookup"><span data-stu-id="49292-117">DueDate</span></span>](duedate.md) <br/> |<span data-ttu-id="49292-118">Представляет дату, когда срок выполнения элемента.</span><span class="sxs-lookup"><span data-stu-id="49292-118">Represents the date when an item is due.</span></span>  <br/> |
|[<span data-ttu-id="49292-119">CompleteDate</span><span class="sxs-lookup"><span data-stu-id="49292-119">CompleteDate</span></span>](completedate.md) <br/> |<span data-ttu-id="49292-120">Представляет дату, на котором был выполнен элемента.</span><span class="sxs-lookup"><span data-stu-id="49292-120">Represents the date on which an item was completed.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="49292-121">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="49292-121">Parent elements</span></span>

|<span data-ttu-id="49292-122">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="49292-122">**Element**</span></span>|<span data-ttu-id="49292-123">**Описание**</span><span class="sxs-lookup"><span data-stu-id="49292-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="49292-124">ConversationAction</span><span class="sxs-lookup"><span data-stu-id="49292-124">ConversationAction</span></span>](conversationaction.md) <br/> |<span data-ttu-id="49292-125">Содержит одно действие должен применяться к разговора.</span><span class="sxs-lookup"><span data-stu-id="49292-125">Contains a single action to be applied to a single conversation.</span></span>  <br/> |
|[<span data-ttu-id="49292-126">Элемент</span><span class="sxs-lookup"><span data-stu-id="49292-126">Item</span></span>](item.md) <br/> |<span data-ttu-id="49292-127">Представляет универсальный элемент в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="49292-127">Represents a generic item in the Exchange store.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="49292-128">Замечания</span><span class="sxs-lookup"><span data-stu-id="49292-128">Remarks</span></span>

<span data-ttu-id="49292-129">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="49292-129">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="49292-130">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="49292-130">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="49292-131">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="49292-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="49292-132">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="49292-132">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="49292-133">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="49292-133">Schema Name</span></span>  <br/> |<span data-ttu-id="49292-134">Схема типа</span><span class="sxs-lookup"><span data-stu-id="49292-134">Type schema</span></span>  <br/> |
|<span data-ttu-id="49292-135">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="49292-135">Validation File</span></span>  <br/> |<span data-ttu-id="49292-136">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="49292-136">types.xsd</span></span>  <br/> |
|<span data-ttu-id="49292-137">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="49292-137">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="49292-138">См. также</span><span class="sxs-lookup"><span data-stu-id="49292-138">See also</span></span>



- [<span data-ttu-id="49292-139">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="49292-139">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

