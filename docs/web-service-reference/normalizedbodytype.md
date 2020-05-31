---
title: нормализедбодитипе
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: c6973aee-ec7b-44c1-b328-f2204d9de5d1
description: Элемент Нормализедбодитипе указывает, возвращается ли нормализованный текст в текстовом формате или HTML-формате.
ms.openlocfilehash: 33575594b22f972a9eb762dfac884fa91459f04a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834554"
---
# <a name="normalizedbodytype"></a><span data-ttu-id="af133-103">нормализедбодитипе</span><span class="sxs-lookup"><span data-stu-id="af133-103">NormalizedBodyType</span></span>

<span data-ttu-id="af133-104">Элемент **нормализедбодитипе** указывает, возвращается ли нормализованный текст в текстовом формате или HTML-формате.</span><span class="sxs-lookup"><span data-stu-id="af133-104">The **NormalizedBodyType** element specifies whether the normalized body is returned in text or HTML format.</span></span> 
  
```XML
<NormalizedBodyType> Best | HTML | Text </NormalizedBodyType>
```

 <span data-ttu-id="af133-105">**бодитипереспонсетипе**</span><span class="sxs-lookup"><span data-stu-id="af133-105">**BodyTypeResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="af133-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="af133-106">Attributes and elements</span></span>

<span data-ttu-id="af133-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="af133-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="af133-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="af133-108">Attributes</span></span>

<span data-ttu-id="af133-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="af133-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="af133-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="af133-110">Child elements</span></span>

<span data-ttu-id="af133-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="af133-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="af133-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="af133-112">Parent elements</span></span>

[<span data-ttu-id="af133-113">итемшапе</span><span class="sxs-lookup"><span data-stu-id="af133-113">ItemShape</span></span>](itemshape.md)
  
## <a name="text-value"></a><span data-ttu-id="af133-114">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="af133-114">Text value</span></span>

<span data-ttu-id="af133-115">Текстовое значение элемента **нормализедбодитипе** указывает формат, в котором возвращается нормализованный текст.</span><span class="sxs-lookup"><span data-stu-id="af133-115">The text value of the **NormalizedBodyType** element indicates format the normalized body is returned in.</span></span> <span data-ttu-id="af133-116">В таблице ниже перечислены возможные варианты последнего.</span><span class="sxs-lookup"><span data-stu-id="af133-116">The following table lists the possible values for this element.</span></span> 
  
****

|<span data-ttu-id="af133-117">**Значение**</span><span class="sxs-lookup"><span data-stu-id="af133-117">**Value**</span></span>|<span data-ttu-id="af133-118">**Описание**</span><span class="sxs-lookup"><span data-stu-id="af133-118">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="af133-119">Лучший</span><span class="sxs-lookup"><span data-stu-id="af133-119">Best</span></span>  <br/> |<span data-ttu-id="af133-120">Ответ будет возвращать наиболее широко доступное содержимое основного текста.</span><span class="sxs-lookup"><span data-stu-id="af133-120">The response will return the richest available content of body text.</span></span> <span data-ttu-id="af133-121">Это полезно, если он неизвестен, является ли контент текстовым или HTML-кодом.</span><span class="sxs-lookup"><span data-stu-id="af133-121">This is useful if it is unknown whether the content is text or HTML.</span></span>  <br/> <span data-ttu-id="af133-122">Возвращаемый текст будет содержать текст, если сохраненный текст является обычным текстом.</span><span class="sxs-lookup"><span data-stu-id="af133-122">The returned body will be text if the stored body is plain text.</span></span> <span data-ttu-id="af133-123">В противном случае ответ вернет HTML, если сохраненный текст имеет формат HTML или RTF.</span><span class="sxs-lookup"><span data-stu-id="af133-123">Otherwise, the response will return HTML if the stored body is in either HTML or RTF format.</span></span>  <br/> <span data-ttu-id="af133-124">Это значение используется по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="af133-124">This is the default value.</span></span>  <br/> |
|<span data-ttu-id="af133-125">HTML</span><span class="sxs-lookup"><span data-stu-id="af133-125">HTML</span></span>  <br/> |<span data-ttu-id="af133-126">Ответ вернет нормализованный текст в формате HTML.</span><span class="sxs-lookup"><span data-stu-id="af133-126">The response will return a normalized body as HTML.</span></span>  <br/> |
|<span data-ttu-id="af133-127">Текст</span><span class="sxs-lookup"><span data-stu-id="af133-127">Text</span></span>  <br/> |<span data-ttu-id="af133-128">Ответ вернет нормализованный текст в виде обычного текста.</span><span class="sxs-lookup"><span data-stu-id="af133-128">The response will return a normalized body as plain text.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="af133-129">Примечания</span><span class="sxs-lookup"><span data-stu-id="af133-129">Remarks</span></span>

<span data-ttu-id="af133-130">Этот элемент появился в Exchange Server 2013 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="af133-130">This element was introduced in Exchange Server 2013 Service Pack 1 (SP1).</span></span>
  
<span data-ttu-id="af133-131">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="af133-131">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="af133-132">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="af133-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="af133-133">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="af133-133">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="af133-134">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="af133-134">Schema Name</span></span>  <br/> |<span data-ttu-id="af133-135">Схема Types</span><span class="sxs-lookup"><span data-stu-id="af133-135">Types schema</span></span>  <br/> |
|<span data-ttu-id="af133-136">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="af133-136">Validation File</span></span>  <br/> |<span data-ttu-id="af133-137">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="af133-137">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="af133-138">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="af133-138">Can be Empty</span></span>  <br/> |<span data-ttu-id="af133-139">True</span><span class="sxs-lookup"><span data-stu-id="af133-139">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="af133-140">См. также</span><span class="sxs-lookup"><span data-stu-id="af133-140">See also</span></span>



[<span data-ttu-id="af133-141">итемшапе</span><span class="sxs-lookup"><span data-stu-id="af133-141">ItemShape</span></span>](itemshape.md)


- [<span data-ttu-id="af133-142">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="af133-142">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

