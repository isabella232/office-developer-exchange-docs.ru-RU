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
description: Элемент Condition определяет условие, которое должно быть удовлетворено для части действия правила, которое необходимо выполнить.
ms.openlocfilehash: d49f2984799b15c0499af59abecbb34abe15f7c3
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/28/2018
ms.locfileid: "21353562"
---
# <a name="condition"></a><span data-ttu-id="f876f-103">Условие</span><span class="sxs-lookup"><span data-stu-id="f876f-103">Condition</span></span>

<span data-ttu-id="f876f-104">Элемент **Condition** определяет условие, которое должно быть удовлетворено для части действия правила, которое необходимо выполнить.</span><span class="sxs-lookup"><span data-stu-id="f876f-104">The **Condition** element identifies the condition that must be satisfied for the action part of the rule to be executed.</span></span> 
  
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

<span data-ttu-id="f876f-105">**протектионрулекондитионтипе**</span><span class="sxs-lookup"><span data-stu-id="f876f-105">**ProtectionRuleConditionType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="f876f-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="f876f-106">Attributes and elements</span></span>

<span data-ttu-id="f876f-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="f876f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f876f-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="f876f-108">Attributes</span></span>

<span data-ttu-id="f876f-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="f876f-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f876f-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="f876f-110">Child elements</span></span>

|<span data-ttu-id="f876f-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="f876f-111">**Element**</span></span>|<span data-ttu-id="f876f-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="f876f-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f876f-113">аллинтернал</span><span class="sxs-lookup"><span data-stu-id="f876f-113">AllInternal</span></span>](allinternal.md) <br/> |<span data-ttu-id="f876f-114">Возвращает **значение true** , если все получатели сообщения электронной почты являются внутренними для организации отправителя.</span><span class="sxs-lookup"><span data-stu-id="f876f-114">Evaluates to **true** if all recipients of an e-mail message are internal to the sender's organization.</span></span>  <br/> |
|[<span data-ttu-id="f876f-115">И (Протектионрулеандтипе)</span><span class="sxs-lookup"><span data-stu-id="f876f-115">And (ProtectionRuleAndType)</span></span>](and-protectionruleandtype.md) <br/> |<span data-ttu-id="f876f-116">Указывает, что все дочерние элементы должны сопоставляться со значением **true**.</span><span class="sxs-lookup"><span data-stu-id="f876f-116">Specifies that all child elements must match to evaluate to **true**.</span></span> <span data-ttu-id="f876f-117">Указывает, что должно быть больше одного дочернего условия правила защиты.</span><span class="sxs-lookup"><span data-stu-id="f876f-117">Specifies that there must be more than one protection rule child condition.</span></span>  <br/> |
|[<span data-ttu-id="f876f-118">Получательявляется</span><span class="sxs-lookup"><span data-stu-id="f876f-118">RecipientIs</span></span>](recipientis.md) <br/> |<span data-ttu-id="f876f-119">Указывает, что любой получатель сообщения электронной почты соответствует любому из указанных получателей в дочерних элементах [value (протектионрулевалуетипе)](value-protectionrulevaluetype.md) .</span><span class="sxs-lookup"><span data-stu-id="f876f-119">Specifies that any recipient of the e-mail message matches any of the specified recipients in the child [Value (ProtectionRuleValueType)](value-protectionrulevaluetype.md) elements.</span></span>  <br/> |
|[<span data-ttu-id="f876f-120">сендердепартментс</span><span class="sxs-lookup"><span data-stu-id="f876f-120">SenderDepartments</span></span>](senderdepartments.md) <br/> |<span data-ttu-id="f876f-121">Указывает, что отдел отправителя соответствует любой из указанных отделов в дочерних элементах [value (протектионрулевалуетипе)](value-protectionrulevaluetype.md) .</span><span class="sxs-lookup"><span data-stu-id="f876f-121">Specifies that the department of the sender matches any of the specified departments in the child [Value (ProtectionRuleValueType)](value-protectionrulevaluetype.md) elements.</span></span>  <br/> |
|[<span data-ttu-id="f876f-122">True</span><span class="sxs-lookup"><span data-stu-id="f876f-122">True</span></span>](true.md) <br/> |<span data-ttu-id="f876f-123">Задает условие, которое всегда соответствует.</span><span class="sxs-lookup"><span data-stu-id="f876f-123">Specifies a condition that always matches.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f876f-124">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="f876f-124">Parent elements</span></span>

|<span data-ttu-id="f876f-125">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="f876f-125">**Element**</span></span>|<span data-ttu-id="f876f-126">**Описание**</span><span class="sxs-lookup"><span data-stu-id="f876f-126">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f876f-127">Rule</span><span class="sxs-lookup"><span data-stu-id="f876f-127">Rule</span></span>](rule.md) <br/> |<span data-ttu-id="f876f-128">Содержит одно правило защиты.</span><span class="sxs-lookup"><span data-stu-id="f876f-128">Contains a single protection rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="f876f-129">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="f876f-129">Text value</span></span>

<span data-ttu-id="f876f-130">Нет.</span><span class="sxs-lookup"><span data-stu-id="f876f-130">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="f876f-131">Примечания</span><span class="sxs-lookup"><span data-stu-id="f876f-131">Remarks</span></span>

<span data-ttu-id="f876f-132">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="f876f-132">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f876f-133">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="f876f-133">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f876f-134">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="f876f-134">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="f876f-135">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="f876f-135">Schema Name</span></span>  <br/> |<span data-ttu-id="f876f-136">Схема Types</span><span class="sxs-lookup"><span data-stu-id="f876f-136">Types schema</span></span>  <br/> |
|<span data-ttu-id="f876f-137">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="f876f-137">Validation File</span></span>  <br/> |<span data-ttu-id="f876f-138">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="f876f-138">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="f876f-139">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="f876f-139">Can be Empty</span></span>  <br/> |<span data-ttu-id="f876f-140">False</span><span class="sxs-lookup"><span data-stu-id="f876f-140">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f876f-141">См. также</span><span class="sxs-lookup"><span data-stu-id="f876f-141">See also</span></span>

- [<span data-ttu-id="f876f-142">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="f876f-142">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

