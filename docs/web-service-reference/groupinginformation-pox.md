---
title: Граупингинформатион (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 2d8a007f-d79c-43c8-90e3-2c6d883f3a7c
description: Элемент Граупингинформатион содержит значение, используемое для группировки почтового ящика пользователя при подписке на уведомления через несколько почтовых ящиков.
ms.openlocfilehash: bcde002c794ac79d9515befc0755c1f954ee8706
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833781"
---
# <a name="groupinginformation-pox"></a><span data-ttu-id="087cd-103">Граупингинформатион (POX)</span><span class="sxs-lookup"><span data-stu-id="087cd-103">GroupingInformation (POX)</span></span>

<span data-ttu-id="087cd-104">Элемент **граупингинформатион** содержит значение, используемое для группировки почтового ящика [пользователя при](http://msdn.microsoft.com/library/1bda4094-88c3-4f61-9219-6ee70f6e81cf%28Office.15%29.aspx) подписке на уведомления через несколько почтовых ящиков.</span><span class="sxs-lookup"><span data-stu-id="087cd-104">The **GroupingInformation** element contains a value that is used to group the user's mailbox to [maintain affinity](http://msdn.microsoft.com/library/1bda4094-88c3-4f61-9219-6ee70f6e81cf%28Office.15%29.aspx) when subscribing to notifications across multiple mailboxes.</span></span> 
  
[<span data-ttu-id="087cd-105">Служба автообнаружения (POX)</span><span class="sxs-lookup"><span data-stu-id="087cd-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="087cd-106">Ответ (POX)</span><span class="sxs-lookup"><span data-stu-id="087cd-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="087cd-107">Учетная запись (POX)</span><span class="sxs-lookup"><span data-stu-id="087cd-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="087cd-108">Протокол (POX)</span><span class="sxs-lookup"><span data-stu-id="087cd-108">Protocol (POX)</span></span>](protocol-pox.md)
  
[<span data-ttu-id="087cd-109">Граупингинформатион (POX)</span><span class="sxs-lookup"><span data-stu-id="087cd-109">GroupingInformation (POX)</span></span>](groupinginformation-pox.md)
  
```XML
<GroupingInformation/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="087cd-110">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="087cd-110">Attributes and elements</span></span>

<span data-ttu-id="087cd-111">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="087cd-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="087cd-112">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="087cd-112">Attributes</span></span>

<span data-ttu-id="087cd-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="087cd-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="087cd-114">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="087cd-114">Child elements</span></span>

<span data-ttu-id="087cd-115">Нет.</span><span class="sxs-lookup"><span data-stu-id="087cd-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="087cd-116">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="087cd-116">Parent elements</span></span>

|<span data-ttu-id="087cd-117">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="087cd-117">**Element**</span></span>|<span data-ttu-id="087cd-118">**Описание**</span><span class="sxs-lookup"><span data-stu-id="087cd-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="087cd-119">Протокол (POX)</span><span class="sxs-lookup"><span data-stu-id="087cd-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="087cd-120">Содержит спецификации для подключения клиента к серверу Exchange Server.</span><span class="sxs-lookup"><span data-stu-id="087cd-120">Contains the specifications for connecting a client to the Exchange server.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="087cd-121">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="087cd-121">Text value</span></span>

<span data-ttu-id="087cd-122">Текстовое значение сравнивается со значением элемента **граупингинформатион** для других почтовых ящиков.</span><span class="sxs-lookup"><span data-stu-id="087cd-122">The text value is compared to the value of the **GroupingInformation** element for other mailboxes.</span></span> <span data-ttu-id="087cd-123">Почтовые ящики, имеющие одинаковое значение и использующие одну конечную точку веб-служб Exchange (EWS), можно объединять для поддержания сходства.</span><span class="sxs-lookup"><span data-stu-id="087cd-123">Mailboxes that have the same value and use the same Exchange Web Services (EWS) endpoint can be grouped together to maintain affinity.</span></span> <span data-ttu-id="087cd-124">Более подробную информацию можно узнать [в статье поддержание сходства между группой подписок и сервером почтовых ящиков в Exchange](http://msdn.microsoft.com/library/1bda4094-88c3-4f61-9219-6ee70f6e81cf%28Office.15%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="087cd-124">For more details, see [Maintain affinity between a group of subscriptions and the Mailbox server in Exchange](http://msdn.microsoft.com/library/1bda4094-88c3-4f61-9219-6ee70f6e81cf%28Office.15%29.aspx).</span></span>
  
## <a name="remarks"></a><span data-ttu-id="087cd-125">Примечания</span><span class="sxs-lookup"><span data-stu-id="087cd-125">Remarks</span></span>

<span data-ttu-id="087cd-126">Элемент **граупингинформатион** применяется только к элементам **протокола** , имеющим дочерний элемент [Type (POX)](type-pox.md) со значением "expr".</span><span class="sxs-lookup"><span data-stu-id="087cd-126">The **GroupingInformation** element is only applicable to **Protocol** elements that have a [Type (POX)](type-pox.md) child element with a value of "EXPR".</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="087cd-127">См. также</span><span class="sxs-lookup"><span data-stu-id="087cd-127">See also</span></span>

- [<span data-ttu-id="087cd-128">XML-элементы автообнаружения POX для Exchange</span><span class="sxs-lookup"><span data-stu-id="087cd-128">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)
- [<span data-ttu-id="087cd-129">Поддержание сходства между группой подписок и сервером почтовых ящиков в Exchange</span><span class="sxs-lookup"><span data-stu-id="087cd-129">Maintain affinity between a group of subscriptions and the Mailbox server in Exchange</span></span>](http://msdn.microsoft.com/library/1bda4094-88c3-4f61-9219-6ee70f6e81cf%28Office.15%29.aspx)

