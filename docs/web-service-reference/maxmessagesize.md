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
ms.openlocfilehash: 727eed38a129800b7d38aa49c41cdacfa13e7a36
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44468413"
---
# <a name="maxmessagesize"></a><span data-ttu-id="7ddf2-103">MaxMessageSize</span><span class="sxs-lookup"><span data-stu-id="7ddf2-103">MaxMessageSize</span></span>

<span data-ttu-id="7ddf2-104">Элемент **MaxMessageSize** представляет максимальный размер сообщения, которое может принимать получатель.</span><span class="sxs-lookup"><span data-stu-id="7ddf2-104">The **MaxMessageSize** element represents the maximum message size a recipient can accept.</span></span> 
  
```XML
<MaxMessageSize/>
```

 <span data-ttu-id="7ddf2-105">**int**</span><span class="sxs-lookup"><span data-stu-id="7ddf2-105">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7ddf2-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="7ddf2-106">Attributes and elements</span></span>

<span data-ttu-id="7ddf2-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="7ddf2-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7ddf2-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="7ddf2-108">Attributes</span></span>

<span data-ttu-id="7ddf2-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="7ddf2-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7ddf2-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="7ddf2-110">Child elements</span></span>

<span data-ttu-id="7ddf2-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="7ddf2-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="7ddf2-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="7ddf2-112">Parent elements</span></span>

|<span data-ttu-id="7ddf2-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="7ddf2-113">**Element**</span></span>|<span data-ttu-id="7ddf2-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="7ddf2-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7ddf2-115">Подсказки</span><span class="sxs-lookup"><span data-stu-id="7ddf2-115">MailTips</span></span>](mailtips.md) <br/> |<span data-ttu-id="7ddf2-116">Представляет значения для различных типов советов по использованию электронной почты.</span><span class="sxs-lookup"><span data-stu-id="7ddf2-116">Represents values for various types of mail tips.</span></span>  <br/> |
|[<span data-ttu-id="7ddf2-117">Маилтипсконфигуратион (Маилтипссервицеконфигуратион)</span><span class="sxs-lookup"><span data-stu-id="7ddf2-117">MailTipsConfiguration (MailTipsServiceConfiguration)</span></span>](mailtipsconfiguration-mailtipsserviceconfiguration.md) <br/> |<span data-ttu-id="7ddf2-118">Содержит сведения о конфигурации службы для советов почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="7ddf2-118">Contains service configuration information for the mail tips service.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="7ddf2-119">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="7ddf2-119">Text value</span></span>

<span data-ttu-id="7ddf2-120">Текстовое значение — это целое число, представляющее максимальный размер сообщения, которое может принимать получатель.</span><span class="sxs-lookup"><span data-stu-id="7ddf2-120">The text value is an integer that represents the maximum message size a recipient can accept.</span></span> <span data-ttu-id="7ddf2-121">Это значение можно измерять в килобайтах или мегабайтах.</span><span class="sxs-lookup"><span data-stu-id="7ddf2-121">This value can be measured in kilobytes or megabytes.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="7ddf2-122">Примечания</span><span class="sxs-lookup"><span data-stu-id="7ddf2-122">Remarks</span></span>

<span data-ttu-id="7ddf2-123">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="7ddf2-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7ddf2-124">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="7ddf2-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7ddf2-125">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="7ddf2-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="7ddf2-126">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="7ddf2-126">Schema Name</span></span>  <br/> |<span data-ttu-id="7ddf2-127">Схема Types</span><span class="sxs-lookup"><span data-stu-id="7ddf2-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="7ddf2-128">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="7ddf2-128">Validation File</span></span>  <br/> |<span data-ttu-id="7ddf2-129">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="7ddf2-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="7ddf2-130">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="7ddf2-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="7ddf2-131">False</span><span class="sxs-lookup"><span data-stu-id="7ddf2-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7ddf2-132">См. также</span><span class="sxs-lookup"><span data-stu-id="7ddf2-132">See also</span></span>



- [<span data-ttu-id="7ddf2-133">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="7ddf2-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

