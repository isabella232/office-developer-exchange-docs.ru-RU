---
title: SenderDepartments
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SenderDepartments
api_type:
- schema
ms.assetid: b016cdde-d597-40ac-87c4-63ca68bd539d
description: Элемент SenderDepartments указывает, что отдела отправителя соответствует любому из указанного подразделения в дочерних элементов значение (ProtectionRuleValueType).
ms.openlocfilehash: d40e6299bd46ede559cc2cce3bcc9d1611e96bd7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835331"
---
# <a name="senderdepartments"></a><span data-ttu-id="cda14-103">SenderDepartments</span><span class="sxs-lookup"><span data-stu-id="cda14-103">SenderDepartments</span></span>

<span data-ttu-id="cda14-104">Элемент **SenderDepartments** указывает, что отдела отправителя соответствует любому из указанного подразделения в дочерних элементов [значение (ProtectionRuleValueType)](value-protectionrulevaluetype.md) .</span><span class="sxs-lookup"><span data-stu-id="cda14-104">The **SenderDepartments** element specifies that the department of the sender matches any of the specified departments in the child [Value (ProtectionRuleValueType)](value-protectionrulevaluetype.md) elements.</span></span> 
  
```XML
<SenderDepartments>
   <Value/>
</SenderDepartments>
```

 <span data-ttu-id="cda14-105">**ProtectionRuleSenderDepartmentsType**</span><span class="sxs-lookup"><span data-stu-id="cda14-105">**ProtectionRuleSenderDepartmentsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="cda14-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="cda14-106">Attributes and elements</span></span>

<span data-ttu-id="cda14-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="cda14-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="cda14-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="cda14-108">Attributes</span></span>

<span data-ttu-id="cda14-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="cda14-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="cda14-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="cda14-110">Child elements</span></span>

|<span data-ttu-id="cda14-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="cda14-111">**Element**</span></span>|<span data-ttu-id="cda14-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="cda14-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="cda14-113">Значение (ProtectionRuleValueType)</span><span class="sxs-lookup"><span data-stu-id="cda14-113">Value (ProtectionRuleValueType)</span></span>](value-protectionrulevaluetype.md) <br/> |<span data-ttu-id="cda14-114">Идентифицирует отдела одного отправителя.</span><span class="sxs-lookup"><span data-stu-id="cda14-114">Identifies a single sender department.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="cda14-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="cda14-115">Parent elements</span></span>

|<span data-ttu-id="cda14-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="cda14-116">**Element**</span></span>|<span data-ttu-id="cda14-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="cda14-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="cda14-118">Условие</span><span class="sxs-lookup"><span data-stu-id="cda14-118">Condition</span></span>](condition.md) <br/> |<span data-ttu-id="cda14-119">Определяет условие, которое должно выполняться для части действия правила для выполнения.</span><span class="sxs-lookup"><span data-stu-id="cda14-119">Identifies the condition that must be satisfied for the action part of the rule to be executed.</span></span>  <br/> |
|[<span data-ttu-id="cda14-120">И (ProtectionRuleAndType)</span><span class="sxs-lookup"><span data-stu-id="cda14-120">And (ProtectionRuleAndType)</span></span>](and-protectionruleandtype.md) <br/> |<span data-ttu-id="cda14-121">Указывает, что все дочерние элементы должны соответствовать значение **true**.</span><span class="sxs-lookup"><span data-stu-id="cda14-121">Specifies that all child elements must match to evaluate to **true**.</span></span> <span data-ttu-id="cda14-122">Указывает, что должно быть более одного условия дочерних правила защиты.</span><span class="sxs-lookup"><span data-stu-id="cda14-122">Specifies that there must be more than one protection rule child condition.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="cda14-123">Замечания</span><span class="sxs-lookup"><span data-stu-id="cda14-123">Remarks</span></span>

<span data-ttu-id="cda14-124">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="cda14-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="cda14-125">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="cda14-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="cda14-126">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="cda14-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="cda14-127">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="cda14-127">Schema Name</span></span>  <br/> |<span data-ttu-id="cda14-128">Схема Types</span><span class="sxs-lookup"><span data-stu-id="cda14-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="cda14-129">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="cda14-129">Validation File</span></span>  <br/> |<span data-ttu-id="cda14-130">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="cda14-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="cda14-131">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="cda14-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="cda14-132">False</span><span class="sxs-lookup"><span data-stu-id="cda14-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="cda14-133">См. также</span><span class="sxs-lookup"><span data-stu-id="cda14-133">See also</span></span>



- [<span data-ttu-id="cda14-134">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="cda14-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

