---
title: Время ожидания (длительность)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: bb15f9a7-8ea5-4765-9877-762c3f98bf50
description: Элемент timeout указывает продолжительность времени до истечения срока действия подписки по запросу на сервере.
ms.openlocfilehash: 23b210dcdd87f2388aecec246068f12ec6c69a78
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19840162"
---
# <a name="timeout-duration"></a><span data-ttu-id="ac1bc-103">Время ожидания (длительность)</span><span class="sxs-lookup"><span data-stu-id="ac1bc-103">Timeout (duration)</span></span>

<span data-ttu-id="ac1bc-104">Элемент **timeout** указывает продолжительность времени до истечения срока действия подписки по запросу на сервере.</span><span class="sxs-lookup"><span data-stu-id="ac1bc-104">The **Timeout** element specifies the length of time before a pull subscription is timed out by the server.</span></span> 
  
```XML
<Timeout></Timeout>
```

 <span data-ttu-id="ac1bc-105">**субскриптионтимеауттипе**</span><span class="sxs-lookup"><span data-stu-id="ac1bc-105">**SubscriptionTimeoutType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ac1bc-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="ac1bc-106">Attributes and elements</span></span>

<span data-ttu-id="ac1bc-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="ac1bc-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ac1bc-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="ac1bc-108">Attributes</span></span>

<span data-ttu-id="ac1bc-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="ac1bc-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ac1bc-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="ac1bc-110">Child elements</span></span>

<span data-ttu-id="ac1bc-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="ac1bc-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="ac1bc-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="ac1bc-112">Parent elements</span></span>

[<span data-ttu-id="ac1bc-113">пуллсубскриптионрекуест</span><span class="sxs-lookup"><span data-stu-id="ac1bc-113">PullSubscriptionRequest</span></span>](pullsubscriptionrequest.md)
  
## <a name="text-value"></a><span data-ttu-id="ac1bc-114">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="ac1bc-114">Text value</span></span>

<span data-ttu-id="ac1bc-115">Текстовое значение элемента **timeout** — это продолжительность времени в минутах до истечения времени ожидания подписки по запросу на сервере.</span><span class="sxs-lookup"><span data-stu-id="ac1bc-115">The text value of the **Timeout** element is the length of time, in minutes, before a pull subscription is timed out by the server.</span></span> <span data-ttu-id="ac1bc-116">Минимальное значение — 1; Максимальное значение — 1440.</span><span class="sxs-lookup"><span data-stu-id="ac1bc-116">The minimum value is 1; the maximum value is 1440.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="ac1bc-117">Примечания</span><span class="sxs-lookup"><span data-stu-id="ac1bc-117">Remarks</span></span>

<span data-ttu-id="ac1bc-118">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="ac1bc-118">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="ac1bc-119">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="ac1bc-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ac1bc-120">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="ac1bc-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ac1bc-121">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="ac1bc-121">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="ac1bc-122">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="ac1bc-122">Schema name</span></span>  <br/> |<span data-ttu-id="ac1bc-123">Схема Types</span><span class="sxs-lookup"><span data-stu-id="ac1bc-123">Types schema</span></span>  <br/> |
|<span data-ttu-id="ac1bc-124">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="ac1bc-124">Validation file</span></span>  <br/> |<span data-ttu-id="ac1bc-125">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="ac1bc-125">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="ac1bc-126">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="ac1bc-126">Can be empty</span></span>  <br/> ||
   

