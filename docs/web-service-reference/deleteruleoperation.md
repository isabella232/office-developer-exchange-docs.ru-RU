---
title: DeleteRuleOperation
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DeleteRuleOperation
api_type:
- schema
ms.assetid: c5e251af-f795-43cc-baaf-95d84475677c
description: Элемент DeleteRuleOperation содержит операцию для удаления существующего правила папки «Входящие».
ms.openlocfilehash: 3410361e0b896fb0ef01c1873c9f8b0ac99afe58
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762051"
---
# <a name="deleteruleoperation"></a><span data-ttu-id="74020-103">DeleteRuleOperation</span><span class="sxs-lookup"><span data-stu-id="74020-103">DeleteRuleOperation</span></span>

<span data-ttu-id="74020-104">Элемент **DeleteRuleOperation** содержит операцию для удаления существующего правила папки «Входящие».</span><span class="sxs-lookup"><span data-stu-id="74020-104">The **DeleteRuleOperation** element contains an operation to delete an existing Inbox rule.</span></span> 
  
- [<span data-ttu-id="74020-105">UpdateInboxRules</span><span class="sxs-lookup"><span data-stu-id="74020-105">UpdateInboxRules</span></span>](updateinboxrules.md)
- [<span data-ttu-id="74020-106">Операции</span><span class="sxs-lookup"><span data-stu-id="74020-106">Operations</span></span>](operations.md)
  
```XML
<DeleteRuleOperation>
    <RuleId/>
</DeleteRuleOperation>
```

 <span data-ttu-id="74020-107">**DeleteRuleOperationType**</span><span class="sxs-lookup"><span data-stu-id="74020-107">**DeleteRuleOperationType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="74020-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="74020-108">Attributes and elements</span></span>

<span data-ttu-id="74020-109">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="74020-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="74020-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="74020-110">Attributes</span></span>

<span data-ttu-id="74020-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="74020-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="74020-112">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="74020-112">Child elements</span></span>

|<span data-ttu-id="74020-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="74020-113">**Element**</span></span>|<span data-ttu-id="74020-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="74020-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="74020-115">RuleId</span><span class="sxs-lookup"><span data-stu-id="74020-115">RuleId</span></span>](ruleid.md) <br/> |<span data-ttu-id="74020-116">Задает идентификатор правило, которое требуется удалить.</span><span class="sxs-lookup"><span data-stu-id="74020-116">Specifies the identifier of the rule to delete.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="74020-117">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="74020-117">Parent elements</span></span>

|<span data-ttu-id="74020-118">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="74020-118">**Element**</span></span>|<span data-ttu-id="74020-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="74020-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="74020-120">Операции</span><span class="sxs-lookup"><span data-stu-id="74020-120">Operations</span></span>](operations.md) <br/> |<span data-ttu-id="74020-121">Содержит набор операций правила, которые могут выполняться в папке "Входящие".</span><span class="sxs-lookup"><span data-stu-id="74020-121">Contains an array of rule operations that can be performed on an Inbox.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="74020-122">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="74020-122">Text value</span></span>

<span data-ttu-id="74020-123">Нет.</span><span class="sxs-lookup"><span data-stu-id="74020-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="74020-124">Замечания</span><span class="sxs-lookup"><span data-stu-id="74020-124">Remarks</span></span>

<span data-ttu-id="74020-125">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="74020-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="74020-126">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="74020-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="74020-127">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="74020-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="74020-128">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="74020-128">Schema Name</span></span>  <br/> |<span data-ttu-id="74020-129">Схема Types</span><span class="sxs-lookup"><span data-stu-id="74020-129">Types schema</span></span>  <br/> |
|<span data-ttu-id="74020-130">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="74020-130">Validation File</span></span>  <br/> |<span data-ttu-id="74020-131">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="74020-131">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="74020-132">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="74020-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="74020-133">False</span><span class="sxs-lookup"><span data-stu-id="74020-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="74020-134">См. также</span><span class="sxs-lookup"><span data-stu-id="74020-134">See also</span></span>

- [<span data-ttu-id="74020-135">UpdateInboxRules</span><span class="sxs-lookup"><span data-stu-id="74020-135">UpdateInboxRules</span></span>](updateinboxrules.md) 
- [<span data-ttu-id="74020-136">SetRuleOperation</span><span class="sxs-lookup"><span data-stu-id="74020-136">SetRuleOperation</span></span>](setruleoperation.md) 
- [<span data-ttu-id="74020-137">CreateRuleOperation</span><span class="sxs-lookup"><span data-stu-id="74020-137">CreateRuleOperation</span></span>](createruleoperation.md)
- [<span data-ttu-id="74020-138">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="74020-138">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

