---
title: ResultType
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 488ee828-343f-4382-a5e8-eed1005f5dbc
description: Элемент ResultType содержит тип поиска для выполнения. Тип поиска можно только статистика или только предварительный просмотр.
ms.openlocfilehash: 750f53ae05a7ad9f5aefc9396911a23ef32cdfc2
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835211"
---
# <a name="resulttype"></a><span data-ttu-id="dfbbd-104">ResultType</span><span class="sxs-lookup"><span data-stu-id="dfbbd-104">ResultType</span></span>

<span data-ttu-id="dfbbd-105">Элемент **ResultType** содержит тип поиска для выполнения.</span><span class="sxs-lookup"><span data-stu-id="dfbbd-105">The **ResultType** element contains the type of search to perform.</span></span> <span data-ttu-id="dfbbd-106">Тип поиска можно только статистика или только предварительный просмотр.</span><span class="sxs-lookup"><span data-stu-id="dfbbd-106">The type of search can be statistics only or preview only.</span></span> 
  
```XML
<ResultType>StatisticsOnly | PreviewOnly</ResultType>
```

 <span data-ttu-id="dfbbd-107">**SearchResultType**</span><span class="sxs-lookup"><span data-stu-id="dfbbd-107">**SearchResultType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="dfbbd-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="dfbbd-108">Attributes and elements</span></span>

<span data-ttu-id="dfbbd-109">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="dfbbd-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="dfbbd-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="dfbbd-110">Attributes</span></span>

<span data-ttu-id="dfbbd-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="dfbbd-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="dfbbd-112">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="dfbbd-112">Child elements</span></span>

<span data-ttu-id="dfbbd-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="dfbbd-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="dfbbd-114">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="dfbbd-114">Parent elements</span></span>

<span data-ttu-id="dfbbd-115">[SearchMailboxesResult](searchmailboxesresult.md) | [SearchMailboxes](searchmailboxes.md)</span><span class="sxs-lookup"><span data-stu-id="dfbbd-115">[SearchMailboxesResult](searchmailboxesresult.md) | [SearchMailboxes](searchmailboxes.md)</span></span>
  
## <a name="text-value"></a><span data-ttu-id="dfbbd-116">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="dfbbd-116">Text value</span></span>

<span data-ttu-id="dfbbd-117">Текстовое значение элемента **ResultType** — тип результата, возвращаемого при поиске обнаружения.</span><span class="sxs-lookup"><span data-stu-id="dfbbd-117">The text value of the **ResultType** element is the type of result that is returned for a discovery search.</span></span> <span data-ttu-id="dfbbd-118">Текстовое значение **только статистика** возвращает статистику поиска.</span><span class="sxs-lookup"><span data-stu-id="dfbbd-118">A text value of **StatisticsOnly** will return the search statistics.</span></span> <span data-ttu-id="dfbbd-119">Текстовое значение **PreviewOnly** будет возвращать сведения предварительной версии элемента.</span><span class="sxs-lookup"><span data-stu-id="dfbbd-119">A text value of **PreviewOnly** will return item preview information.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="dfbbd-120">Замечания</span><span class="sxs-lookup"><span data-stu-id="dfbbd-120">Remarks</span></span>

<span data-ttu-id="dfbbd-121">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="dfbbd-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="dfbbd-122">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="dfbbd-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="dfbbd-123">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="dfbbd-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="dfbbd-124">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="dfbbd-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="dfbbd-125">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="dfbbd-125">Schema name</span></span>  <br/> |<span data-ttu-id="dfbbd-126">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="dfbbd-126">Messages schema</span></span>  <br/> |
|<span data-ttu-id="dfbbd-127">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="dfbbd-127">Validation file</span></span>  <br/> |<span data-ttu-id="dfbbd-128">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="dfbbd-128">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="dfbbd-129">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="dfbbd-129">Can be empty</span></span>  <br/> |<span data-ttu-id="dfbbd-130">Нет</span><span class="sxs-lookup"><span data-stu-id="dfbbd-130">false</span></span>  <br/> |
   

