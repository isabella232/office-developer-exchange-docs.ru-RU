---
title: Rule
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Rule
api_type:
- schema
ms.assetid: c30f3851-bd56-4473-9106-dc85e9619486
description: Элемент Rule содержит правило одного защиты.
ms.openlocfilehash: 9abbb70381c214211172d2d5ba1ed43ee4797f17
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835263"
---
# <a name="rule"></a><span data-ttu-id="e3c4d-103">Rule</span><span class="sxs-lookup"><span data-stu-id="e3c4d-103">Rule</span></span>

<span data-ttu-id="e3c4d-104">Элемент **Rule** содержит правило одного защиты.</span><span class="sxs-lookup"><span data-stu-id="e3c4d-104">The **Rule** element contains a single protection rule.</span></span> 
  
```XML
<Rule Name="" UserOverridable=="" Priority="">
   <Condition/>
   <Action/>
</Rule>
```

 <span data-ttu-id="e3c4d-105">**ProtectionRuleType**</span><span class="sxs-lookup"><span data-stu-id="e3c4d-105">**ProtectionRuleType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e3c4d-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="e3c4d-106">Attributes and elements</span></span>

<span data-ttu-id="e3c4d-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="e3c4d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e3c4d-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="e3c4d-108">Attributes</span></span>

|<span data-ttu-id="e3c4d-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="e3c4d-109">**Attribute**</span></span>|<span data-ttu-id="e3c4d-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="e3c4d-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="e3c4d-111">**Name**</span><span class="sxs-lookup"><span data-stu-id="e3c4d-111">**Name**</span></span> <br/> |<span data-ttu-id="e3c4d-112">Определяет имя правила.</span><span class="sxs-lookup"><span data-stu-id="e3c4d-112">Identifies the name of the rule.</span></span> <span data-ttu-id="e3c4d-113">Обязательный атрибут типа String Минимальная длина равна 1.</span><span class="sxs-lookup"><span data-stu-id="e3c4d-113">A required attribute of type string with a minimum length of 1.</span></span>  <br/> |
|<span data-ttu-id="e3c4d-114">**UserOverridable**</span><span class="sxs-lookup"><span data-stu-id="e3c4d-114">**UserOverridable**</span></span> <br/> |<span data-ttu-id="e3c4d-115">Указывает, будет ли правило является обязательным.</span><span class="sxs-lookup"><span data-stu-id="e3c4d-115">Specifies whether the rule is mandatory.</span></span> <span data-ttu-id="e3c4d-116">Если правило является обязательным, это значение атрибута должно быть **значение false**.</span><span class="sxs-lookup"><span data-stu-id="e3c4d-116">If the rule is mandatory, this attribute value must be **false**.</span></span> <span data-ttu-id="e3c4d-117">Обязательный атрибут типа Boolean.</span><span class="sxs-lookup"><span data-stu-id="e3c4d-117">A required attribute of type Boolean.</span></span>  <br/> |
|<span data-ttu-id="e3c4d-118">**Приоритет**</span><span class="sxs-lookup"><span data-stu-id="e3c4d-118">**Priority**</span></span> <br/> |<span data-ttu-id="e3c4d-119">Указывает приоритет правила.</span><span class="sxs-lookup"><span data-stu-id="e3c4d-119">Specifies the rule priority.</span></span> <span data-ttu-id="e3c4d-120">Обязательный атрибут типа int с минимальное значение 1.</span><span class="sxs-lookup"><span data-stu-id="e3c4d-120">A required attribute of type int with a minimum value of 1.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="e3c4d-121">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="e3c4d-121">Child elements</span></span>

|<span data-ttu-id="e3c4d-122">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="e3c4d-122">**Element**</span></span>|<span data-ttu-id="e3c4d-123">**Описание**</span><span class="sxs-lookup"><span data-stu-id="e3c4d-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e3c4d-124">Условие</span><span class="sxs-lookup"><span data-stu-id="e3c4d-124">Condition</span></span>](condition.md) <br/> |<span data-ttu-id="e3c4d-125">Определяет условие, которое должно выполняться для части действия правила для выполнения.</span><span class="sxs-lookup"><span data-stu-id="e3c4d-125">Identifies the condition that must be satisfied for the action part of the rule to be executed.</span></span>  <br/> |
|[<span data-ttu-id="e3c4d-126">Действие (ProtectionRuleActionType)</span><span class="sxs-lookup"><span data-stu-id="e3c4d-126">Action (ProtectionRuleActionType)</span></span>](action-protectionruleactiontype.md) <br/> |<span data-ttu-id="e3c4d-127">Определяет, какое действие необходимо выполнить Если соответствует части условие правила.</span><span class="sxs-lookup"><span data-stu-id="e3c4d-127">Identifies what action must be executed if the condition part of the rule matches.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="e3c4d-128">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="e3c4d-128">Parent elements</span></span>

|<span data-ttu-id="e3c4d-129">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="e3c4d-129">**Element**</span></span>|<span data-ttu-id="e3c4d-130">**Описание**</span><span class="sxs-lookup"><span data-stu-id="e3c4d-130">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e3c4d-131">Правила</span><span class="sxs-lookup"><span data-stu-id="e3c4d-131">Rules </span></span>](rules-ex15websvcsotherref.md) <br/> |<span data-ttu-id="e3c4d-132">Содержит набор правил защиты.</span><span class="sxs-lookup"><span data-stu-id="e3c4d-132">Contains an array of protection rules.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="e3c4d-133">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="e3c4d-133">Text value</span></span>

<span data-ttu-id="e3c4d-134">Нет.</span><span class="sxs-lookup"><span data-stu-id="e3c4d-134">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="e3c4d-135">Замечания</span><span class="sxs-lookup"><span data-stu-id="e3c4d-135">Remarks</span></span>

<span data-ttu-id="e3c4d-136">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="e3c4d-136">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e3c4d-137">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="e3c4d-137">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e3c4d-138">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="e3c4d-138">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="e3c4d-139">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="e3c4d-139">Schema Name</span></span>  <br/> |<span data-ttu-id="e3c4d-140">Схема Types</span><span class="sxs-lookup"><span data-stu-id="e3c4d-140">Types schema</span></span>  <br/> |
|<span data-ttu-id="e3c4d-141">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="e3c4d-141">Validation File</span></span>  <br/> |<span data-ttu-id="e3c4d-142">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="e3c4d-142">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="e3c4d-143">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="e3c4d-143">Can be Empty</span></span>  <br/> |<span data-ttu-id="e3c4d-144">False</span><span class="sxs-lookup"><span data-stu-id="e3c4d-144">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e3c4d-145">См. также</span><span class="sxs-lookup"><span data-stu-id="e3c4d-145">See also</span></span>



- [<span data-ttu-id="e3c4d-146">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="e3c4d-146">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

