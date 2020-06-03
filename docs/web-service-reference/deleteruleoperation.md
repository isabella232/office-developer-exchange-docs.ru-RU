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
ms.openlocfilehash: 6b17f7f99f1fd9b9889db00fdf55fba5eef5aba8
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44526923"
---
# <a name="deleteruleoperation"></a><span data-ttu-id="93e99-103">делетерулеоператион</span><span class="sxs-lookup"><span data-stu-id="93e99-103">DeleteRuleOperation</span></span>

<span data-ttu-id="93e99-104">Элемент **делетерулеоператион** содержит операцию удаления существующего правила для папки "Входящие".</span><span class="sxs-lookup"><span data-stu-id="93e99-104">The **DeleteRuleOperation** element contains an operation to delete an existing Inbox rule.</span></span> 
  
- [<span data-ttu-id="93e99-105">UpdateInboxRules</span><span class="sxs-lookup"><span data-stu-id="93e99-105">UpdateInboxRules</span></span>](updateinboxrules.md)
- [<span data-ttu-id="93e99-106">Operations</span><span class="sxs-lookup"><span data-stu-id="93e99-106">Operations</span></span>](operations.md)
  
```XML
<DeleteRuleOperation>
    <RuleId/>
</DeleteRuleOperation>
```

 <span data-ttu-id="93e99-107">**делетерулеоператионтипе**</span><span class="sxs-lookup"><span data-stu-id="93e99-107">**DeleteRuleOperationType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="93e99-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="93e99-108">Attributes and elements</span></span>

<span data-ttu-id="93e99-109">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="93e99-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="93e99-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="93e99-110">Attributes</span></span>

<span data-ttu-id="93e99-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="93e99-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="93e99-112">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="93e99-112">Child elements</span></span>

|<span data-ttu-id="93e99-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="93e99-113">**Element**</span></span>|<span data-ttu-id="93e99-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="93e99-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="93e99-115">RuleId</span><span class="sxs-lookup"><span data-stu-id="93e99-115">RuleId</span></span>](ruleid.md) <br/> |<span data-ttu-id="93e99-116">Указывает идентификатор удаляемого правила.</span><span class="sxs-lookup"><span data-stu-id="93e99-116">Specifies the identifier of the rule to delete.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="93e99-117">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="93e99-117">Parent elements</span></span>

|<span data-ttu-id="93e99-118">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="93e99-118">**Element**</span></span>|<span data-ttu-id="93e99-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="93e99-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="93e99-120">Операции</span><span class="sxs-lookup"><span data-stu-id="93e99-120">Operations</span></span>](operations.md) <br/> |<span data-ttu-id="93e99-121">Содержит набор операций правила, которые могут выполняться в папке "Входящие".</span><span class="sxs-lookup"><span data-stu-id="93e99-121">Contains an array of rule operations that can be performed on an Inbox.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="93e99-122">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="93e99-122">Text value</span></span>

<span data-ttu-id="93e99-123">Нет.</span><span class="sxs-lookup"><span data-stu-id="93e99-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="93e99-124">Примечания</span><span class="sxs-lookup"><span data-stu-id="93e99-124">Remarks</span></span>

<span data-ttu-id="93e99-125">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="93e99-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="93e99-126">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="93e99-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="93e99-127">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="93e99-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="93e99-128">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="93e99-128">Schema Name</span></span>  <br/> |<span data-ttu-id="93e99-129">Схема Types</span><span class="sxs-lookup"><span data-stu-id="93e99-129">Types schema</span></span>  <br/> |
|<span data-ttu-id="93e99-130">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="93e99-130">Validation File</span></span>  <br/> |<span data-ttu-id="93e99-131">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="93e99-131">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="93e99-132">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="93e99-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="93e99-133">False</span><span class="sxs-lookup"><span data-stu-id="93e99-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="93e99-134">См. также</span><span class="sxs-lookup"><span data-stu-id="93e99-134">See also</span></span>

- [<span data-ttu-id="93e99-135">UpdateInboxRules</span><span class="sxs-lookup"><span data-stu-id="93e99-135">UpdateInboxRules</span></span>](updateinboxrules.md) 
- [<span data-ttu-id="93e99-136">сетрулеоператион</span><span class="sxs-lookup"><span data-stu-id="93e99-136">SetRuleOperation</span></span>](setruleoperation.md) 
- [<span data-ttu-id="93e99-137">креатерулеоператион</span><span class="sxs-lookup"><span data-stu-id="93e99-137">CreateRuleOperation</span></span>](createruleoperation.md)
- [<span data-ttu-id="93e99-138">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="93e99-138">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

