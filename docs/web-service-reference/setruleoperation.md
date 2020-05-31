---
title: сетрулеоператион
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
description: Элемент Сетрулеоператион представляет операцию для обновления существующего правила.
ms.openlocfilehash: 9c956394d14c510e8dcc95110ef1874ea7010be0
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835451"
---
# <a name="setruleoperation"></a><span data-ttu-id="62445-103">сетрулеоператион</span><span class="sxs-lookup"><span data-stu-id="62445-103">SetRuleOperation</span></span>

<span data-ttu-id="62445-104">Элемент **сетрулеоператион** представляет операцию для обновления существующего правила.</span><span class="sxs-lookup"><span data-stu-id="62445-104">The **SetRuleOperation** element represents an operation to update an existing rule.</span></span> 
  
[<span data-ttu-id="62445-105">UpdateInboxRules</span><span class="sxs-lookup"><span data-stu-id="62445-105">UpdateInboxRules</span></span>](updateinboxrules.md)
  
[<span data-ttu-id="62445-106">Operations</span><span class="sxs-lookup"><span data-stu-id="62445-106">Operations</span></span>](operations.md)
  
```XML
<SetRuleOperation>
    <Rule/>
</SetRuleOperation>
```

 <span data-ttu-id="62445-107">**сетрулеоператионтипе**</span><span class="sxs-lookup"><span data-stu-id="62445-107">**SetRuleOperationType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="62445-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="62445-108">Attributes and elements</span></span>

<span data-ttu-id="62445-109">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="62445-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="62445-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="62445-110">Attributes</span></span>

<span data-ttu-id="62445-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="62445-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="62445-112">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="62445-112">Child elements</span></span>

|<span data-ttu-id="62445-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="62445-113">**Element**</span></span>|<span data-ttu-id="62445-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="62445-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="62445-115">Правило (RuleType)</span><span class="sxs-lookup"><span data-stu-id="62445-115">Rule (RuleType)</span></span>](rule-ruletype.md) <br/> |<span data-ttu-id="62445-116">Представляет правило в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="62445-116">Represents a rule in a user's mailbox.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="62445-117">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="62445-117">Parent elements</span></span>

|<span data-ttu-id="62445-118">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="62445-118">**Element**</span></span>|<span data-ttu-id="62445-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="62445-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="62445-120">Операции</span><span class="sxs-lookup"><span data-stu-id="62445-120">Operations</span></span>](operations.md) <br/> |<span data-ttu-id="62445-121">Содержит набор операций правила, которые могут выполняться в папке "Входящие".</span><span class="sxs-lookup"><span data-stu-id="62445-121">Contains an array of rule operations that can be performed on an Inbox.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="62445-122">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="62445-122">Text value</span></span>

<span data-ttu-id="62445-123">Нет.</span><span class="sxs-lookup"><span data-stu-id="62445-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="62445-124">Примечания</span><span class="sxs-lookup"><span data-stu-id="62445-124">Remarks</span></span>

<span data-ttu-id="62445-125">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="62445-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="62445-126">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="62445-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="62445-127">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="62445-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="62445-128">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="62445-128">Schema Name</span></span>  <br/> |<span data-ttu-id="62445-129">Схема Types</span><span class="sxs-lookup"><span data-stu-id="62445-129">Types schema</span></span>  <br/> |
|<span data-ttu-id="62445-130">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="62445-130">Validation File</span></span>  <br/> |<span data-ttu-id="62445-131">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="62445-131">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="62445-132">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="62445-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="62445-133">False</span><span class="sxs-lookup"><span data-stu-id="62445-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="62445-134">См. также</span><span class="sxs-lookup"><span data-stu-id="62445-134">See also</span></span>



[<span data-ttu-id="62445-135">UpdateInboxRules</span><span class="sxs-lookup"><span data-stu-id="62445-135">UpdateInboxRules</span></span>](updateinboxrules.md)
  
[<span data-ttu-id="62445-136">делетерулеоператион</span><span class="sxs-lookup"><span data-stu-id="62445-136">DeleteRuleOperation</span></span>](deleteruleoperation.md)
  
[<span data-ttu-id="62445-137">креатерулеоператион</span><span class="sxs-lookup"><span data-stu-id="62445-137">CreateRuleOperation</span></span>](createruleoperation.md)


- [<span data-ttu-id="62445-138">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="62445-138">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

