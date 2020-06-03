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
description: Элемент value содержит значение расширенного свойства.
ms.openlocfilehash: 5de1528dda6d58ea772d050e709c0720e389fae6
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465214"
---
# <a name="value"></a><span data-ttu-id="7c12a-103">Значение</span><span class="sxs-lookup"><span data-stu-id="7c12a-103">Value</span></span>

<span data-ttu-id="7c12a-104">Элемент **value** содержит значение расширенного свойства.</span><span class="sxs-lookup"><span data-stu-id="7c12a-104">The **Value** element contains the value of an extended property.</span></span> 
  
```xml
<Value/>
```

<span data-ttu-id="7c12a-105">**String**</span><span class="sxs-lookup"><span data-stu-id="7c12a-105">**String**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="7c12a-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="7c12a-106">Attributes and elements</span></span>

<span data-ttu-id="7c12a-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="7c12a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7c12a-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="7c12a-108">Attributes</span></span>

<span data-ttu-id="7c12a-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="7c12a-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7c12a-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="7c12a-110">Child elements</span></span>

<span data-ttu-id="7c12a-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="7c12a-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="7c12a-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="7c12a-112">Parent elements</span></span>

|<span data-ttu-id="7c12a-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="7c12a-113">**Element**</span></span>|<span data-ttu-id="7c12a-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="7c12a-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7c12a-115">Значения</span><span class="sxs-lookup"><span data-stu-id="7c12a-115">Values</span></span>](values.md) <br/> |<span data-ttu-id="7c12a-116">Содержит коллекцию значений для расширенного свойства.</span><span class="sxs-lookup"><span data-stu-id="7c12a-116">Contains a collection of values for an extended property.</span></span>  <br/> |
|[<span data-ttu-id="7c12a-117">ExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="7c12a-117">ExtendedProperty</span></span>](extendedproperty.md) <br/> |<span data-ttu-id="7c12a-118">Определяет расширенные свойства для папок и элементов.</span><span class="sxs-lookup"><span data-stu-id="7c12a-118">Identifies extended properties on folders and items.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="7c12a-119">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="7c12a-119">Text value</span></span>

<span data-ttu-id="7c12a-120">Текстовое значение должно быть совместимо с типом, указанным в атрибуте PropertyType объекта Екстендедфиелдури.</span><span class="sxs-lookup"><span data-stu-id="7c12a-120">The text value must be compatible with the type that is indicated by the PropertyType attribute of the ExtendedFieldURI.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="7c12a-121">Примечания</span><span class="sxs-lookup"><span data-stu-id="7c12a-121">Remarks</span></span>

<span data-ttu-id="7c12a-122">Элемент **value** может находиться в экземплярах расширенных свойств с одним и многозначным.</span><span class="sxs-lookup"><span data-stu-id="7c12a-122">A **Value** element can occur in both single and multivalued extended property instances.</span></span> <span data-ttu-id="7c12a-123">Для экземпляров с одним значением он существует как прямой дочерний элемент элемента [ExtendedProperty](extendedproperty.md) .</span><span class="sxs-lookup"><span data-stu-id="7c12a-123">For single-valued instances, it exists as a direct child of the [ExtendedProperty](extendedproperty.md) element.</span></span> <span data-ttu-id="7c12a-124">Для многозначного экземпляра он существует как прямой дочерний объект коллекции **Values** .</span><span class="sxs-lookup"><span data-stu-id="7c12a-124">For multivalued instance, it exists as a direct child of the **Values** collection.</span></span> 
  
<span data-ttu-id="7c12a-125">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="7c12a-125">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7c12a-126">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="7c12a-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7c12a-127">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="7c12a-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="7c12a-128">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="7c12a-128">Schema Name</span></span>  <br/> |<span data-ttu-id="7c12a-129">Схема Types</span><span class="sxs-lookup"><span data-stu-id="7c12a-129">Types schema</span></span>  <br/> |
|<span data-ttu-id="7c12a-130">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="7c12a-130">Validation File</span></span>  <br/> |<span data-ttu-id="7c12a-131">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="7c12a-131">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="7c12a-132">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="7c12a-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="7c12a-133">False</span><span class="sxs-lookup"><span data-stu-id="7c12a-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7c12a-134">См. также</span><span class="sxs-lookup"><span data-stu-id="7c12a-134">See also</span></span>

- [<span data-ttu-id="7c12a-135">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="7c12a-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

