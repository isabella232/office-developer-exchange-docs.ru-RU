---
title: Выражение IsEqualTo
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsEqualTo
api_type:
- schema
ms.assetid: 48e7e067-049c-4184-8026-071e6f558e8a
description: Выражение IsEqualTo элемент представляет выражение поиска, которое сравнивает свойство с постоянным значением или другим свойством и возвращает значение true, если они равны.
ms.openlocfilehash: a7a7deed79c271be74bb2ff16dd86605d468721b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19834013"
---
# <a name="isequalto"></a><span data-ttu-id="e8b66-103">Выражение IsEqualTo</span><span class="sxs-lookup"><span data-stu-id="e8b66-103">IsEqualTo</span></span>

<span data-ttu-id="e8b66-104">**Выражение IsEqualTo** элемент представляет выражение поиска, которое сравнивает свойство с постоянным значением или другим свойством и возвращает значение true, если они равны.</span><span class="sxs-lookup"><span data-stu-id="e8b66-104">The **IsEqualTo** element represents a search expression that compares a property with either a constant value or another property and evaluates to true if they are equal.</span></span> 
  
```xml
<IsEqualTo>
   <FieldURI/>
   <FieldURIOrConstant/>
</IsEqualTo>
```

 <span data-ttu-id="e8b66-105">**IsEqualToType**</span><span class="sxs-lookup"><span data-stu-id="e8b66-105">**IsEqualToType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e8b66-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="e8b66-106">Attributes and elements</span></span>

<span data-ttu-id="e8b66-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="e8b66-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e8b66-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="e8b66-108">Attributes</span></span>

<span data-ttu-id="e8b66-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="e8b66-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e8b66-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="e8b66-110">Child elements</span></span>

|<span data-ttu-id="e8b66-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="e8b66-111">**Element**</span></span>|<span data-ttu-id="e8b66-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="e8b66-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e8b66-113">FieldURI</span><span class="sxs-lookup"><span data-stu-id="e8b66-113">FieldURI</span></span>](fielduri.md) <br/> |<span data-ttu-id="e8b66-114">Идентифицирует часто упоминаемые свойства по URI.</span><span class="sxs-lookup"><span data-stu-id="e8b66-114">Identifies frequently referenced properties by URI.</span></span>  <br/> |
|[<span data-ttu-id="e8b66-115">IndexedFieldURI</span><span class="sxs-lookup"><span data-stu-id="e8b66-115">IndexedFieldURI</span></span>](indexedfielduri.md) <br/> |<span data-ttu-id="e8b66-116">Идентифицирует отдельных элементов словаря.</span><span class="sxs-lookup"><span data-stu-id="e8b66-116">Identifies individual members of a dictionary.</span></span>  <br/> |
|[<span data-ttu-id="e8b66-117">ExtendedFieldURI</span><span class="sxs-lookup"><span data-stu-id="e8b66-117">ExtendedFieldURI</span></span>](extendedfielduri.md) <br/> |<span data-ttu-id="e8b66-118">Задает свойства MAPI.</span><span class="sxs-lookup"><span data-stu-id="e8b66-118">Identifies MAPI properties.</span></span>  <br/> |
|[<span data-ttu-id="e8b66-119">FieldURIOrConstant</span><span class="sxs-lookup"><span data-stu-id="e8b66-119">FieldURIOrConstant</span></span>](fielduriorconstant.md) <br/> |<span data-ttu-id="e8b66-120">Представляет свойство или постоянное значение для использования при сравнении с другого свойства.</span><span class="sxs-lookup"><span data-stu-id="e8b66-120">Represents either a property or a constant value to be used when comparing with another property.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="e8b66-121">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="e8b66-121">Parent elements</span></span>

