---
title: сеарчекспрессион
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
description: Элемент Сеарчекспрессион является абстрактным элементом, представляющим замещенный элемент в ограничении. Все выражения поиска являются производными от базового типа. Этот элемент не используется в экземпляре XML-документа.
ms.openlocfilehash: 8e0d09aec079280816cd9dfe2c1a55c88bb959a7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835286"
---
# <a name="searchexpression"></a><span data-ttu-id="3718e-105">сеарчекспрессион</span><span class="sxs-lookup"><span data-stu-id="3718e-105">SearchExpression</span></span>

<span data-ttu-id="3718e-106">Элемент **сеарчекспрессион** является абстрактным элементом, представляющим замещенный элемент в ограничении.</span><span class="sxs-lookup"><span data-stu-id="3718e-106">The **SearchExpression** element is an abstract element that represents the substituted element within a restriction.</span></span> <span data-ttu-id="3718e-107">Все выражения поиска являются производными от базового типа.</span><span class="sxs-lookup"><span data-stu-id="3718e-107">All search expressions derive from this base type.</span></span> <span data-ttu-id="3718e-108">Этот элемент не используется в экземпляре XML-документа.</span><span class="sxs-lookup"><span data-stu-id="3718e-108">This element is not used in an XML instance document.</span></span> 
  
```xml
<SearchExpression/>
```

 <span data-ttu-id="3718e-109">**сеарчекспрессионтипе**</span><span class="sxs-lookup"><span data-stu-id="3718e-109">**SearchExpressionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3718e-110">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="3718e-110">Attributes and elements</span></span>

<span data-ttu-id="3718e-111">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="3718e-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3718e-112">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="3718e-112">Attributes</span></span>

<span data-ttu-id="3718e-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="3718e-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3718e-114">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="3718e-114">Child elements</span></span>

<span data-ttu-id="3718e-115">Нет.</span><span class="sxs-lookup"><span data-stu-id="3718e-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="3718e-116">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="3718e-116">Parent elements</span></span>

|<span data-ttu-id="3718e-117">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="3718e-117">**Element**</span></span>|<span data-ttu-id="3718e-118">**Описание**</span><span class="sxs-lookup"><span data-stu-id="3718e-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3718e-119">Restriction</span><span class="sxs-lookup"><span data-stu-id="3718e-119">Restriction</span></span>](restriction.md) <br/> |<span data-ttu-id="3718e-120">Представляет ограничение или запрос, используемый для фильтрации элементов или папок в операциях FindItem/FindFolder и папках поиска.</span><span class="sxs-lookup"><span data-stu-id="3718e-120">Represents the restriction or query that is used to filter items or folders in FindItem/FindFolder and search folder operations.</span></span>  <br/> |
|[<span data-ttu-id="3718e-121">Not</span><span class="sxs-lookup"><span data-stu-id="3718e-121">Not</span></span>](not.md) <br/> |<span data-ttu-id="3718e-122">Представляет выражение поиска, которое инвертирует логическое значение содержащегося в нем выражения поиска.</span><span class="sxs-lookup"><span data-stu-id="3718e-122">Represents a search expression that negates the Boolean value of the search expression that it contains.</span></span>  <br/> |
|[<span data-ttu-id="3718e-123">And</span><span class="sxs-lookup"><span data-stu-id="3718e-123">And</span></span>](and.md) <br/> |<span data-ttu-id="3718e-124">Представляет выражение поиска, которое позволяет выполнять логическую операцию **и** операцию между двумя или более выражениями поиска.</span><span class="sxs-lookup"><span data-stu-id="3718e-124">Represents a search expression that allows you to perform a Boolean **AND** operation between two or more search expressions.</span></span> <span data-ttu-id="3718e-125">Результат операции **and** имеет **значение true** , если все выражения поиска, содержащиеся в элементе **и** , имеют **значение true**.</span><span class="sxs-lookup"><span data-stu-id="3718e-125">The result of the **AND** operation is **true** if all the search expressions contained within the **And** element are **true**.</span></span>  <br/> |
|[<span data-ttu-id="3718e-126">Or</span><span class="sxs-lookup"><span data-stu-id="3718e-126">Or</span></span>](or.md) <br/> |<span data-ttu-id="3718e-127">Представляет выражение поиска, которое выполняет логическую операцию **or** над выражением поиска, которое оно содержит.</span><span class="sxs-lookup"><span data-stu-id="3718e-127">Represents a search expression that performs a logical **OR** operation on the search expression that it contains.</span></span> <span data-ttu-id="3718e-128">**Или** возвращает **значение true** , если любой из дочерних элементов возвращает **значение true**.</span><span class="sxs-lookup"><span data-stu-id="3718e-128">**Or** will return **true** if any of its children return **true**.</span></span> <span data-ttu-id="3718e-129">**Или** должно иметь не менее двух дочерних элементов.</span><span class="sxs-lookup"><span data-stu-id="3718e-129">**Or** must have two or more children.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="3718e-130">Примечания</span><span class="sxs-lookup"><span data-stu-id="3718e-130">Remarks</span></span>

