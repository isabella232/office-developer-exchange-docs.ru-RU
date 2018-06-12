---
title: Значение
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Value
api_type:
- schema
ms.assetid: 9a30cadd-909e-41b1-b4e9-291643dd89c6
description: Значение элемента содержит значение расширенного свойства.
ms.openlocfilehash: 4b8674d267b78f0384f9457e794e88ace8234826
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19840472"
---
# <a name="value"></a><span data-ttu-id="09138-103">Значение</span><span class="sxs-lookup"><span data-stu-id="09138-103">Value</span></span>

<span data-ttu-id="09138-104">**Значение** элемента содержит значение расширенного свойства.</span><span class="sxs-lookup"><span data-stu-id="09138-104">The **Value** element contains the value of an extended property.</span></span> 
  
```xml
<Value/>
```

<span data-ttu-id="09138-105">**Строка**</span><span class="sxs-lookup"><span data-stu-id="09138-105">**String**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="09138-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="09138-106">Attributes and elements</span></span>

<span data-ttu-id="09138-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="09138-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="09138-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="09138-108">Attributes</span></span>

<span data-ttu-id="09138-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="09138-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="09138-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="09138-110">Child elements</span></span>

<span data-ttu-id="09138-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="09138-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="09138-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="09138-112">Parent elements</span></span>

|<span data-ttu-id="09138-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="09138-113">**Element**</span></span>|<span data-ttu-id="09138-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="09138-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="09138-115">Значения</span><span class="sxs-lookup"><span data-stu-id="09138-115">Values</span></span>](values.md) <br/> |<span data-ttu-id="09138-116">Содержит коллекцию значений для расширенного свойства.</span><span class="sxs-lookup"><span data-stu-id="09138-116">Contains a collection of values for an extended property.</span></span>  <br/> |
|[<span data-ttu-id="09138-117">ExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="09138-117">ExtendedProperty</span></span>](extendedproperty.md) <br/> |<span data-ttu-id="09138-118">Определяет расширенные свойства для папок и элементов.</span><span class="sxs-lookup"><span data-stu-id="09138-118">Identifies extended properties on folders and items.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="09138-119">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="09138-119">Text value</span></span>

<span data-ttu-id="09138-120">Текстовое значение должно быть совместим с типом, указанного в атрибуте PropertyType ExtendedFieldURI.</span><span class="sxs-lookup"><span data-stu-id="09138-120">The text value must be compatible with the type that is indicated by the PropertyType attribute of the ExtendedFieldURI.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="09138-121">Замечания</span><span class="sxs-lookup"><span data-stu-id="09138-121">Remarks</span></span>

<span data-ttu-id="09138-122">Элемент **Value** может возникнуть в обоих случаях одним или несколькими значениями расширенные свойства.</span><span class="sxs-lookup"><span data-stu-id="09138-122">A **Value** element can occur in both single and multivalued extended property instances.</span></span> <span data-ttu-id="09138-123">Для однозначного экземпляров по-прежнему прямым потомком элемент [ExtendedProperty](extendedproperty.md) .</span><span class="sxs-lookup"><span data-stu-id="09138-123">For single-valued instances, it exists as a direct child of the [ExtendedProperty](extendedproperty.md) element.</span></span> <span data-ttu-id="09138-124">Для многозначных экземпляра по-прежнему прямым потомком коллекцию **значений** .</span><span class="sxs-lookup"><span data-stu-id="09138-124">For multivalued instance, it exists as a direct child of the **Values** collection.</span></span> 
  
<span data-ttu-id="09138-125">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="09138-125">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="09138-126">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="09138-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="09138-127">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="09138-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="09138-128">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="09138-128">Schema Name</span></span>  <br/> |<span data-ttu-id="09138-129">Схема Types</span><span class="sxs-lookup"><span data-stu-id="09138-129">Types schema</span></span>  <br/> |
|<span data-ttu-id="09138-130">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="09138-130">Validation File</span></span>  <br/> |<span data-ttu-id="09138-131">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="09138-131">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="09138-132">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="09138-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="09138-133">False</span><span class="sxs-lookup"><span data-stu-id="09138-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="09138-134">См. также</span><span class="sxs-lookup"><span data-stu-id="09138-134">See also</span></span>

- [<span data-ttu-id="09138-135">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="09138-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

