---
title: сендердепартментс
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
description: Элемент Сендердепартментс указывает, что отдел отправителя соответствует любой из указанных отделов в дочерних элементах value (Протектионрулевалуетипе).
ms.openlocfilehash: cf15b974b9c0cfb09767661f17334defc4041e43
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530347"
---
# <a name="senderdepartments"></a><span data-ttu-id="64a94-103">сендердепартментс</span><span class="sxs-lookup"><span data-stu-id="64a94-103">SenderDepartments</span></span>

<span data-ttu-id="64a94-104">Элемент **сендердепартментс** указывает, что отдел отправителя соответствует любой из указанных отделов в дочерних элементах [value (протектионрулевалуетипе)](value-protectionrulevaluetype.md) .</span><span class="sxs-lookup"><span data-stu-id="64a94-104">The **SenderDepartments** element specifies that the department of the sender matches any of the specified departments in the child [Value (ProtectionRuleValueType)](value-protectionrulevaluetype.md) elements.</span></span> 
  
```XML
<SenderDepartments>
   <Value/>
</SenderDepartments>
```

 <span data-ttu-id="64a94-105">**протектионрулесендердепартментстипе**</span><span class="sxs-lookup"><span data-stu-id="64a94-105">**ProtectionRuleSenderDepartmentsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="64a94-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="64a94-106">Attributes and elements</span></span>

<span data-ttu-id="64a94-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="64a94-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="64a94-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="64a94-108">Attributes</span></span>

<span data-ttu-id="64a94-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="64a94-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="64a94-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="64a94-110">Child elements</span></span>

|<span data-ttu-id="64a94-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="64a94-111">**Element**</span></span>|<span data-ttu-id="64a94-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="64a94-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="64a94-113">Значение (Протектионрулевалуетипе)</span><span class="sxs-lookup"><span data-stu-id="64a94-113">Value (ProtectionRuleValueType)</span></span>](value-protectionrulevaluetype.md) <br/> |<span data-ttu-id="64a94-114">Определяет один отдел отправителя.</span><span class="sxs-lookup"><span data-stu-id="64a94-114">Identifies a single sender department.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="64a94-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="64a94-115">Parent elements</span></span>

|<span data-ttu-id="64a94-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="64a94-116">**Element**</span></span>|<span data-ttu-id="64a94-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="64a94-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="64a94-118">Условие</span><span class="sxs-lookup"><span data-stu-id="64a94-118">Condition</span></span>](condition.md) <br/> |<span data-ttu-id="64a94-119">Определяет условие, которое должно быть удовлетворено для части действия правила, которое необходимо выполнить.</span><span class="sxs-lookup"><span data-stu-id="64a94-119">Identifies the condition that must be satisfied for the action part of the rule to be executed.</span></span>  <br/> |
|[<span data-ttu-id="64a94-120">И (Протектионрулеандтипе)</span><span class="sxs-lookup"><span data-stu-id="64a94-120">And (ProtectionRuleAndType)</span></span>](and-protectionruleandtype.md) <br/> |<span data-ttu-id="64a94-121">Указывает, что все дочерние элементы должны сопоставляться со значением **true**.</span><span class="sxs-lookup"><span data-stu-id="64a94-121">Specifies that all child elements must match to evaluate to **true**.</span></span> <span data-ttu-id="64a94-122">Указывает, что должно быть больше одного дочернего условия правила защиты.</span><span class="sxs-lookup"><span data-stu-id="64a94-122">Specifies that there must be more than one protection rule child condition.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="64a94-123">Примечания</span><span class="sxs-lookup"><span data-stu-id="64a94-123">Remarks</span></span>

<span data-ttu-id="64a94-124">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="64a94-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="64a94-125">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="64a94-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="64a94-126">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="64a94-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="64a94-127">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="64a94-127">Schema Name</span></span>  <br/> |<span data-ttu-id="64a94-128">Схема Types</span><span class="sxs-lookup"><span data-stu-id="64a94-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="64a94-129">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="64a94-129">Validation File</span></span>  <br/> |<span data-ttu-id="64a94-130">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="64a94-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="64a94-131">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="64a94-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="64a94-132">False</span><span class="sxs-lookup"><span data-stu-id="64a94-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="64a94-133">См. также</span><span class="sxs-lookup"><span data-stu-id="64a94-133">See also</span></span>



- [<span data-ttu-id="64a94-134">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="64a94-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

