---
title: Строка запроса (строка)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f81b1b3d-9fe4-4ab3-b517-42e4207fa596
description: Элемент QueryString указывает набор значений, которые должны быть возвращены, чтобы соответствовать строке запроса в запросе операции FindPeople. Поиск без указания строки запроса возвращает все элементы из указанной папки.
ms.openlocfilehash: ec025f86d3e6fb74810e9c539eba102d05adbb93
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465326"
---
# <a name="querystring-string"></a><span data-ttu-id="780f9-104">Строка запроса (строка)</span><span class="sxs-lookup"><span data-stu-id="780f9-104">QueryString (String)</span></span>

<span data-ttu-id="780f9-105">Элемент **QueryString** указывает набор значений, которые должны быть возвращены, чтобы соответствовать строке запроса в запросе [операции FindPeople](findpeople-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="780f9-105">The **QueryString** element specifies a set of values to be returned that match the query string in a [FindPeople operation](findpeople-operation.md) request.</span></span> <span data-ttu-id="780f9-106">Поиск без указания **строки запроса** возвращает все элементы из указанной папки.</span><span class="sxs-lookup"><span data-stu-id="780f9-106">A search with no **QueryString** specified returns all items from the specified folder.</span></span> 
  
```XML
<QueryString/> 
```

 <span data-ttu-id="780f9-107">**строка**</span><span class="sxs-lookup"><span data-stu-id="780f9-107">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="780f9-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="780f9-108">Attributes and elements</span></span>

<span data-ttu-id="780f9-109">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="780f9-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="780f9-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="780f9-110">Attributes</span></span>

<span data-ttu-id="780f9-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="780f9-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="780f9-112">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="780f9-112">Child elements</span></span>

<span data-ttu-id="780f9-113">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="780f9-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="780f9-114">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="780f9-114">Parent elements</span></span>

|<span data-ttu-id="780f9-115">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="780f9-115">**Element**</span></span>|<span data-ttu-id="780f9-116">**Описание**</span><span class="sxs-lookup"><span data-stu-id="780f9-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="780f9-117">FindPeople</span><span class="sxs-lookup"><span data-stu-id="780f9-117">FindPeople</span></span>](findpeople.md) <br/> |<span data-ttu-id="780f9-118">Содержит аргументы для поиска [операции FindPeople](findpeople-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="780f9-118">Contains the arguments for a [FindPeople operation](findpeople-operation.md) search.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="780f9-119">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="780f9-119">Text value</span></span>

<span data-ttu-id="780f9-120">Текстовое значение **QueryString** представляет запрос почтового ящика, выполненный с помощью подмножества [расширенного синтаксиса запросов (AQS)](https://msdn.microsoft.com/library/aa965711%28VS.85%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="780f9-120">The **QueryString** text value represents a mailbox query made by using a subset of [Advanced Query Syntax (AQS)](https://msdn.microsoft.com/library/aa965711%28VS.85%29.aspx).</span></span> <span data-ttu-id="780f9-121">Сведения о синтаксисе этого элемента см. в статье [QueryString (куеристрингтипе)](querystring-querystringtype.md).</span><span class="sxs-lookup"><span data-stu-id="780f9-121">For information about the syntax for this element, see [QueryString (QueryStringType)](querystring-querystringtype.md).</span></span>
  
## <a name="remarks"></a><span data-ttu-id="780f9-122">Примечания</span><span class="sxs-lookup"><span data-stu-id="780f9-122">Remarks</span></span>

<span data-ttu-id="780f9-123">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="780f9-123">This element was introduced in Exchange Server 2013.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="780f9-124">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="780f9-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="780f9-125">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="780f9-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="780f9-126">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="780f9-126">Schema name</span></span>  <br/> |<span data-ttu-id="780f9-127">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="780f9-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="780f9-128">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="780f9-128">Validation file</span></span>  <br/> |<span data-ttu-id="780f9-129">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="780f9-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="780f9-130">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="780f9-130">Can be empty</span></span>  <br/> |<span data-ttu-id="780f9-131">False</span><span class="sxs-lookup"><span data-stu-id="780f9-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="780f9-132">См. также</span><span class="sxs-lookup"><span data-stu-id="780f9-132">See also</span></span>



[<span data-ttu-id="780f9-133">Операция FindPeople</span><span class="sxs-lookup"><span data-stu-id="780f9-133">FindPeople operation</span></span>](findpeople-operation.md)


- [<span data-ttu-id="780f9-134">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="780f9-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

