---
title: ItemHoldPeriod
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 30369db5-4d45-40e8-bc83-3236667fc404
description: Элемент ItemHoldPeriod указывает количество времени для хранения контента, соответствующего запроса почтового ящика.
ms.openlocfilehash: 212d765aa3f0493dd4f3051de483fa08a6fa8ac7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834144"
---
# <a name="itemholdperiod"></a><span data-ttu-id="bdf20-103">ItemHoldPeriod</span><span class="sxs-lookup"><span data-stu-id="bdf20-103">ItemHoldPeriod</span></span>

<span data-ttu-id="bdf20-104">Элемент **ItemHoldPeriod** указывает количество времени для хранения контента, соответствующего запроса почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="bdf20-104">The **ItemHoldPeriod** element specifies the amount of time to hold content that matches the mailbox query.</span></span> 
  
```XML
<ItemHoldPeriod/>
```

 <span data-ttu-id="bdf20-105">**string**</span><span class="sxs-lookup"><span data-stu-id="bdf20-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="bdf20-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="bdf20-106">Attributes and elements</span></span>

<span data-ttu-id="bdf20-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="bdf20-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="bdf20-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="bdf20-108">Attributes</span></span>

<span data-ttu-id="bdf20-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="bdf20-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="bdf20-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="bdf20-110">Child elements</span></span>

<span data-ttu-id="bdf20-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="bdf20-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="bdf20-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="bdf20-112">Parent elements</span></span>

[<span data-ttu-id="bdf20-113">SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="bdf20-113">SetHoldOnMailboxes</span></span>](setholdonmailboxes.md)
  
## <a name="text-value"></a><span data-ttu-id="bdf20-114">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="bdf20-114">Text value</span></span>

<span data-ttu-id="bdf20-115">Текстовое значение может быть «Unlimited» или строковое значение любое значение [Timespan](http://msdn.microsoft.com/ru-ru/library/1ecy8h51%28v=vs.110%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="bdf20-115">The text value can be "Unlimited" or the string value of any [Timespan](http://msdn.microsoft.com/ru-ru/library/1ecy8h51%28v=vs.110%29.aspx) value.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="bdf20-116">Замечания</span><span class="sxs-lookup"><span data-stu-id="bdf20-116">Remarks</span></span>

<span data-ttu-id="bdf20-117">Этот элемент появился в Exchange Server 2013 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="bdf20-117">This element was introduced in Exchange Server 2013 Service Pack 1 (SP1).</span></span>
  
<span data-ttu-id="bdf20-118">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="bdf20-118">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="bdf20-119">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="bdf20-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="bdf20-120">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="bdf20-120">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="bdf20-121">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="bdf20-121">Schema Name</span></span>  <br/> |<span data-ttu-id="bdf20-122">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="bdf20-122">Messages schema</span></span>  <br/> |
|<span data-ttu-id="bdf20-123">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="bdf20-123">Validation File</span></span>  <br/> |<span data-ttu-id="bdf20-124">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="bdf20-124">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="bdf20-125">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="bdf20-125">Can be Empty</span></span>  <br/> |<span data-ttu-id="bdf20-126">True</span><span class="sxs-lookup"><span data-stu-id="bdf20-126">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="bdf20-127">См. также</span><span class="sxs-lookup"><span data-stu-id="bdf20-127">See also</span></span>



[<span data-ttu-id="bdf20-128">SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="bdf20-128">SetHoldOnMailboxes</span></span>](setholdonmailboxes.md)


- [<span data-ttu-id="bdf20-129">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="bdf20-129">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

