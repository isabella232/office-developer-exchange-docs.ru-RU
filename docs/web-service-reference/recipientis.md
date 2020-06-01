---
title: Получательявляется
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
description: Элемент Recipient указывает на то, что любой получатель сообщения электронной почты соответствует любому из указанных получателей в дочерних элементах value (Протектионрулевалуетипе).
ms.openlocfilehash: 8f27c4484ce310c62f9bab0e6ffeea2bfac1d3ef
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463883"
---
# <a name="recipientis"></a><span data-ttu-id="7d154-103">Получательявляется</span><span class="sxs-lookup"><span data-stu-id="7d154-103">RecipientIs</span></span>

<span data-ttu-id="7d154-104">Элемент **Recipient** указывает на то, что любой получатель сообщения электронной почты соответствует любому из указанных получателей в дочерних элементах [value (протектионрулевалуетипе)](value-protectionrulevaluetype.md) .</span><span class="sxs-lookup"><span data-stu-id="7d154-104">The **RecipientIs** element specifies that any recipient of the e-mail message matches any of the specified recipients in the child [Value (ProtectionRuleValueType)](value-protectionrulevaluetype.md) elements.</span></span> 
  
```xml
<RecipientIs>   <Value/></RecipientIs>
```

 <span data-ttu-id="7d154-105">**протектионрулереЦипиентистипе**</span><span class="sxs-lookup"><span data-stu-id="7d154-105">**ProtectionRuleRecipientIsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7d154-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="7d154-106">Attributes and elements</span></span>

<span data-ttu-id="7d154-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="7d154-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7d154-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="7d154-108">Attributes</span></span>

<span data-ttu-id="7d154-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="7d154-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7d154-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="7d154-110">Child elements</span></span>

|<span data-ttu-id="7d154-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="7d154-111">**Element**</span></span>|<span data-ttu-id="7d154-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="7d154-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7d154-113">Значение (Протектионрулевалуетипе)</span><span class="sxs-lookup"><span data-stu-id="7d154-113">Value (ProtectionRuleValueType)</span></span>](value-protectionrulevaluetype.md) <br/> |<span data-ttu-id="7d154-114">Идентифицирует получателя.</span><span class="sxs-lookup"><span data-stu-id="7d154-114">Identifies a recipient.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="7d154-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="7d154-115">Parent elements</span></span>

|<span data-ttu-id="7d154-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="7d154-116">**Element**</span></span>|<span data-ttu-id="7d154-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="7d154-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7d154-118">Условие</span><span class="sxs-lookup"><span data-stu-id="7d154-118">Condition</span></span>](condition.md) <br/> |<span data-ttu-id="7d154-119">Определяет условие, которое должно быть удовлетворено для части действия правила, которое необходимо выполнить.</span><span class="sxs-lookup"><span data-stu-id="7d154-119">Identifies the condition that must be satisfied for the action part of the rule to be executed.</span></span>  <br/> |
|[<span data-ttu-id="7d154-120">И (Протектионрулеандтипе)</span><span class="sxs-lookup"><span data-stu-id="7d154-120">And (ProtectionRuleAndType)</span></span>](and-protectionruleandtype.md) <br/> |<span data-ttu-id="7d154-121">Указывает, что все дочерние элементы должны сопоставляться со значением **true**.</span><span class="sxs-lookup"><span data-stu-id="7d154-121">Indicates that all child elements must match to evaluate to **true**.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="7d154-122">Примечания</span><span class="sxs-lookup"><span data-stu-id="7d154-122">Remarks</span></span>

<span data-ttu-id="7d154-123">Схема, описывающая этот элемент, находится в виртуальном каталоге EWS компьютера под управлением Microsoft Exchange Server 2010, на котором установлена роль сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="7d154-123">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7d154-124">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="7d154-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7d154-125">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="7d154-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="7d154-126">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="7d154-126">Schema Name</span></span>  <br/> |<span data-ttu-id="7d154-127">Схема Types</span><span class="sxs-lookup"><span data-stu-id="7d154-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="7d154-128">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="7d154-128">Validation File</span></span>  <br/> |<span data-ttu-id="7d154-129">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="7d154-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="7d154-130">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="7d154-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="7d154-131">False</span><span class="sxs-lookup"><span data-stu-id="7d154-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7d154-132">См. также</span><span class="sxs-lookup"><span data-stu-id="7d154-132">See also</span></span>



- [<span data-ttu-id="7d154-133">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="7d154-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

