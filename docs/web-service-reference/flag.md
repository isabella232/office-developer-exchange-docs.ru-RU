---
title: Флаг
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 7b47bc74-a60d-4308-8674-5d52444a1753
description: Элемент Flag указывает флаг для элемента почтового ящика.
ms.openlocfilehash: 7229a26181ee9baf80be5c32c0ef99483310ccb3
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44466264"
---
# <a name="flag"></a><span data-ttu-id="9e2eb-103">Флаг</span><span class="sxs-lookup"><span data-stu-id="9e2eb-103">Flag</span></span>

<span data-ttu-id="9e2eb-104">Элемент **Flag** указывает флаг для элемента почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="9e2eb-104">The **Flag** element specifies a flag on a mailbox item.</span></span> 
  
```XML
<Flag>
    <FlagStatus/>
    <StartDate/>
    <DueDate/>
    <CompleteDate/>
</Flag>
```

 <span data-ttu-id="9e2eb-105">**флагтипе**</span><span class="sxs-lookup"><span data-stu-id="9e2eb-105">**FlagType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9e2eb-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="9e2eb-106">Attributes and elements</span></span>

<span data-ttu-id="9e2eb-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="9e2eb-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9e2eb-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="9e2eb-108">Attributes</span></span>

<span data-ttu-id="9e2eb-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="9e2eb-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9e2eb-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="9e2eb-110">Child elements</span></span>

|<span data-ttu-id="9e2eb-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="9e2eb-111">**Element**</span></span>|<span data-ttu-id="9e2eb-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="9e2eb-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9e2eb-113">FlagStatus</span><span class="sxs-lookup"><span data-stu-id="9e2eb-113">FlagStatus</span></span>](flagstatus.md) <br/> |<span data-ttu-id="9e2eb-114">Содержит сводный статус флагов для элементов в текущей папке.</span><span class="sxs-lookup"><span data-stu-id="9e2eb-114">Contains the aggregated flag status for items in the current folder.</span></span>  <br/> |
|[<span data-ttu-id="9e2eb-115">StartDate</span><span class="sxs-lookup"><span data-stu-id="9e2eb-115">StartDate</span></span>](startdate.md) <br/> |<span data-ttu-id="9e2eb-116">Представляет дату начала элемента.</span><span class="sxs-lookup"><span data-stu-id="9e2eb-116">Represents the start date of an item.</span></span>  <br/> |
|[<span data-ttu-id="9e2eb-117">DueDate</span><span class="sxs-lookup"><span data-stu-id="9e2eb-117">DueDate</span></span>](duedate.md) <br/> |<span data-ttu-id="9e2eb-118">Представляет дату выполнения элемента.</span><span class="sxs-lookup"><span data-stu-id="9e2eb-118">Represents the date when an item is due.</span></span>  <br/> |
|[<span data-ttu-id="9e2eb-119">комплетедате</span><span class="sxs-lookup"><span data-stu-id="9e2eb-119">CompleteDate</span></span>](completedate.md) <br/> |<span data-ttu-id="9e2eb-120">Представляет дату завершения элемента.</span><span class="sxs-lookup"><span data-stu-id="9e2eb-120">Represents the date on which an item was completed.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="9e2eb-121">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="9e2eb-121">Parent elements</span></span>

|<span data-ttu-id="9e2eb-122">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="9e2eb-122">**Element**</span></span>|<span data-ttu-id="9e2eb-123">**Описание**</span><span class="sxs-lookup"><span data-stu-id="9e2eb-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9e2eb-124">конверсатионактион</span><span class="sxs-lookup"><span data-stu-id="9e2eb-124">ConversationAction</span></span>](conversationaction.md) <br/> |<span data-ttu-id="9e2eb-125">Содержит одно действие, которое будет применено к одной беседе.</span><span class="sxs-lookup"><span data-stu-id="9e2eb-125">Contains a single action to be applied to a single conversation.</span></span>  <br/> |
|[<span data-ttu-id="9e2eb-126">Ресурс</span><span class="sxs-lookup"><span data-stu-id="9e2eb-126">Item</span></span>](item.md) <br/> |<span data-ttu-id="9e2eb-127">Представляет общий элемент в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="9e2eb-127">Represents a generic item in the Exchange store.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="9e2eb-128">Примечания</span><span class="sxs-lookup"><span data-stu-id="9e2eb-128">Remarks</span></span>

<span data-ttu-id="9e2eb-129">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="9e2eb-129">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="9e2eb-130">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="9e2eb-130">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9e2eb-131">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="9e2eb-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9e2eb-132">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="9e2eb-132">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="9e2eb-133">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="9e2eb-133">Schema Name</span></span>  <br/> |<span data-ttu-id="9e2eb-134">Схема типа</span><span class="sxs-lookup"><span data-stu-id="9e2eb-134">Type schema</span></span>  <br/> |
|<span data-ttu-id="9e2eb-135">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="9e2eb-135">Validation File</span></span>  <br/> |<span data-ttu-id="9e2eb-136">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="9e2eb-136">types.xsd</span></span>  <br/> |
|<span data-ttu-id="9e2eb-137">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="9e2eb-137">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="9e2eb-138">См. также</span><span class="sxs-lookup"><span data-stu-id="9e2eb-138">See also</span></span>



- [<span data-ttu-id="9e2eb-139">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="9e2eb-139">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

