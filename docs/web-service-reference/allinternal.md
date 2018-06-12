---
title: AllInternal
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AllInternal
api_type:
- schema
ms.assetid: b7e5072f-5d9f-4ee0-b58b-4d75d878ea1c
description: Элемент AllInternal принимает значение true, если всех получателей сообщения электронной почты являются внутренними относительно организации отправителя.
ms.openlocfilehash: 0ffd4178e711e3117497eed682e3fd3e0594989b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761368"
---
# <a name="allinternal"></a><span data-ttu-id="96457-103">AllInternal</span><span class="sxs-lookup"><span data-stu-id="96457-103">AllInternal</span></span>

<span data-ttu-id="96457-104">Элемент **AllInternal** имеет значение **true** , если все получатели сообщения электронной почты являются внутренними относительно организации отправителя.</span><span class="sxs-lookup"><span data-stu-id="96457-104">The **AllInternal** element evaluates to **true** if all recipients of an e-mail message are internal to the sender's organization.</span></span> 
  
```xml
<AllInternal/>
```

 <span data-ttu-id="96457-105">**ProtectionRuleAllInternalType**</span><span class="sxs-lookup"><span data-stu-id="96457-105">**ProtectionRuleAllInternalType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="96457-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="96457-106">Attributes and elements</span></span>

<span data-ttu-id="96457-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="96457-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="96457-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="96457-108">Attributes</span></span>

<span data-ttu-id="96457-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="96457-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="96457-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="96457-110">Child elements</span></span>

<span data-ttu-id="96457-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="96457-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="96457-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="96457-112">Parent elements</span></span>

|<span data-ttu-id="96457-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="96457-113">**Element**</span></span>|<span data-ttu-id="96457-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="96457-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="96457-115">Условие</span><span class="sxs-lookup"><span data-stu-id="96457-115">Condition</span></span>](condition.md) <br/> |<span data-ttu-id="96457-116">Определяет условие, которое должно выполняться для части действия правила для выполнения.</span><span class="sxs-lookup"><span data-stu-id="96457-116">Identifies the condition that must be satisfied for the action part of the rule to be executed.</span></span>  <br/> |
|[<span data-ttu-id="96457-117">И (ProtectionRuleAndType)</span><span class="sxs-lookup"><span data-stu-id="96457-117">And (ProtectionRuleAndType)</span></span>](and-protectionruleandtype.md) <br/> |<span data-ttu-id="96457-118">Указывает, что все дочерние элементы должны соответствовать значение **true**.</span><span class="sxs-lookup"><span data-stu-id="96457-118">Specifies that all child elements must match to evaluate to **true**.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="96457-119">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="96457-119">Text value</span></span>

<span data-ttu-id="96457-120">Элемент **AllInternal** должен быть пустым.</span><span class="sxs-lookup"><span data-stu-id="96457-120">The **AllInternal** element must be empty.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="96457-121">Замечания</span><span class="sxs-lookup"><span data-stu-id="96457-121">Remarks</span></span>

<span data-ttu-id="96457-122">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="96457-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="96457-123">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="96457-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="96457-124">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="96457-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="96457-125">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="96457-125">Schema Name</span></span>  <br/> |<span data-ttu-id="96457-126">Схема Types</span><span class="sxs-lookup"><span data-stu-id="96457-126">Types schema</span></span>  <br/> |
|<span data-ttu-id="96457-127">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="96457-127">Validation File</span></span>  <br/> |<span data-ttu-id="96457-128">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="96457-128">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="96457-129">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="96457-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="96457-130">False</span><span class="sxs-lookup"><span data-stu-id="96457-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="96457-131">См. также</span><span class="sxs-lookup"><span data-stu-id="96457-131">See also</span></span>

- [<span data-ttu-id="96457-132">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="96457-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

