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
description: Элемент restriction представляет ограничение или запрос, используемый для фильтрации элементов или папок в операциях FindItem/FindFolder и папках поиска.
ms.openlocfilehash: 6037ba15417d67d393ca70f3edf2248749c396e1
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465291"
---
# <a name="restriction"></a><span data-ttu-id="c67ec-103">Ограничение</span><span class="sxs-lookup"><span data-stu-id="c67ec-103">Restriction</span></span>

<span data-ttu-id="c67ec-104">Элемент **restriction** представляет ограничение или запрос, используемый для фильтрации элементов или папок в операциях FindItem/FindFolder и папках поиска.</span><span class="sxs-lookup"><span data-stu-id="c67ec-104">The **Restriction** element represents the restriction or query that is used to filter items or folders in FindItem/FindFolder and search folder operations.</span></span> 
  
```xml
<Restriction>
   <SearchExpression/>
</Restriction>
```

 <span data-ttu-id="c67ec-105">**рестриктионтипе**</span><span class="sxs-lookup"><span data-stu-id="c67ec-105">**RestrictionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c67ec-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="c67ec-106">Attributes and elements</span></span>

<span data-ttu-id="c67ec-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="c67ec-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c67ec-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="c67ec-108">Attributes</span></span>

<span data-ttu-id="c67ec-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="c67ec-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c67ec-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="c67ec-110">Child elements</span></span>

|<span data-ttu-id="c67ec-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="c67ec-111">**Element**</span></span>|<span data-ttu-id="c67ec-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="c67ec-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c67ec-113">And</span><span class="sxs-lookup"><span data-stu-id="c67ec-113">And</span></span>](and.md) <br/> |<span data-ttu-id="c67ec-114">Представляет выражение поиска, которое позволяет выполнять логическое действие **и** операцию между двумя или более выражениями поиска.</span><span class="sxs-lookup"><span data-stu-id="c67ec-114">Represents a search expression that enables you to perform a Boolean **AND** operation between two or more search expressions.</span></span>  <br/> |
|[<span data-ttu-id="c67ec-115">Contains</span><span class="sxs-lookup"><span data-stu-id="c67ec-115">Contains</span></span>](contains.md) <br/> |<span data-ttu-id="c67ec-116">Представляет выражение поиска, которое определяет, содержит ли данное свойство предоставленное строковое значение константы.</span><span class="sxs-lookup"><span data-stu-id="c67ec-116">Represents a search expression that determines whether a given property contains the supplied constant string value.</span></span>  <br/> |
|[<span data-ttu-id="c67ec-117">Исключает</span><span class="sxs-lookup"><span data-stu-id="c67ec-117">Excludes</span></span>](excludes.md) <br/> |<span data-ttu-id="c67ec-118">Выполняет битовую маску для свойств.</span><span class="sxs-lookup"><span data-stu-id="c67ec-118">Performs a bitwise mask of the properties.</span></span>  <br/> |
|[<span data-ttu-id="c67ec-119">Exists</span><span class="sxs-lookup"><span data-stu-id="c67ec-119">Exists</span></span>](exists.md) <br/> |<span data-ttu-id="c67ec-120">Представляет выражение поиска, которое возвращает **значение true** , если указанное свойство существует для элемента.</span><span class="sxs-lookup"><span data-stu-id="c67ec-120">Represents a search expression that returns **true** if the supplied property exists on an item.</span></span>  <br/> |
|[<span data-ttu-id="c67ec-121">исекуалто</span><span class="sxs-lookup"><span data-stu-id="c67ec-121">IsEqualTo</span></span>](isequalto.md) <br/> |<span data-ttu-id="c67ec-122">Представляет выражение поиска, которое сравнивает свойство со значением константы или другим свойством и принимает **значение true** , если они равны.</span><span class="sxs-lookup"><span data-stu-id="c67ec-122">Represents a search expression that compares a property with either a constant value or another property and evaluates to **true** if they are equal.</span></span>  <br/> |
|[<span data-ttu-id="c67ec-123">исгреатерсан</span><span class="sxs-lookup"><span data-stu-id="c67ec-123">IsGreaterThan</span></span>](isgreaterthan.md) <br/> |<span data-ttu-id="c67ec-124">Представляет выражение поиска, которое сравнивает свойство со значением константы или другим свойством и возвращает **значение true** , если первое свойство больше значения или свойства.</span><span class="sxs-lookup"><span data-stu-id="c67ec-124">Represents a search expression that compares a property with either a constant value or another property and returns **true** if the first property is greater than the value or property.</span></span>  <br/> |
|[<span data-ttu-id="c67ec-125">исгреатерсанорекуалто</span><span class="sxs-lookup"><span data-stu-id="c67ec-125">IsGreaterThanOrEqualTo</span></span>](isgreaterthanorequalto.md) <br/> |<span data-ttu-id="c67ec-126">Представляет выражение поиска, которое сравнивает свойство со значением константы или другим свойством и возвращает **значение true** , если первое свойство больше или равно значению или свойству.</span><span class="sxs-lookup"><span data-stu-id="c67ec-126">Represents a search expression that compares a property with either a constant value or another property and returns **true** if the first property is greater than or equal to the value or property.</span></span>  <br/> |
|[<span data-ttu-id="c67ec-127">ислесссан</span><span class="sxs-lookup"><span data-stu-id="c67ec-127">IsLessThan</span></span>](islessthan.md) <br/> |<span data-ttu-id="c67ec-128">Представляет выражение поиска, которое сравнивает свойство со значением константы или другим свойством и возвращает **значение true** , если первое свойство меньше значения или свойства.</span><span class="sxs-lookup"><span data-stu-id="c67ec-128">Represents a search expression that compares a property with either a constant value or another property and returns **true** if the first property is less than the value or property.</span></span>  <br/> |
|[<span data-ttu-id="c67ec-129">ислесссанорекуалто</span><span class="sxs-lookup"><span data-stu-id="c67ec-129">IsLessThanOrEqualTo</span></span>](islessthanorequalto.md) <br/> |<span data-ttu-id="c67ec-130">Представляет выражение поиска, которое сравнивает свойство со значением константы или другим свойством и возвращает **значение true** , если первое свойство меньше или равно значению или свойству.</span><span class="sxs-lookup"><span data-stu-id="c67ec-130">Represents a search expression that compares a property with either a constant value or another property and returns **true** if the first property is less than or equal to the value or property.</span></span>  <br/> |
|[<span data-ttu-id="c67ec-131">иснотекуалто</span><span class="sxs-lookup"><span data-stu-id="c67ec-131">IsNotEqualTo</span></span>](isnotequalto.md) <br/> |<span data-ttu-id="c67ec-132">Представляет выражение поиска, которое сравнивает свойство со значением константы или другим свойством и возвращает **значение true** , если значения не совпадают.</span><span class="sxs-lookup"><span data-stu-id="c67ec-132">Represents a search expression that compares a property with either a constant value or another property and returns **true** if the values are not the same.</span></span>  <br/> |
|[<span data-ttu-id="c67ec-133">Not</span><span class="sxs-lookup"><span data-stu-id="c67ec-133">Not</span></span>](not.md) <br/> |<span data-ttu-id="c67ec-134">Представляет выражение поиска, которое инвертирует логическое значение содержащегося в нем выражения поиска.</span><span class="sxs-lookup"><span data-stu-id="c67ec-134">Represents a search expression that negates the Boolean value of the search expression it contains.</span></span>  <br/> |
|[<span data-ttu-id="c67ec-135">Or</span><span class="sxs-lookup"><span data-stu-id="c67ec-135">Or</span></span>](or.md) <br/> |<span data-ttu-id="c67ec-136">Представляет выражение поиска, которое выполняет логическую операцию **or** над искомым выражением.</span><span class="sxs-lookup"><span data-stu-id="c67ec-136">Represents a search expression that performs a logical **OR** operation on the search expression it contains.</span></span> <span data-ttu-id="c67ec-137">Элемент **or** возвращает **значение true** , если любой из дочерних элементов возвращает **значение true**.</span><span class="sxs-lookup"><span data-stu-id="c67ec-137">The **Or** element will return **true** if any of its children return **true**.</span></span>  <br/> |
|[<span data-ttu-id="c67ec-138">сеарчекспрессион</span><span class="sxs-lookup"><span data-stu-id="c67ec-138">SearchExpression</span></span>](searchexpression.md) <br/> |<span data-ttu-id="c67ec-139">Представляет замененный элемент в ограничении.</span><span class="sxs-lookup"><span data-stu-id="c67ec-139">Represents the substituted element within a restriction.</span></span> <span data-ttu-id="c67ec-140">Этот элемент не используется в экземпляре XML-документа.</span><span class="sxs-lookup"><span data-stu-id="c67ec-140">This element is not used in an XML instance document.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="c67ec-141">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="c67ec-141">Parent elements</span></span>

