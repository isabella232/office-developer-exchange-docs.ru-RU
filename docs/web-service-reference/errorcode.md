---
title: Код ошибки
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 0bb00cee-c66b-4f34-b99d-355458f5e83b
description: Элемент ErrorCode представляет код ошибки проверки правила, который описывает, что не удалось средства проверки для каждого правила предикат или действие.
ms.openlocfilehash: ed8e2fa72b0eb007925742e6d194f3a391b3f3cb
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762384"
---
# <a name="errorcode"></a><span data-ttu-id="5ff09-103">Код ошибки</span><span class="sxs-lookup"><span data-stu-id="5ff09-103">ErrorCode</span></span>

<span data-ttu-id="5ff09-104">Элемент **ErrorCode** представляет код ошибки проверки правила, который описывает, что не удалось средства проверки для каждого правила предикат или действие.</span><span class="sxs-lookup"><span data-stu-id="5ff09-104">The **ErrorCode** element represents a rule validation error code that describes what failed validation for each rule predicate or action.</span></span> 
  
```XML
<ErrorCode/>
```

 <span data-ttu-id="5ff09-105">**RuleValidationErrorCodeType**</span><span class="sxs-lookup"><span data-stu-id="5ff09-105">**RuleValidationErrorCodeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5ff09-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="5ff09-106">Attributes and elements</span></span>

<span data-ttu-id="5ff09-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="5ff09-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5ff09-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="5ff09-108">Attributes</span></span>

<span data-ttu-id="5ff09-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="5ff09-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5ff09-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="5ff09-110">Child elements</span></span>

<span data-ttu-id="5ff09-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="5ff09-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="5ff09-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="5ff09-112">Parent elements</span></span>

|<span data-ttu-id="5ff09-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="5ff09-113">**Element**</span></span>|<span data-ttu-id="5ff09-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="5ff09-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5ff09-115">Error</span><span class="sxs-lookup"><span data-stu-id="5ff09-115">Error</span></span>](error.md) <br/> |<span data-ttu-id="5ff09-116">Представляет ошибку одной проверки на значение свойства определенное правило, значение свойства предиката или значение свойства действия.</span><span class="sxs-lookup"><span data-stu-id="5ff09-116">Represents a single validation error on a particular rule property value, predicate property value, or action property value.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="5ff09-117">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="5ff09-117">Text value</span></span>

<span data-ttu-id="5ff09-118">Текстовое значение для этого элемента есть только один из следующих строк:</span><span class="sxs-lookup"><span data-stu-id="5ff09-118">The text value for this element is restricted to one of the following strings:</span></span>
  
- <span data-ttu-id="5ff09-119">ADOperationFailure</span><span class="sxs-lookup"><span data-stu-id="5ff09-119">ADOperationFailure</span></span>
    
- <span data-ttu-id="5ff09-120">ConnectedAccountNotFound</span><span class="sxs-lookup"><span data-stu-id="5ff09-120">ConnectedAccountNotFound</span></span>
    
- <span data-ttu-id="5ff09-121">CreateWithRuleId</span><span class="sxs-lookup"><span data-stu-id="5ff09-121">CreateWithRuleId</span></span>
    
- <span data-ttu-id="5ff09-122">EmptyValueFound</span><span class="sxs-lookup"><span data-stu-id="5ff09-122">EmptyValueFound</span></span>
    
- <span data-ttu-id="5ff09-123">DuplicatedPriority</span><span class="sxs-lookup"><span data-stu-id="5ff09-123">DuplicatedPriority</span></span>
    
- <span data-ttu-id="5ff09-124">DuplicatedOperationOnTheSameRule</span><span class="sxs-lookup"><span data-stu-id="5ff09-124">DuplicatedOperationOnTheSameRule</span></span>
    
- <span data-ttu-id="5ff09-125">FolderDoesNotExist</span><span class="sxs-lookup"><span data-stu-id="5ff09-125">FolderDoesNotExist</span></span>
    
- <span data-ttu-id="5ff09-126">InvalidAddress</span><span class="sxs-lookup"><span data-stu-id="5ff09-126">InvalidAddress</span></span>
    
