---
title: Condition
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
ms.openlocfilehash: d49f2984799b15c0499af59abecbb34abe15f7c3
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/28/2018
ms.locfileid: "21353562"
---
# <a name="condition"></a><span data-ttu-id="536fa-103">Condition</span><span class="sxs-lookup"><span data-stu-id="536fa-103">Condition</span></span>

<span data-ttu-id="536fa-104">Элемент **условие** определяет условие, которое должно выполняться для части действия правила для выполнения.</span><span class="sxs-lookup"><span data-stu-id="536fa-104">The **Condition** element identifies the condition that must be satisfied for the action part of the rule to be executed.</span></span> 
  
```xml
<Condition>
   <AllInternal/>
</Condition>
```

```xml
<Condition> 
    <SenderDepartments/> 
</Condition>
```

```xml
<Condition> 
    <True/> 
</Condition>
```

```xml
<Condition> 
    <Recipients/> 
</Condition>
```

```xml
<Condition> 
    <And/> 
</Condition>
```

<span data-ttu-id="536fa-105">**ProtectionRuleConditionType**</span><span class="sxs-lookup"><span data-stu-id="536fa-105">**ProtectionRuleConditionType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="536fa-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="536fa-106">Attributes and elements</span></span>

<span data-ttu-id="536fa-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="536fa-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="536fa-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="536fa-108">Attributes</span></span>

<span data-ttu-id="536fa-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="536fa-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="536fa-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="536fa-110">Child elements</span></span>

|<span data-ttu-id="536fa-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="536fa-111">**Element**</span></span>|<span data-ttu-id="536fa-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="536fa-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="536fa-113">AllInternal</span><span class="sxs-lookup"><span data-stu-id="536fa-113">AllInternal</span></span>](allinternal.md) <br/> |<span data-ttu-id="536fa-114">Имеет значение **true** , если все получатели сообщения электронной почты являются внутренними относительно организации отправителя.</span><span class="sxs-lookup"><span data-stu-id="536fa-114">Evaluates to **true** if all recipients of an e-mail message are internal to the sender's organization.</span></span>  <br/> |
|[<span data-ttu-id="536fa-115">And (ProtectionRuleAndType)</span><span class="sxs-lookup"><span data-stu-id="536fa-115">And (ProtectionRuleAndType)</span></span>](and-protectionruleandtype.md) <br/> |<span data-ttu-id="536fa-116">Указывает, что все дочерние элементы должны соответствовать значение **true**.</span><span class="sxs-lookup"><span data-stu-id="536fa-116">Specifies that all child elements must match to evaluate to **true**.</span></span> <span data-ttu-id="536fa-117">Указывает, что должно быть более одного условия дочерних правила защиты.</span><span class="sxs-lookup"><span data-stu-id="536fa-117">Specifies that there must be more than one protection rule child condition.</span></span>  <br/> |
|[<span data-ttu-id="536fa-118">RecipientIs</span><span class="sxs-lookup"><span data-stu-id="536fa-118">RecipientIs</span></span>](recipientis.md) <br/> |<span data-ttu-id="536fa-119">Указывает, что какого-либо получателя сообщения электронной почты, соответствует любому из заданных получателей в дочерних элементов [значение (ProtectionRuleValueType)](value-protectionrulevaluetype.md) .</span><span class="sxs-lookup"><span data-stu-id="536fa-119">Specifies that any recipient of the e-mail message matches any of the specified recipients in the child [Value (ProtectionRuleValueType)](value-protectionrulevaluetype.md) elements.</span></span>  <br/> |
|[<span data-ttu-id="536fa-120">SenderDepartments</span><span class="sxs-lookup"><span data-stu-id="536fa-120">SenderDepartments</span></span>](senderdepartments.md) <br/> |<span data-ttu-id="536fa-121">Указывает, что отдела отправителя соответствует любому из указанного подразделения в дочерних элементов [значение (ProtectionRuleValueType)](value-protectionrulevaluetype.md) .</span><span class="sxs-lookup"><span data-stu-id="536fa-121">Specifies that the department of the sender matches any of the specified departments in the child [Value (ProtectionRuleValueType)](value-protectionrulevaluetype.md) elements.</span></span>  <br/> |
|[<span data-ttu-id="536fa-122">True</span><span class="sxs-lookup"><span data-stu-id="536fa-122">True</span></span>](true.md) <br/> |<span data-ttu-id="536fa-123">Указывает условие, которое всегда соответствует.</span><span class="sxs-lookup"><span data-stu-id="536fa-123">Specifies a condition that always matches.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="536fa-124">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="536fa-124">Parent elements</span></span>

|<span data-ttu-id="536fa-125">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="536fa-125">**Element**</span></span>|<span data-ttu-id="536fa-126">**Описание**</span><span class="sxs-lookup"><span data-stu-id="536fa-126">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="536fa-127">Rule</span><span class="sxs-lookup"><span data-stu-id="536fa-127">Rule</span></span>](rule.md) <br/> |<span data-ttu-id="536fa-128">Содержит правило одного защиты.</span><span class="sxs-lookup"><span data-stu-id="536fa-128">Contains a single protection rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="536fa-129">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="536fa-129">Text value</span></span>

<span data-ttu-id="536fa-130">Нет.</span><span class="sxs-lookup"><span data-stu-id="536fa-130">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="536fa-131">Замечания</span><span class="sxs-lookup"><span data-stu-id="536fa-131">Remarks</span></span>

<span data-ttu-id="536fa-132">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="536fa-132">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="536fa-133">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="536fa-133">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="536fa-134">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="536fa-134">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="536fa-135">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="536fa-135">Schema Name</span></span>  <br/> |<span data-ttu-id="536fa-136">Схема Types</span><span class="sxs-lookup"><span data-stu-id="536fa-136">Types schema</span></span>  <br/> |
|<span data-ttu-id="536fa-137">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="536fa-137">Validation File</span></span>  <br/> |<span data-ttu-id="536fa-138">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="536fa-138">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="536fa-139">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="536fa-139">Can be Empty</span></span>  <br/> |<span data-ttu-id="536fa-140">False</span><span class="sxs-lookup"><span data-stu-id="536fa-140">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="536fa-141">См. также</span><span class="sxs-lookup"><span data-stu-id="536fa-141">See also</span></span>

- [<span data-ttu-id="536fa-142">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="536fa-142">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

