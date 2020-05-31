---
title: Аргументация
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Argument
api_type:
- schema
ms.assetid: 15b0bfb8-2448-4ceb-aeac-965115e0fb72
description: Элемент Argument указывает аргументы для действия.
ms.openlocfilehash: ed4e46a8d9897516e9c96bf3930f7d488bc06714
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761496"
---
# <a name="argument"></a><span data-ttu-id="7e48b-103">Аргументация</span><span class="sxs-lookup"><span data-stu-id="7e48b-103">Argument</span></span>

<span data-ttu-id="7e48b-104">Элемент **Argument** указывает аргументы для действия.</span><span class="sxs-lookup"><span data-stu-id="7e48b-104">The **Argument** element specifies arguments to the action.</span></span> 
  
```xml
<Argument Value=""/>
```

 <span data-ttu-id="7e48b-105">**протектионрулеаргументтипе**</span><span class="sxs-lookup"><span data-stu-id="7e48b-105">**ProtectionRuleArgumentType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7e48b-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="7e48b-106">Attributes and elements</span></span>

<span data-ttu-id="7e48b-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="7e48b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7e48b-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="7e48b-108">Attributes</span></span>

|<span data-ttu-id="7e48b-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="7e48b-109">**Attribute**</span></span>|<span data-ttu-id="7e48b-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="7e48b-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="7e48b-111">**Значение**</span><span class="sxs-lookup"><span data-stu-id="7e48b-111">**Value**</span></span> <br/> |<span data-ttu-id="7e48b-112">Непустое строковое значение, представляющее значение аргумента для части действия правила защиты.</span><span class="sxs-lookup"><span data-stu-id="7e48b-112">A non-empty string value that represents the value of an argument to the action part of a protection rule.</span></span> <span data-ttu-id="7e48b-113">Этот атрибут является обязательным.</span><span class="sxs-lookup"><span data-stu-id="7e48b-113">This attribute is required.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="7e48b-114">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="7e48b-114">Child elements</span></span>

<span data-ttu-id="7e48b-115">Нет.</span><span class="sxs-lookup"><span data-stu-id="7e48b-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="7e48b-116">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="7e48b-116">Parent elements</span></span>

|<span data-ttu-id="7e48b-117">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="7e48b-117">**Element**</span></span>|<span data-ttu-id="7e48b-118">**Описание**</span><span class="sxs-lookup"><span data-stu-id="7e48b-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7e48b-119">Action (Протектионрулеактионтипе)</span><span class="sxs-lookup"><span data-stu-id="7e48b-119">Action (ProtectionRuleActionType)</span></span>](action-protectionruleactiontype.md) <br/> |<span data-ttu-id="7e48b-120">Определяет действие, которое должно выполняться, если условная часть правила соответствует.</span><span class="sxs-lookup"><span data-stu-id="7e48b-120">Identifies what action must be executed if the condition part of the rule matches.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="7e48b-121">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="7e48b-121">Text value</span></span>

<span data-ttu-id="7e48b-122">Нет.</span><span class="sxs-lookup"><span data-stu-id="7e48b-122">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="7e48b-123">Примечания</span><span class="sxs-lookup"><span data-stu-id="7e48b-123">Remarks</span></span>

<span data-ttu-id="7e48b-124">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="7e48b-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7e48b-125">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="7e48b-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7e48b-126">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="7e48b-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="7e48b-127">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="7e48b-127">Schema Name</span></span>  <br/> |<span data-ttu-id="7e48b-128">Схема Types</span><span class="sxs-lookup"><span data-stu-id="7e48b-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="7e48b-129">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="7e48b-129">Validation File</span></span>  <br/> |<span data-ttu-id="7e48b-130">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="7e48b-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="7e48b-131">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="7e48b-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="7e48b-132">False</span><span class="sxs-lookup"><span data-stu-id="7e48b-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7e48b-133">См. также</span><span class="sxs-lookup"><span data-stu-id="7e48b-133">See also</span></span>

- [<span data-ttu-id="7e48b-134">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="7e48b-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