|<span data-ttu-id="c67ec-142">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="c67ec-142">**Element**</span></span>|<span data-ttu-id="c67ec-143">**Описание**</span><span class="sxs-lookup"><span data-stu-id="c67ec-143">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c67ec-144">FindFolder</span><span class="sxs-lookup"><span data-stu-id="c67ec-144">FindFolder</span></span>](findfolder.md) <br/> |<span data-ttu-id="c67ec-145">Определяет запрос на идентификацию папок в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="c67ec-145">Defines a request to identify folders in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="c67ec-146">FindItem</span><span class="sxs-lookup"><span data-stu-id="c67ec-146">FindItem</span></span>](finditem.md) <br/> |<span data-ttu-id="c67ec-147">Определяет запрос на поиск элементов в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="c67ec-147">Defines a request to find items in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="c67ec-148">сеарчпараметерс</span><span class="sxs-lookup"><span data-stu-id="c67ec-148">SearchParameters</span></span>](searchparameters.md) <br/> |<span data-ttu-id="c67ec-149">Представляет параметры, определяющие папку поиска.</span><span class="sxs-lookup"><span data-stu-id="c67ec-149">Represents the parameters that define a search folder.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="c67ec-150">Примечания</span><span class="sxs-lookup"><span data-stu-id="c67ec-150">Remarks</span></span>

<span data-ttu-id="c67ec-151">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="c67ec-151">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c67ec-152">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="c67ec-152">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c67ec-153">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="c67ec-153">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="c67ec-154">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="c67ec-154">Schema Name</span></span>  <br/> |<span data-ttu-id="c67ec-155">Схема Types</span><span class="sxs-lookup"><span data-stu-id="c67ec-155">Types schema</span></span>  <br/> |
|<span data-ttu-id="c67ec-156">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="c67ec-156">Validation File</span></span>  <br/> |<span data-ttu-id="c67ec-157">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="c67ec-157">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="c67ec-158">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="c67ec-158">Can be Empty</span></span>  <br/> |<span data-ttu-id="c67ec-159">False</span><span class="sxs-lookup"><span data-stu-id="c67ec-159">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c67ec-160">См. также</span><span class="sxs-lookup"><span data-stu-id="c67ec-160">See also</span></span>



- [<span data-ttu-id="c67ec-161">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="c67ec-161">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

