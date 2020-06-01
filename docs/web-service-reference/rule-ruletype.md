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
ms.openlocfilehash: cdbd21df235a62a9e201e1eaae1d82a8ac10cdd2
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/01/2020
ms.locfileid: "44465081"
---
# <a name="rule-ruletype"></a><span data-ttu-id="6e945-103">Правило (RuleType)</span><span class="sxs-lookup"><span data-stu-id="6e945-103">Rule (RuleType)</span></span>

<span data-ttu-id="6e945-104">Элемент **rule** содержит одно правило и представляет правило в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="6e945-104">The **Rule** element contains a single rule and represents a rule in a user's mailbox.</span></span> 
  
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

 <span data-ttu-id="6e945-105">**RuleType**</span><span class="sxs-lookup"><span data-stu-id="6e945-105">**RuleType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6e945-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="6e945-106">Attributes and elements</span></span>

<span data-ttu-id="6e945-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="6e945-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6e945-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="6e945-108">Attributes</span></span>

<span data-ttu-id="6e945-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="6e945-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6e945-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="6e945-110">Child elements</span></span>

|<span data-ttu-id="6e945-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="6e945-111">**Element**</span></span>|<span data-ttu-id="6e945-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="6e945-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6e945-113">RuleId</span><span class="sxs-lookup"><span data-stu-id="6e945-113">RuleId</span></span>](ruleid.md) <br/> |<span data-ttu-id="6e945-114">Задает идентификатор правила.</span><span class="sxs-lookup"><span data-stu-id="6e945-114">Specifies the rule identifier.</span></span>  <br/> |
|[<span data-ttu-id="6e945-115">DisplayName (строка)</span><span class="sxs-lookup"><span data-stu-id="6e945-115">DisplayName (string)</span></span>](displayname-string.md) <br/> |<span data-ttu-id="6e945-116">Содержит отображаемое имя правила.</span><span class="sxs-lookup"><span data-stu-id="6e945-116">Contains the display name of a rule.</span></span>  <br/> |
|[<span data-ttu-id="6e945-117">Priority</span><span class="sxs-lookup"><span data-stu-id="6e945-117">Priority</span></span>](priority.md) <br/> |<span data-ttu-id="6e945-118">Указывает порядок запуска правила.</span><span class="sxs-lookup"><span data-stu-id="6e945-118">Indicates the order in which a rule is to be run.</span></span>  <br/> |
|[<span data-ttu-id="6e945-119">IsEnabled</span><span class="sxs-lookup"><span data-stu-id="6e945-119">IsEnabled</span></span>](isenabled.md) <br/> |<span data-ttu-id="6e945-120">Указывает, включено ли правило.</span><span class="sxs-lookup"><span data-stu-id="6e945-120">Indicates whether the rule is enabled.</span></span>  <br/> |
|[<span data-ttu-id="6e945-121">иснотсуппортед</span><span class="sxs-lookup"><span data-stu-id="6e945-121">IsNotSupported</span></span>](isnotsupported.md) <br/> |<span data-ttu-id="6e945-122">Указывает, может ли правило измениться с помощью API управляемого кода.</span><span class="sxs-lookup"><span data-stu-id="6e945-122">Indicates whether the rule cannot be modified with the managed code APIs.</span></span>  <br/> |
|[<span data-ttu-id="6e945-123">исинеррор</span><span class="sxs-lookup"><span data-stu-id="6e945-123">IsInError</span></span>](isinerror.md) <br/> |<span data-ttu-id="6e945-124">Указывает, является ли правило ошибкой.</span><span class="sxs-lookup"><span data-stu-id="6e945-124">Indicates whether the rule is in an error condition.</span></span>  <br/> |
|[<span data-ttu-id="6e945-125">Conditions</span><span class="sxs-lookup"><span data-stu-id="6e945-125">Conditions</span></span>](conditions.md) <br/> |<span data-ttu-id="6e945-126">Определяет условия, при выполнении которых будут запускаться действия правил для правила.</span><span class="sxs-lookup"><span data-stu-id="6e945-126">Identifies the conditions that, when fulfilled, will trigger the rule actions for a rule.</span></span>  <br/> |
|[<span data-ttu-id="6e945-127">Exceptions</span><span class="sxs-lookup"><span data-stu-id="6e945-127">Exceptions</span></span>](exceptions.md) <br/> |<span data-ttu-id="6e945-128">Определяет исключения, которые представляют все доступные условия исключения правила для правила папки "Входящие".</span><span class="sxs-lookup"><span data-stu-id="6e945-128">Identifies the exceptions that represent all the available rule exception conditions for the inbox rule.</span></span>  <br/> |
|[<span data-ttu-id="6e945-129">Actions</span><span class="sxs-lookup"><span data-stu-id="6e945-129">Actions</span></span>](actions.md) <br/> |<span data-ttu-id="6e945-130">Представляет действия, выполняемые над сообщением при выполнении условий.</span><span class="sxs-lookup"><span data-stu-id="6e945-130">Represents the actions to be taken on a message when the conditions are fulfilled.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="6e945-131">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="6e945-131">Parent elements</span></span>

