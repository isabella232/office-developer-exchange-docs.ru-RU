---
title: рутаддресс
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RootAddress
api_type:
- schema
ms.assetid: 1dbb130a-e4eb-4baf-ae07-2568a8375bff
description: Элемент Рутаддресс представляет первый адрес, с которого начинается событие для события РеЦипиенттраккинжевент.
ms.openlocfilehash: e020ff07f271bdde6c2a4172141097dcba66f64e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465095"
---
# <a name="rootaddress"></a><span data-ttu-id="f1052-103">рутаддресс</span><span class="sxs-lookup"><span data-stu-id="f1052-103">RootAddress</span></span>

<span data-ttu-id="f1052-104">Элемент **рутаддресс** представляет первый адрес, с которого начинается событие для события [реЦипиенттраккинжевент](recipienttrackingevent.md) .</span><span class="sxs-lookup"><span data-stu-id="f1052-104">The **RootAddress** element represents the first address that starts the event for a [RecipientTrackingEvent](recipienttrackingevent.md) event.</span></span> 
  
```xml
<RootAddress/>
```

 <span data-ttu-id="f1052-105">**нонемптистрингтипе**</span><span class="sxs-lookup"><span data-stu-id="f1052-105">**NonEmptyStringType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f1052-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="f1052-106">Attributes and elements</span></span>

<span data-ttu-id="f1052-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="f1052-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f1052-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="f1052-108">Attributes</span></span>

<span data-ttu-id="f1052-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="f1052-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f1052-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="f1052-110">Child elements</span></span>

<span data-ttu-id="f1052-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="f1052-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="f1052-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="f1052-112">Parent elements</span></span>

|<span data-ttu-id="f1052-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="f1052-113">**Element**</span></span>|<span data-ttu-id="f1052-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="f1052-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f1052-115">реЦипиенттраккинжевент</span><span class="sxs-lookup"><span data-stu-id="f1052-115">RecipientTrackingEvent</span></span>](recipienttrackingevent.md) <br/> |<span data-ttu-id="f1052-116">Содержит сведения об отдельном событии получателя.</span><span class="sxs-lookup"><span data-stu-id="f1052-116">Contains information for a single event for a recipient.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="f1052-117">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="f1052-117">Text value</span></span>

<span data-ttu-id="f1052-118">Текстовое значение — это адрес, с которого начинается отслеживание события.</span><span class="sxs-lookup"><span data-stu-id="f1052-118">The text value is the address that starts the tracking event.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="f1052-119">Примечания</span><span class="sxs-lookup"><span data-stu-id="f1052-119">Remarks</span></span>

<span data-ttu-id="f1052-120">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.Этот элемент появился в Exchange Server 2010 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="f1052-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f1052-121">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="f1052-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f1052-122">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="f1052-122">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="f1052-123">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="f1052-123">Schema Name</span></span>  <br/> |<span data-ttu-id="f1052-124">Схема Types</span><span class="sxs-lookup"><span data-stu-id="f1052-124">Types schema</span></span>  <br/> |
|<span data-ttu-id="f1052-125">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="f1052-125">Validation File</span></span>  <br/> |<span data-ttu-id="f1052-126">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="f1052-126">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="f1052-127">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="f1052-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="f1052-128">False</span><span class="sxs-lookup"><span data-stu-id="f1052-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f1052-129">См. также</span><span class="sxs-lookup"><span data-stu-id="f1052-129">See also</span></span>



[<span data-ttu-id="f1052-130">Операция GetMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="f1052-130">GetMessageTrackingReport operation</span></span>](getmessagetrackingreport-operation.md)


- [<span data-ttu-id="f1052-131">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="f1052-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

