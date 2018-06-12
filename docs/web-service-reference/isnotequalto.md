---
title: IsNotEqualTo
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsNotEqualTo
api_type:
- schema
ms.assetid: e2eff26c-3403-45cd-bb74-1eb98c7dbfcd
description: Элемент IsNotEqualTo представляет выражение поиска, которое сравнивает свойство с постоянным значением или другим свойством и возвращает значение true, если значения не совпадают.
ms.openlocfilehash: c11f5ba5b8c0672bba0b9ae2a76211ac7d5d94ad
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19834059"
---
# <a name="isnotequalto"></a><span data-ttu-id="838f4-103">IsNotEqualTo</span><span class="sxs-lookup"><span data-stu-id="838f4-103">IsNotEqualTo</span></span>

<span data-ttu-id="838f4-104">Элемент **IsNotEqualTo** представляет выражение поиска, которое сравнивает свойство с постоянным значением или другим свойством и возвращает **значение true,** Если значения не совпадают.</span><span class="sxs-lookup"><span data-stu-id="838f4-104">The **IsNotEqualTo** element represents a search expression that compares a property with either a constant value or another property and returns **true** if the values are not the same.</span></span> 
  
```xml
<IsNotEqualTo>
   <FieldURI/>
   <FieldURIOrConstant/>
</IsNotEqualTo>
```

 <span data-ttu-id="838f4-105">**IsNotEqualToType**</span><span class="sxs-lookup"><span data-stu-id="838f4-105">**IsNotEqualToType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="838f4-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="838f4-106">Attributes and elements</span></span>

<span data-ttu-id="838f4-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="838f4-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="838f4-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="838f4-108">Attributes</span></span>

<span data-ttu-id="838f4-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="838f4-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="838f4-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="838f4-110">Child elements</span></span>

|<span data-ttu-id="838f4-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="838f4-111">**Element**</span></span>|<span data-ttu-id="838f4-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="838f4-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="838f4-113">FieldURI</span><span class="sxs-lookup"><span data-stu-id="838f4-113">FieldURI</span></span>](fielduri.md) <br/> |<span data-ttu-id="838f4-114">Идентифицирует часто упоминаемые свойства по URI.</span><span class="sxs-lookup"><span data-stu-id="838f4-114">Identifies frequently referenced properties by URI.</span></span>  <br/> |
|[<span data-ttu-id="838f4-115">IndexedFieldURI</span><span class="sxs-lookup"><span data-stu-id="838f4-115">IndexedFieldURI</span></span>](indexedfielduri.md) <br/> |<span data-ttu-id="838f4-116">Идентифицирует отдельных элементов словаря.</span><span class="sxs-lookup"><span data-stu-id="838f4-116">Identifies individual members of a dictionary.</span></span>  <br/> |
|[<span data-ttu-id="838f4-117">ExtendedFieldURI</span><span class="sxs-lookup"><span data-stu-id="838f4-117">ExtendedFieldURI</span></span>](extendedfielduri.md) <br/> |<span data-ttu-id="838f4-118">Задает свойства MAPI.</span><span class="sxs-lookup"><span data-stu-id="838f4-118">Identifies MAPI properties.</span></span>  <br/> |
|[<span data-ttu-id="838f4-119">FieldURIOrConstant</span><span class="sxs-lookup"><span data-stu-id="838f4-119">FieldURIOrConstant</span></span>](fielduriorconstant.md) <br/> |<span data-ttu-id="838f4-120">Представляет свойство или постоянное значение для использования при сравнении с другого свойства.</span><span class="sxs-lookup"><span data-stu-id="838f4-120">Represents either a property or a constant value to be used when comparing with another property.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="838f4-121">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="838f4-121">Parent elements</span></span>

