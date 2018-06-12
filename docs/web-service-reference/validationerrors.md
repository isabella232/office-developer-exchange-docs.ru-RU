---
title: ValidationErrors
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ValidationErrors
api_type:
- schema
ms.assetid: 009526aa-22e7-4f5c-be88-079175aa9122
description: Элемент ValidationErrors представляет массив ошибок проверки правил для каждого правила поля, имеющего ошибку.
ms.openlocfilehash: c95c8057ad2d16a314d33e3738553b495355fd76
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19840449"
---
# <a name="validationerrors"></a><span data-ttu-id="8ea41-103">ValidationErrors</span><span class="sxs-lookup"><span data-stu-id="8ea41-103">ValidationErrors</span></span>

<span data-ttu-id="8ea41-104">Элемент **ValidationErrors** представляет массив ошибок проверки правил для каждого правила поля, имеющего ошибку.</span><span class="sxs-lookup"><span data-stu-id="8ea41-104">The **ValidationErrors** element represents an array of rule validation errors on each rule field that has an error.</span></span> 
  
```XML
<VaidationErrors>
   <Error/>
</ValidationErrors>
```

 <span data-ttu-id="8ea41-105">**ArrayOfRuleValidationErrorsType**</span><span class="sxs-lookup"><span data-stu-id="8ea41-105">**ArrayOfRuleValidationErrorsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="8ea41-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="8ea41-106">Attributes and elements</span></span>

<span data-ttu-id="8ea41-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="8ea41-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8ea41-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="8ea41-108">Attributes</span></span>

<span data-ttu-id="8ea41-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="8ea41-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8ea41-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="8ea41-110">Child elements</span></span>

|<span data-ttu-id="8ea41-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="8ea41-111">**Element**</span></span>|<span data-ttu-id="8ea41-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="8ea41-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8ea41-113">Error</span><span class="sxs-lookup"><span data-stu-id="8ea41-113">Error</span></span>](error.md) <br/> |<span data-ttu-id="8ea41-114">Представляет ошибку одной проверки на значение свойства определенное правило, значение свойства предиката или значение свойства действия</span><span class="sxs-lookup"><span data-stu-id="8ea41-114">Represents a single validation error on a particular rule property value, predicate property value, or action property value</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="8ea41-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="8ea41-115">Parent elements</span></span>

|<span data-ttu-id="8ea41-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="8ea41-116">**Element**</span></span>|<span data-ttu-id="8ea41-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="8ea41-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8ea41-118">RuleOperationError</span><span class="sxs-lookup"><span data-stu-id="8ea41-118">RuleOperationError</span></span>](ruleoperationerror.md) <br/> |<span data-ttu-id="8ea41-119">Представляет ошибку операции правила.</span><span class="sxs-lookup"><span data-stu-id="8ea41-119">Represents a rule operation error.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="8ea41-120">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="8ea41-120">Text value</span></span>

<span data-ttu-id="8ea41-121">Нет.</span><span class="sxs-lookup"><span data-stu-id="8ea41-121">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="8ea41-122">Замечания</span><span class="sxs-lookup"><span data-stu-id="8ea41-122">Remarks</span></span>

<span data-ttu-id="8ea41-123">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="8ea41-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="8ea41-124">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="8ea41-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8ea41-125">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="8ea41-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="8ea41-126">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="8ea41-126">Schema Name</span></span>  <br/> |<span data-ttu-id="8ea41-127">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="8ea41-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="8ea41-128">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="8ea41-128">Validation File</span></span>  <br/> |<span data-ttu-id="8ea41-129">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="8ea41-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="8ea41-130">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="8ea41-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="8ea41-131">True</span><span class="sxs-lookup"><span data-stu-id="8ea41-131">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="8ea41-132">См. также</span><span class="sxs-lookup"><span data-stu-id="8ea41-132">See also</span></span>



- [<span data-ttu-id="8ea41-133">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="8ea41-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