|<span data-ttu-id="e8b66-122">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="e8b66-122">**Element**</span></span>|<span data-ttu-id="e8b66-123">**Описание**</span><span class="sxs-lookup"><span data-stu-id="e8b66-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e8b66-124">Ограничения</span><span class="sxs-lookup"><span data-stu-id="e8b66-124">Restriction</span></span>](restriction.md) <br/> |<span data-ttu-id="e8b66-125">Представляет ограничение или запрос, используемый для фильтрации элементов или папок в папке операциях FindItem/FindFolder и поиска.</span><span class="sxs-lookup"><span data-stu-id="e8b66-125">Represents the restriction or query that is used to filter items or folders in FindItem/FindFolder and search folder operations.</span></span>  <br/> |
|[<span data-ttu-id="e8b66-126">Не</span><span class="sxs-lookup"><span data-stu-id="e8b66-126">Not</span></span>](not.md) <br/> |<span data-ttu-id="e8b66-127">Представляет выражение поиска, которое Инвертирует логическое значение выражения поиска, который он содержит.</span><span class="sxs-lookup"><span data-stu-id="e8b66-127">Represents a search expression that negates the Boolean value of the search expression that it contains.</span></span>  <br/> |
|[<span data-ttu-id="e8b66-128">И</span><span class="sxs-lookup"><span data-stu-id="e8b66-128">And</span></span>](and.md) <br/> |<span data-ttu-id="e8b66-129">Представляет выражение поиска, которое позволяет выполнять логическое и операции между двумя или более выражений для поиска.</span><span class="sxs-lookup"><span data-stu-id="e8b66-129">Represents a search expression that allows you to perform a Boolean And operation between two or more search expressions.</span></span> <span data-ttu-id="e8b66-130">Операции получается **значение true,** **Если все выражения поиска, содержащихся в And**.</span><span class="sxs-lookup"><span data-stu-id="e8b66-130">The result of the And operation is **true** if all of the search expressions contained within the And are **true**.</span></span>  <br/> |
|[<span data-ttu-id="e8b66-131">Или</span><span class="sxs-lookup"><span data-stu-id="e8b66-131">Or</span></span>](or.md) <br/> |<span data-ttu-id="e8b66-132">Представляет выражение поиска, используемая для выполнения логического или на нем выражением поиска.</span><span class="sxs-lookup"><span data-stu-id="e8b66-132">Represents a search expression that performs a logical OR on the search expression that it contains.</span></span> <span data-ttu-id="e8b66-133">[Или](or.md) возвращает значение true, если какие-либо из их дочерних элементов возвращало значение true.</span><span class="sxs-lookup"><span data-stu-id="e8b66-133">[Or](or.md) will return true if any of its children return true.</span></span> <span data-ttu-id="e8b66-134">**Или** должен иметь два или несколько дочерних элементов.</span><span class="sxs-lookup"><span data-stu-id="e8b66-134">**Or** must have two or more children.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="e8b66-135">Замечания</span><span class="sxs-lookup"><span data-stu-id="e8b66-135">Remarks</span></span>

<span data-ttu-id="e8b66-136">Для выполнения сравнения строк, рекомендуется использовать элемент [Contains](contains.md) , как она предоставляет параметры для соответствия параметров, таких как case и пробела.</span><span class="sxs-lookup"><span data-stu-id="e8b66-136">To perform string comparisons, consider using the [Contains](contains.md) element, as it provides options for matching parameters, such as case and white space.</span></span> <span data-ttu-id="e8b66-137">Используйте элемент [не](not.md) в сочетании с элемент [Contains](contains.md) для отрицания результат.</span><span class="sxs-lookup"><span data-stu-id="e8b66-137">Use the [Not](not.md) element in conjunction with the [Contains](contains.md) element to negate the result.</span></span> 
  
<span data-ttu-id="e8b66-138">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="e8b66-138">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e8b66-139">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="e8b66-139">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e8b66-140">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="e8b66-140">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="e8b66-141">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="e8b66-141">Schema Name</span></span>  <br/> |<span data-ttu-id="e8b66-142">Схема Types</span><span class="sxs-lookup"><span data-stu-id="e8b66-142">Types schema</span></span>  <br/> |
|<span data-ttu-id="e8b66-143">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="e8b66-143">Validation File</span></span>  <br/> |<span data-ttu-id="e8b66-144">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="e8b66-144">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="e8b66-145">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="e8b66-145">Can be Empty</span></span>  <br/> |<span data-ttu-id="e8b66-146">False</span><span class="sxs-lookup"><span data-stu-id="e8b66-146">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e8b66-147">См. также</span><span class="sxs-lookup"><span data-stu-id="e8b66-147">See also</span></span>



- [<span data-ttu-id="e8b66-148">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="e8b66-148">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

