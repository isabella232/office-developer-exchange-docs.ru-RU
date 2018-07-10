---
title: Строка запроса (строка)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f81b1b3d-9fe4-4ab3-b517-42e4207fa596
description: Элемент строки запроса указывает набор значений, возвращаемых, соответствующих строки запроса в запрос операции FindPeople. Поиск по не указан строки запроса возвращает все элементы в указанной папке.
ms.openlocfilehash: 9c5c733adcec1496e36986fd720b56b0a0274593
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834935"
---
# <a name="querystring-string"></a><span data-ttu-id="fee9a-104">Строка запроса (строка)</span><span class="sxs-lookup"><span data-stu-id="fee9a-104">QueryString (String)</span></span>

<span data-ttu-id="fee9a-105">Элемент **строки запроса** указывает набор значений, возвращаемых, соответствующих строки запроса в запрос [FindPeople операции](findpeople-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="fee9a-105">The **QueryString** element specifies a set of values to be returned that match the query string in a [FindPeople operation](findpeople-operation.md) request.</span></span> <span data-ttu-id="fee9a-106">Поиск по не указан **строки запроса** возвращает все элементы в указанной папке.</span><span class="sxs-lookup"><span data-stu-id="fee9a-106">A search with no **QueryString** specified returns all items from the specified folder.</span></span> 
  
```XML
<QueryString/> 
```

 <span data-ttu-id="fee9a-107">**string**</span><span class="sxs-lookup"><span data-stu-id="fee9a-107">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="fee9a-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="fee9a-108">Attributes and elements</span></span>

<span data-ttu-id="fee9a-109">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="fee9a-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="fee9a-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="fee9a-110">Attributes</span></span>

<span data-ttu-id="fee9a-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="fee9a-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="fee9a-112">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="fee9a-112">Child elements</span></span>

<span data-ttu-id="fee9a-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="fee9a-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="fee9a-114">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="fee9a-114">Parent elements</span></span>

|<span data-ttu-id="fee9a-115">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="fee9a-115">**Element**</span></span>|<span data-ttu-id="fee9a-116">**Описание**</span><span class="sxs-lookup"><span data-stu-id="fee9a-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fee9a-117">FindPeople</span><span class="sxs-lookup"><span data-stu-id="fee9a-117">FindPeople</span></span>](findpeople.md) <br/> |<span data-ttu-id="fee9a-118">Содержит аргументы для [FindPeople операции](findpeople-operation.md) поиска.</span><span class="sxs-lookup"><span data-stu-id="fee9a-118">Contains the arguments for a [FindPeople operation](findpeople-operation.md) search.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="fee9a-119">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="fee9a-119">Text value</span></span>

<span data-ttu-id="fee9a-120">Текстовое значение **строки запроса** представляет запрос почтового ящика, выполненные с помощью подмножество [Расширенного синтаксиса запроса (AQS)](http://msdn.microsoft.com/ru-ru/library/aa965711%28VS.85%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="fee9a-120">The **QueryString** text value represents a mailbox query made by using a subset of [Advanced Query Syntax (AQS)](http://msdn.microsoft.com/ru-ru/library/aa965711%28VS.85%29.aspx).</span></span> <span data-ttu-id="fee9a-121">Сведения о синтаксисе для этого элемента содержатся [строки запроса (QueryStringType)](querystring-querystringtype.md).</span><span class="sxs-lookup"><span data-stu-id="fee9a-121">For information about the syntax for this element, see [QueryString (QueryStringType)](querystring-querystringtype.md).</span></span>
  
## <a name="remarks"></a><span data-ttu-id="fee9a-122">Замечания</span><span class="sxs-lookup"><span data-stu-id="fee9a-122">Remarks</span></span>

<span data-ttu-id="fee9a-123">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="fee9a-123">This element was introduced in Exchange Server 2013.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="fee9a-124">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="fee9a-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="fee9a-125">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="fee9a-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="fee9a-126">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="fee9a-126">Schema name</span></span>  <br/> |<span data-ttu-id="fee9a-127">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="fee9a-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="fee9a-128">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="fee9a-128">Validation file</span></span>  <br/> |<span data-ttu-id="fee9a-129">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="fee9a-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="fee9a-130">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="fee9a-130">Can be empty</span></span>  <br/> |<span data-ttu-id="fee9a-131">False</span><span class="sxs-lookup"><span data-stu-id="fee9a-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="fee9a-132">См. также</span><span class="sxs-lookup"><span data-stu-id="fee9a-132">See also</span></span>



[<span data-ttu-id="fee9a-133">Операция FindPeople</span><span class="sxs-lookup"><span data-stu-id="fee9a-133">FindPeople operation</span></span>](findpeople-operation.md)


- [<span data-ttu-id="fee9a-134">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="fee9a-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

