---
title: MaxMessageSize
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MaxMessageSize
api_type:
- schema
ms.assetid: bb98ac72-9409-4332-81bb-ee3bebb9a00e
description: Элемент MaxMessageSize представляет максимальный размер сообщения, можно принять получателя.
ms.openlocfilehash: 13a5679a03420655356269a7e8b5e22950724164
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19834383"
---
# <a name="maxmessagesize"></a><span data-ttu-id="ad87c-103">MaxMessageSize</span><span class="sxs-lookup"><span data-stu-id="ad87c-103">MaxMessageSize</span></span>

<span data-ttu-id="ad87c-104">Элемент **MaxMessageSize** представляет максимальный размер сообщения, можно принять получателя.</span><span class="sxs-lookup"><span data-stu-id="ad87c-104">The **MaxMessageSize** element represents the maximum message size a recipient can accept.</span></span> 
  
```XML
<MaxMessageSize/>
```

 <span data-ttu-id="ad87c-105">**int**</span><span class="sxs-lookup"><span data-stu-id="ad87c-105">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ad87c-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="ad87c-106">Attributes and elements</span></span>

<span data-ttu-id="ad87c-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="ad87c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ad87c-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="ad87c-108">Attributes</span></span>

<span data-ttu-id="ad87c-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="ad87c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ad87c-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="ad87c-110">Child elements</span></span>

<span data-ttu-id="ad87c-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="ad87c-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="ad87c-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="ad87c-112">Parent elements</span></span>

|<span data-ttu-id="ad87c-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="ad87c-113">**Element**</span></span>|<span data-ttu-id="ad87c-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="ad87c-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ad87c-115">Почтовые подсказки</span><span class="sxs-lookup"><span data-stu-id="ad87c-115">MailTips</span></span>](mailtips.md) <br/> |<span data-ttu-id="ad87c-116">Представляет значения для различных типов почтовые подсказки.</span><span class="sxs-lookup"><span data-stu-id="ad87c-116">Represents values for various types of mail tips.</span></span>  <br/> |
|[<span data-ttu-id="ad87c-117">MailTipsConfiguration (MailTipsServiceConfiguration)</span><span class="sxs-lookup"><span data-stu-id="ad87c-117">MailTipsConfiguration (MailTipsServiceConfiguration)</span></span>](mailtipsconfiguration-mailtipsserviceconfiguration.md) <br/> |<span data-ttu-id="ad87c-118">Содержит сведения о конфигурации службы для службы советы почты.</span><span class="sxs-lookup"><span data-stu-id="ad87c-118">Contains service configuration information for the mail tips service.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="ad87c-119">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="ad87c-119">Text value</span></span>

<span data-ttu-id="ad87c-120">Текстовое значение — целое число, представляющее максимальный размер сообщения получателя может принимать.</span><span class="sxs-lookup"><span data-stu-id="ad87c-120">The text value is an integer that represents the maximum message size a recipient can accept.</span></span> <span data-ttu-id="ad87c-121">Это значение может быть измеряемую в килобайт или мегабайт.</span><span class="sxs-lookup"><span data-stu-id="ad87c-121">This value can be measured in kilobytes or megabytes.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="ad87c-122">Замечания</span><span class="sxs-lookup"><span data-stu-id="ad87c-122">Remarks</span></span>

<span data-ttu-id="ad87c-123">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="ad87c-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ad87c-124">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="ad87c-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ad87c-125">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="ad87c-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="ad87c-126">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="ad87c-126">Schema Name</span></span>  <br/> |<span data-ttu-id="ad87c-127">Схема Types</span><span class="sxs-lookup"><span data-stu-id="ad87c-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="ad87c-128">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="ad87c-128">Validation File</span></span>  <br/> |<span data-ttu-id="ad87c-129">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="ad87c-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="ad87c-130">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="ad87c-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="ad87c-131">False</span><span class="sxs-lookup"><span data-stu-id="ad87c-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ad87c-132">См. также</span><span class="sxs-lookup"><span data-stu-id="ad87c-132">See also</span></span>



- [<span data-ttu-id="ad87c-133">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="ad87c-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