|<span data-ttu-id="6e945-132">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="6e945-132">**Element**</span></span>|<span data-ttu-id="6e945-133">**Описание**</span><span class="sxs-lookup"><span data-stu-id="6e945-133">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6e945-134">креатерулеоператион</span><span class="sxs-lookup"><span data-stu-id="6e945-134">CreateRuleOperation</span></span>](createruleoperation.md) <br/> |<span data-ttu-id="6e945-135">Представляет операцию для создания нового правила.</span><span class="sxs-lookup"><span data-stu-id="6e945-135">Represents an operation to create a new rule.</span></span>  <br/> |
|[<span data-ttu-id="6e945-136">инбоксрулес</span><span class="sxs-lookup"><span data-stu-id="6e945-136">InboxRules</span></span>](inboxrules.md) <br/> |<span data-ttu-id="6e945-137">Представляет массив правил в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="6e945-137">Represents an array of rules in the user's mailbox.</span></span>  <br/> |
|[<span data-ttu-id="6e945-138">сетрулеоператион</span><span class="sxs-lookup"><span data-stu-id="6e945-138">SetRuleOperation</span></span>](setruleoperation.md) <br/> |<span data-ttu-id="6e945-139">Представляет операцию для обновления существующего правила.</span><span class="sxs-lookup"><span data-stu-id="6e945-139">Represents an operation to update an existing rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="6e945-140">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="6e945-140">Text value</span></span>

<span data-ttu-id="6e945-141">Нет.</span><span class="sxs-lookup"><span data-stu-id="6e945-141">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="6e945-142">Примечания</span><span class="sxs-lookup"><span data-stu-id="6e945-142">Remarks</span></span>

<span data-ttu-id="6e945-143">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="6e945-143">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6e945-144">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="6e945-144">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6e945-145">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="6e945-145">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="6e945-146">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="6e945-146">Schema Name</span></span>  <br/> |<span data-ttu-id="6e945-147">Схема Types</span><span class="sxs-lookup"><span data-stu-id="6e945-147">Types schema</span></span>  <br/> |
|<span data-ttu-id="6e945-148">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="6e945-148">Validation File</span></span>  <br/> |<span data-ttu-id="6e945-149">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="6e945-149">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="6e945-150">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="6e945-150">Can be Empty</span></span>  <br/> |<span data-ttu-id="6e945-151">True</span><span class="sxs-lookup"><span data-stu-id="6e945-151">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6e945-152">См. также</span><span class="sxs-lookup"><span data-stu-id="6e945-152">See also</span></span>



[<span data-ttu-id="6e945-153">UpdateInboxRules</span><span class="sxs-lookup"><span data-stu-id="6e945-153">UpdateInboxRules</span></span>](updateinboxrules.md)
  
[<span data-ttu-id="6e945-154">сетрулеоператион</span><span class="sxs-lookup"><span data-stu-id="6e945-154">SetRuleOperation</span></span>](setruleoperation.md)
  
[<span data-ttu-id="6e945-155">креатерулеоператион</span><span class="sxs-lookup"><span data-stu-id="6e945-155">CreateRuleOperation</span></span>](createruleoperation.md)


- [<span data-ttu-id="6e945-156">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="6e945-156">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

