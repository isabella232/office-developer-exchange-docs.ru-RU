---
title: Правило (RuleType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Rule
api_type:
- schema
ms.assetid: 259a1f62-b235-4964-88bf-2d1f1c05a563
description: Элемент Rule содержит одно правило и представляет правило в почтовом ящике пользователя.
ms.openlocfilehash: b1f9f058213543633335db11f03729964baf98ad
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19835259"
---
# <a name="rule-ruletype"></a><span data-ttu-id="7b085-103">Правило (RuleType)</span><span class="sxs-lookup"><span data-stu-id="7b085-103">Rule (RuleType)</span></span>

<span data-ttu-id="7b085-104">Элемент **Rule** содержит одно правило и представляет правило в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="7b085-104">The **Rule** element contains a single rule and represents a rule in a user's mailbox.</span></span> 
  
```XML
<Rule>
    <RuleId>
    <DisplayName>
    <Priority>
    <IsEnabled>
    <IsNotSupported>
    <IsInError>
    <Conditions>
    <Exceptions>
    <Actions>
</Rule>
```

 <span data-ttu-id="7b085-105">**RuleType**</span><span class="sxs-lookup"><span data-stu-id="7b085-105">**RuleType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7b085-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="7b085-106">Attributes and elements</span></span>

<span data-ttu-id="7b085-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="7b085-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7b085-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="7b085-108">Attributes</span></span>

<span data-ttu-id="7b085-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="7b085-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7b085-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="7b085-110">Child elements</span></span>

|<span data-ttu-id="7b085-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="7b085-111">**Element**</span></span>|<span data-ttu-id="7b085-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="7b085-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7b085-113">RuleId</span><span class="sxs-lookup"><span data-stu-id="7b085-113">RuleId</span></span>](ruleid.md) <br/> |<span data-ttu-id="7b085-114">Указывает идентификатор правила.</span><span class="sxs-lookup"><span data-stu-id="7b085-114">Specifies the rule identifier.</span></span>  <br/> |
|[<span data-ttu-id="7b085-115">Отображаемое имя (строка)</span><span class="sxs-lookup"><span data-stu-id="7b085-115">DisplayName (string)</span></span>](displayname-string.md) <br/> |<span data-ttu-id="7b085-116">Содержит отображаемое имя правила.</span><span class="sxs-lookup"><span data-stu-id="7b085-116">Contains the display name of a rule.</span></span>  <br/> |
|[<span data-ttu-id="7b085-117">Приоритет</span><span class="sxs-lookup"><span data-stu-id="7b085-117">Priority</span></span>](priority.md) <br/> |<span data-ttu-id="7b085-118">Указывает порядок, в котором будет выполняться правило.</span><span class="sxs-lookup"><span data-stu-id="7b085-118">Indicates the order in which a rule is to be run.</span></span>  <br/> |
|[<span data-ttu-id="7b085-119">Свойства IsEnabled</span><span class="sxs-lookup"><span data-stu-id="7b085-119">IsEnabled</span></span>](isenabled.md) <br/> |<span data-ttu-id="7b085-120">Указывает, включена ли правило.</span><span class="sxs-lookup"><span data-stu-id="7b085-120">Indicates whether the rule is enabled.</span></span>  <br/> |
|[<span data-ttu-id="7b085-121">IsNotSupported</span><span class="sxs-lookup"><span data-stu-id="7b085-121">IsNotSupported</span></span>](isnotsupported.md) <br/> |<span data-ttu-id="7b085-122">Указывает ли правило не могут быть изменены с управляемым кодом API-интерфейсы.</span><span class="sxs-lookup"><span data-stu-id="7b085-122">Indicates whether the rule cannot be modified with the managed code APIs.</span></span>  <br/> |
|[<span data-ttu-id="7b085-123">IsInError</span><span class="sxs-lookup"><span data-stu-id="7b085-123">IsInError</span></span>](isinerror.md) <br/> |<span data-ttu-id="7b085-124">Указывает, является ли правило ошибкой.</span><span class="sxs-lookup"><span data-stu-id="7b085-124">Indicates whether the rule is in an error condition.</span></span>  <br/> |
|[<span data-ttu-id="7b085-125">Условия</span><span class="sxs-lookup"><span data-stu-id="7b085-125">Conditions</span></span>](conditions.md) <br/> |<span data-ttu-id="7b085-126">Определяет условия, если выполнены, запустит действия правил для правила.</span><span class="sxs-lookup"><span data-stu-id="7b085-126">Identifies the conditions that, when fulfilled, will trigger the rule actions for a rule.</span></span>  <br/> |
|[<span data-ttu-id="7b085-127">Исключения</span><span class="sxs-lookup"><span data-stu-id="7b085-127">Exceptions</span></span>](exceptions.md) <br/> |<span data-ttu-id="7b085-128">Определяет исключения, которые представляют все доступные правила условия исключений для правила папки «Входящие».</span><span class="sxs-lookup"><span data-stu-id="7b085-128">Identifies the exceptions that represent all the available rule exception conditions for the inbox rule.</span></span>  <br/> |
|[<span data-ttu-id="7b085-129">Действия</span><span class="sxs-lookup"><span data-stu-id="7b085-129">Actions</span></span>](actions.md) <br/> |<span data-ttu-id="7b085-130">Представляет действия, которые необходимо выполнить на сообщение, если будут выполнены условия.</span><span class="sxs-lookup"><span data-stu-id="7b085-130">Represents the actions to be taken on a message when the conditions are fulfilled.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="7b085-131">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="7b085-131">Parent elements</span></span>

