---
title: Тип
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 488ee828-343f-4382-a5e8-eed1005f5dbc
description: Элемент ResultType содержит тип выполняемого поиска. Тип поиска может иметь только статистику или только предварительный просмотр.
ms.openlocfilehash: 750f53ae05a7ad9f5aefc9396911a23ef32cdfc2
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835211"
---
# <a name="resulttype"></a><span data-ttu-id="02123-104">Тип</span><span class="sxs-lookup"><span data-stu-id="02123-104">ResultType</span></span>

<span data-ttu-id="02123-105">Элемент **resultType** содержит тип выполняемого поиска.</span><span class="sxs-lookup"><span data-stu-id="02123-105">The **ResultType** element contains the type of search to perform.</span></span> <span data-ttu-id="02123-106">Тип поиска может иметь только статистику или только предварительный просмотр.</span><span class="sxs-lookup"><span data-stu-id="02123-106">The type of search can be statistics only or preview only.</span></span> 
  
```XML
<ResultType>StatisticsOnly | PreviewOnly</ResultType>
```

 <span data-ttu-id="02123-107">**сеарчресулттипе**</span><span class="sxs-lookup"><span data-stu-id="02123-107">**SearchResultType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="02123-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="02123-108">Attributes and elements</span></span>

<span data-ttu-id="02123-109">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="02123-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="02123-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="02123-110">Attributes</span></span>

<span data-ttu-id="02123-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="02123-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="02123-112">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="02123-112">Child elements</span></span>

<span data-ttu-id="02123-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="02123-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="02123-114">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="02123-114">Parent elements</span></span>

<span data-ttu-id="02123-115">[Сеарчмаилбоксесресулт](searchmailboxesresult.md) | [SearchMailboxes](searchmailboxes.md)</span><span class="sxs-lookup"><span data-stu-id="02123-115">[SearchMailboxesResult](searchmailboxesresult.md) | [SearchMailboxes](searchmailboxes.md)</span></span>
  
## <a name="text-value"></a><span data-ttu-id="02123-116">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="02123-116">Text value</span></span>

<span data-ttu-id="02123-117">Текстовое значение элемента **resultType** — это тип результата, возвращаемого для поиска при обнаружении.</span><span class="sxs-lookup"><span data-stu-id="02123-117">The text value of the **ResultType** element is the type of result that is returned for a discovery search.</span></span> <span data-ttu-id="02123-118">Текстовое значение **статистиксонли** будет возвращать статистику поиска.</span><span class="sxs-lookup"><span data-stu-id="02123-118">A text value of **StatisticsOnly** will return the search statistics.</span></span> <span data-ttu-id="02123-119">Текстовое значение **превиевонли** будет возвращать сведения о предварительном просмотре элемента.</span><span class="sxs-lookup"><span data-stu-id="02123-119">A text value of **PreviewOnly** will return item preview information.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="02123-120">Примечания</span><span class="sxs-lookup"><span data-stu-id="02123-120">Remarks</span></span>

<span data-ttu-id="02123-121">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="02123-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="02123-122">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="02123-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="02123-123">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="02123-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="02123-124">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="02123-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="02123-125">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="02123-125">Schema name</span></span>  <br/> |<span data-ttu-id="02123-126">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="02123-126">Messages schema</span></span>  <br/> |
|<span data-ttu-id="02123-127">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="02123-127">Validation file</span></span>  <br/> |<span data-ttu-id="02123-128">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="02123-128">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="02123-129">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="02123-129">Can be empty</span></span>  <br/> |<span data-ttu-id="02123-130">false</span><span class="sxs-lookup"><span data-stu-id="02123-130">false</span></span>  <br/> |
   

