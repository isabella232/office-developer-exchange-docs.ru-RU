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
description: Элемент Rule содержит одно правило защиты.
ms.openlocfilehash: 9abbb70381c214211172d2d5ba1ed43ee4797f17
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835263"
---
# <a name="rule"></a><span data-ttu-id="f15a5-103">Rule</span><span class="sxs-lookup"><span data-stu-id="f15a5-103">Rule</span></span>

<span data-ttu-id="f15a5-104">Элемент **rule** содержит одно правило защиты.</span><span class="sxs-lookup"><span data-stu-id="f15a5-104">The **Rule** element contains a single protection rule.</span></span> 
  
```XML
<Rule Name="" UserOverridable=="" Priority="">
   <Condition/>
   <Action/>
</Rule>
```

 <span data-ttu-id="f15a5-105">**протектионрулетипе**</span><span class="sxs-lookup"><span data-stu-id="f15a5-105">**ProtectionRuleType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f15a5-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="f15a5-106">Attributes and elements</span></span>

<span data-ttu-id="f15a5-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="f15a5-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f15a5-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="f15a5-108">Attributes</span></span>

|<span data-ttu-id="f15a5-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="f15a5-109">**Attribute**</span></span>|<span data-ttu-id="f15a5-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="f15a5-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="f15a5-111">**Name**</span><span class="sxs-lookup"><span data-stu-id="f15a5-111">**Name**</span></span> <br/> |<span data-ttu-id="f15a5-112">Определяет имя правила.</span><span class="sxs-lookup"><span data-stu-id="f15a5-112">Identifies the name of the rule.</span></span> <span data-ttu-id="f15a5-113">Обязательный атрибут типа String с минимальной длиной 1.</span><span class="sxs-lookup"><span data-stu-id="f15a5-113">A required attribute of type string with a minimum length of 1.</span></span>  <br/> |
|<span data-ttu-id="f15a5-114">**усероверридабле**</span><span class="sxs-lookup"><span data-stu-id="f15a5-114">**UserOverridable**</span></span> <br/> |<span data-ttu-id="f15a5-115">Указывает, является ли правило обязательным.</span><span class="sxs-lookup"><span data-stu-id="f15a5-115">Specifies whether the rule is mandatory.</span></span> <span data-ttu-id="f15a5-116">Если правило является обязательным, значение этого атрибута должно быть равно **false**.</span><span class="sxs-lookup"><span data-stu-id="f15a5-116">If the rule is mandatory, this attribute value must be **false**.</span></span> <span data-ttu-id="f15a5-117">Обязательный атрибут типа Boolean.</span><span class="sxs-lookup"><span data-stu-id="f15a5-117">A required attribute of type Boolean.</span></span>  <br/> |
|<span data-ttu-id="f15a5-118">**Priority**</span><span class="sxs-lookup"><span data-stu-id="f15a5-118">**Priority**</span></span> <br/> |<span data-ttu-id="f15a5-119">Задает приоритет правила.</span><span class="sxs-lookup"><span data-stu-id="f15a5-119">Specifies the rule priority.</span></span> <span data-ttu-id="f15a5-120">Обязательный атрибут типа int с минимальным значением 1.</span><span class="sxs-lookup"><span data-stu-id="f15a5-120">A required attribute of type int with a minimum value of 1.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="f15a5-121">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="f15a5-121">Child elements</span></span>

|<span data-ttu-id="f15a5-122">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="f15a5-122">**Element**</span></span>|<span data-ttu-id="f15a5-123">**Описание**</span><span class="sxs-lookup"><span data-stu-id="f15a5-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f15a5-124">Условие</span><span class="sxs-lookup"><span data-stu-id="f15a5-124">Condition</span></span>](condition.md) <br/> |<span data-ttu-id="f15a5-125">Определяет условие, которое должно быть удовлетворено для части действия правила, которое необходимо выполнить.</span><span class="sxs-lookup"><span data-stu-id="f15a5-125">Identifies the condition that must be satisfied for the action part of the rule to be executed.</span></span>  <br/> |
|[<span data-ttu-id="f15a5-126">Action (Протектионрулеактионтипе)</span><span class="sxs-lookup"><span data-stu-id="f15a5-126">Action (ProtectionRuleActionType)</span></span>](action-protectionruleactiontype.md) <br/> |<span data-ttu-id="f15a5-127">Определяет действие, которое должно выполняться, если условная часть правила соответствует.</span><span class="sxs-lookup"><span data-stu-id="f15a5-127">Identifies what action must be executed if the condition part of the rule matches.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f15a5-128">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="f15a5-128">Parent elements</span></span>

|<span data-ttu-id="f15a5-129">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="f15a5-129">**Element**</span></span>|<span data-ttu-id="f15a5-130">**Описание**</span><span class="sxs-lookup"><span data-stu-id="f15a5-130">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f15a5-131">Условия</span><span class="sxs-lookup"><span data-stu-id="f15a5-131">Rules </span></span>](rules-ex15websvcsotherref.md) <br/> |<span data-ttu-id="f15a5-132">Содержит массив правил защиты.</span><span class="sxs-lookup"><span data-stu-id="f15a5-132">Contains an array of protection rules.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="f15a5-133">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="f15a5-133">Text value</span></span>

<span data-ttu-id="f15a5-134">Нет.</span><span class="sxs-lookup"><span data-stu-id="f15a5-134">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="f15a5-135">Примечания</span><span class="sxs-lookup"><span data-stu-id="f15a5-135">Remarks</span></span>

<span data-ttu-id="f15a5-136">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="f15a5-136">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f15a5-137">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="f15a5-137">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f15a5-138">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="f15a5-138">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="f15a5-139">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="f15a5-139">Schema Name</span></span>  <br/> |<span data-ttu-id="f15a5-140">Схема Types</span><span class="sxs-lookup"><span data-stu-id="f15a5-140">Types schema</span></span>  <br/> |
|<span data-ttu-id="f15a5-141">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="f15a5-141">Validation File</span></span>  <br/> |<span data-ttu-id="f15a5-142">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="f15a5-142">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="f15a5-143">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="f15a5-143">Can be Empty</span></span>  <br/> |<span data-ttu-id="f15a5-144">False</span><span class="sxs-lookup"><span data-stu-id="f15a5-144">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f15a5-145">См. также</span><span class="sxs-lookup"><span data-stu-id="f15a5-145">See also</span></span>



- [<span data-ttu-id="f15a5-146">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="f15a5-146">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

