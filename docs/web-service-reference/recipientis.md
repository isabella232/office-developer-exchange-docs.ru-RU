---
title: RecipientIs
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RecipientIs
api_type:
- schema
ms.assetid: 5d2fd7ce-6137-4b3c-a716-c0218dcc8a09
description: Элемент RecipientIs указывает, что какого-либо получателя сообщения электронной почты, соответствует любому из заданных получателей в дочерних элементов значение (ProtectionRuleValueType).
ms.openlocfilehash: b6d5c150cd874d1aced7f2d83ff36409e0738728
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834975"
---
# <a name="recipientis"></a><span data-ttu-id="abb73-103">RecipientIs</span><span class="sxs-lookup"><span data-stu-id="abb73-103">RecipientIs</span></span>

<span data-ttu-id="abb73-104">Элемент **RecipientIs** указывает, что какого-либо получателя сообщения электронной почты, соответствует любому из заданных получателей в дочерних элементов [значение (ProtectionRuleValueType)](value-protectionrulevaluetype.md) .</span><span class="sxs-lookup"><span data-stu-id="abb73-104">The **RecipientIs** element specifies that any recipient of the e-mail message matches any of the specified recipients in the child [Value (ProtectionRuleValueType)](value-protectionrulevaluetype.md) elements.</span></span> 
  
```xml
<RecipientIs>   <Value/></RecipientIs>
```

 <span data-ttu-id="abb73-105">**ProtectionRuleRecipientIsType**</span><span class="sxs-lookup"><span data-stu-id="abb73-105">**ProtectionRuleRecipientIsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="abb73-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="abb73-106">Attributes and elements</span></span>

<span data-ttu-id="abb73-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="abb73-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="abb73-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="abb73-108">Attributes</span></span>

<span data-ttu-id="abb73-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="abb73-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="abb73-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="abb73-110">Child elements</span></span>

|<span data-ttu-id="abb73-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="abb73-111">**Element**</span></span>|<span data-ttu-id="abb73-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="abb73-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="abb73-113">Значение (ProtectionRuleValueType)</span><span class="sxs-lookup"><span data-stu-id="abb73-113">Value (ProtectionRuleValueType)</span></span>](value-protectionrulevaluetype.md) <br/> |<span data-ttu-id="abb73-114">Идентифицирует получателя.</span><span class="sxs-lookup"><span data-stu-id="abb73-114">Identifies a recipient.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="abb73-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="abb73-115">Parent elements</span></span>

|<span data-ttu-id="abb73-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="abb73-116">**Element**</span></span>|<span data-ttu-id="abb73-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="abb73-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="abb73-118">Условие</span><span class="sxs-lookup"><span data-stu-id="abb73-118">Condition</span></span>](condition.md) <br/> |<span data-ttu-id="abb73-119">Определяет условие, которое должно выполняться для части действия правила для выполнения.</span><span class="sxs-lookup"><span data-stu-id="abb73-119">Identifies the condition that must be satisfied for the action part of the rule to be executed.</span></span>  <br/> |
|[<span data-ttu-id="abb73-120">И (ProtectionRuleAndType)</span><span class="sxs-lookup"><span data-stu-id="abb73-120">And (ProtectionRuleAndType)</span></span>](and-protectionruleandtype.md) <br/> |<span data-ttu-id="abb73-121">Указывает, что все дочерние элементы должны соответствовать значение **true**.</span><span class="sxs-lookup"><span data-stu-id="abb73-121">Indicates that all child elements must match to evaluate to **true**.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="abb73-122">Замечания</span><span class="sxs-lookup"><span data-stu-id="abb73-122">Remarks</span></span>

<span data-ttu-id="abb73-123">Схема, описывающая этот элемент находится в виртуальном каталоге EWS компьютера, на котором выполняется Microsoft Exchange Server 2010 с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="abb73-123">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="abb73-124">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="abb73-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="abb73-125">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="abb73-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="abb73-126">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="abb73-126">Schema Name</span></span>  <br/> |<span data-ttu-id="abb73-127">Схема Types</span><span class="sxs-lookup"><span data-stu-id="abb73-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="abb73-128">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="abb73-128">Validation File</span></span>  <br/> |<span data-ttu-id="abb73-129">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="abb73-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="abb73-130">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="abb73-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="abb73-131">False</span><span class="sxs-lookup"><span data-stu-id="abb73-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="abb73-132">См. также</span><span class="sxs-lookup"><span data-stu-id="abb73-132">See also</span></span>



- [<span data-ttu-id="abb73-133">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="abb73-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

