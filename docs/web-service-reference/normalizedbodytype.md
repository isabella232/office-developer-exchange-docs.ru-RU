---
title: NormalizedBodyType
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: c6973aee-ec7b-44c1-b328-f2204d9de5d1
description: Элемент NormalizedBodyType указывает, возвращается ли нормализованный текст в формате HTML или текст.
ms.openlocfilehash: 33575594b22f972a9eb762dfac884fa91459f04a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19834554"
---
# <a name="normalizedbodytype"></a><span data-ttu-id="8adcb-103">NormalizedBodyType</span><span class="sxs-lookup"><span data-stu-id="8adcb-103">NormalizedBodyType</span></span>

<span data-ttu-id="8adcb-104">Элемент **NormalizedBodyType** указывает, возвращается ли нормализованный текст в формате HTML или текст.</span><span class="sxs-lookup"><span data-stu-id="8adcb-104">The **NormalizedBodyType** element specifies whether the normalized body is returned in text or HTML format.</span></span> 
  
```XML
<NormalizedBodyType> Best | HTML | Text </NormalizedBodyType>
```

 <span data-ttu-id="8adcb-105">**BodyTypeResponseType**</span><span class="sxs-lookup"><span data-stu-id="8adcb-105">**BodyTypeResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="8adcb-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="8adcb-106">Attributes and elements</span></span>

<span data-ttu-id="8adcb-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="8adcb-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8adcb-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="8adcb-108">Attributes</span></span>

<span data-ttu-id="8adcb-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="8adcb-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8adcb-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="8adcb-110">Child elements</span></span>

<span data-ttu-id="8adcb-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="8adcb-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="8adcb-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="8adcb-112">Parent elements</span></span>

[<span data-ttu-id="8adcb-113">ItemShape</span><span class="sxs-lookup"><span data-stu-id="8adcb-113">ItemShape</span></span>](itemshape.md)
  
## <a name="text-value"></a><span data-ttu-id="8adcb-114">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="8adcb-114">Text value</span></span>

<span data-ttu-id="8adcb-115">Текстовое значение элемента **NormalizedBodyType** указывает, что формат нормализованный body, возвращается в.</span><span class="sxs-lookup"><span data-stu-id="8adcb-115">The text value of the **NormalizedBodyType** element indicates format the normalized body is returned in.</span></span> <span data-ttu-id="8adcb-116">В таблице ниже перечислены возможные варианты последнего.</span><span class="sxs-lookup"><span data-stu-id="8adcb-116">The following table lists the possible values for this element.</span></span> 
  
****

|<span data-ttu-id="8adcb-117">**Значение**</span><span class="sxs-lookup"><span data-stu-id="8adcb-117">**Value**</span></span>|<span data-ttu-id="8adcb-118">**Описание**</span><span class="sxs-lookup"><span data-stu-id="8adcb-118">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="8adcb-119">Рекомендации</span><span class="sxs-lookup"><span data-stu-id="8adcb-119">Best</span></span>  <br/> |<span data-ttu-id="8adcb-120">В ответе будут возвращены содержательности доступное содержимое основного текста.</span><span class="sxs-lookup"><span data-stu-id="8adcb-120">The response will return the richest available content of body text.</span></span> <span data-ttu-id="8adcb-121">Это полезно, если не известно, является ли содержимое текста или HTML.</span><span class="sxs-lookup"><span data-stu-id="8adcb-121">This is useful if it is unknown whether the content is text or HTML.</span></span>  <br/> <span data-ttu-id="8adcb-122">Возвращаемое значение body будет текст основному сохраненных обычного текста.</span><span class="sxs-lookup"><span data-stu-id="8adcb-122">The returned body will be text if the stored body is plain text.</span></span> <span data-ttu-id="8adcb-123">В противном случае ответ вернет HTML Если сохраненные текст в формате HTML или RTF.</span><span class="sxs-lookup"><span data-stu-id="8adcb-123">Otherwise, the response will return HTML if the stored body is in either HTML or RTF format.</span></span>  <br/> <span data-ttu-id="8adcb-124">Это значение используется по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="8adcb-124">This is the default value.</span></span>  <br/> |
|<span data-ttu-id="8adcb-125">HTML</span><span class="sxs-lookup"><span data-stu-id="8adcb-125">HTML</span></span>  <br/> |<span data-ttu-id="8adcb-126">В ответе будут возвращены нормализованный body как HTML.</span><span class="sxs-lookup"><span data-stu-id="8adcb-126">The response will return a normalized body as HTML.</span></span>  <br/> |
|<span data-ttu-id="8adcb-127">Text</span><span class="sxs-lookup"><span data-stu-id="8adcb-127">Text</span></span>  <br/> |<span data-ttu-id="8adcb-128">В ответе будут возвращены нормализованный body как обычный текст.</span><span class="sxs-lookup"><span data-stu-id="8adcb-128">The response will return a normalized body as plain text.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="8adcb-129">Замечания</span><span class="sxs-lookup"><span data-stu-id="8adcb-129">Remarks</span></span>

<span data-ttu-id="8adcb-130">Этот элемент появился в Exchange Server 2013 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="8adcb-130">This element was introduced in Exchange Server 2013 Service Pack 1 (SP1).</span></span>
  
<span data-ttu-id="8adcb-131">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="8adcb-131">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="8adcb-132">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="8adcb-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8adcb-133">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="8adcb-133">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="8adcb-134">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="8adcb-134">Schema Name</span></span>  <br/> |<span data-ttu-id="8adcb-135">Схема Types</span><span class="sxs-lookup"><span data-stu-id="8adcb-135">Types schema</span></span>  <br/> |
|<span data-ttu-id="8adcb-136">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="8adcb-136">Validation File</span></span>  <br/> |<span data-ttu-id="8adcb-137">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="8adcb-137">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="8adcb-138">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="8adcb-138">Can be Empty</span></span>  <br/> |<span data-ttu-id="8adcb-139">True</span><span class="sxs-lookup"><span data-stu-id="8adcb-139">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="8adcb-140">См. также</span><span class="sxs-lookup"><span data-stu-id="8adcb-140">See also</span></span>



[<span data-ttu-id="8adcb-141">ItemShape</span><span class="sxs-lookup"><span data-stu-id="8adcb-141">ItemShape</span></span>](itemshape.md)


- [<span data-ttu-id="8adcb-142">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="8adcb-142">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

