---
title: максреЦипиентспержетмаилтипсрекуест
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MaxRecipientsPerGetMailTipsRequest
api_type:
- schema
ms.assetid: 8ff5df18-1989-4217-b4c0-599232911d0c
description: Элемент МаксреЦипиентспержетмаилтипсрекуест указывает максимальное количество получателей, которые могут быть переданы в операцию с помощью подсказок.
ms.openlocfilehash: 4c873fe534582e582bf5b1c1d5fd2789616e056a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834386"
---
# <a name="maxrecipientspergetmailtipsrequest"></a><span data-ttu-id="9c3e5-103">максреЦипиентспержетмаилтипсрекуест</span><span class="sxs-lookup"><span data-stu-id="9c3e5-103">MaxRecipientsPerGetMailTipsRequest</span></span>

<span data-ttu-id="9c3e5-104">Элемент **максреЦипиентспержетмаилтипсрекуест** указывает максимальное количество получателей, которые могут быть переданы в операцию с помощью [подсказок](getmailtips-operation.md).</span><span class="sxs-lookup"><span data-stu-id="9c3e5-104">The **MaxRecipientsPerGetMailTipsRequest** element indicates the maximum number of recipients that can be passed to the [GetMailTips operation](getmailtips-operation.md).</span></span>
  
```XML
<MaxRecipientsPerGetMailTipsRequest/>
```

 <span data-ttu-id="9c3e5-105">**int**</span><span class="sxs-lookup"><span data-stu-id="9c3e5-105">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9c3e5-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="9c3e5-106">Attributes and elements</span></span>

<span data-ttu-id="9c3e5-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="9c3e5-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9c3e5-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="9c3e5-108">Attributes</span></span>

<span data-ttu-id="9c3e5-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="9c3e5-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9c3e5-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="9c3e5-110">Child elements</span></span>

<span data-ttu-id="9c3e5-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="9c3e5-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="9c3e5-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="9c3e5-112">Parent elements</span></span>

|<span data-ttu-id="9c3e5-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="9c3e5-113">**Element**</span></span>|<span data-ttu-id="9c3e5-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="9c3e5-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9c3e5-115">Маилтипсконфигуратион (Маилтипссервицеконфигуратион)</span><span class="sxs-lookup"><span data-stu-id="9c3e5-115">MailTipsConfiguration (MailTipsServiceConfiguration)</span></span>](mailtipsconfiguration-mailtipsserviceconfiguration.md) <br/> |<span data-ttu-id="9c3e5-116">Содержит сведения о конфигурации службы для советов почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="9c3e5-116">Contains service configuration information for the mail tips service.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="9c3e5-117">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="9c3e5-117">Text value</span></span>

<span data-ttu-id="9c3e5-118">Текстовое значение это целое число, представляющее максимальное количество получателей, которые могут быть переданы в [операцию с помощью подсказок](getmailtips-operation.md).</span><span class="sxs-lookup"><span data-stu-id="9c3e5-118">The text value is an integer that represents the maximum number of recipients that can be passed to the [GetMailTips operation](getmailtips-operation.md).</span></span>
  
## <a name="remarks"></a><span data-ttu-id="9c3e5-119">Примечания</span><span class="sxs-lookup"><span data-stu-id="9c3e5-119">Remarks</span></span>

<span data-ttu-id="9c3e5-120">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="9c3e5-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9c3e5-121">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="9c3e5-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9c3e5-122">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="9c3e5-122">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="9c3e5-123">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="9c3e5-123">Schema Name</span></span>  <br/> |<span data-ttu-id="9c3e5-124">Схема Types</span><span class="sxs-lookup"><span data-stu-id="9c3e5-124">Types schema</span></span>  <br/> |
|<span data-ttu-id="9c3e5-125">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="9c3e5-125">Validation File</span></span>  <br/> |<span data-ttu-id="9c3e5-126">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="9c3e5-126">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="9c3e5-127">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="9c3e5-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="9c3e5-128">False</span><span class="sxs-lookup"><span data-stu-id="9c3e5-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9c3e5-129">См. также</span><span class="sxs-lookup"><span data-stu-id="9c3e5-129">See also</span></span>



[<span data-ttu-id="9c3e5-130">Операция GetMailTips</span><span class="sxs-lookup"><span data-stu-id="9c3e5-130">GetMailTips operation</span></span>](getmailtips-operation.md)


- [<span data-ttu-id="9c3e5-131">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="9c3e5-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

