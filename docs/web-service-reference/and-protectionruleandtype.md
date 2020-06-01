---
title: И (Протектионрулеандтипе)
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
description: Элемент и указывает, что все дочерние элементы должны сопоставляться со значением true.
ms.openlocfilehash: ba898ccd77518971afaf713d1c7c7955f46465d5
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44464737"
---
# <a name="and-protectionruleandtype"></a><span data-ttu-id="36edc-103">И (Протектионрулеандтипе)</span><span class="sxs-lookup"><span data-stu-id="36edc-103">And (ProtectionRuleAndType)</span></span>

<span data-ttu-id="36edc-104">Элемент **и** указывает, что все дочерние элементы должны сопоставляться со значением **true**.</span><span class="sxs-lookup"><span data-stu-id="36edc-104">The **And** element specifies that all child elements must match to evaluate to **true**.</span></span>
  
```xml
<And>
   <AllInternal/>
   <And/>
   <RecipientIs/>
   <SenderDepartments/>
   <True/>
</And>
```

 <span data-ttu-id="36edc-105">**протектионрулеандтипе**</span><span class="sxs-lookup"><span data-stu-id="36edc-105">**ProtectionRuleAndType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="36edc-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="36edc-106">Attributes and elements</span></span>

<span data-ttu-id="36edc-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="36edc-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="36edc-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="36edc-108">Attributes</span></span>

<span data-ttu-id="36edc-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="36edc-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="36edc-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="36edc-110">Child elements</span></span>

|<span data-ttu-id="36edc-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="36edc-111">**Element**</span></span>|<span data-ttu-id="36edc-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="36edc-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="36edc-113">аллинтернал</span><span class="sxs-lookup"><span data-stu-id="36edc-113">AllInternal</span></span>](allinternal.md) <br/> |<span data-ttu-id="36edc-114">Возвращает **значение true** , если все получатели сообщения электронной почты являются внутренними для организации отправителя.</span><span class="sxs-lookup"><span data-stu-id="36edc-114">Evaluates to **true** if all recipients of an e-mail message are internal to the sender's organization.</span></span>  <br/> |
|<span data-ttu-id="36edc-115">**And**</span><span class="sxs-lookup"><span data-stu-id="36edc-115">**And**</span></span> <br/> |<span data-ttu-id="36edc-116">Указывает, что все дочерние элементы должны сопоставляться со значением **true**.</span><span class="sxs-lookup"><span data-stu-id="36edc-116">Specifies that all child elements must match to evaluate to **true**.</span></span>  <br/> |
|[<span data-ttu-id="36edc-117">Получательявляется</span><span class="sxs-lookup"><span data-stu-id="36edc-117">RecipientIs</span></span>](recipientis.md) <br/> |<span data-ttu-id="36edc-118">Указывает, что любой получатель сообщения электронной почты соответствует любому из указанных получателей в дочерних элементах [value (протектионрулевалуетипе)](value-protectionrulevaluetype.md) .</span><span class="sxs-lookup"><span data-stu-id="36edc-118">Specifies that any recipient of the e-mail message matches any of the specified recipients in the child [Value (ProtectionRuleValueType)](value-protectionrulevaluetype.md) elements.</span></span>  <br/> |
|[<span data-ttu-id="36edc-119">сендердепартментс</span><span class="sxs-lookup"><span data-stu-id="36edc-119">SenderDepartments</span></span>](senderdepartments.md) <br/> |<span data-ttu-id="36edc-120">Указывает, что отдел отправителя соответствует любой из указанных отделов в дочерних элементах [value (протектионрулевалуетипе)](value-protectionrulevaluetype.md) .</span><span class="sxs-lookup"><span data-stu-id="36edc-120">Specifies that the department of the sender matches any of the specified departments in the child [Value (ProtectionRuleValueType)](value-protectionrulevaluetype.md) elements.</span></span>  <br/> |
|[<span data-ttu-id="36edc-121">True</span><span class="sxs-lookup"><span data-stu-id="36edc-121">True</span></span>](true.md) <br/> |<span data-ttu-id="36edc-122">Задает условие, которое всегда соответствует.</span><span class="sxs-lookup"><span data-stu-id="36edc-122">Specifies a condition that always matches.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="36edc-123">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="36edc-123">Parent elements</span></span>

|<span data-ttu-id="36edc-124">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="36edc-124">**Element**</span></span>|<span data-ttu-id="36edc-125">**Описание**</span><span class="sxs-lookup"><span data-stu-id="36edc-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="36edc-126">Условие</span><span class="sxs-lookup"><span data-stu-id="36edc-126">Condition</span></span>](condition.md) <br/> |<span data-ttu-id="36edc-127">Определяет условие, которое должно быть удовлетворено для части действия правила, которое необходимо выполнить.</span><span class="sxs-lookup"><span data-stu-id="36edc-127">Identifies the condition that must be satisfied for the action part of the rule to be executed.</span></span>  <br/> |
|<span data-ttu-id="36edc-128">**And**</span><span class="sxs-lookup"><span data-stu-id="36edc-128">**And**</span></span> <br/> |<span data-ttu-id="36edc-129">Указывает, что все дочерние элементы должны сопоставляться со значением **true**.</span><span class="sxs-lookup"><span data-stu-id="36edc-129">Specifies that all child elements must match to evaluate to **true**.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="36edc-130">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="36edc-130">Text value</span></span>

<span data-ttu-id="36edc-131">Нет.</span><span class="sxs-lookup"><span data-stu-id="36edc-131">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="36edc-132">Примечания</span><span class="sxs-lookup"><span data-stu-id="36edc-132">Remarks</span></span>

<span data-ttu-id="36edc-133">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="36edc-133">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="36edc-134">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="36edc-134">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="36edc-135">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="36edc-135">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="36edc-136">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="36edc-136">Schema Name</span></span>  <br/> |<span data-ttu-id="36edc-137">Схема Types</span><span class="sxs-lookup"><span data-stu-id="36edc-137">Types schema</span></span>  <br/> |
|<span data-ttu-id="36edc-138">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="36edc-138">Validation File</span></span>  <br/> |<span data-ttu-id="36edc-139">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="36edc-139">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="36edc-140">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="36edc-140">Can be Empty</span></span>  <br/> |<span data-ttu-id="36edc-141">False</span><span class="sxs-lookup"><span data-stu-id="36edc-141">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="36edc-142">См. также</span><span class="sxs-lookup"><span data-stu-id="36edc-142">See also</span></span>

- [<span data-ttu-id="36edc-143">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="36edc-143">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