|<span data-ttu-id="838f4-122">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="838f4-122">**Element**</span></span>|<span data-ttu-id="838f4-123">**Описание**</span><span class="sxs-lookup"><span data-stu-id="838f4-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="838f4-124">Ограничения</span><span class="sxs-lookup"><span data-stu-id="838f4-124">Restriction</span></span>](restriction.md) <br/> |<span data-ttu-id="838f4-125">Представляет ограничение или запрос, используемый для фильтрации элементов или папок в папке операциях FindItem/FindFolder и поиска.</span><span class="sxs-lookup"><span data-stu-id="838f4-125">Represents the restriction or query that is used to filter items or folders in FindItem/FindFolder and search folder operations.</span></span>  <br/> |
|[<span data-ttu-id="838f4-126">Не</span><span class="sxs-lookup"><span data-stu-id="838f4-126">Not</span></span>](not.md) <br/> |<span data-ttu-id="838f4-127">Представляет выражение поиска, которое Инвертирует логическое значение выражения поиска, который он содержит.</span><span class="sxs-lookup"><span data-stu-id="838f4-127">Represents a search expression that negates the Boolean value of the search expression that it contains.</span></span>  <br/> |
|[<span data-ttu-id="838f4-128">И</span><span class="sxs-lookup"><span data-stu-id="838f4-128">And</span></span>](and.md) <br/> |<span data-ttu-id="838f4-129">Представляет выражение поиска, которое позволяет выполнять логическое и операции между двумя или более выражений для поиска.</span><span class="sxs-lookup"><span data-stu-id="838f4-129">Represents a search expression that allows you to perform a Boolean And operation between two or more search expressions.</span></span> <span data-ttu-id="838f4-130">Операции получается **значение true,** **Если все выражения поиска, содержащихся в And**.</span><span class="sxs-lookup"><span data-stu-id="838f4-130">The result of the And operation is **true** if all of the search expressions contained within the And are **true**.</span></span>  <br/> |
|[<span data-ttu-id="838f4-131">Или</span><span class="sxs-lookup"><span data-stu-id="838f4-131">Or</span></span>](or.md) <br/> |<span data-ttu-id="838f4-132">Представляет выражение поиска, используемая для выполнения логического или на нем выражением поиска.</span><span class="sxs-lookup"><span data-stu-id="838f4-132">Represents a search expression that performs a logical OR on the search expression that it contains.</span></span> <span data-ttu-id="838f4-133">[Или](or.md) возвращает **значение true,** Если какие-либо из их дочерних элементов возвращало **значение true**.</span><span class="sxs-lookup"><span data-stu-id="838f4-133">[Or](or.md) will return **true** if any of its children return **true**.</span></span> <span data-ttu-id="838f4-134">**Или** должен иметь два или несколько дочерних элементов.</span><span class="sxs-lookup"><span data-stu-id="838f4-134">**Or** must have two or more children.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="838f4-135">Замечания</span><span class="sxs-lookup"><span data-stu-id="838f4-135">Remarks</span></span>

<span data-ttu-id="838f4-136">Для выполнения сравнения строк, рекомендуется использовать элемент [Contains](contains.md) , как она предоставляет параметры для соответствия параметров, таких как case и пробела.</span><span class="sxs-lookup"><span data-stu-id="838f4-136">To perform string comparisons, consider using the [Contains](contains.md) element, as it provides options for matching parameters such as case and white space.</span></span> <span data-ttu-id="838f4-137">Используйте элемент [не](not.md) в сочетании с элемент [Contains](contains.md) для отрицания результат.</span><span class="sxs-lookup"><span data-stu-id="838f4-137">Use the [Not](not.md) element in conjunction with the [Contains](contains.md) element to negate the result.</span></span> 
  
<span data-ttu-id="838f4-138">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="838f4-138">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="838f4-139">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="838f4-139">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="838f4-140">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="838f4-140">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="838f4-141">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="838f4-141">Schema Name</span></span>  <br/> |<span data-ttu-id="838f4-142">Схема Types</span><span class="sxs-lookup"><span data-stu-id="838f4-142">Types schema</span></span>  <br/> |
|<span data-ttu-id="838f4-143">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="838f4-143">Validation File</span></span>  <br/> |<span data-ttu-id="838f4-144">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="838f4-144">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="838f4-145">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="838f4-145">Can be Empty</span></span>  <br/> |<span data-ttu-id="838f4-146">False</span><span class="sxs-lookup"><span data-stu-id="838f4-146">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="838f4-147">См. также</span><span class="sxs-lookup"><span data-stu-id="838f4-147">See also</span></span>



- [<span data-ttu-id="838f4-148">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="838f4-148">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

