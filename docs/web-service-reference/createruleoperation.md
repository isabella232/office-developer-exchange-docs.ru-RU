---
title: CreateRuleOperation
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CreateRuleOperation
api_type:
- schema
ms.assetid: e9f70726-db08-4089-839e-a41007d0a473
description: Элемент CreateRuleOperation представляет операцию для создания нового правила папки «Входящие».
ms.openlocfilehash: c531f222ffe886e6ef53a99609cfa27e84fd6107
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761912"
---
# <a name="createruleoperation"></a><span data-ttu-id="36496-103">CreateRuleOperation</span><span class="sxs-lookup"><span data-stu-id="36496-103">CreateRuleOperation</span></span>

<span data-ttu-id="36496-104">Элемент **CreateRuleOperation** представляет операцию для создания нового правила папки «Входящие».</span><span class="sxs-lookup"><span data-stu-id="36496-104">The **CreateRuleOperation** element represents an operation to create a new Inbox rule.</span></span> 
  
[<span data-ttu-id="36496-105">UpdateInboxRules</span><span class="sxs-lookup"><span data-stu-id="36496-105">UpdateInboxRules</span></span>](updateinboxrules.md)
  
[<span data-ttu-id="36496-106">Операции</span><span class="sxs-lookup"><span data-stu-id="36496-106">Operations</span></span>](operations.md)
  
```xml
<CreateRuleOperation>
    <Rule/>
</CreateRuleOperation>
```

 <span data-ttu-id="36496-107">**CreateRuleOperationType**</span><span class="sxs-lookup"><span data-stu-id="36496-107">**CreateRuleOperationType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="36496-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="36496-108">Attributes and elements</span></span>

<span data-ttu-id="36496-109">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="36496-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="36496-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="36496-110">Attributes</span></span>

<span data-ttu-id="36496-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="36496-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="36496-112">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="36496-112">Child elements</span></span>

|<span data-ttu-id="36496-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="36496-113">**Element**</span></span>|<span data-ttu-id="36496-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="36496-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="36496-115">Правило (RuleType)</span><span class="sxs-lookup"><span data-stu-id="36496-115">Rule (RuleType)</span></span>](rule-ruletype.md) <br/> |<span data-ttu-id="36496-116">Представляет правило будет создан в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="36496-116">Represents a rule to be created in a user's mailbox.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="36496-117">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="36496-117">Parent elements</span></span>

|<span data-ttu-id="36496-118">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="36496-118">**Element**</span></span>|<span data-ttu-id="36496-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="36496-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="36496-120">Операции</span><span class="sxs-lookup"><span data-stu-id="36496-120">Operations</span></span>](operations.md) <br/> |<span data-ttu-id="36496-121">Содержит операции, которые могут быть выполнены в папке "Входящие".</span><span class="sxs-lookup"><span data-stu-id="36496-121">Contains the operations that can be performed on an Inbox.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="36496-122">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="36496-122">Text value</span></span>

<span data-ttu-id="36496-123">Нет.</span><span class="sxs-lookup"><span data-stu-id="36496-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="36496-124">Замечания</span><span class="sxs-lookup"><span data-stu-id="36496-124">Remarks</span></span>

<span data-ttu-id="36496-125">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="36496-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="36496-126">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="36496-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="36496-127">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="36496-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="36496-128">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="36496-128">Schema Name</span></span>  <br/> |<span data-ttu-id="36496-129">Схема Types</span><span class="sxs-lookup"><span data-stu-id="36496-129">Types schema</span></span>  <br/> |
|<span data-ttu-id="36496-130">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="36496-130">Validation File</span></span>  <br/> |<span data-ttu-id="36496-131">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="36496-131">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="36496-132">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="36496-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="36496-133">False</span><span class="sxs-lookup"><span data-stu-id="36496-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="36496-134">См. также</span><span class="sxs-lookup"><span data-stu-id="36496-134">See also</span></span>



[<span data-ttu-id="36496-135">UpdateInboxRules</span><span class="sxs-lookup"><span data-stu-id="36496-135">UpdateInboxRules</span></span>](updateinboxrules.md)
  
[<span data-ttu-id="36496-136">SetRuleOperation</span><span class="sxs-lookup"><span data-stu-id="36496-136">SetRuleOperation</span></span>](setruleoperation.md)
  
[<span data-ttu-id="36496-137">DeleteRuleOperation</span><span class="sxs-lookup"><span data-stu-id="36496-137">DeleteRuleOperation</span></span>](deleteruleoperation.md)


- [<span data-ttu-id="36496-138">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="36496-138">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

