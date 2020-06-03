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
ms.openlocfilehash: f05be466d05b13f8f362afb5fc0552653a532475
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458812"
---
# <a name="bitmask"></a><span data-ttu-id="4f5e3-103">Маски</span><span class="sxs-lookup"><span data-stu-id="4f5e3-103">Bitmask</span></span>

<span data-ttu-id="4f5e3-104">Элемент **Битовая** маска представляет шестнадцатеричную или десятичную маску, используемую во время операции ограничения [исключений](excludes.md) .</span><span class="sxs-lookup"><span data-stu-id="4f5e3-104">The **Bitmask** element represents a hexadecimal or decimal mask to be used during an [Excludes](excludes.md) restriction operation.</span></span> 
  
```xml
<Bitmask Value="" />
```

<span data-ttu-id="4f5e3-105">**ексклудесвалуетипе**</span><span class="sxs-lookup"><span data-stu-id="4f5e3-105">**ExcludesValueType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="4f5e3-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="4f5e3-106">Attributes and elements</span></span>

<span data-ttu-id="4f5e3-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="4f5e3-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4f5e3-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="4f5e3-108">Attributes</span></span>

|<span data-ttu-id="4f5e3-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="4f5e3-109">**Attribute**</span></span>|<span data-ttu-id="4f5e3-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="4f5e3-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="4f5e3-111">**Значение**</span><span class="sxs-lookup"><span data-stu-id="4f5e3-111">**Value**</span></span> | <span data-ttu-id="4f5e3-112">Представляет десятичную или шестнадцатеричную битовую маску.</span><span class="sxs-lookup"><span data-stu-id="4f5e3-112">Represents a decimal or hexadecimal bitmask.</span></span> <span data-ttu-id="4f5e3-113">Значение представлено следующим регулярным выражением:</span><span class="sxs-lookup"><span data-stu-id="4f5e3-113">The value is represented by the following regular expression:</span></span><br/><span data-ttu-id="4f5e3-114">`((0x|0X)[0-9A-Fa-f]*)|([0-9]*)`.</span><span class="sxs-lookup"><span data-stu-id="4f5e3-114">`((0x|0X)[0-9A-Fa-f]*)|([0-9]*)`.</span></span><br/><br/><span data-ttu-id="4f5e3-115">Ниже приведены примеры шестнадцатеричных значений для этого атрибута.</span><span class="sxs-lookup"><span data-stu-id="4f5e3-115">The following are examples of hexadecimal values for this attribute:</span></span><br/><span data-ttu-id="4f5e3-116">- 0x12AF</span><span class="sxs-lookup"><span data-stu-id="4f5e3-116">- 0x12AF</span></span><br/><span data-ttu-id="4f5e3-117">- 0X334AE</span><span class="sxs-lookup"><span data-stu-id="4f5e3-117">- 0X334AE</span></span><br/><br/><span data-ttu-id="4f5e3-118">Ниже приведены примеры десятичных значений для этого атрибута.</span><span class="sxs-lookup"><span data-stu-id="4f5e3-118">The following are examples of decimal values for this attribute:</span></span><br/><span data-ttu-id="4f5e3-119">– 10</span><span class="sxs-lookup"><span data-stu-id="4f5e3-119">- 10</span></span><br/><span data-ttu-id="4f5e3-120">— 255</span><span class="sxs-lookup"><span data-stu-id="4f5e3-120">- 255</span></span><br/><span data-ttu-id="4f5e3-121">— 4562</span><span class="sxs-lookup"><span data-stu-id="4f5e3-121">- 4562</span></span> |
   
### <a name="child-elements"></a><span data-ttu-id="4f5e3-122">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="4f5e3-122">Child elements</span></span>

<span data-ttu-id="4f5e3-123">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="4f5e3-123">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="4f5e3-124">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="4f5e3-124">Parent elements</span></span>

|<span data-ttu-id="4f5e3-125">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="4f5e3-125">**Element**</span></span>|<span data-ttu-id="4f5e3-126">**Описание**</span><span class="sxs-lookup"><span data-stu-id="4f5e3-126">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4f5e3-127">Исключает</span><span class="sxs-lookup"><span data-stu-id="4f5e3-127">Excludes</span></span>](excludes.md) <br/> |<span data-ttu-id="4f5e3-128">Выполняет битовую маску для свойств.</span><span class="sxs-lookup"><span data-stu-id="4f5e3-128">Performs a bitwise mask of the properties.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="4f5e3-129">Примечания</span><span class="sxs-lookup"><span data-stu-id="4f5e3-129">Remarks</span></span>

<span data-ttu-id="4f5e3-130">Шестнадцатеричные значения должны иметь префикс 0x или 0X.</span><span class="sxs-lookup"><span data-stu-id="4f5e3-130">Hexadecimal values must have a prefix of either 0x or 0X.</span></span> <span data-ttu-id="4f5e3-131">Если этот префикс не существует, предполагается, что значение равно десятичному числу.</span><span class="sxs-lookup"><span data-stu-id="4f5e3-131">If this prefix does not exist, the value is assumed to be a decimal number.</span></span>
  
<span data-ttu-id="4f5e3-132">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="4f5e3-132">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4f5e3-133">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="4f5e3-133">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4f5e3-134">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="4f5e3-134">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="4f5e3-135">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="4f5e3-135">Schema name</span></span>  <br/> |<span data-ttu-id="4f5e3-136">Схема Types</span><span class="sxs-lookup"><span data-stu-id="4f5e3-136">Types schema</span></span>  <br/> |
|<span data-ttu-id="4f5e3-137">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="4f5e3-137">Validation file</span></span>  <br/> |<span data-ttu-id="4f5e3-138">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="4f5e3-138">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="4f5e3-139">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="4f5e3-139">Can be empty</span></span>  <br/> |<span data-ttu-id="4f5e3-140">False</span><span class="sxs-lookup"><span data-stu-id="4f5e3-140">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="4f5e3-141">См. также</span><span class="sxs-lookup"><span data-stu-id="4f5e3-141">See also</span></span>

- [<span data-ttu-id="4f5e3-142">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="4f5e3-142">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

