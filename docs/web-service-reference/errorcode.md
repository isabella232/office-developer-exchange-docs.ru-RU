---
title: ErrorCode
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 0bb00cee-c66b-4f34-b99d-355458f5e83b
description: Элемент ErrorCode представляет код ошибки проверки правила, указывающий, что не прошло проверку для каждого предиката правила или действия.
ms.openlocfilehash: ed8e2fa72b0eb007925742e6d194f3a391b3f3cb
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762384"
---
# <a name="errorcode"></a><span data-ttu-id="25824-103">ErrorCode</span><span class="sxs-lookup"><span data-stu-id="25824-103">ErrorCode</span></span>

<span data-ttu-id="25824-104">Элемент **ErrorCode** представляет код ошибки проверки правила, указывающий, что не прошло проверку для каждого предиката правила или действия.</span><span class="sxs-lookup"><span data-stu-id="25824-104">The **ErrorCode** element represents a rule validation error code that describes what failed validation for each rule predicate or action.</span></span> 
  
```XML
<ErrorCode/>
```

 <span data-ttu-id="25824-105">**рулевалидатионерроркодетипе**</span><span class="sxs-lookup"><span data-stu-id="25824-105">**RuleValidationErrorCodeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="25824-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="25824-106">Attributes and elements</span></span>

<span data-ttu-id="25824-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="25824-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="25824-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="25824-108">Attributes</span></span>

<span data-ttu-id="25824-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="25824-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="25824-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="25824-110">Child elements</span></span>

<span data-ttu-id="25824-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="25824-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="25824-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="25824-112">Parent elements</span></span>

|<span data-ttu-id="25824-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="25824-113">**Element**</span></span>|<span data-ttu-id="25824-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="25824-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="25824-115">Ошибка</span><span class="sxs-lookup"><span data-stu-id="25824-115">Error</span></span>](error.md) <br/> |<span data-ttu-id="25824-116">Представляет одну ошибку проверки для определенного значения свойства правила, значения свойства предиката или значения свойства Action.</span><span class="sxs-lookup"><span data-stu-id="25824-116">Represents a single validation error on a particular rule property value, predicate property value, or action property value.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="25824-117">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="25824-117">Text value</span></span>

<span data-ttu-id="25824-118">Текстовое значение для этого элемента ограничено одной из следующих строк:</span><span class="sxs-lookup"><span data-stu-id="25824-118">The text value for this element is restricted to one of the following strings:</span></span>
  
- <span data-ttu-id="25824-119">адоператионфаилуре</span><span class="sxs-lookup"><span data-stu-id="25824-119">ADOperationFailure</span></span>
    
- <span data-ttu-id="25824-120">коннектедаккаунтнотфаунд</span><span class="sxs-lookup"><span data-stu-id="25824-120">ConnectedAccountNotFound</span></span>
    
- <span data-ttu-id="25824-121">креатевисрулеид</span><span class="sxs-lookup"><span data-stu-id="25824-121">CreateWithRuleId</span></span>
    
- <span data-ttu-id="25824-122">емптивалуефаунд</span><span class="sxs-lookup"><span data-stu-id="25824-122">EmptyValueFound</span></span>
    
- <span data-ttu-id="25824-123">дупликатедприорити</span><span class="sxs-lookup"><span data-stu-id="25824-123">DuplicatedPriority</span></span>
    
- <span data-ttu-id="25824-124">дупликатедоператиононсесамеруле</span><span class="sxs-lookup"><span data-stu-id="25824-124">DuplicatedOperationOnTheSameRule</span></span>
    
- <span data-ttu-id="25824-125">фолдердоеснотексист</span><span class="sxs-lookup"><span data-stu-id="25824-125">FolderDoesNotExist</span></span>
    
- <span data-ttu-id="25824-126">InvalidAddress</span><span class="sxs-lookup"><span data-stu-id="25824-126">InvalidAddress</span></span>
    
- <span data-ttu-id="25824-127">инвалиддатеранже</span><span class="sxs-lookup"><span data-stu-id="25824-127">InvalidDateRange</span></span>
    
- <span data-ttu-id="25824-128">инвалидфолдерид</span><span class="sxs-lookup"><span data-stu-id="25824-128">InvalidFolderId</span></span>
    
- <span data-ttu-id="25824-129">инвалидсизеранже</span><span class="sxs-lookup"><span data-stu-id="25824-129">InvalidSizeRange</span></span>
    
- <span data-ttu-id="25824-130">инвалидвалуе</span><span class="sxs-lookup"><span data-stu-id="25824-130">InvalidValue</span></span>
    
- <span data-ttu-id="25824-131">мессажеклассификатионнотфаунд</span><span class="sxs-lookup"><span data-stu-id="25824-131">MessageClassificationNotFound</span></span>
    
- <span data-ttu-id="25824-132">миссингактион</span><span class="sxs-lookup"><span data-stu-id="25824-132">MissingAction</span></span>
    
- <span data-ttu-id="25824-133">миссингпараметер</span><span class="sxs-lookup"><span data-stu-id="25824-133">MissingParameter</span></span>
    
- <span data-ttu-id="25824-134">миссингранжевалуе</span><span class="sxs-lookup"><span data-stu-id="25824-134">MissingRangeValue</span></span>
    
- <span data-ttu-id="25824-135">нотсеттабле</span><span class="sxs-lookup"><span data-stu-id="25824-135">NotSettable</span></span>
    
- <span data-ttu-id="25824-136">реЦипиентдоеснотексист</span><span class="sxs-lookup"><span data-stu-id="25824-136">RecipientDoesNotExist</span></span>
    
- <span data-ttu-id="25824-137">руленотфаунд</span><span class="sxs-lookup"><span data-stu-id="25824-137">RuleNotFound</span></span>
    
- <span data-ttu-id="25824-138">сизелесссанзеро</span><span class="sxs-lookup"><span data-stu-id="25824-138">SizeLessThanZero</span></span>
    
- <span data-ttu-id="25824-139">стрингвалуетубиг</span><span class="sxs-lookup"><span data-stu-id="25824-139">StringValueTooBig</span></span>
    
- <span data-ttu-id="25824-140">унсуппортедаддресс</span><span class="sxs-lookup"><span data-stu-id="25824-140">UnsupportedAddress</span></span>
    
- <span data-ttu-id="25824-141">унекспектедеррор</span><span class="sxs-lookup"><span data-stu-id="25824-141">UnexpectedError</span></span>
    
- <span data-ttu-id="25824-142">унсуппортедруле</span><span class="sxs-lookup"><span data-stu-id="25824-142">UnsupportedRule</span></span>
    
## <a name="remarks"></a><span data-ttu-id="25824-143">Примечания</span><span class="sxs-lookup"><span data-stu-id="25824-143">Remarks</span></span>

<span data-ttu-id="25824-144">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="25824-144">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="25824-145">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="25824-145">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="25824-146">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="25824-146">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="25824-147">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="25824-147">Schema Name</span></span>  <br/> |<span data-ttu-id="25824-148">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="25824-148">Messages schema</span></span>  <br/> |
|<span data-ttu-id="25824-149">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="25824-149">Validation File</span></span>  <br/> |<span data-ttu-id="25824-150">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="25824-150">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="25824-151">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="25824-151">Can be Empty</span></span>  <br/> |<span data-ttu-id="25824-152">False</span><span class="sxs-lookup"><span data-stu-id="25824-152">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="25824-153">См. также</span><span class="sxs-lookup"><span data-stu-id="25824-153">See also</span></span>



- [<span data-ttu-id="25824-154">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="25824-154">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

