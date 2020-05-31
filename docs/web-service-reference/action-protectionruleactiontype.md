---
title: Action (Протектионрулеактионтипе)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Action
api_type:
- schema
ms.assetid: ca090dec-e2c5-49c8-a057-8d1f2409147f
description: Элемент Action определяет действие, которое должно выполняться, если условная часть правила соответствует.
ms.openlocfilehash: 8f699e698d3159c5ff2636da506542da3b218251
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762504"
---
# <a name="action-protectionruleactiontype"></a><span data-ttu-id="721ec-103">Action (Протектионрулеактионтипе)</span><span class="sxs-lookup"><span data-stu-id="721ec-103">Action (ProtectionRuleActionType)</span></span>

<span data-ttu-id="721ec-104">Элемент **Action** определяет действие, которое должно выполняться, если условная часть правила соответствует.</span><span class="sxs-lookup"><span data-stu-id="721ec-104">The **Action** element identifies what action must be executed if the condition part of the rule matches.</span></span> 
  
```xml
<Action Name="">
   <Argument/>
</Action>

```

 <span data-ttu-id="721ec-105">**протектионрулеактионтипе**</span><span class="sxs-lookup"><span data-stu-id="721ec-105">**ProtectionRuleActionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="721ec-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="721ec-106">Attributes and elements</span></span>

<span data-ttu-id="721ec-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="721ec-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="721ec-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="721ec-108">Attributes</span></span>

|<span data-ttu-id="721ec-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="721ec-109">**Attribute**</span></span>|<span data-ttu-id="721ec-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="721ec-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="721ec-111">**Name**</span><span class="sxs-lookup"><span data-stu-id="721ec-111">**Name**</span></span> <br/> |<span data-ttu-id="721ec-112">Определяет имя действия.</span><span class="sxs-lookup"><span data-stu-id="721ec-112">Identifies the name of the action.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="721ec-113">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="721ec-113">Child elements</span></span>

|<span data-ttu-id="721ec-114">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="721ec-114">**Element**</span></span>|<span data-ttu-id="721ec-115">**Описание**</span><span class="sxs-lookup"><span data-stu-id="721ec-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="721ec-116">Аргумент</span><span class="sxs-lookup"><span data-stu-id="721ec-116">Argument</span></span>](argument.md) <br/> |<span data-ttu-id="721ec-117">Задает аргументы для действия.</span><span class="sxs-lookup"><span data-stu-id="721ec-117">Specifies arguments to the action.</span></span> <span data-ttu-id="721ec-118">Этот элемент не будет выполняться, если заданное действие не требует указания аргументов.</span><span class="sxs-lookup"><span data-stu-id="721ec-118">This element will not occur if the specified action does not require arguments to be specified.</span></span> <span data-ttu-id="721ec-119">Этот элемент может встретиться один или несколько раз, если для действия требуется один или несколько аргументов.</span><span class="sxs-lookup"><span data-stu-id="721ec-119">This element can occur one or more times if an action requires one or more arguments.</span></span> <span data-ttu-id="721ec-120">Действие **ригхтспротектмессаже** будет содержать один аргумент.</span><span class="sxs-lookup"><span data-stu-id="721ec-120">The **RightsProtectMessage** action will contain a single argument.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="721ec-121">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="721ec-121">Parent elements</span></span>

|<span data-ttu-id="721ec-122">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="721ec-122">**Element**</span></span>|<span data-ttu-id="721ec-123">**Описание**</span><span class="sxs-lookup"><span data-stu-id="721ec-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="721ec-124">Rule</span><span class="sxs-lookup"><span data-stu-id="721ec-124">Rule</span></span>](rule.md) <br/> |<span data-ttu-id="721ec-125">Содержит одно правило защиты.</span><span class="sxs-lookup"><span data-stu-id="721ec-125">Contains a single protection rule.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="721ec-126">Примечания</span><span class="sxs-lookup"><span data-stu-id="721ec-126">Remarks</span></span>

<span data-ttu-id="721ec-127">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="721ec-127">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="721ec-128">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="721ec-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="721ec-129">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="721ec-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="721ec-130">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="721ec-130">Schema Name</span></span>  <br/> |<span data-ttu-id="721ec-131">Схема Types</span><span class="sxs-lookup"><span data-stu-id="721ec-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="721ec-132">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="721ec-132">Validation File</span></span>  <br/> |<span data-ttu-id="721ec-133">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="721ec-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="721ec-134">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="721ec-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="721ec-135">False</span><span class="sxs-lookup"><span data-stu-id="721ec-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="721ec-136">См. также</span><span class="sxs-lookup"><span data-stu-id="721ec-136">See also</span></span>

- [<span data-ttu-id="721ec-137">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="721ec-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

