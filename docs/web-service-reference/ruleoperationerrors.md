---
title: RuleOperationErrors
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f15c7b9e-a670-4a11-bb62-2a298c91f142
description: Элемент RuleOperationErrors представляет массив ошибок проверки правил для каждого правила поля, имеющего ошибку.
ms.openlocfilehash: 7dc85b5cd84af5ad00511a3df2b31ee3541e12b7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835261"
---
# <a name="ruleoperationerrors"></a><span data-ttu-id="e181e-103">RuleOperationErrors</span><span class="sxs-lookup"><span data-stu-id="e181e-103">RuleOperationErrors</span></span>

<span data-ttu-id="e181e-104">Элемент **RuleOperationErrors** представляет массив ошибок проверки правил для каждого правила поля, имеющего ошибку.</span><span class="sxs-lookup"><span data-stu-id="e181e-104">The **RuleOperationErrors** element represents an array of rule validation errors on each rule field that has an error.</span></span> 
  
[<span data-ttu-id="e181e-105">UpdateInboxRulesResponse</span><span class="sxs-lookup"><span data-stu-id="e181e-105">UpdateInboxRulesResponse</span></span>](updateinboxrulesresponse.md)
  
[<span data-ttu-id="e181e-106">RuleOperationErrors</span><span class="sxs-lookup"><span data-stu-id="e181e-106">RuleOperationErrors</span></span>](ruleoperationerrors.md)
  
```XML
<RuleOperationErrors>
    <RuleOperationError>
</RuleOperationErrors>
```

 <span data-ttu-id="e181e-107">**ArrayOfRuleOperationErrorsType**</span><span class="sxs-lookup"><span data-stu-id="e181e-107">**ArrayOfRuleOperationErrorsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e181e-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="e181e-108">Attributes and elements</span></span>

<span data-ttu-id="e181e-109">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="e181e-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e181e-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="e181e-110">Attributes</span></span>

<span data-ttu-id="e181e-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="e181e-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e181e-112">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="e181e-112">Child elements</span></span>

|<span data-ttu-id="e181e-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="e181e-113">**Element**</span></span>|<span data-ttu-id="e181e-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="e181e-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e181e-115">RuleOperationError</span><span class="sxs-lookup"><span data-stu-id="e181e-115">RuleOperationError</span></span>](ruleoperationerror.md) <br/> |<span data-ttu-id="e181e-116">Представляет ошибку операции правила.</span><span class="sxs-lookup"><span data-stu-id="e181e-116">Represents a rule operation error.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="e181e-117">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="e181e-117">Parent elements</span></span>

|<span data-ttu-id="e181e-118">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="e181e-118">**Element**</span></span>|<span data-ttu-id="e181e-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="e181e-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e181e-120">UpdateInboxRulesResponse</span><span class="sxs-lookup"><span data-stu-id="e181e-120">UpdateInboxRulesResponse</span></span>](updateinboxrulesresponse.md) <br/> |<span data-ttu-id="e181e-121">Определяет ответ на запрос [UpdateInboxRules](updateinboxrules.md) .</span><span class="sxs-lookup"><span data-stu-id="e181e-121">Defines a response to an [UpdateInboxRules](updateinboxrules.md) request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="e181e-122">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="e181e-122">Text value</span></span>

<span data-ttu-id="e181e-123">Нет.</span><span class="sxs-lookup"><span data-stu-id="e181e-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="e181e-124">Замечания</span><span class="sxs-lookup"><span data-stu-id="e181e-124">Remarks</span></span>

<span data-ttu-id="e181e-125">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="e181e-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e181e-126">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="e181e-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e181e-127">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="e181e-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="e181e-128">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="e181e-128">Schema name</span></span>  <br/> |<span data-ttu-id="e181e-129">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="e181e-129">Messages schema</span></span>  <br/> |
|<span data-ttu-id="e181e-130">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="e181e-130">Validation file</span></span>  <br/> |<span data-ttu-id="e181e-131">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="e181e-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="e181e-132">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="e181e-132">Can be empty</span></span>  <br/> |<span data-ttu-id="e181e-133">True</span><span class="sxs-lookup"><span data-stu-id="e181e-133">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e181e-134">См. также</span><span class="sxs-lookup"><span data-stu-id="e181e-134">See also</span></span>



[<span data-ttu-id="e181e-135">UpdateInboxRules</span><span class="sxs-lookup"><span data-stu-id="e181e-135">UpdateInboxRules</span></span>](updateinboxrules.md)


- [<span data-ttu-id="e181e-136">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="e181e-136">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

