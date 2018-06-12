---
title: RuleOperationError
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RuleOperationError
api_type:
- schema
ms.assetid: b447e610-d37c-40d3-9158-aa108a9f248e
description: Элемент RuleOperationError — ошибка при операции правила.
ms.openlocfilehash: ff42addea0f55b13794e2c910d4d865ad0b17bc3
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19835265"
---
# <a name="ruleoperationerror"></a><span data-ttu-id="01996-103">RuleOperationError</span><span class="sxs-lookup"><span data-stu-id="01996-103">RuleOperationError</span></span>

<span data-ttu-id="01996-104">Элемент **RuleOperationError** — ошибка при операции правила.</span><span class="sxs-lookup"><span data-stu-id="01996-104">The **RuleOperationError** element represents a rule operation error.</span></span> 
  
```XML
<RuleOperationError>
    <OperationIndex/>
    <ValidationErrors/>
</RuleOperationError>
```

 <span data-ttu-id="01996-105">**RuleOperationErrorType**</span><span class="sxs-lookup"><span data-stu-id="01996-105">**RuleOperationErrorType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="01996-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="01996-106">Attributes and elements</span></span>

<span data-ttu-id="01996-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="01996-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="01996-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="01996-108">Attributes</span></span>

<span data-ttu-id="01996-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="01996-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="01996-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="01996-110">Child elements</span></span>

|<span data-ttu-id="01996-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="01996-111">**Element**</span></span>|<span data-ttu-id="01996-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="01996-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="01996-113">OperationIndex</span><span class="sxs-lookup"><span data-stu-id="01996-113">OperationIndex</span></span>](operationindex.md) <br/> |<span data-ttu-id="01996-114">Указывает индекс операции в запросе, вызвавшей ошибку операции правила.</span><span class="sxs-lookup"><span data-stu-id="01996-114">Indicates the index of the operation in the request that caused the rule operation error.</span></span>  <br/> |
|[<span data-ttu-id="01996-115">ValidationErrors</span><span class="sxs-lookup"><span data-stu-id="01996-115">ValidationErrors</span></span>](validationerrors.md) <br/> |<span data-ttu-id="01996-116">Представляет массив ошибок проверки правил для каждого правила поля, имеющего ошибку.</span><span class="sxs-lookup"><span data-stu-id="01996-116">Represents an array of rule validation errors on each rule field that has an error.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="01996-117">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="01996-117">Parent elements</span></span>

|<span data-ttu-id="01996-118">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="01996-118">**Element**</span></span>|<span data-ttu-id="01996-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="01996-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="01996-120">RuleOperationErrors</span><span class="sxs-lookup"><span data-stu-id="01996-120">RuleOperationErrors</span></span>](ruleoperationerrors.md) <br/> |<span data-ttu-id="01996-121">Представляет массив ошибок проверки правил для каждого правила поля, имеющего ошибку.</span><span class="sxs-lookup"><span data-stu-id="01996-121">Represents an array of rule validation errors on each rule field that has an error.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="01996-122">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="01996-122">Text value</span></span>

<span data-ttu-id="01996-123">Нет.</span><span class="sxs-lookup"><span data-stu-id="01996-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="01996-124">Замечания</span><span class="sxs-lookup"><span data-stu-id="01996-124">Remarks</span></span>

<span data-ttu-id="01996-125">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="01996-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="01996-126">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="01996-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="01996-127">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="01996-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="01996-128">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="01996-128">Schema Name</span></span>  <br/> |<span data-ttu-id="01996-129">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="01996-129">Messages schema</span></span>  <br/> |
|<span data-ttu-id="01996-130">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="01996-130">Validation File</span></span>  <br/> |<span data-ttu-id="01996-131">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="01996-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="01996-132">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="01996-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="01996-133">True</span><span class="sxs-lookup"><span data-stu-id="01996-133">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="01996-134">См. также</span><span class="sxs-lookup"><span data-stu-id="01996-134">See also</span></span>



- [<span data-ttu-id="01996-135">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="01996-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

