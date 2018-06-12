---
title: Операции
manager: sethgros
ms.date: 09/17/2015
ms.audience: ITPro
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Operations
api_type:
- schema
ms.assetid: d8cd41b1-28ae-4c95-9ff6-8b25c8e18306
description: Элемент операции содержит массив операции правила, которые могут выполняться в папке "Входящие".
ms.openlocfilehash: 1030703d5e496be391d557e99e1420f9fddfdb36
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19834655"
---
# <a name="operations"></a><span data-ttu-id="facb1-103">Операции</span><span class="sxs-lookup"><span data-stu-id="facb1-103">Operations</span></span>

<span data-ttu-id="facb1-104">Элемент **операции** содержит массив операции правила, которые могут выполняться в папке "Входящие".</span><span class="sxs-lookup"><span data-stu-id="facb1-104">The **Operations** element contains an array of rule operations that can be performed on an Inbox.</span></span> 
  
[<span data-ttu-id="facb1-105">UpdateInboxRules</span><span class="sxs-lookup"><span data-stu-id="facb1-105">UpdateInboxRules</span></span>](updateinboxrules.md)
  
```XML
<Operations>
    <CreateRuleOperation/>
    <SetRuleOperation/>
    <DeleteRuleOperation/>
</Operations>
```

 <span data-ttu-id="facb1-106">**ArrayOfRuleOperationsType**</span><span class="sxs-lookup"><span data-stu-id="facb1-106">**ArrayOfRuleOperationsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="facb1-107">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="facb1-107">Attributes and elements</span></span>

<span data-ttu-id="facb1-108">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="facb1-108">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="facb1-109">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="facb1-109">Attributes</span></span>

<span data-ttu-id="facb1-110">Нет.</span><span class="sxs-lookup"><span data-stu-id="facb1-110">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="facb1-111">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="facb1-111">Child elements</span></span>

|<span data-ttu-id="facb1-112">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="facb1-112">**Element**</span></span>|<span data-ttu-id="facb1-113">**Описание**</span><span class="sxs-lookup"><span data-stu-id="facb1-113">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="facb1-114">CreateRuleOperation</span><span class="sxs-lookup"><span data-stu-id="facb1-114">CreateRuleOperation</span></span>](createruleoperation.md) <br/> |<span data-ttu-id="facb1-115">Представляет операцию для создания нового правила папки «Входящие».</span><span class="sxs-lookup"><span data-stu-id="facb1-115">Represents an operation to create a new Inbox rule.</span></span>  <br/> |
|[<span data-ttu-id="facb1-116">SetRuleOperation</span><span class="sxs-lookup"><span data-stu-id="facb1-116">SetRuleOperation</span></span>](setruleoperation.md) <br/> |<span data-ttu-id="facb1-117">Представляет операцию, чтобы обновить правила папки «Входящие».</span><span class="sxs-lookup"><span data-stu-id="facb1-117">Represents an operation to update an Inbox rule.</span></span>  <br/> |
|[<span data-ttu-id="facb1-118">DeleteRuleOperation</span><span class="sxs-lookup"><span data-stu-id="facb1-118">DeleteRuleOperation</span></span>](deleteruleoperation.md) <br/> |<span data-ttu-id="facb1-119">Представляет операцию для удаления правила папки «Входящие».</span><span class="sxs-lookup"><span data-stu-id="facb1-119">Represents an operation to delete an Inbox rule.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="facb1-120">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="facb1-120">Parent elements</span></span>

|<span data-ttu-id="facb1-121">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="facb1-121">**Element**</span></span>|<span data-ttu-id="facb1-122">**Описание**</span><span class="sxs-lookup"><span data-stu-id="facb1-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="facb1-123">UpdateInboxRules</span><span class="sxs-lookup"><span data-stu-id="facb1-123">UpdateInboxRules</span></span>](updateinboxrules.md) <br/> |<span data-ttu-id="facb1-124">Определяет запрос на обновление правил папки "Входящие" почтового ящика в хранилище сервера.</span><span class="sxs-lookup"><span data-stu-id="facb1-124">Defines a request to update the Inbox rules in a mailbox in the server store.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="facb1-125">Замечания</span><span class="sxs-lookup"><span data-stu-id="facb1-125">Remarks</span></span>

<span data-ttu-id="facb1-126">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="facb1-126">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="facb1-127">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="facb1-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="facb1-128">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="facb1-128">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="facb1-129">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="facb1-129">Schema Name</span></span>  <br/> |<span data-ttu-id="facb1-130">Схема Types</span><span class="sxs-lookup"><span data-stu-id="facb1-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="facb1-131">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="facb1-131">Validation File</span></span>  <br/> |<span data-ttu-id="facb1-132">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="facb1-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="facb1-133">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="facb1-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="facb1-134">False</span><span class="sxs-lookup"><span data-stu-id="facb1-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="facb1-135">См. также</span><span class="sxs-lookup"><span data-stu-id="facb1-135">See also</span></span>



[<span data-ttu-id="facb1-136">Операция UpdateInboxRules</span><span class="sxs-lookup"><span data-stu-id="facb1-136">UpdateInboxRules operation</span></span>](updateinboxrules-operation.md)


- [<span data-ttu-id="facb1-137">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="facb1-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

