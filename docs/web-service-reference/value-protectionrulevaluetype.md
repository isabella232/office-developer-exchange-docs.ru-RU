---
title: Значение (ProtectionRuleValueType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Value
api_type:
- schema
ms.assetid: b039bd6e-2198-47cf-9c78-a5e8b9d51c98
description: Элемент Value определяет одного подразделения получателю и отправителю.
ms.openlocfilehash: 6173f94dcfb83eafd62e35f185a5e8c669d50f6c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19840463"
---
# <a name="value-protectionrulevaluetype"></a><span data-ttu-id="fc7ca-103">Значение (ProtectionRuleValueType)</span><span class="sxs-lookup"><span data-stu-id="fc7ca-103">Value (ProtectionRuleValueType)</span></span>

<span data-ttu-id="fc7ca-104">Элемент **Value** определяет одного подразделения получателю и отправителю.</span><span class="sxs-lookup"><span data-stu-id="fc7ca-104">The **Value** element identifies a single recipient or sender department.</span></span> 
  
```XML
<Value/>
```

<span data-ttu-id="fc7ca-105">**ProtectionRuleValueType**</span><span class="sxs-lookup"><span data-stu-id="fc7ca-105">**ProtectionRuleValueType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="fc7ca-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="fc7ca-106">Attributes and elements</span></span>

<span data-ttu-id="fc7ca-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="fc7ca-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="fc7ca-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="fc7ca-108">Attributes</span></span>

<span data-ttu-id="fc7ca-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="fc7ca-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="fc7ca-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="fc7ca-110">Child elements</span></span>

<span data-ttu-id="fc7ca-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="fc7ca-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="fc7ca-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="fc7ca-112">Parent elements</span></span>

|<span data-ttu-id="fc7ca-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="fc7ca-113">**Element**</span></span>|<span data-ttu-id="fc7ca-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="fc7ca-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fc7ca-115">RecipientIs</span><span class="sxs-lookup"><span data-stu-id="fc7ca-115">RecipientIs</span></span>](recipientis.md) <br/> |<span data-ttu-id="fc7ca-116">Указывает, что какого-либо получателя сообщения электронной почты соответствует любому из заданных получателей в **значение** дочерние элементы.</span><span class="sxs-lookup"><span data-stu-id="fc7ca-116">Specifies that any recipient of the email message matches any of the specified recipients in the child **Value** elements.</span></span>  <br/> |
|[<span data-ttu-id="fc7ca-117">SenderDepartments</span><span class="sxs-lookup"><span data-stu-id="fc7ca-117">SenderDepartments</span></span>](senderdepartments.md) <br/> |<span data-ttu-id="fc7ca-118">Указывает, что отдела отправителя соответствует любому из указанного подразделения в **значение** дочерние элементы.</span><span class="sxs-lookup"><span data-stu-id="fc7ca-118">Specifies that the department of the sender matches any of the specified departments in the child **Value** elements.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="fc7ca-119">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="fc7ca-119">Text value</span></span>

<span data-ttu-id="fc7ca-120">Этот элемент должен содержать значение пустая строка.</span><span class="sxs-lookup"><span data-stu-id="fc7ca-120">This element must contain a nonempty string value.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="fc7ca-121">Замечания</span><span class="sxs-lookup"><span data-stu-id="fc7ca-121">Remarks</span></span>

<span data-ttu-id="fc7ca-122">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="fc7ca-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="fc7ca-123">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="fc7ca-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="fc7ca-124">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="fc7ca-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="fc7ca-125">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="fc7ca-125">Schema Name</span></span>  <br/> |<span data-ttu-id="fc7ca-126">Схема Types</span><span class="sxs-lookup"><span data-stu-id="fc7ca-126">Types schema</span></span>  <br/> |
|<span data-ttu-id="fc7ca-127">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="fc7ca-127">Validation File</span></span>  <br/> |<span data-ttu-id="fc7ca-128">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="fc7ca-128">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="fc7ca-129">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="fc7ca-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="fc7ca-130">False</span><span class="sxs-lookup"><span data-stu-id="fc7ca-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="fc7ca-131">См. также</span><span class="sxs-lookup"><span data-stu-id="fc7ca-131">See also</span></span>

- [<span data-ttu-id="fc7ca-132">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="fc7ca-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

