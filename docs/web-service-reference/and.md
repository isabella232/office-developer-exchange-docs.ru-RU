---
title: и
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- And
api_type:
- schema
ms.assetid: 790246c2-37ad-49a8-91b9-6186d743b011
description: Элемент And представляет выражение поиска, который позволяет выполнить операцию логическое и между двумя или более выражений для поиска. Значение true, если все выражения поиска, содержащиеся в элементе и результат операции.
ms.openlocfilehash: d287d57d68aeca7127325dc8fb65fd0190e5b5eb
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761381"
---
# <a name="and"></a><span data-ttu-id="55386-104">и</span><span class="sxs-lookup"><span data-stu-id="55386-104">And</span></span>

<span data-ttu-id="55386-105">Элемент **и** представляет выражение поиска, которое позволяет выполнять операцию логическое **AND** между двумя или более выражений для поиска.</span><span class="sxs-lookup"><span data-stu-id="55386-105">The **And** element represents a search expression that allows you to perform a Boolean **AND** operation between two or more search expressions.</span></span> <span data-ttu-id="55386-106">Результат **операции** является **значение true** , если все выражения поиска, содержащиеся в элементе **и** имеют **значение true**.</span><span class="sxs-lookup"><span data-stu-id="55386-106">The result of the **AND** operation is **true** if all the search expressions contained within the **And** element are **true**.</span></span>
  
```xml
<And>
   <SearchExpression/>
   <SearchExpression/>
</And>
```

 <span data-ttu-id="55386-107">**AndType**</span><span class="sxs-lookup"><span data-stu-id="55386-107">**AndType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="55386-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="55386-108">Attributes and elements</span></span>

<span data-ttu-id="55386-109">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="55386-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="55386-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="55386-110">Attributes</span></span>

<span data-ttu-id="55386-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="55386-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="55386-112">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="55386-112">Child elements</span></span>

|<span data-ttu-id="55386-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="55386-113">**Element**</span></span>|<span data-ttu-id="55386-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="55386-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="55386-115">SearchExpression</span><span class="sxs-lookup"><span data-stu-id="55386-115">SearchExpression</span></span>](searchexpression.md) <br/> | <span data-ttu-id="55386-116">Представляет базовый класс для выражений с ограничением.</span><span class="sxs-lookup"><span data-stu-id="55386-116">Represents the base class for expressions within a restriction.</span></span> <span data-ttu-id="55386-117">Должен быть более двух выражений поиска в операции.</span><span class="sxs-lookup"><span data-stu-id="55386-117">There must be two or more search expressions in an And operation.</span></span><br/><br/>  <span data-ttu-id="55386-118">Элемент **SearchExpression** необходимо заменить один из следующих элементов:</span><span class="sxs-lookup"><span data-stu-id="55386-118">One of the following elements must be substituted for the **SearchExpression** element:</span></span><ul><li> [<span data-ttu-id="55386-119">Существует</span><span class="sxs-lookup"><span data-stu-id="55386-119">Exists</span></span>](exists.md)</li><li>[<span data-ttu-id="55386-120">Исключает</span><span class="sxs-lookup"><span data-stu-id="55386-120">Excludes</span></span>](excludes.md)</li><li>[<span data-ttu-id="55386-121">Выражение IsEqualTo</span><span class="sxs-lookup"><span data-stu-id="55386-121">IsEqualTo</span></span>](isequalto.md)</li><li>[<span data-ttu-id="55386-122">IsNotEqualTo</span><span class="sxs-lookup"><span data-stu-id="55386-122">IsNotEqualTo</span></span>](isnotequalto.md)</li><li>[<span data-ttu-id="55386-123">IsGreaterThan</span><span class="sxs-lookup"><span data-stu-id="55386-123">IsGreaterThan</span></span>](isgreaterthan.md)</li><li>[<span data-ttu-id="55386-124">IsGreaterThanOrEqualTo</span><span class="sxs-lookup"><span data-stu-id="55386-124">IsGreaterThanOrEqualTo</span></span>](isgreaterthanorequalto.md)</li><li>[<span data-ttu-id="55386-125">IsLessThan</span><span class="sxs-lookup"><span data-stu-id="55386-125">IsLessThan</span></span>](islessthan.md)</li><li>[<span data-ttu-id="55386-126">IsLessThanOrEqualTo</span><span class="sxs-lookup"><span data-stu-id="55386-126">IsLessThanOrEqualTo</span></span>](islessthanorequalto.md)</li><li>[<span data-ttu-id="55386-127">Contains</span><span class="sxs-lookup"><span data-stu-id="55386-127">Contains</span></span>](contains.md)</li><li>[<span data-ttu-id="55386-128">Не</span><span class="sxs-lookup"><span data-stu-id="55386-128">Not</span></span>](not.md)</li><li><span data-ttu-id="55386-129">**И**</span><span class="sxs-lookup"><span data-stu-id="55386-129">**And**</span></span></li><li>[<span data-ttu-id="55386-130">Или</span><span class="sxs-lookup"><span data-stu-id="55386-130">Or</span></span>](or.md) </li></ul> |
   
