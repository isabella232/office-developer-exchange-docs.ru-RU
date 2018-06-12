---
title: Битовая маска
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Bitmask
api_type:
- schema
ms.assetid: fc7eeac2-555f-4cbc-8b48-26d9ed67748a
description: Элемент Битовая маска представляет шестнадцатеричном или десятичном маска для использования во время операции ограничения Excludes.
ms.openlocfilehash: 86c8c61f22d8d620a9139280b2a43ed7fec4727d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761575"
---
# <a name="bitmask"></a><span data-ttu-id="f87db-103">Битовая маска</span><span class="sxs-lookup"><span data-stu-id="f87db-103">Bitmask</span></span>

<span data-ttu-id="f87db-104">Элемент **Битовая маска** представляет шестнадцатеричном или десятичном маска для использования во время операции ограничения [Excludes](excludes.md) .</span><span class="sxs-lookup"><span data-stu-id="f87db-104">The **Bitmask** element represents a hexadecimal or decimal mask to be used during an [Excludes](excludes.md) restriction operation.</span></span> 
  
```xml
<Bitmask Value="" />
```

<span data-ttu-id="f87db-105">**ExcludesValueType**</span><span class="sxs-lookup"><span data-stu-id="f87db-105">**ExcludesValueType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="f87db-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="f87db-106">Attributes and elements</span></span>

<span data-ttu-id="f87db-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="f87db-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f87db-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="f87db-108">Attributes</span></span>

|<span data-ttu-id="f87db-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="f87db-109">**Attribute**</span></span>|<span data-ttu-id="f87db-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="f87db-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="f87db-111">**Значение**</span><span class="sxs-lookup"><span data-stu-id="f87db-111">**Value**</span></span> | <span data-ttu-id="f87db-112">Представляет decimal или шестнадцатеричную битовую маску.</span><span class="sxs-lookup"><span data-stu-id="f87db-112">Represents a decimal or hexadecimal bitmask.</span></span> <span data-ttu-id="f87db-113">Значение, представленное следующее регулярное выражение:</span><span class="sxs-lookup"><span data-stu-id="f87db-113">The value is represented by the following regular expression:</span></span><br/><span data-ttu-id="f87db-114">"((0 x</span><span class="sxs-lookup"><span data-stu-id="f87db-114">\`((0x</span></span>|<span data-ttu-id="f87db-115">0x)[0-9A-Fa-f]\*)</span><span class="sxs-lookup"><span data-stu-id="f87db-115">0X)[0-9A-Fa-f]\*)</span></span>|<span data-ttu-id="f87db-116">([0-9] \*) ".</span><span class="sxs-lookup"><span data-stu-id="f87db-116">([0-9]\*)\`.</span></span><br/><br/><span data-ttu-id="f87db-117">Ниже приведены примеры шестнадцатеричные значения этого атрибута.</span><span class="sxs-lookup"><span data-stu-id="f87db-117">The following are examples of hexadecimal values for this attribute:</span></span><br/><span data-ttu-id="f87db-118">-0x12AF</span><span class="sxs-lookup"><span data-stu-id="f87db-118">- 0x12AF</span></span><br/><span data-ttu-id="f87db-119">-0X334AE</span><span class="sxs-lookup"><span data-stu-id="f87db-119">- 0X334AE</span></span><br/><br/><span data-ttu-id="f87db-120">Ниже приведены примеры decimal значения этого атрибута.</span><span class="sxs-lookup"><span data-stu-id="f87db-120">The following are examples of decimal values for this attribute:</span></span><br/><span data-ttu-id="f87db-121">-10</span><span class="sxs-lookup"><span data-stu-id="f87db-121">- 10</span></span><br/><span data-ttu-id="f87db-122">-255</span><span class="sxs-lookup"><span data-stu-id="f87db-122">- 255</span></span><br/><span data-ttu-id="f87db-123">-4562</span><span class="sxs-lookup"><span data-stu-id="f87db-123">- 4562</span></span> |
   
### <a name="child-elements"></a><span data-ttu-id="f87db-124">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="f87db-124">Child elements</span></span>

<span data-ttu-id="f87db-125">Нет.</span><span class="sxs-lookup"><span data-stu-id="f87db-125">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="f87db-126">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="f87db-126">Parent elements</span></span>

|<span data-ttu-id="f87db-127">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="f87db-127">**Element**</span></span>|<span data-ttu-id="f87db-128">**Описание**</span><span class="sxs-lookup"><span data-stu-id="f87db-128">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f87db-129">Исключает</span><span class="sxs-lookup"><span data-stu-id="f87db-129">Excludes</span></span>](excludes.md) <br/> |<span data-ttu-id="f87db-130">Выполняет битовую маску свойства.</span><span class="sxs-lookup"><span data-stu-id="f87db-130">Performs a bitwise mask of the properties.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="f87db-131">Замечания</span><span class="sxs-lookup"><span data-stu-id="f87db-131">Remarks</span></span>

<span data-ttu-id="f87db-132">Шестнадцатеричные значения должны иметь префикс 0 x или 0 X.</span><span class="sxs-lookup"><span data-stu-id="f87db-132">Hexadecimal values must have a prefix of either 0x or 0X.</span></span> <span data-ttu-id="f87db-133">Если этот префикс не существует, значение считается десятичного числа.</span><span class="sxs-lookup"><span data-stu-id="f87db-133">If this prefix does not exist, the value is assumed to be a decimal number.</span></span>
  
<span data-ttu-id="f87db-134">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="f87db-134">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f87db-135">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="f87db-135">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f87db-136">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="f87db-136">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="f87db-137">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="f87db-137">Schema name</span></span>  <br/> |<span data-ttu-id="f87db-138">Схема Types</span><span class="sxs-lookup"><span data-stu-id="f87db-138">Types schema</span></span>  <br/> |
|<span data-ttu-id="f87db-139">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="f87db-139">Validation file</span></span>  <br/> |<span data-ttu-id="f87db-140">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="f87db-140">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="f87db-141">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="f87db-141">Can be empty</span></span>  <br/> |<span data-ttu-id="f87db-142">False</span><span class="sxs-lookup"><span data-stu-id="f87db-142">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f87db-143">См. также</span><span class="sxs-lookup"><span data-stu-id="f87db-143">See also</span></span>

- [<span data-ttu-id="f87db-144">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="f87db-144">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

