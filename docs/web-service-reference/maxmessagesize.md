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
description: Элемент MaxMessageSize представляет максимальный размер сообщения, которое может принимать получатель.
ms.openlocfilehash: 13a5679a03420655356269a7e8b5e22950724164
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834383"
---
# <a name="maxmessagesize"></a><span data-ttu-id="97e1b-103">MaxMessageSize</span><span class="sxs-lookup"><span data-stu-id="97e1b-103">MaxMessageSize</span></span>

<span data-ttu-id="97e1b-104">Элемент **MaxMessageSize** представляет максимальный размер сообщения, которое может принимать получатель.</span><span class="sxs-lookup"><span data-stu-id="97e1b-104">The **MaxMessageSize** element represents the maximum message size a recipient can accept.</span></span> 
  
```XML
<MaxMessageSize/>
```

 <span data-ttu-id="97e1b-105">**int**</span><span class="sxs-lookup"><span data-stu-id="97e1b-105">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="97e1b-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="97e1b-106">Attributes and elements</span></span>

<span data-ttu-id="97e1b-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="97e1b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="97e1b-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="97e1b-108">Attributes</span></span>

<span data-ttu-id="97e1b-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="97e1b-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="97e1b-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="97e1b-110">Child elements</span></span>

<span data-ttu-id="97e1b-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="97e1b-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="97e1b-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="97e1b-112">Parent elements</span></span>

|<span data-ttu-id="97e1b-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="97e1b-113">**Element**</span></span>|<span data-ttu-id="97e1b-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="97e1b-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="97e1b-115">Подсказки</span><span class="sxs-lookup"><span data-stu-id="97e1b-115">MailTips</span></span>](mailtips.md) <br/> |<span data-ttu-id="97e1b-116">Представляет значения для различных типов советов по использованию электронной почты.</span><span class="sxs-lookup"><span data-stu-id="97e1b-116">Represents values for various types of mail tips.</span></span>  <br/> |
|[<span data-ttu-id="97e1b-117">Маилтипсконфигуратион (Маилтипссервицеконфигуратион)</span><span class="sxs-lookup"><span data-stu-id="97e1b-117">MailTipsConfiguration (MailTipsServiceConfiguration)</span></span>](mailtipsconfiguration-mailtipsserviceconfiguration.md) <br/> |<span data-ttu-id="97e1b-118">Содержит сведения о конфигурации службы для советов почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="97e1b-118">Contains service configuration information for the mail tips service.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="97e1b-119">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="97e1b-119">Text value</span></span>

<span data-ttu-id="97e1b-120">Текстовое значение — это целое число, представляющее максимальный размер сообщения, которое может принимать получатель.</span><span class="sxs-lookup"><span data-stu-id="97e1b-120">The text value is an integer that represents the maximum message size a recipient can accept.</span></span> <span data-ttu-id="97e1b-121">Это значение можно измерять в килобайтах или мегабайтах.</span><span class="sxs-lookup"><span data-stu-id="97e1b-121">This value can be measured in kilobytes or megabytes.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="97e1b-122">Примечания</span><span class="sxs-lookup"><span data-stu-id="97e1b-122">Remarks</span></span>

<span data-ttu-id="97e1b-123">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="97e1b-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="97e1b-124">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="97e1b-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="97e1b-125">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="97e1b-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="97e1b-126">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="97e1b-126">Schema Name</span></span>  <br/> |<span data-ttu-id="97e1b-127">Схема Types</span><span class="sxs-lookup"><span data-stu-id="97e1b-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="97e1b-128">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="97e1b-128">Validation File</span></span>  <br/> |<span data-ttu-id="97e1b-129">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="97e1b-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="97e1b-130">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="97e1b-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="97e1b-131">False</span><span class="sxs-lookup"><span data-stu-id="97e1b-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="97e1b-132">См. также</span><span class="sxs-lookup"><span data-stu-id="97e1b-132">See also</span></span>



- [<span data-ttu-id="97e1b-133">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="97e1b-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