<span data-ttu-id="3718e-131">Любой элемент Filter, являющийся частью группы подстановки Сеарчекспрессион, может отображаться вместо элемента Сеарчекспрессион.</span><span class="sxs-lookup"><span data-stu-id="3718e-131">Any filter element that is part of the SearchExpression substitution group can appear in place of the SearchExpression element.</span></span>
  
> [!NOTE]
> <span data-ttu-id="3718e-132">Этот элемент никогда не будет выполняться непосредственно в экземпляре документа.</span><span class="sxs-lookup"><span data-stu-id="3718e-132">This element will never occur directly within an instance document.</span></span> 
  
<span data-ttu-id="3718e-133">Следующие элементы являются членами группы подстановки Сеарчекспрессион:</span><span class="sxs-lookup"><span data-stu-id="3718e-133">The following elements are members of the SearchExpression substitution group:</span></span>
  
- [<span data-ttu-id="3718e-134">Exists</span><span class="sxs-lookup"><span data-stu-id="3718e-134">Exists</span></span>](exists.md)
    
- [<span data-ttu-id="3718e-135">Исключает</span><span class="sxs-lookup"><span data-stu-id="3718e-135">Excludes</span></span>](excludes.md)
    
- [<span data-ttu-id="3718e-136">исекуалто</span><span class="sxs-lookup"><span data-stu-id="3718e-136">IsEqualTo</span></span>](isequalto.md)
    
- [<span data-ttu-id="3718e-137">иснотекуалто</span><span class="sxs-lookup"><span data-stu-id="3718e-137">IsNotEqualTo</span></span>](isnotequalto.md)
    
- [<span data-ttu-id="3718e-138">исгреатерсан</span><span class="sxs-lookup"><span data-stu-id="3718e-138">IsGreaterThan</span></span>](isgreaterthan.md)
    
- [<span data-ttu-id="3718e-139">исгреатерсанорекуалто</span><span class="sxs-lookup"><span data-stu-id="3718e-139">IsGreaterThanOrEqualTo</span></span>](isgreaterthanorequalto.md)
    
- [<span data-ttu-id="3718e-140">ислесссан</span><span class="sxs-lookup"><span data-stu-id="3718e-140">IsLessThan</span></span>](islessthan.md)
    
- [<span data-ttu-id="3718e-141">ислесссанорекуалто</span><span class="sxs-lookup"><span data-stu-id="3718e-141">IsLessThanOrEqualTo</span></span>](islessthanorequalto.md)
    
- [<span data-ttu-id="3718e-142">Contains</span><span class="sxs-lookup"><span data-stu-id="3718e-142">Contains</span></span>](contains.md)
    
- [<span data-ttu-id="3718e-143">Not</span><span class="sxs-lookup"><span data-stu-id="3718e-143">Not</span></span>](not.md)
    
- [<span data-ttu-id="3718e-144">And</span><span class="sxs-lookup"><span data-stu-id="3718e-144">And</span></span>](and.md)
    
- [<span data-ttu-id="3718e-145">Or</span><span class="sxs-lookup"><span data-stu-id="3718e-145">Or</span></span>](or.md)
    
<span data-ttu-id="3718e-146">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="3718e-146">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3718e-147">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="3718e-147">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3718e-148">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="3718e-148">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="3718e-149">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="3718e-149">Schema Name</span></span>  <br/> |<span data-ttu-id="3718e-150">Схема Types</span><span class="sxs-lookup"><span data-stu-id="3718e-150">Types schema</span></span>  <br/> |
|<span data-ttu-id="3718e-151">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="3718e-151">Validation File</span></span>  <br/> |<span data-ttu-id="3718e-152">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="3718e-152">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="3718e-153">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="3718e-153">Can be Empty</span></span>  <br/> |<span data-ttu-id="3718e-154">False</span><span class="sxs-lookup"><span data-stu-id="3718e-154">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3718e-155">См. также</span><span class="sxs-lookup"><span data-stu-id="3718e-155">See also</span></span>



- [<span data-ttu-id="3718e-156">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="3718e-156">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