- <span data-ttu-id="5ff09-127">InvalidDateRange</span><span class="sxs-lookup"><span data-stu-id="5ff09-127">InvalidDateRange</span></span>
    
- <span data-ttu-id="5ff09-128">InvalidFolderId</span><span class="sxs-lookup"><span data-stu-id="5ff09-128">InvalidFolderId</span></span>
    
- <span data-ttu-id="5ff09-129">InvalidSizeRange</span><span class="sxs-lookup"><span data-stu-id="5ff09-129">InvalidSizeRange</span></span>
    
- <span data-ttu-id="5ff09-130">InvalidValue</span><span class="sxs-lookup"><span data-stu-id="5ff09-130">InvalidValue</span></span>
    
- <span data-ttu-id="5ff09-131">MessageClassificationNotFound</span><span class="sxs-lookup"><span data-stu-id="5ff09-131">MessageClassificationNotFound</span></span>
    
- <span data-ttu-id="5ff09-132">MissingAction</span><span class="sxs-lookup"><span data-stu-id="5ff09-132">MissingAction</span></span>
    
- <span data-ttu-id="5ff09-133">MissingParameter</span><span class="sxs-lookup"><span data-stu-id="5ff09-133">MissingParameter</span></span>
    
- <span data-ttu-id="5ff09-134">MissingRangeValue</span><span class="sxs-lookup"><span data-stu-id="5ff09-134">MissingRangeValue</span></span>
    
- <span data-ttu-id="5ff09-135">NotSettable</span><span class="sxs-lookup"><span data-stu-id="5ff09-135">NotSettable</span></span>
    
- <span data-ttu-id="5ff09-136">RecipientDoesNotExist</span><span class="sxs-lookup"><span data-stu-id="5ff09-136">RecipientDoesNotExist</span></span>
    
- <span data-ttu-id="5ff09-137">RuleNotFound</span><span class="sxs-lookup"><span data-stu-id="5ff09-137">RuleNotFound</span></span>
    
- <span data-ttu-id="5ff09-138">SizeLessThanZero</span><span class="sxs-lookup"><span data-stu-id="5ff09-138">SizeLessThanZero</span></span>
    
- <span data-ttu-id="5ff09-139">StringValueTooBig</span><span class="sxs-lookup"><span data-stu-id="5ff09-139">StringValueTooBig</span></span>
    
- <span data-ttu-id="5ff09-140">UnsupportedAddress</span><span class="sxs-lookup"><span data-stu-id="5ff09-140">UnsupportedAddress</span></span>
    
- <span data-ttu-id="5ff09-141">UnexpectedError</span><span class="sxs-lookup"><span data-stu-id="5ff09-141">UnexpectedError</span></span>
    
- <span data-ttu-id="5ff09-142">UnsupportedRule</span><span class="sxs-lookup"><span data-stu-id="5ff09-142">UnsupportedRule</span></span>
    
## <a name="remarks"></a><span data-ttu-id="5ff09-143">Замечания</span><span class="sxs-lookup"><span data-stu-id="5ff09-143">Remarks</span></span>

<span data-ttu-id="5ff09-144">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="5ff09-144">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5ff09-145">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="5ff09-145">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5ff09-146">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="5ff09-146">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="5ff09-147">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="5ff09-147">Schema Name</span></span>  <br/> |<span data-ttu-id="5ff09-148">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="5ff09-148">Messages schema</span></span>  <br/> |
|<span data-ttu-id="5ff09-149">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="5ff09-149">Validation File</span></span>  <br/> |<span data-ttu-id="5ff09-150">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="5ff09-150">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="5ff09-151">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="5ff09-151">Can be Empty</span></span>  <br/> |<span data-ttu-id="5ff09-152">False</span><span class="sxs-lookup"><span data-stu-id="5ff09-152">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="5ff09-153">См. также</span><span class="sxs-lookup"><span data-stu-id="5ff09-153">See also</span></span>



- [<span data-ttu-id="5ff09-154">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="5ff09-154">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