### <a name="parent-elements"></a><span data-ttu-id="55386-131">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="55386-131">Parent elements</span></span>

|<span data-ttu-id="55386-132">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="55386-132">**Element**</span></span>|<span data-ttu-id="55386-133">**Описание**</span><span class="sxs-lookup"><span data-stu-id="55386-133">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="55386-134">Ограничения</span><span class="sxs-lookup"><span data-stu-id="55386-134">Restriction</span></span>](restriction.md) <br/> |<span data-ttu-id="55386-135">Представляет ограничение или запрос, используемый для фильтрации элементов или папок в папке операциях FindItem/FindFolder и поиска.</span><span class="sxs-lookup"><span data-stu-id="55386-135">Represents the restriction or query that is used to filter items or folders in FindItem/FindFolder and search folder operations.</span></span>  <br/> |
|[<span data-ttu-id="55386-136">Не</span><span class="sxs-lookup"><span data-stu-id="55386-136">Not</span></span>](not.md) <br/> |<span data-ttu-id="55386-137">Представляет выражение поиска, которое Инвертирует логическое значение выражения поиска, который он содержит.</span><span class="sxs-lookup"><span data-stu-id="55386-137">Represents a search expression that negates the Boolean value of the search expression that it contains.</span></span>  <br/> |
|<span data-ttu-id="55386-138">**И**</span><span class="sxs-lookup"><span data-stu-id="55386-138">**And**</span></span> <br/> |<span data-ttu-id="55386-139">Представляет выражение поиска, которое позволяет выполнять операцию логическое **AND** между двумя или более выражений для поиска.</span><span class="sxs-lookup"><span data-stu-id="55386-139">Represents a search expression that allows you to perform a Boolean **AND** operation between two or more search expressions.</span></span> <span data-ttu-id="55386-140">**Операции** получается **значение true,** **Если все выражения поиска, содержащиеся в элементе **и** **.</span><span class="sxs-lookup"><span data-stu-id="55386-140">The result of the **AND** operation is **true** if all of the search expressions contained within the **And** element are **true**.</span></span>  <br/> |
|[<span data-ttu-id="55386-141">Или</span><span class="sxs-lookup"><span data-stu-id="55386-141">Or</span></span>](or.md) <br/> |<span data-ttu-id="55386-142">Представляет выражение поиска, которое выполняет операцию логической **или** на нем выражением поиска.</span><span class="sxs-lookup"><span data-stu-id="55386-142">Represents a search expression that performs a logical **OR** operation on the search expression that it contains.</span></span> <span data-ttu-id="55386-143">**Или** возвращает **значение true,** Если какие-либо из их дочерних элементов возвращало **значение true**.</span><span class="sxs-lookup"><span data-stu-id="55386-143">**Or** will return **true** if any of its children return **true**.</span></span> <span data-ttu-id="55386-144">**Или** должен иметь два или несколько дочерних элементов.</span><span class="sxs-lookup"><span data-stu-id="55386-144">**Or** must have two or more children.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="55386-145">Замечания</span><span class="sxs-lookup"><span data-stu-id="55386-145">Remarks</span></span>

<span data-ttu-id="55386-146">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="55386-146">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="55386-147">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="55386-147">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="55386-148">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="55386-148">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="55386-149">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="55386-149">Schema Name</span></span>  <br/> |<span data-ttu-id="55386-150">Схема Types</span><span class="sxs-lookup"><span data-stu-id="55386-150">Types schema</span></span>  <br/> |
|<span data-ttu-id="55386-151">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="55386-151">Validation File</span></span>  <br/> |<span data-ttu-id="55386-152">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="55386-152">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="55386-153">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="55386-153">Can be Empty</span></span>  <br/> |<span data-ttu-id="55386-154">False</span><span class="sxs-lookup"><span data-stu-id="55386-154">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="55386-155">См. также</span><span class="sxs-lookup"><span data-stu-id="55386-155">See also</span></span>

- [<span data-ttu-id="55386-156">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="55386-156">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

