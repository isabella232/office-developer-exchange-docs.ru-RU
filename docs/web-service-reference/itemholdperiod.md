---
title: ItemHoldPeriod
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 30369db5-4d45-40e8-bc83-3236667fc404
description: Элемент ItemHoldPeriod указывает количество времени, в течение которого будет храниться контент, соответствующий запросу почтовых ящиков.
ms.openlocfilehash: 185666b72cc96dd88605b7baa6433d070e7ebc91
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44452288"
---
# <a name="itemholdperiod"></a><span data-ttu-id="4f2a3-103">ItemHoldPeriod</span><span class="sxs-lookup"><span data-stu-id="4f2a3-103">ItemHoldPeriod</span></span>

<span data-ttu-id="4f2a3-104">Элемент **ItemHoldPeriod** указывает количество времени, в течение которого будет храниться контент, соответствующий запросу почтовых ящиков.</span><span class="sxs-lookup"><span data-stu-id="4f2a3-104">The **ItemHoldPeriod** element specifies the amount of time to hold content that matches the mailbox query.</span></span> 
  
```XML
<ItemHoldPeriod/>
```

 <span data-ttu-id="4f2a3-105">**строка**</span><span class="sxs-lookup"><span data-stu-id="4f2a3-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4f2a3-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="4f2a3-106">Attributes and elements</span></span>

<span data-ttu-id="4f2a3-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="4f2a3-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4f2a3-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="4f2a3-108">Attributes</span></span>

<span data-ttu-id="4f2a3-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="4f2a3-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4f2a3-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="4f2a3-110">Child elements</span></span>

<span data-ttu-id="4f2a3-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="4f2a3-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="4f2a3-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="4f2a3-112">Parent elements</span></span>

[<span data-ttu-id="4f2a3-113">SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="4f2a3-113">SetHoldOnMailboxes</span></span>](setholdonmailboxes.md)
  
## <a name="text-value"></a><span data-ttu-id="4f2a3-114">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="4f2a3-114">Text value</span></span>

<span data-ttu-id="4f2a3-115">Текстовое значение может быть "unlimited" или строковым значением любого значения [TimeSpan](https://msdn.microsoft.com/library/1ecy8h51%28v=vs.110%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="4f2a3-115">The text value can be "Unlimited" or the string value of any [Timespan](https://msdn.microsoft.com/library/1ecy8h51%28v=vs.110%29.aspx) value.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="4f2a3-116">Примечания</span><span class="sxs-lookup"><span data-stu-id="4f2a3-116">Remarks</span></span>

<span data-ttu-id="4f2a3-117">Этот элемент появился в Exchange Server 2013 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="4f2a3-117">This element was introduced in Exchange Server 2013 Service Pack 1 (SP1).</span></span>
  
<span data-ttu-id="4f2a3-118">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="4f2a3-118">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4f2a3-119">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="4f2a3-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4f2a3-120">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="4f2a3-120">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="4f2a3-121">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="4f2a3-121">Schema Name</span></span>  <br/> |<span data-ttu-id="4f2a3-122">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="4f2a3-122">Messages schema</span></span>  <br/> |
|<span data-ttu-id="4f2a3-123">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="4f2a3-123">Validation File</span></span>  <br/> |<span data-ttu-id="4f2a3-124">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="4f2a3-124">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="4f2a3-125">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="4f2a3-125">Can be Empty</span></span>  <br/> |<span data-ttu-id="4f2a3-126">True</span><span class="sxs-lookup"><span data-stu-id="4f2a3-126">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="4f2a3-127">См. также</span><span class="sxs-lookup"><span data-stu-id="4f2a3-127">See also</span></span>



[<span data-ttu-id="4f2a3-128">SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="4f2a3-128">SetHoldOnMailboxes</span></span>](setholdonmailboxes.md)


- [<span data-ttu-id="4f2a3-129">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="4f2a3-129">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

