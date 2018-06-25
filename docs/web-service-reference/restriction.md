---
title: Ограничение
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Restriction
api_type:
- schema
ms.assetid: 77f19014-d112-4999-8e83-ecc32a117a73
description: Ограничение элемент представляет ограничение или запрос, используемый для фильтрации элементов или папок в папке операциях FindItem/FindFolder и поиска.
ms.openlocfilehash: 6b5702696db29910ae476a370bf362fe6a036ae7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835213"
---
# <a name="restriction"></a><span data-ttu-id="b0c96-103">Ограничение</span><span class="sxs-lookup"><span data-stu-id="b0c96-103">Restriction</span></span>

<span data-ttu-id="b0c96-104">**Ограничение** элемент представляет ограничение или запрос, используемый для фильтрации элементов или папок в папке операциях FindItem/FindFolder и поиска.</span><span class="sxs-lookup"><span data-stu-id="b0c96-104">The **Restriction** element represents the restriction or query that is used to filter items or folders in FindItem/FindFolder and search folder operations.</span></span> 
  
```xml
<Restriction>
   <SearchExpression/>
</Restriction>
```

 <span data-ttu-id="b0c96-105">**RestrictionType**</span><span class="sxs-lookup"><span data-stu-id="b0c96-105">**RestrictionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b0c96-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="b0c96-106">Attributes and elements</span></span>

<span data-ttu-id="b0c96-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="b0c96-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b0c96-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="b0c96-108">Attributes</span></span>

<span data-ttu-id="b0c96-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="b0c96-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b0c96-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="b0c96-110">Child elements</span></span>

|<span data-ttu-id="b0c96-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="b0c96-111">**Element**</span></span>|<span data-ttu-id="b0c96-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="b0c96-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b0c96-113">И</span><span class="sxs-lookup"><span data-stu-id="b0c96-113">And</span></span>](and.md) <br/> |<span data-ttu-id="b0c96-114">Представляет выражение поиска, которое позволяет выполнять операцию логическое **AND** между двумя или более выражений для поиска.</span><span class="sxs-lookup"><span data-stu-id="b0c96-114">Represents a search expression that enables you to perform a Boolean **AND** operation between two or more search expressions.</span></span>  <br/> |
|[<span data-ttu-id="b0c96-115">Contains</span><span class="sxs-lookup"><span data-stu-id="b0c96-115">Contains</span></span>](contains.md) <br/> |<span data-ttu-id="b0c96-116">Представляет выражение поиска, которое определяет, содержит ли данное свойство указанную константу строчного типа.</span><span class="sxs-lookup"><span data-stu-id="b0c96-116">Represents a search expression that determines whether a given property contains the supplied constant string value.</span></span>  <br/> |
|[<span data-ttu-id="b0c96-117">Исключает</span><span class="sxs-lookup"><span data-stu-id="b0c96-117">Excludes</span></span>](excludes.md) <br/> |<span data-ttu-id="b0c96-118">Выполняет битовую маску свойства.</span><span class="sxs-lookup"><span data-stu-id="b0c96-118">Performs a bitwise mask of the properties.</span></span>  <br/> |
|[<span data-ttu-id="b0c96-119">Существует</span><span class="sxs-lookup"><span data-stu-id="b0c96-119">Exists</span></span>](exists.md) <br/> |<span data-ttu-id="b0c96-120">Представляет выражение поиска, которое возвращает **значение true, если существует указанное свойство элемента** .</span><span class="sxs-lookup"><span data-stu-id="b0c96-120">Represents a search expression that returns **true** if the supplied property exists on an item.</span></span>  <br/> |
|[<span data-ttu-id="b0c96-121">Выражение IsEqualTo</span><span class="sxs-lookup"><span data-stu-id="b0c96-121">IsEqualTo</span></span>](isequalto.md) <br/> |<span data-ttu-id="b0c96-122">Представляет выражение поиска, которое сравнивает свойство с постоянным значением или другим свойством и имеет значение **true** , если они равны.</span><span class="sxs-lookup"><span data-stu-id="b0c96-122">Represents a search expression that compares a property with either a constant value or another property and evaluates to **true** if they are equal.</span></span>  <br/> |
|[<span data-ttu-id="b0c96-123">IsGreaterThan</span><span class="sxs-lookup"><span data-stu-id="b0c96-123">IsGreaterThan</span></span>](isgreaterthan.md) <br/> |<span data-ttu-id="b0c96-124">Представляет выражение поиска, которое сравнивает свойство с постоянным значением или другим свойством и возвращает **значение true,** Если первое свойство больше, чем значение или свойство.</span><span class="sxs-lookup"><span data-stu-id="b0c96-124">Represents a search expression that compares a property with either a constant value or another property and returns **true** if the first property is greater than the value or property.</span></span>  <br/> |
|[<span data-ttu-id="b0c96-125">IsGreaterThanOrEqualTo</span><span class="sxs-lookup"><span data-stu-id="b0c96-125">IsGreaterThanOrEqualTo</span></span>](isgreaterthanorequalto.md) <br/> |<span data-ttu-id="b0c96-126">Представляет выражение поиска, которое сравнивает свойство с постоянным значением или другим свойством и возвращает **значение true,** Если первое свойство больше или равно значению или свойство.</span><span class="sxs-lookup"><span data-stu-id="b0c96-126">Represents a search expression that compares a property with either a constant value or another property and returns **true** if the first property is greater than or equal to the value or property.</span></span>  <br/> |
|[<span data-ttu-id="b0c96-127">IsLessThan</span><span class="sxs-lookup"><span data-stu-id="b0c96-127">IsLessThan</span></span>](islessthan.md) <br/> |<span data-ttu-id="b0c96-128">Представляет выражение поиска, которое сравнивает свойство с постоянным значением или другим свойством и возвращает **значение true,** Если первое свойство меньше значения или свойства.</span><span class="sxs-lookup"><span data-stu-id="b0c96-128">Represents a search expression that compares a property with either a constant value or another property and returns **true** if the first property is less than the value or property.</span></span>  <br/> |
|[<span data-ttu-id="b0c96-129">IsLessThanOrEqualTo</span><span class="sxs-lookup"><span data-stu-id="b0c96-129">IsLessThanOrEqualTo</span></span>](islessthanorequalto.md) <br/> |<span data-ttu-id="b0c96-130">Представляет выражение поиска, которое сравнивает свойство с постоянным значением или другим свойством и возвращает **значение true,** Если первое свойство меньше или равно значению или свойство.</span><span class="sxs-lookup"><span data-stu-id="b0c96-130">Represents a search expression that compares a property with either a constant value or another property and returns **true** if the first property is less than or equal to the value or property.</span></span>  <br/> |
|[<span data-ttu-id="b0c96-131">IsNotEqualTo</span><span class="sxs-lookup"><span data-stu-id="b0c96-131">IsNotEqualTo</span></span>](isnotequalto.md) <br/> |<span data-ttu-id="b0c96-132">Представляет выражение поиска, которое сравнивает свойство с постоянным значением или другим свойством и возвращает **значение true,** Если значения не совпадают.</span><span class="sxs-lookup"><span data-stu-id="b0c96-132">Represents a search expression that compares a property with either a constant value or another property and returns **true** if the values are not the same.</span></span>  <br/> |
|[<span data-ttu-id="b0c96-133">Не</span><span class="sxs-lookup"><span data-stu-id="b0c96-133">Not</span></span>](not.md) <br/> |<span data-ttu-id="b0c96-134">Представляет выражение поиска, которое Инвертирует логическое значение выражения поиска, которые он содержит.</span><span class="sxs-lookup"><span data-stu-id="b0c96-134">Represents a search expression that negates the Boolean value of the search expression it contains.</span></span>  <br/> |
|[<span data-ttu-id="b0c96-135">Или</span><span class="sxs-lookup"><span data-stu-id="b0c96-135">Or</span></span>](or.md) <br/> |<span data-ttu-id="b0c96-136">Представляет выражение поиска, которое выполняет операцию логической **или** выражения поиска, которые он содержит.</span><span class="sxs-lookup"><span data-stu-id="b0c96-136">Represents a search expression that performs a logical **OR** operation on the search expression it contains.</span></span> <span data-ttu-id="b0c96-137">Элемент **или** возвращает **значение true** , если какие-либо из их дочерних элементов возвращало **значение true**.</span><span class="sxs-lookup"><span data-stu-id="b0c96-137">The **Or** element will return **true** if any of its children return **true**.</span></span>  <br/> |
|[<span data-ttu-id="b0c96-138">SearchExpression</span><span class="sxs-lookup"><span data-stu-id="b0c96-138">SearchExpression</span></span>](searchexpression.md) <br/> |<span data-ttu-id="b0c96-139">Представляет Замещающий элемент в ограничении.</span><span class="sxs-lookup"><span data-stu-id="b0c96-139">Represents the substituted element within a restriction.</span></span> <span data-ttu-id="b0c96-140">Этот элемент не используется в экземпляре документа XML.</span><span class="sxs-lookup"><span data-stu-id="b0c96-140">This element is not used in an XML instance document.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="b0c96-141">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="b0c96-141">Parent elements</span></span>

