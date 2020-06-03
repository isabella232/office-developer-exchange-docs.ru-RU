---
title: ConvertHtmlCodePageToUTF8
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f02c8331-0a4e-4d01-adc2-2b93ed838a42
description: Элемент ConvertHtmlCodePageToUTF8 указывает, преобразуется ли HTML-текст элемента в формат UTF8.
ms.openlocfilehash: a714eacd8cc105146a1471f062ec35dc16730d61
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457594"
---
# <a name="converthtmlcodepagetoutf8"></a><span data-ttu-id="36ad9-103">ConvertHtmlCodePageToUTF8</span><span class="sxs-lookup"><span data-stu-id="36ad9-103">ConvertHtmlCodePageToUTF8</span></span>

<span data-ttu-id="36ad9-104">Элемент **ConvertHtmlCodePageToUTF8** указывает, преобразуется ли HTML-текст элемента в формат UTF8.</span><span class="sxs-lookup"><span data-stu-id="36ad9-104">The **ConvertHtmlCodePageToUTF8** element indicates whether the item HTML body is converted to UTF8.</span></span> 
  
```XML
<ConvertHtmlCodePageToUTF8/>
```

 <span data-ttu-id="36ad9-105">**xs: Boolean**</span><span class="sxs-lookup"><span data-stu-id="36ad9-105">**xs:boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="36ad9-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="36ad9-106">Attributes and elements</span></span>

<span data-ttu-id="36ad9-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="36ad9-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="36ad9-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="36ad9-108">Attributes</span></span>

<span data-ttu-id="36ad9-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="36ad9-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="36ad9-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="36ad9-110">Child elements</span></span>

<span data-ttu-id="36ad9-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="36ad9-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="36ad9-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="36ad9-112">Parent elements</span></span>

|<span data-ttu-id="36ad9-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="36ad9-113">**Element**</span></span>|<span data-ttu-id="36ad9-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="36ad9-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="36ad9-115">итемшапе</span><span class="sxs-lookup"><span data-stu-id="36ad9-115">ItemShape</span></span>](itemshape.md) <br/> |<span data-ttu-id="36ad9-116">Определяет набор свойств, возвращаемых в ответе.</span><span class="sxs-lookup"><span data-stu-id="36ad9-116">Identifies a set of properties to return in a response.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="36ad9-117">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="36ad9-117">Text value</span></span>

<span data-ttu-id="36ad9-118">Текстовое значение **true** для элемента **ConvertHtmlCodePageToUTF8** указывает на то, что HTML-текст преобразуется в кодировку UTF8.</span><span class="sxs-lookup"><span data-stu-id="36ad9-118">A text value of **true** for the **ConvertHtmlCodePageToUTF8** element indicates that the HTML body is converted to UTF8.</span></span> <span data-ttu-id="36ad9-119">Текстовое значение **false** указывает, что HTML-текст не преобразуется в UTF8.</span><span class="sxs-lookup"><span data-stu-id="36ad9-119">A text value of **false** indicates that the HTML body is not converted to UTF8.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="36ad9-120">Примечания</span><span class="sxs-lookup"><span data-stu-id="36ad9-120">Remarks</span></span>

<span data-ttu-id="36ad9-121">По умолчанию используется значение **true** , если элемент **ConvertHtmlCodePageToUTF8** не указан в запросе.</span><span class="sxs-lookup"><span data-stu-id="36ad9-121">The default value of **true** is used if the **ConvertHtmlCodePageToUTF8** element is not specified in a request.</span></span> 
  
<span data-ttu-id="36ad9-122">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.Этот элемент появился в Exchange Server 2010 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="36ad9-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="36ad9-123">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="36ad9-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="36ad9-124">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="36ad9-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="36ad9-125">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="36ad9-125">Schema Name</span></span>  <br/> |<span data-ttu-id="36ad9-126">Схема Types</span><span class="sxs-lookup"><span data-stu-id="36ad9-126">Types schema</span></span>  <br/> |
|<span data-ttu-id="36ad9-127">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="36ad9-127">Validation File</span></span>  <br/> |<span data-ttu-id="36ad9-128">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="36ad9-128">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="36ad9-129">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="36ad9-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="36ad9-130">False</span><span class="sxs-lookup"><span data-stu-id="36ad9-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="36ad9-131">См. также</span><span class="sxs-lookup"><span data-stu-id="36ad9-131">See also</span></span>



- [<span data-ttu-id="36ad9-132">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="36ad9-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

