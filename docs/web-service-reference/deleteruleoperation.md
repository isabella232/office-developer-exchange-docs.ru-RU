---
title: делетерулеоператион
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DeleteRuleOperation
api_type:
- schema
ms.assetid: c5e251af-f795-43cc-baaf-95d84475677c
description: Элемент Делетерулеоператион содержит операцию удаления существующего правила для папки "Входящие".
ms.openlocfilehash: 3410361e0b896fb0ef01c1873c9f8b0ac99afe58
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762051"
---
# <a name="deleteruleoperation"></a><span data-ttu-id="538bc-103">делетерулеоператион</span><span class="sxs-lookup"><span data-stu-id="538bc-103">DeleteRuleOperation</span></span>

<span data-ttu-id="538bc-104">Элемент **делетерулеоператион** содержит операцию удаления существующего правила для папки "Входящие".</span><span class="sxs-lookup"><span data-stu-id="538bc-104">The **DeleteRuleOperation** element contains an operation to delete an existing Inbox rule.</span></span> 
  
- [<span data-ttu-id="538bc-105">UpdateInboxRules</span><span class="sxs-lookup"><span data-stu-id="538bc-105">UpdateInboxRules</span></span>](updateinboxrules.md)
- [<span data-ttu-id="538bc-106">Operations</span><span class="sxs-lookup"><span data-stu-id="538bc-106">Operations</span></span>](operations.md)
  
```XML
<DeleteRuleOperation>
    <RuleId/>
</DeleteRuleOperation>
```

 <span data-ttu-id="538bc-107">**делетерулеоператионтипе**</span><span class="sxs-lookup"><span data-stu-id="538bc-107">**DeleteRuleOperationType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="538bc-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="538bc-108">Attributes and elements</span></span>

<span data-ttu-id="538bc-109">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="538bc-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="538bc-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="538bc-110">Attributes</span></span>

<span data-ttu-id="538bc-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="538bc-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="538bc-112">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="538bc-112">Child elements</span></span>

|<span data-ttu-id="538bc-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="538bc-113">**Element**</span></span>|<span data-ttu-id="538bc-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="538bc-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="538bc-115">RuleId</span><span class="sxs-lookup"><span data-stu-id="538bc-115">RuleId</span></span>](ruleid.md) <br/> |<span data-ttu-id="538bc-116">Указывает идентификатор удаляемого правила.</span><span class="sxs-lookup"><span data-stu-id="538bc-116">Specifies the identifier of the rule to delete.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="538bc-117">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="538bc-117">Parent elements</span></span>

|<span data-ttu-id="538bc-118">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="538bc-118">**Element**</span></span>|<span data-ttu-id="538bc-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="538bc-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="538bc-120">Операции</span><span class="sxs-lookup"><span data-stu-id="538bc-120">Operations</span></span>](operations.md) <br/> |<span data-ttu-id="538bc-121">Содержит набор операций правила, которые могут выполняться в папке "Входящие".</span><span class="sxs-lookup"><span data-stu-id="538bc-121">Contains an array of rule operations that can be performed on an Inbox.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="538bc-122">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="538bc-122">Text value</span></span>

<span data-ttu-id="538bc-123">Нет.</span><span class="sxs-lookup"><span data-stu-id="538bc-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="538bc-124">Примечания</span><span class="sxs-lookup"><span data-stu-id="538bc-124">Remarks</span></span>

<span data-ttu-id="538bc-125">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="538bc-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="538bc-126">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="538bc-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="538bc-127">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="538bc-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="538bc-128">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="538bc-128">Schema Name</span></span>  <br/> |<span data-ttu-id="538bc-129">Схема Types</span><span class="sxs-lookup"><span data-stu-id="538bc-129">Types schema</span></span>  <br/> |
|<span data-ttu-id="538bc-130">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="538bc-130">Validation File</span></span>  <br/> |<span data-ttu-id="538bc-131">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="538bc-131">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="538bc-132">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="538bc-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="538bc-133">False</span><span class="sxs-lookup"><span data-stu-id="538bc-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="538bc-134">См. также</span><span class="sxs-lookup"><span data-stu-id="538bc-134">See also</span></span>

- [<span data-ttu-id="538bc-135">UpdateInboxRules</span><span class="sxs-lookup"><span data-stu-id="538bc-135">UpdateInboxRules</span></span>](updateinboxrules.md) 
- [<span data-ttu-id="538bc-136">сетрулеоператион</span><span class="sxs-lookup"><span data-stu-id="538bc-136">SetRuleOperation</span></span>](setruleoperation.md) 
- [<span data-ttu-id="538bc-137">креатерулеоператион</span><span class="sxs-lookup"><span data-stu-id="538bc-137">CreateRuleOperation</span></span>](createruleoperation.md)
- [<span data-ttu-id="538bc-138">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="538bc-138">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