|<span data-ttu-id="b0c96-142">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="b0c96-142">**Element**</span></span>|<span data-ttu-id="b0c96-143">**Описание**</span><span class="sxs-lookup"><span data-stu-id="b0c96-143">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b0c96-144">FindFolder</span><span class="sxs-lookup"><span data-stu-id="b0c96-144">FindFolder</span></span>](findfolder.md) <br/> |<span data-ttu-id="b0c96-145">Определяет запрос для определения папок в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="b0c96-145">Defines a request to identify folders in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="b0c96-146">FindItem</span><span class="sxs-lookup"><span data-stu-id="b0c96-146">FindItem</span></span>](finditem.md) <br/> |<span data-ttu-id="b0c96-147">Определяет запрос для поиска элементов в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="b0c96-147">Defines a request to find items in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="b0c96-148">SearchParameters</span><span class="sxs-lookup"><span data-stu-id="b0c96-148">SearchParameters</span></span>](searchparameters.md) <br/> |<span data-ttu-id="b0c96-149">Представляет параметры, определяющие папки поиска.</span><span class="sxs-lookup"><span data-stu-id="b0c96-149">Represents the parameters that define a search folder.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="b0c96-150">Замечания</span><span class="sxs-lookup"><span data-stu-id="b0c96-150">Remarks</span></span>

<span data-ttu-id="b0c96-151">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="b0c96-151">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b0c96-152">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="b0c96-152">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b0c96-153">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="b0c96-153">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="b0c96-154">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="b0c96-154">Schema Name</span></span>  <br/> |<span data-ttu-id="b0c96-155">Схема Types</span><span class="sxs-lookup"><span data-stu-id="b0c96-155">Types schema</span></span>  <br/> |
|<span data-ttu-id="b0c96-156">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="b0c96-156">Validation File</span></span>  <br/> |<span data-ttu-id="b0c96-157">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="b0c96-157">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="b0c96-158">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="b0c96-158">Can be Empty</span></span>  <br/> |<span data-ttu-id="b0c96-159">False</span><span class="sxs-lookup"><span data-stu-id="b0c96-159">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b0c96-160">См. также</span><span class="sxs-lookup"><span data-stu-id="b0c96-160">See also</span></span>



- [<span data-ttu-id="b0c96-161">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="b0c96-161">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

