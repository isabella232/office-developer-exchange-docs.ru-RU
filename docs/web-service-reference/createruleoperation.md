---
title: креатерулеоператион
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
description: Элемент Креатерулеоператион представляет операцию для создания нового правила для папки "Входящие".
ms.openlocfilehash: df857544e6d5840a3f738740114195e4c4bb5798
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460773"
---
# <a name="createruleoperation"></a><span data-ttu-id="88f0a-103">креатерулеоператион</span><span class="sxs-lookup"><span data-stu-id="88f0a-103">CreateRuleOperation</span></span>

<span data-ttu-id="88f0a-104">Элемент **креатерулеоператион** представляет операцию для создания нового правила для папки "Входящие".</span><span class="sxs-lookup"><span data-stu-id="88f0a-104">The **CreateRuleOperation** element represents an operation to create a new Inbox rule.</span></span> 
  
[<span data-ttu-id="88f0a-105">UpdateInboxRules</span><span class="sxs-lookup"><span data-stu-id="88f0a-105">UpdateInboxRules</span></span>](updateinboxrules.md)
  
[<span data-ttu-id="88f0a-106">Operations</span><span class="sxs-lookup"><span data-stu-id="88f0a-106">Operations</span></span>](operations.md)
  
```xml
<CreateRuleOperation>
    <Rule/>
</CreateRuleOperation>
```

 <span data-ttu-id="88f0a-107">**креатерулеоператионтипе**</span><span class="sxs-lookup"><span data-stu-id="88f0a-107">**CreateRuleOperationType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="88f0a-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="88f0a-108">Attributes and elements</span></span>

<span data-ttu-id="88f0a-109">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="88f0a-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="88f0a-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="88f0a-110">Attributes</span></span>

<span data-ttu-id="88f0a-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="88f0a-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="88f0a-112">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="88f0a-112">Child elements</span></span>

|<span data-ttu-id="88f0a-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="88f0a-113">**Element**</span></span>|<span data-ttu-id="88f0a-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="88f0a-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="88f0a-115">Правило (RuleType)</span><span class="sxs-lookup"><span data-stu-id="88f0a-115">Rule (RuleType)</span></span>](rule-ruletype.md) <br/> |<span data-ttu-id="88f0a-116">Представляет правило, которое будет создано в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="88f0a-116">Represents a rule to be created in a user's mailbox.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="88f0a-117">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="88f0a-117">Parent elements</span></span>

|<span data-ttu-id="88f0a-118">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="88f0a-118">**Element**</span></span>|<span data-ttu-id="88f0a-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="88f0a-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="88f0a-120">Operations</span><span class="sxs-lookup"><span data-stu-id="88f0a-120">Operations</span></span>](operations.md) <br/> |<span data-ttu-id="88f0a-121">Содержит операции, которые можно выполнить для папки "Входящие".</span><span class="sxs-lookup"><span data-stu-id="88f0a-121">Contains the operations that can be performed on an Inbox.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="88f0a-122">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="88f0a-122">Text value</span></span>

<span data-ttu-id="88f0a-123">Нет.</span><span class="sxs-lookup"><span data-stu-id="88f0a-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="88f0a-124">Примечания</span><span class="sxs-lookup"><span data-stu-id="88f0a-124">Remarks</span></span>

<span data-ttu-id="88f0a-125">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="88f0a-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="88f0a-126">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="88f0a-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="88f0a-127">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="88f0a-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="88f0a-128">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="88f0a-128">Schema Name</span></span>  <br/> |<span data-ttu-id="88f0a-129">Схема Types</span><span class="sxs-lookup"><span data-stu-id="88f0a-129">Types schema</span></span>  <br/> |
|<span data-ttu-id="88f0a-130">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="88f0a-130">Validation File</span></span>  <br/> |<span data-ttu-id="88f0a-131">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="88f0a-131">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="88f0a-132">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="88f0a-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="88f0a-133">False</span><span class="sxs-lookup"><span data-stu-id="88f0a-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="88f0a-134">См. также</span><span class="sxs-lookup"><span data-stu-id="88f0a-134">See also</span></span>



[<span data-ttu-id="88f0a-135">UpdateInboxRules</span><span class="sxs-lookup"><span data-stu-id="88f0a-135">UpdateInboxRules</span></span>](updateinboxrules.md)
  
[<span data-ttu-id="88f0a-136">сетрулеоператион</span><span class="sxs-lookup"><span data-stu-id="88f0a-136">SetRuleOperation</span></span>](setruleoperation.md)
  
[<span data-ttu-id="88f0a-137">делетерулеоператион</span><span class="sxs-lookup"><span data-stu-id="88f0a-137">DeleteRuleOperation</span></span>](deleteruleoperation.md)


- [<span data-ttu-id="88f0a-138">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="88f0a-138">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