|<span data-ttu-id="7b085-132">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="7b085-132">**Element**</span></span>|<span data-ttu-id="7b085-133">**Описание**</span><span class="sxs-lookup"><span data-stu-id="7b085-133">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7b085-134">CreateRuleOperation</span><span class="sxs-lookup"><span data-stu-id="7b085-134">CreateRuleOperation</span></span>](createruleoperation.md) <br/> |<span data-ttu-id="7b085-135">Представляет операцию, чтобы создать новое правило.</span><span class="sxs-lookup"><span data-stu-id="7b085-135">Represents an operation to create a new rule.</span></span>  <br/> |
|[<span data-ttu-id="7b085-136">InboxRules</span><span class="sxs-lookup"><span data-stu-id="7b085-136">InboxRules</span></span>](inboxrules.md) <br/> |<span data-ttu-id="7b085-137">Представляет собой массив из правил в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="7b085-137">Represents an array of rules in the user's mailbox.</span></span>  <br/> |
|[<span data-ttu-id="7b085-138">SetRuleOperation</span><span class="sxs-lookup"><span data-stu-id="7b085-138">SetRuleOperation</span></span>](setruleoperation.md) <br/> |<span data-ttu-id="7b085-139">Представляет операцию для обновления существующего правила.</span><span class="sxs-lookup"><span data-stu-id="7b085-139">Represents an operation to update an existing rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="7b085-140">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="7b085-140">Text value</span></span>

<span data-ttu-id="7b085-141">Нет.</span><span class="sxs-lookup"><span data-stu-id="7b085-141">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="7b085-142">Замечания</span><span class="sxs-lookup"><span data-stu-id="7b085-142">Remarks</span></span>

<span data-ttu-id="7b085-143">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="7b085-143">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7b085-144">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="7b085-144">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7b085-145">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="7b085-145">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="7b085-146">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="7b085-146">Schema Name</span></span>  <br/> |<span data-ttu-id="7b085-147">Схема Types</span><span class="sxs-lookup"><span data-stu-id="7b085-147">Types schema</span></span>  <br/> |
|<span data-ttu-id="7b085-148">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="7b085-148">Validation File</span></span>  <br/> |<span data-ttu-id="7b085-149">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="7b085-149">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="7b085-150">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="7b085-150">Can be Empty</span></span>  <br/> |<span data-ttu-id="7b085-151">True</span><span class="sxs-lookup"><span data-stu-id="7b085-151">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7b085-152">См. также</span><span class="sxs-lookup"><span data-stu-id="7b085-152">See also</span></span>



[<span data-ttu-id="7b085-153">UpdateInboxRules</span><span class="sxs-lookup"><span data-stu-id="7b085-153">UpdateInboxRules</span></span>](updateinboxrules.md)
  
[<span data-ttu-id="7b085-154">SetRuleOperation</span><span class="sxs-lookup"><span data-stu-id="7b085-154">SetRuleOperation</span></span>](setruleoperation.md)
  
[<span data-ttu-id="7b085-155">CreateRuleOperation</span><span class="sxs-lookup"><span data-stu-id="7b085-155">CreateRuleOperation</span></span>](createruleoperation.md)


- [<span data-ttu-id="7b085-156">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="7b085-156">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

