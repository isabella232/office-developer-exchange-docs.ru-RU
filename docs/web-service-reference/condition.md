---
title: Условие
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Condition
api_type:
- schema
ms.assetid: 0790a3f2-cb31-4036-a757-7821aa0722cb
description: Элемент условие определяет условие, которое должно выполняться для части действия правила для выполнения.
ms.openlocfilehash: ed605946f99aa63416337cd0e731c931176a8ed4
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761705"
---
# <a name="condition"></a><span data-ttu-id="41ff1-103">Условие</span><span class="sxs-lookup"><span data-stu-id="41ff1-103">Condition</span></span>

<span data-ttu-id="41ff1-104">Элемент **условие** определяет условие, которое должно выполняться для части действия правила для выполнения.</span><span class="sxs-lookup"><span data-stu-id="41ff1-104">The **Condition** element identifies the condition that must be satisfied for the action part of the rule to be executed.</span></span> 
  
```xml
<Condition>
   <AllInternal/>
</Condition>
```

 <span data-ttu-id="41ff1-105">**ProtectionRuleConditionType**</span><span class="sxs-lookup"><span data-stu-id="41ff1-105">**ProtectionRuleConditionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="41ff1-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="41ff1-106">Attributes and elements</span></span>

<span data-ttu-id="41ff1-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="41ff1-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="41ff1-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="41ff1-108">Attributes</span></span>

<span data-ttu-id="41ff1-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="41ff1-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="41ff1-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="41ff1-110">Child elements</span></span>

|<span data-ttu-id="41ff1-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="41ff1-111">**Element**</span></span>|<span data-ttu-id="41ff1-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="41ff1-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="41ff1-113">AllInternal</span><span class="sxs-lookup"><span data-stu-id="41ff1-113">AllInternal</span></span>](allinternal.md) <br/> |<span data-ttu-id="41ff1-114">Имеет значение **true** , если все получатели сообщения электронной почты являются внутренними относительно организации отправителя.</span><span class="sxs-lookup"><span data-stu-id="41ff1-114">Evaluates to **true** if all recipients of an e-mail message are internal to the sender's organization.</span></span>  <br/> |
|[<span data-ttu-id="41ff1-115">И (ProtectionRuleAndType)</span><span class="sxs-lookup"><span data-stu-id="41ff1-115">And (ProtectionRuleAndType)</span></span>](and-protectionruleandtype.md) <br/> |<span data-ttu-id="41ff1-116">Указывает, что все дочерние элементы должны соответствовать значение **true**.</span><span class="sxs-lookup"><span data-stu-id="41ff1-116">Specifies that all child elements must match to evaluate to **true**.</span></span> <span data-ttu-id="41ff1-117">Указывает, что должно быть более одного условия дочерних правила защиты.</span><span class="sxs-lookup"><span data-stu-id="41ff1-117">Specifies that there must be more than one protection rule child condition.</span></span>  <br/> |
|[<span data-ttu-id="41ff1-118">RecipientIs</span><span class="sxs-lookup"><span data-stu-id="41ff1-118">RecipientIs</span></span>](recipientis.md) <br/> |<span data-ttu-id="41ff1-119">Указывает, что какого-либо получателя сообщения электронной почты, соответствует любому из заданных получателей в дочерних элементов [значение (ProtectionRuleValueType)](value-protectionrulevaluetype.md) .</span><span class="sxs-lookup"><span data-stu-id="41ff1-119">Specifies that any recipient of the e-mail message matches any of the specified recipients in the child [Value (ProtectionRuleValueType)](value-protectionrulevaluetype.md) elements.</span></span>  <br/> |
|[<span data-ttu-id="41ff1-120">SenderDepartments</span><span class="sxs-lookup"><span data-stu-id="41ff1-120">SenderDepartments</span></span>](senderdepartments.md) <br/> |<span data-ttu-id="41ff1-121">Указывает, что отдела отправителя соответствует любому из указанного подразделения в дочерних элементов [значение (ProtectionRuleValueType)](value-protectionrulevaluetype.md) .</span><span class="sxs-lookup"><span data-stu-id="41ff1-121">Specifies that the department of the sender matches any of the specified departments in the child [Value (ProtectionRuleValueType)](value-protectionrulevaluetype.md) elements.</span></span>  <br/> |
|[<span data-ttu-id="41ff1-122">Значение true</span><span class="sxs-lookup"><span data-stu-id="41ff1-122">True</span></span>](true.md) <br/> |<span data-ttu-id="41ff1-123">Указывает условие, которое всегда соответствует.</span><span class="sxs-lookup"><span data-stu-id="41ff1-123">Specifies a condition that always matches.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="41ff1-124">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="41ff1-124">Parent elements</span></span>

|<span data-ttu-id="41ff1-125">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="41ff1-125">**Element**</span></span>|<span data-ttu-id="41ff1-126">**Описание**</span><span class="sxs-lookup"><span data-stu-id="41ff1-126">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="41ff1-127">Rule</span><span class="sxs-lookup"><span data-stu-id="41ff1-127">Rule</span></span>](rule.md) <br/> |<span data-ttu-id="41ff1-128">Содержит правило одного защиты.</span><span class="sxs-lookup"><span data-stu-id="41ff1-128">Contains a single protection rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="41ff1-129">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="41ff1-129">Text value</span></span>

<span data-ttu-id="41ff1-130">Нет.</span><span class="sxs-lookup"><span data-stu-id="41ff1-130">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="41ff1-131">Замечания</span><span class="sxs-lookup"><span data-stu-id="41ff1-131">Remarks</span></span>

<span data-ttu-id="41ff1-132">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="41ff1-132">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="41ff1-133">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="41ff1-133">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="41ff1-134">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="41ff1-134">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="41ff1-135">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="41ff1-135">Schema Name</span></span>  <br/> |<span data-ttu-id="41ff1-136">Схема Types</span><span class="sxs-lookup"><span data-stu-id="41ff1-136">Types schema</span></span>  <br/> |
|<span data-ttu-id="41ff1-137">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="41ff1-137">Validation File</span></span>  <br/> |<span data-ttu-id="41ff1-138">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="41ff1-138">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="41ff1-139">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="41ff1-139">Can be Empty</span></span>  <br/> |<span data-ttu-id="41ff1-140">False</span><span class="sxs-lookup"><span data-stu-id="41ff1-140">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="41ff1-141">См. также</span><span class="sxs-lookup"><span data-stu-id="41ff1-141">See also</span></span>



- [<span data-ttu-id="41ff1-142">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="41ff1-142">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

