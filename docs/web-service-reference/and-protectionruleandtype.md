---
title: И (ProtectionRuleAndType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- And
api_type:
- schema
ms.assetid: 7fafd1c8-cd29-43a0-b383-f6595f934f48
description: Элемент и указывает, что все дочерние элементы должен соответствовать для оценено как истинное.
ms.openlocfilehash: 9e0128ee3fa2b6ffdc5975946694475afec53c25
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761379"
---
# <a name="and-protectionruleandtype"></a><span data-ttu-id="4ae66-103">И (ProtectionRuleAndType)</span><span class="sxs-lookup"><span data-stu-id="4ae66-103">And (ProtectionRuleAndType)</span></span>

<span data-ttu-id="4ae66-104">Элемент **и** указывает, что все дочерние элементы должны соответствовать значение **true**.</span><span class="sxs-lookup"><span data-stu-id="4ae66-104">The **And** element specifies that all child elements must match to evaluate to **true**.</span></span>
  
```xml
<And>
   <AllInternal/>
   <And/>
   <RecipientIs/>
   <SenderDepartments/>
   <True/>
</And>
```

 <span data-ttu-id="4ae66-105">**ProtectionRuleAndType**</span><span class="sxs-lookup"><span data-stu-id="4ae66-105">**ProtectionRuleAndType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4ae66-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="4ae66-106">Attributes and elements</span></span>

<span data-ttu-id="4ae66-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="4ae66-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4ae66-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="4ae66-108">Attributes</span></span>

<span data-ttu-id="4ae66-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="4ae66-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4ae66-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="4ae66-110">Child elements</span></span>

|<span data-ttu-id="4ae66-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="4ae66-111">**Element**</span></span>|<span data-ttu-id="4ae66-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="4ae66-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4ae66-113">AllInternal</span><span class="sxs-lookup"><span data-stu-id="4ae66-113">AllInternal</span></span>](allinternal.md) <br/> |<span data-ttu-id="4ae66-114">Имеет значение **true** , если все получатели сообщения электронной почты являются внутренними относительно организации отправителя.</span><span class="sxs-lookup"><span data-stu-id="4ae66-114">Evaluates to **true** if all recipients of an e-mail message are internal to the sender's organization.</span></span>  <br/> |
|<span data-ttu-id="4ae66-115">**И**</span><span class="sxs-lookup"><span data-stu-id="4ae66-115">**And**</span></span> <br/> |<span data-ttu-id="4ae66-116">Указывает, что все дочерние элементы должны соответствовать значение **true**.</span><span class="sxs-lookup"><span data-stu-id="4ae66-116">Specifies that all child elements must match to evaluate to **true**.</span></span>  <br/> |
|[<span data-ttu-id="4ae66-117">RecipientIs</span><span class="sxs-lookup"><span data-stu-id="4ae66-117">RecipientIs</span></span>](recipientis.md) <br/> |<span data-ttu-id="4ae66-118">Указывает, что какого-либо получателя сообщения электронной почты, соответствует любому из заданных получателей в дочерних элементов [значение (ProtectionRuleValueType)](value-protectionrulevaluetype.md) .</span><span class="sxs-lookup"><span data-stu-id="4ae66-118">Specifies that any recipient of the e-mail message matches any of the specified recipients in the child [Value (ProtectionRuleValueType)](value-protectionrulevaluetype.md) elements.</span></span>  <br/> |
|[<span data-ttu-id="4ae66-119">SenderDepartments</span><span class="sxs-lookup"><span data-stu-id="4ae66-119">SenderDepartments</span></span>](senderdepartments.md) <br/> |<span data-ttu-id="4ae66-120">Указывает, что отдела отправителя соответствует любому из указанного подразделения в дочерних элементов [значение (ProtectionRuleValueType)](value-protectionrulevaluetype.md) .</span><span class="sxs-lookup"><span data-stu-id="4ae66-120">Specifies that the department of the sender matches any of the specified departments in the child [Value (ProtectionRuleValueType)](value-protectionrulevaluetype.md) elements.</span></span>  <br/> |
|[<span data-ttu-id="4ae66-121">Значение true</span><span class="sxs-lookup"><span data-stu-id="4ae66-121">True</span></span>](true.md) <br/> |<span data-ttu-id="4ae66-122">Указывает условие, которое всегда соответствует.</span><span class="sxs-lookup"><span data-stu-id="4ae66-122">Specifies a condition that always matches.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="4ae66-123">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="4ae66-123">Parent elements</span></span>

|<span data-ttu-id="4ae66-124">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="4ae66-124">**Element**</span></span>|<span data-ttu-id="4ae66-125">**Описание**</span><span class="sxs-lookup"><span data-stu-id="4ae66-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4ae66-126">Условие</span><span class="sxs-lookup"><span data-stu-id="4ae66-126">Condition</span></span>](condition.md) <br/> |<span data-ttu-id="4ae66-127">Определяет условие, которое должно выполняться для части действия правила для выполнения.</span><span class="sxs-lookup"><span data-stu-id="4ae66-127">Identifies the condition that must be satisfied for the action part of the rule to be executed.</span></span>  <br/> |
|<span data-ttu-id="4ae66-128">**И**</span><span class="sxs-lookup"><span data-stu-id="4ae66-128">**And**</span></span> <br/> |<span data-ttu-id="4ae66-129">Указывает, что все дочерние элементы должны соответствовать значение **true**.</span><span class="sxs-lookup"><span data-stu-id="4ae66-129">Specifies that all child elements must match to evaluate to **true**.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="4ae66-130">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="4ae66-130">Text value</span></span>

<span data-ttu-id="4ae66-131">Нет.</span><span class="sxs-lookup"><span data-stu-id="4ae66-131">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="4ae66-132">Замечания</span><span class="sxs-lookup"><span data-stu-id="4ae66-132">Remarks</span></span>

<span data-ttu-id="4ae66-133">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="4ae66-133">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4ae66-134">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="4ae66-134">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4ae66-135">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="4ae66-135">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="4ae66-136">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="4ae66-136">Schema Name</span></span>  <br/> |<span data-ttu-id="4ae66-137">Схема Types</span><span class="sxs-lookup"><span data-stu-id="4ae66-137">Types schema</span></span>  <br/> |
|<span data-ttu-id="4ae66-138">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="4ae66-138">Validation File</span></span>  <br/> |<span data-ttu-id="4ae66-139">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="4ae66-139">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="4ae66-140">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="4ae66-140">Can be Empty</span></span>  <br/> |<span data-ttu-id="4ae66-141">False</span><span class="sxs-lookup"><span data-stu-id="4ae66-141">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="4ae66-142">См. также</span><span class="sxs-lookup"><span data-stu-id="4ae66-142">See also</span></span>

- [<span data-ttu-id="4ae66-143">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="4ae66-143">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

