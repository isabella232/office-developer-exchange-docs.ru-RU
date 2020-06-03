---
title: рулеоператионеррорс
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f15c7b9e-a670-4a11-bb62-2a298c91f142
description: Элемент Рулеоператионеррорс представляет массив ошибок проверки правил для каждого поля правила, которое содержит ошибку.
ms.openlocfilehash: d547155f3cbf9eedd0f9bfac7bf3768b3630b50e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44464954"
---
# <a name="ruleoperationerrors"></a><span data-ttu-id="4d75b-103">рулеоператионеррорс</span><span class="sxs-lookup"><span data-stu-id="4d75b-103">RuleOperationErrors</span></span>

<span data-ttu-id="4d75b-104">Элемент **рулеоператионеррорс** представляет массив ошибок проверки правил для каждого поля правила, которое содержит ошибку.</span><span class="sxs-lookup"><span data-stu-id="4d75b-104">The **RuleOperationErrors** element represents an array of rule validation errors on each rule field that has an error.</span></span> 
  
[<span data-ttu-id="4d75b-105">упдатеинбоксрулесреспонсе</span><span class="sxs-lookup"><span data-stu-id="4d75b-105">UpdateInboxRulesResponse</span></span>](updateinboxrulesresponse.md)
  
[<span data-ttu-id="4d75b-106">рулеоператионеррорс</span><span class="sxs-lookup"><span data-stu-id="4d75b-106">RuleOperationErrors</span></span>](ruleoperationerrors.md)
  
```XML
<RuleOperationErrors>
    <RuleOperationError>
</RuleOperationErrors>
```

 <span data-ttu-id="4d75b-107">**аррайофрулеоператионеррорстипе**</span><span class="sxs-lookup"><span data-stu-id="4d75b-107">**ArrayOfRuleOperationErrorsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4d75b-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="4d75b-108">Attributes and elements</span></span>

<span data-ttu-id="4d75b-109">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="4d75b-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4d75b-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="4d75b-110">Attributes</span></span>

<span data-ttu-id="4d75b-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="4d75b-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4d75b-112">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="4d75b-112">Child elements</span></span>

|<span data-ttu-id="4d75b-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="4d75b-113">**Element**</span></span>|<span data-ttu-id="4d75b-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="4d75b-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4d75b-115">рулеоператионеррор</span><span class="sxs-lookup"><span data-stu-id="4d75b-115">RuleOperationError</span></span>](ruleoperationerror.md) <br/> |<span data-ttu-id="4d75b-116">Представляет ошибку операции с правилом.</span><span class="sxs-lookup"><span data-stu-id="4d75b-116">Represents a rule operation error.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="4d75b-117">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="4d75b-117">Parent elements</span></span>

|<span data-ttu-id="4d75b-118">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="4d75b-118">**Element**</span></span>|<span data-ttu-id="4d75b-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="4d75b-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4d75b-120">упдатеинбоксрулесреспонсе</span><span class="sxs-lookup"><span data-stu-id="4d75b-120">UpdateInboxRulesResponse</span></span>](updateinboxrulesresponse.md) <br/> |<span data-ttu-id="4d75b-121">Определяет ответ на запрос [UpdateInboxRules](updateinboxrules.md) .</span><span class="sxs-lookup"><span data-stu-id="4d75b-121">Defines a response to an [UpdateInboxRules](updateinboxrules.md) request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="4d75b-122">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="4d75b-122">Text value</span></span>

<span data-ttu-id="4d75b-123">Нет.</span><span class="sxs-lookup"><span data-stu-id="4d75b-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="4d75b-124">Примечания</span><span class="sxs-lookup"><span data-stu-id="4d75b-124">Remarks</span></span>

<span data-ttu-id="4d75b-125">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="4d75b-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4d75b-126">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="4d75b-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4d75b-127">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="4d75b-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="4d75b-128">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="4d75b-128">Schema name</span></span>  <br/> |<span data-ttu-id="4d75b-129">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="4d75b-129">Messages schema</span></span>  <br/> |
|<span data-ttu-id="4d75b-130">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="4d75b-130">Validation file</span></span>  <br/> |<span data-ttu-id="4d75b-131">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="4d75b-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="4d75b-132">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="4d75b-132">Can be empty</span></span>  <br/> |<span data-ttu-id="4d75b-133">Верно.</span><span class="sxs-lookup"><span data-stu-id="4d75b-133">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="4d75b-134">См. также</span><span class="sxs-lookup"><span data-stu-id="4d75b-134">See also</span></span>



[<span data-ttu-id="4d75b-135">UpdateInboxRules</span><span class="sxs-lookup"><span data-stu-id="4d75b-135">UpdateInboxRules</span></span>](updateinboxrules.md)


- [<span data-ttu-id="4d75b-136">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="4d75b-136">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

