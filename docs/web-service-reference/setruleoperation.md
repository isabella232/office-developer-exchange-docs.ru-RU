---
title: SetRuleOperation
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SetRuleOperation
api_type:
- schema
ms.assetid: 2106a85b-58fe-49be-b71d-4ca6aa66e060
description: Элемент SetRuleOperation представляет операцию для обновления существующего правила.
ms.openlocfilehash: 9c956394d14c510e8dcc95110ef1874ea7010be0
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19835451"
---
# <a name="setruleoperation"></a><span data-ttu-id="fa502-103">SetRuleOperation</span><span class="sxs-lookup"><span data-stu-id="fa502-103">SetRuleOperation</span></span>

<span data-ttu-id="fa502-104">Элемент **SetRuleOperation** представляет операцию для обновления существующего правила.</span><span class="sxs-lookup"><span data-stu-id="fa502-104">The **SetRuleOperation** element represents an operation to update an existing rule.</span></span> 
  
[<span data-ttu-id="fa502-105">UpdateInboxRules</span><span class="sxs-lookup"><span data-stu-id="fa502-105">UpdateInboxRules</span></span>](updateinboxrules.md)
  
[<span data-ttu-id="fa502-106">Операции</span><span class="sxs-lookup"><span data-stu-id="fa502-106">Operations</span></span>](operations.md)
  
```XML
<SetRuleOperation>
    <Rule/>
</SetRuleOperation>
```

 <span data-ttu-id="fa502-107">**SetRuleOperationType**</span><span class="sxs-lookup"><span data-stu-id="fa502-107">**SetRuleOperationType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="fa502-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="fa502-108">Attributes and elements</span></span>

<span data-ttu-id="fa502-109">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="fa502-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="fa502-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="fa502-110">Attributes</span></span>

<span data-ttu-id="fa502-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="fa502-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="fa502-112">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="fa502-112">Child elements</span></span>

|<span data-ttu-id="fa502-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="fa502-113">**Element**</span></span>|<span data-ttu-id="fa502-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="fa502-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fa502-115">Правило (RuleType)</span><span class="sxs-lookup"><span data-stu-id="fa502-115">Rule (RuleType)</span></span>](rule-ruletype.md) <br/> |<span data-ttu-id="fa502-116">Представляет правило в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="fa502-116">Represents a rule in a user's mailbox.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="fa502-117">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="fa502-117">Parent elements</span></span>

|<span data-ttu-id="fa502-118">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="fa502-118">**Element**</span></span>|<span data-ttu-id="fa502-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="fa502-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fa502-120">Операции</span><span class="sxs-lookup"><span data-stu-id="fa502-120">Operations</span></span>](operations.md) <br/> |<span data-ttu-id="fa502-121">Содержит набор операций правила, которые могут выполняться в папке "Входящие".</span><span class="sxs-lookup"><span data-stu-id="fa502-121">Contains an array of rule operations that can be performed on an Inbox.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="fa502-122">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="fa502-122">Text value</span></span>

<span data-ttu-id="fa502-123">Нет.</span><span class="sxs-lookup"><span data-stu-id="fa502-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="fa502-124">Замечания</span><span class="sxs-lookup"><span data-stu-id="fa502-124">Remarks</span></span>

<span data-ttu-id="fa502-125">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="fa502-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="fa502-126">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="fa502-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="fa502-127">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="fa502-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="fa502-128">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="fa502-128">Schema Name</span></span>  <br/> |<span data-ttu-id="fa502-129">Схема Types</span><span class="sxs-lookup"><span data-stu-id="fa502-129">Types schema</span></span>  <br/> |
|<span data-ttu-id="fa502-130">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="fa502-130">Validation File</span></span>  <br/> |<span data-ttu-id="fa502-131">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="fa502-131">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="fa502-132">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="fa502-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="fa502-133">False</span><span class="sxs-lookup"><span data-stu-id="fa502-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="fa502-134">См. также</span><span class="sxs-lookup"><span data-stu-id="fa502-134">See also</span></span>



[<span data-ttu-id="fa502-135">UpdateInboxRules</span><span class="sxs-lookup"><span data-stu-id="fa502-135">UpdateInboxRules</span></span>](updateinboxrules.md)
  
[<span data-ttu-id="fa502-136">DeleteRuleOperation</span><span class="sxs-lookup"><span data-stu-id="fa502-136">DeleteRuleOperation</span></span>](deleteruleoperation.md)
  
[<span data-ttu-id="fa502-137">CreateRuleOperation</span><span class="sxs-lookup"><span data-stu-id="fa502-137">CreateRuleOperation</span></span>](createruleoperation.md)


- [<span data-ttu-id="fa502-138">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="fa502-138">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

