---
title: SearchExpression
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SearchExpression
api_type:
- schema
ms.assetid: daa179b6-8c7f-4268-a312-c2acc67fa7c3
description: Элемент SearchExpression является абстрактный элемент, представляющий переданный элемент с ограничением. Все выражения поиска являются производными от этого базового типа. Этот элемент не используется в экземпляре документа XML.
ms.openlocfilehash: 8e0d09aec079280816cd9dfe2c1a55c88bb959a7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19835286"
---
# <a name="searchexpression"></a><span data-ttu-id="f06a6-105">SearchExpression</span><span class="sxs-lookup"><span data-stu-id="f06a6-105">SearchExpression</span></span>

<span data-ttu-id="f06a6-106">Элемент **SearchExpression** является абстрактный элемент, представляющий переданный элемент с ограничением.</span><span class="sxs-lookup"><span data-stu-id="f06a6-106">The **SearchExpression** element is an abstract element that represents the substituted element within a restriction.</span></span> <span data-ttu-id="f06a6-107">Все выражения поиска являются производными от этого базового типа.</span><span class="sxs-lookup"><span data-stu-id="f06a6-107">All search expressions derive from this base type.</span></span> <span data-ttu-id="f06a6-108">Этот элемент не используется в экземпляре документа XML.</span><span class="sxs-lookup"><span data-stu-id="f06a6-108">This element is not used in an XML instance document.</span></span> 
  
```xml
<SearchExpression/>
```

 <span data-ttu-id="f06a6-109">**SearchExpressionType**</span><span class="sxs-lookup"><span data-stu-id="f06a6-109">**SearchExpressionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f06a6-110">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="f06a6-110">Attributes and elements</span></span>

<span data-ttu-id="f06a6-111">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="f06a6-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f06a6-112">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="f06a6-112">Attributes</span></span>

<span data-ttu-id="f06a6-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="f06a6-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f06a6-114">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="f06a6-114">Child elements</span></span>

<span data-ttu-id="f06a6-115">Нет.</span><span class="sxs-lookup"><span data-stu-id="f06a6-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="f06a6-116">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="f06a6-116">Parent elements</span></span>

|<span data-ttu-id="f06a6-117">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="f06a6-117">**Element**</span></span>|<span data-ttu-id="f06a6-118">**Описание**</span><span class="sxs-lookup"><span data-stu-id="f06a6-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f06a6-119">Ограничения</span><span class="sxs-lookup"><span data-stu-id="f06a6-119">Restriction</span></span>](restriction.md) <br/> |<span data-ttu-id="f06a6-120">Представляет ограничение или запрос, используемый для фильтрации элементов или папок в папке операциях FindItem/FindFolder и поиска.</span><span class="sxs-lookup"><span data-stu-id="f06a6-120">Represents the restriction or query that is used to filter items or folders in FindItem/FindFolder and search folder operations.</span></span>  <br/> |
|[<span data-ttu-id="f06a6-121">Не</span><span class="sxs-lookup"><span data-stu-id="f06a6-121">Not</span></span>](not.md) <br/> |<span data-ttu-id="f06a6-122">Представляет выражение поиска, которое Инвертирует логическое значение выражения поиска, который он содержит.</span><span class="sxs-lookup"><span data-stu-id="f06a6-122">Represents a search expression that negates the Boolean value of the search expression that it contains.</span></span>  <br/> |
|[<span data-ttu-id="f06a6-123">И</span><span class="sxs-lookup"><span data-stu-id="f06a6-123">And</span></span>](and.md) <br/> |<span data-ttu-id="f06a6-124">Представляет выражение поиска, которое позволяет выполнять операцию логическое **AND** между двумя или более выражений для поиска.</span><span class="sxs-lookup"><span data-stu-id="f06a6-124">Represents a search expression that allows you to perform a Boolean **AND** operation between two or more search expressions.</span></span> <span data-ttu-id="f06a6-125">Результат **операции** является **значение true** , если все выражения поиска, содержащиеся в элементе **и** имеют **значение true**.</span><span class="sxs-lookup"><span data-stu-id="f06a6-125">The result of the **AND** operation is **true** if all the search expressions contained within the **And** element are **true**.</span></span>  <br/> |
|[<span data-ttu-id="f06a6-126">Или</span><span class="sxs-lookup"><span data-stu-id="f06a6-126">Or</span></span>](or.md) <br/> |<span data-ttu-id="f06a6-127">Представляет выражение поиска, которое выполняет операцию логической **или** на нем выражением поиска.</span><span class="sxs-lookup"><span data-stu-id="f06a6-127">Represents a search expression that performs a logical **OR** operation on the search expression that it contains.</span></span> <span data-ttu-id="f06a6-128">**Или** возвращает **значение true,** Если какие-либо из их дочерних элементов возвращало **значение true**.</span><span class="sxs-lookup"><span data-stu-id="f06a6-128">**Or** will return **true** if any of its children return **true**.</span></span> <span data-ttu-id="f06a6-129">**Или** должен иметь два или несколько дочерних элементов.</span><span class="sxs-lookup"><span data-stu-id="f06a6-129">**Or** must have two or more children.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="f06a6-130">Замечания</span><span class="sxs-lookup"><span data-stu-id="f06a6-130">Remarks</span></span>

