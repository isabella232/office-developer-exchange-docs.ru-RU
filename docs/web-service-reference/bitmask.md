---
title: Маски
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
description: Элемент битовая маска представляет шестнадцатеричную или десятичную маску, используемую во время операции ограничения исключений.
ms.openlocfilehash: 86c8c61f22d8d620a9139280b2a43ed7fec4727d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761575"
---
# <a name="bitmask"></a><span data-ttu-id="f047a-103">Маски</span><span class="sxs-lookup"><span data-stu-id="f047a-103">Bitmask</span></span>

<span data-ttu-id="f047a-104">Элемент **Битовая** маска представляет шестнадцатеричную или десятичную маску, используемую во время операции ограничения [исключений](excludes.md) .</span><span class="sxs-lookup"><span data-stu-id="f047a-104">The **Bitmask** element represents a hexadecimal or decimal mask to be used during an [Excludes](excludes.md) restriction operation.</span></span> 
  
```xml
<Bitmask Value="" />
```

<span data-ttu-id="f047a-105">**ексклудесвалуетипе**</span><span class="sxs-lookup"><span data-stu-id="f047a-105">**ExcludesValueType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="f047a-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="f047a-106">Attributes and elements</span></span>

<span data-ttu-id="f047a-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="f047a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f047a-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="f047a-108">Attributes</span></span>

|<span data-ttu-id="f047a-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="f047a-109">**Attribute**</span></span>|<span data-ttu-id="f047a-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="f047a-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="f047a-111">**Значение**</span><span class="sxs-lookup"><span data-stu-id="f047a-111">**Value**</span></span> | <span data-ttu-id="f047a-112">Представляет десятичную или шестнадцатеричную битовую маску.</span><span class="sxs-lookup"><span data-stu-id="f047a-112">Represents a decimal or hexadecimal bitmask.</span></span> <span data-ttu-id="f047a-113">Значение представлено следующим регулярным выражением:</span><span class="sxs-lookup"><span data-stu-id="f047a-113">The value is represented by the following regular expression:</span></span><br/><span data-ttu-id="f047a-114">"((0x</span><span class="sxs-lookup"><span data-stu-id="f047a-114">\`((0x</span></span>|<span data-ttu-id="f047a-115">0X) [0-9A-Fa-f] \*)</span><span class="sxs-lookup"><span data-stu-id="f047a-115">0X)[0-9A-Fa-f]\*)</span></span>|<span data-ttu-id="f047a-116">([0-9] \*) '.</span><span class="sxs-lookup"><span data-stu-id="f047a-116">([0-9]\*)\`.</span></span><br/><br/><span data-ttu-id="f047a-117">Ниже приведены примеры шестнадцатеричных значений для этого атрибута.</span><span class="sxs-lookup"><span data-stu-id="f047a-117">The following are examples of hexadecimal values for this attribute:</span></span><br/><span data-ttu-id="f047a-118">- 0x12AF</span><span class="sxs-lookup"><span data-stu-id="f047a-118">- 0x12AF</span></span><br/><span data-ttu-id="f047a-119">- 0X334AE</span><span class="sxs-lookup"><span data-stu-id="f047a-119">- 0X334AE</span></span><br/><br/><span data-ttu-id="f047a-120">Ниже приведены примеры десятичных значений для этого атрибута.</span><span class="sxs-lookup"><span data-stu-id="f047a-120">The following are examples of decimal values for this attribute:</span></span><br/><span data-ttu-id="f047a-121">– 10</span><span class="sxs-lookup"><span data-stu-id="f047a-121">- 10</span></span><br/><span data-ttu-id="f047a-122">— 255</span><span class="sxs-lookup"><span data-stu-id="f047a-122">- 255</span></span><br/><span data-ttu-id="f047a-123">— 4562</span><span class="sxs-lookup"><span data-stu-id="f047a-123">- 4562</span></span> |
   
### <a name="child-elements"></a><span data-ttu-id="f047a-124">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="f047a-124">Child elements</span></span>

<span data-ttu-id="f047a-125">Нет.</span><span class="sxs-lookup"><span data-stu-id="f047a-125">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="f047a-126">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="f047a-126">Parent elements</span></span>

|<span data-ttu-id="f047a-127">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="f047a-127">**Element**</span></span>|<span data-ttu-id="f047a-128">**Описание**</span><span class="sxs-lookup"><span data-stu-id="f047a-128">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f047a-129">Исключает</span><span class="sxs-lookup"><span data-stu-id="f047a-129">Excludes</span></span>](excludes.md) <br/> |<span data-ttu-id="f047a-130">Выполняет битовую маску для свойств.</span><span class="sxs-lookup"><span data-stu-id="f047a-130">Performs a bitwise mask of the properties.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="f047a-131">Примечания</span><span class="sxs-lookup"><span data-stu-id="f047a-131">Remarks</span></span>

<span data-ttu-id="f047a-132">Шестнадцатеричные значения должны иметь префикс 0x или 0X.</span><span class="sxs-lookup"><span data-stu-id="f047a-132">Hexadecimal values must have a prefix of either 0x or 0X.</span></span> <span data-ttu-id="f047a-133">Если этот префикс не существует, предполагается, что значение равно десятичному числу.</span><span class="sxs-lookup"><span data-stu-id="f047a-133">If this prefix does not exist, the value is assumed to be a decimal number.</span></span>
  
<span data-ttu-id="f047a-134">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="f047a-134">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f047a-135">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="f047a-135">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f047a-136">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="f047a-136">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="f047a-137">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="f047a-137">Schema name</span></span>  <br/> |<span data-ttu-id="f047a-138">Схема Types</span><span class="sxs-lookup"><span data-stu-id="f047a-138">Types schema</span></span>  <br/> |
|<span data-ttu-id="f047a-139">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="f047a-139">Validation file</span></span>  <br/> |<span data-ttu-id="f047a-140">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="f047a-140">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="f047a-141">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="f047a-141">Can be empty</span></span>  <br/> |<span data-ttu-id="f047a-142">False</span><span class="sxs-lookup"><span data-stu-id="f047a-142">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f047a-143">См. также</span><span class="sxs-lookup"><span data-stu-id="f047a-143">See also</span></span>

- [<span data-ttu-id="f047a-144">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="f047a-144">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

