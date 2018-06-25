---
title: Константа
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Constant
api_type:
- schema
ms.assetid: 340af0cd-9f12-44ab-b8f1-21d107c8d0c9
description: Элемент константу определяет значение константы в качестве ограничения.
ms.openlocfilehash: 73912bc1981c5d54040f7c4a563ad805916fe721
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761721"
---
# <a name="constant"></a><span data-ttu-id="5b2b8-103">Константа</span><span class="sxs-lookup"><span data-stu-id="5b2b8-103">Constant</span></span>

<span data-ttu-id="5b2b8-104">Элемент **константу** определяет значение константы в качестве ограничения.</span><span class="sxs-lookup"><span data-stu-id="5b2b8-104">The **Constant** element identifies a constant value in a restriction.</span></span> 
  
```xml
<Constant Value="" />
```

 <span data-ttu-id="5b2b8-105">**ConstantValueType**</span><span class="sxs-lookup"><span data-stu-id="5b2b8-105">**ConstantValueType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5b2b8-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="5b2b8-106">Attributes and elements</span></span>

<span data-ttu-id="5b2b8-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="5b2b8-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5b2b8-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="5b2b8-108">Attributes</span></span>

|<span data-ttu-id="5b2b8-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="5b2b8-109">**Attribute**</span></span>|<span data-ttu-id="5b2b8-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="5b2b8-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="5b2b8-111">**Значение**</span><span class="sxs-lookup"><span data-stu-id="5b2b8-111">**Value**</span></span> <br/> |<span data-ttu-id="5b2b8-112">Задает значение для сравнения в ограничении.</span><span class="sxs-lookup"><span data-stu-id="5b2b8-112">Specifies the value to compare in the restriction.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="5b2b8-113">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="5b2b8-113">Child elements</span></span>

<span data-ttu-id="5b2b8-114">Нет.</span><span class="sxs-lookup"><span data-stu-id="5b2b8-114">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="5b2b8-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="5b2b8-115">Parent elements</span></span>

|<span data-ttu-id="5b2b8-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="5b2b8-116">**Element**</span></span>|<span data-ttu-id="5b2b8-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="5b2b8-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5b2b8-118">Contains</span><span class="sxs-lookup"><span data-stu-id="5b2b8-118">Contains</span></span>](contains.md) <br/> |<span data-ttu-id="5b2b8-119">Представляет выражение поиска, которое определяет, содержит ли данное свойство указанную константу строчного типа.</span><span class="sxs-lookup"><span data-stu-id="5b2b8-119">Represents a search expression that determines whether a given property contains the supplied constant string value.</span></span>  <br/> |
|[<span data-ttu-id="5b2b8-120">FieldURIOrConstant</span><span class="sxs-lookup"><span data-stu-id="5b2b8-120">FieldURIOrConstant</span></span>](fielduriorconstant.md) <br/> |<span data-ttu-id="5b2b8-121">Представляет свойство или постоянное значение для использования при сравнении с другого свойства.</span><span class="sxs-lookup"><span data-stu-id="5b2b8-121">Represents either a property or a constant value to be used when comparing with another property.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="5b2b8-122">Замечания</span><span class="sxs-lookup"><span data-stu-id="5b2b8-122">Remarks</span></span>

<span data-ttu-id="5b2b8-123">Строковое значение атрибута **Value** должен быть принудительного в тип, который вы пытаетесь сравнения.</span><span class="sxs-lookup"><span data-stu-id="5b2b8-123">The string value in the **Value** attribute must be coercible into the type you are trying to compare against.</span></span> <span data-ttu-id="5b2b8-124">Например при сравнении соответствия константное значение свойства даты и времени строковое значение должно представлять даты и времени.</span><span class="sxs-lookup"><span data-stu-id="5b2b8-124">For example, if you are comparing a date/time property against a constant value, the string value must represent a date/time.</span></span> 
  
<span data-ttu-id="5b2b8-125">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="5b2b8-125">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5b2b8-126">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="5b2b8-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5b2b8-127">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="5b2b8-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="5b2b8-128">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="5b2b8-128">Schema Name</span></span>  <br/> |<span data-ttu-id="5b2b8-129">Схема Types</span><span class="sxs-lookup"><span data-stu-id="5b2b8-129">Types schema</span></span>  <br/> |
|<span data-ttu-id="5b2b8-130">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="5b2b8-130">Validation File</span></span>  <br/> |<span data-ttu-id="5b2b8-131">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="5b2b8-131">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="5b2b8-132">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="5b2b8-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="5b2b8-133">False</span><span class="sxs-lookup"><span data-stu-id="5b2b8-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="5b2b8-134">См. также</span><span class="sxs-lookup"><span data-stu-id="5b2b8-134">See also</span></span>



- [<span data-ttu-id="5b2b8-135">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="5b2b8-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