<span data-ttu-id="f06a6-131">Любой элемент фильтра, который является частью группы подстановки SearchExpression могут появляться, вместо SearchExpression элемента.</span><span class="sxs-lookup"><span data-stu-id="f06a6-131">Any filter element that is part of the SearchExpression substitution group can appear in place of the SearchExpression element.</span></span>
  
> [!NOTE]
> <span data-ttu-id="f06a6-132">Этот элемент никогда не происходит непосредственно в экземпляре документа.</span><span class="sxs-lookup"><span data-stu-id="f06a6-132">This element will never occur directly within an instance document.</span></span> 
  
<span data-ttu-id="f06a6-133">Следующие элементы являются участниками группы подстановки SearchExpression:</span><span class="sxs-lookup"><span data-stu-id="f06a6-133">The following elements are members of the SearchExpression substitution group:</span></span>
  
- [<span data-ttu-id="f06a6-134">Существует</span><span class="sxs-lookup"><span data-stu-id="f06a6-134">Exists</span></span>](exists.md)
    
- [<span data-ttu-id="f06a6-135">Исключает</span><span class="sxs-lookup"><span data-stu-id="f06a6-135">Excludes</span></span>](excludes.md)
    
- [<span data-ttu-id="f06a6-136">Выражение IsEqualTo</span><span class="sxs-lookup"><span data-stu-id="f06a6-136">IsEqualTo</span></span>](isequalto.md)
    
- [<span data-ttu-id="f06a6-137">IsNotEqualTo</span><span class="sxs-lookup"><span data-stu-id="f06a6-137">IsNotEqualTo</span></span>](isnotequalto.md)
    
- [<span data-ttu-id="f06a6-138">IsGreaterThan</span><span class="sxs-lookup"><span data-stu-id="f06a6-138">IsGreaterThan</span></span>](isgreaterthan.md)
    
- [<span data-ttu-id="f06a6-139">IsGreaterThanOrEqualTo</span><span class="sxs-lookup"><span data-stu-id="f06a6-139">IsGreaterThanOrEqualTo</span></span>](isgreaterthanorequalto.md)
    
- [<span data-ttu-id="f06a6-140">IsLessThan</span><span class="sxs-lookup"><span data-stu-id="f06a6-140">IsLessThan</span></span>](islessthan.md)
    
- [<span data-ttu-id="f06a6-141">IsLessThanOrEqualTo</span><span class="sxs-lookup"><span data-stu-id="f06a6-141">IsLessThanOrEqualTo</span></span>](islessthanorequalto.md)
    
- [<span data-ttu-id="f06a6-142">Contains</span><span class="sxs-lookup"><span data-stu-id="f06a6-142">Contains</span></span>](contains.md)
    
- [<span data-ttu-id="f06a6-143">Не</span><span class="sxs-lookup"><span data-stu-id="f06a6-143">Not</span></span>](not.md)
    
- [<span data-ttu-id="f06a6-144">И</span><span class="sxs-lookup"><span data-stu-id="f06a6-144">And</span></span>](and.md)
    
- [<span data-ttu-id="f06a6-145">Или</span><span class="sxs-lookup"><span data-stu-id="f06a6-145">Or</span></span>](or.md)
    
<span data-ttu-id="f06a6-146">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="f06a6-146">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f06a6-147">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="f06a6-147">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f06a6-148">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="f06a6-148">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="f06a6-149">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="f06a6-149">Schema Name</span></span>  <br/> |<span data-ttu-id="f06a6-150">Схема Types</span><span class="sxs-lookup"><span data-stu-id="f06a6-150">Types schema</span></span>  <br/> |
|<span data-ttu-id="f06a6-151">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="f06a6-151">Validation File</span></span>  <br/> |<span data-ttu-id="f06a6-152">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="f06a6-152">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="f06a6-153">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="f06a6-153">Can be Empty</span></span>  <br/> |<span data-ttu-id="f06a6-154">False</span><span class="sxs-lookup"><span data-stu-id="f06a6-154">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f06a6-155">См. также</span><span class="sxs-lookup"><span data-stu-id="f06a6-155">See also</span></span>



- [<span data-ttu-id="f06a6-156">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="f06a6-156">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

