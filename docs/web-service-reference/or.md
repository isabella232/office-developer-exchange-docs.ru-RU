---
title: Или
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Or
api_type:
- schema
ms.assetid: 4876d83a-73a3-4953-9d95-3048e6b76ccb
description: Элемент или представляет выражение поиска, используемая для выполнения логического или на нем выражением поиска. Или возвращает значение true, если какие-либо из их дочерних элементов возвращало значение true. Или должны иметь два или несколько дочерних элементов.
ms.openlocfilehash: 46cf031047aeb09e05a385150ab7587968aef345
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19834661"
---
# <a name="or"></a><span data-ttu-id="242f4-105">Или</span><span class="sxs-lookup"><span data-stu-id="242f4-105">Or</span></span>

<span data-ttu-id="242f4-106">Элемент **или** представляет выражение поиска, которое выполняет логической **или** на нем выражением поиска.</span><span class="sxs-lookup"><span data-stu-id="242f4-106">The **Or** element represents a search expression that performs a logical **OR** on the search expression that it contains.</span></span> <span data-ttu-id="242f4-107">**Или** возвращает **значение true,** Если какие-либо из их дочерних элементов возвращало **значение true**.</span><span class="sxs-lookup"><span data-stu-id="242f4-107">**Or** will return **true** if any of its children return **true**.</span></span> <span data-ttu-id="242f4-108">**Или** должен иметь два или несколько дочерних элементов.</span><span class="sxs-lookup"><span data-stu-id="242f4-108">**Or** must have two or more children.</span></span> 
  
```xml
<Or>
   <SearchExpression/>
   <SearchExpression/>
</Or>
```

 <span data-ttu-id="242f4-109">**OrType**</span><span class="sxs-lookup"><span data-stu-id="242f4-109">**OrType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="242f4-110">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="242f4-110">Attributes and elements</span></span>

<span data-ttu-id="242f4-111">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="242f4-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="242f4-112">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="242f4-112">Attributes</span></span>

<span data-ttu-id="242f4-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="242f4-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="242f4-114">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="242f4-114">Child elements</span></span>

|<span data-ttu-id="242f4-115">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="242f4-115">**Element**</span></span>|<span data-ttu-id="242f4-116">**Описание**</span><span class="sxs-lookup"><span data-stu-id="242f4-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="242f4-117">SearchExpression</span><span class="sxs-lookup"><span data-stu-id="242f4-117">SearchExpression</span></span>](searchexpression.md) <br/> | <span data-ttu-id="242f4-118">Представляет базовый класс для выражений с ограничением.</span><span class="sxs-lookup"><span data-stu-id="242f4-118">Represents the base class for expressions within a restriction.</span></span> <br/><br/><span data-ttu-id="242f4-119">Элемент **SearchExpression** необходимо заменить один из следующих элементов:</span><span class="sxs-lookup"><span data-stu-id="242f4-119">One of the following elements must be substituted for the **SearchExpression** element:</span></span> <br/> <br/><span data-ttu-id="242f4-120">- [Существует](exists.md)</span><span class="sxs-lookup"><span data-stu-id="242f4-120">- [Exists](exists.md)</span></span> <br/><span data-ttu-id="242f4-121">- [Исключает](excludes.md)</span><span class="sxs-lookup"><span data-stu-id="242f4-121">- [Excludes](excludes.md)</span></span> <br/><span data-ttu-id="242f4-122">- [Выражение IsEqualTo](isequalto.md)</span><span class="sxs-lookup"><span data-stu-id="242f4-122">- [IsEqualTo](isequalto.md)</span></span> <br/><span data-ttu-id="242f4-123">- [IsNotEqualTo](isnotequalto.md)</span><span class="sxs-lookup"><span data-stu-id="242f4-123">- [IsNotEqualTo](isnotequalto.md)</span></span> <br/><span data-ttu-id="242f4-124">- [IsGreaterThan](isgreaterthan.md)</span><span class="sxs-lookup"><span data-stu-id="242f4-124">- [IsGreaterThan](isgreaterthan.md)</span></span> <br/><span data-ttu-id="242f4-125">- [IsGreaterThanOrEqualTo](isgreaterthanorequalto.md)</span><span class="sxs-lookup"><span data-stu-id="242f4-125">- [IsGreaterThanOrEqualTo](isgreaterthanorequalto.md)</span></span> <br/><span data-ttu-id="242f4-126">- [IsLessThan](islessthan.md)</span><span class="sxs-lookup"><span data-stu-id="242f4-126">- [IsLessThan](islessthan.md)</span></span> <br/><span data-ttu-id="242f4-127">- [IsLessThanOrEqualTo](islessthanorequalto.md)</span><span class="sxs-lookup"><span data-stu-id="242f4-127">- [IsLessThanOrEqualTo](islessthanorequalto.md)</span></span> <br/><span data-ttu-id="242f4-128">- [Содержит](contains.md)</span><span class="sxs-lookup"><span data-stu-id="242f4-128">- [Contains](contains.md)</span></span> <br/><span data-ttu-id="242f4-129">- [Не](not.md)</span><span class="sxs-lookup"><span data-stu-id="242f4-129">- [Not](not.md)</span></span> <br/><span data-ttu-id="242f4-130">- [И](and.md)</span><span class="sxs-lookup"><span data-stu-id="242f4-130">- [And](and.md)</span></span> <br/><span data-ttu-id="242f4-131">- **Или**</span><span class="sxs-lookup"><span data-stu-id="242f4-131">- **Or**</span></span> <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="242f4-132">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="242f4-132">Parent elements</span></span>

|<span data-ttu-id="242f4-133">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="242f4-133">**Element**</span></span>|<span data-ttu-id="242f4-134">**Описание**</span><span class="sxs-lookup"><span data-stu-id="242f4-134">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="242f4-135">Ограничения</span><span class="sxs-lookup"><span data-stu-id="242f4-135">Restriction</span></span>](restriction.md) <br/> |<span data-ttu-id="242f4-136">Представляет ограничение или запрос, используемый для фильтрации элементов или папок в папке операциях FindItem/FindFolder и поиска.</span><span class="sxs-lookup"><span data-stu-id="242f4-136">Represents the restriction or query that is used to filter items or folders in FindItem/FindFolder and search folder operations.</span></span>  <br/> |
|[<span data-ttu-id="242f4-137">Не</span><span class="sxs-lookup"><span data-stu-id="242f4-137">Not</span></span>](not.md) <br/> |<span data-ttu-id="242f4-138">Представляет выражение поиска, которое Инвертирует логическое значение выражения поиска, который он содержит.</span><span class="sxs-lookup"><span data-stu-id="242f4-138">Represents a search expression that negates the Boolean value of the search expression that it contains.</span></span>  <br/> |
|[<span data-ttu-id="242f4-139">И</span><span class="sxs-lookup"><span data-stu-id="242f4-139">And</span></span>](and.md) <br/> |<span data-ttu-id="242f4-140">Представляет выражение поиска, которое позволяет выполнять операцию логическое **AND** между двумя или более выражений для поиска.</span><span class="sxs-lookup"><span data-stu-id="242f4-140">Represents a search expression that allows you to perform a Boolean **AND** operation between two or more search expressions.</span></span> <span data-ttu-id="242f4-141">Результат **операции** является **значение true** , если все выражения поиска, содержащиеся в элементе **и** имеют **значение true**.</span><span class="sxs-lookup"><span data-stu-id="242f4-141">The result of the **AND** operation is **true** if all the search expressions contained within the **And** element are **true**.</span></span>  <br/> |
|<span data-ttu-id="242f4-142">**Или**</span><span class="sxs-lookup"><span data-stu-id="242f4-142">**Or**</span></span> <br/> |<span data-ttu-id="242f4-143">Представляет выражение поиска, которое выполняет операцию логической **или** на нем выражением поиска.</span><span class="sxs-lookup"><span data-stu-id="242f4-143">Represents a search expression that performs a logical **OR** operation on the search expression that it contains.</span></span> <span data-ttu-id="242f4-144">**Или** возвращает **значение true,** Если какие-либо из их дочерних элементов возвращало **значение true**.</span><span class="sxs-lookup"><span data-stu-id="242f4-144">**Or** will return **true** if any of its children return **true**.</span></span> <span data-ttu-id="242f4-145">**Или** должен иметь два или несколько дочерних элементов.</span><span class="sxs-lookup"><span data-stu-id="242f4-145">**Or** must have two or more children.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="242f4-146">Замечания</span><span class="sxs-lookup"><span data-stu-id="242f4-146">Remarks</span></span>

<span data-ttu-id="242f4-147">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="242f4-147">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="242f4-148">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="242f4-148">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="242f4-149">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="242f4-149">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="242f4-150">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="242f4-150">Schema Name</span></span>  <br/> |<span data-ttu-id="242f4-151">Схема Types</span><span class="sxs-lookup"><span data-stu-id="242f4-151">Types schema</span></span>  <br/> |
|<span data-ttu-id="242f4-152">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="242f4-152">Validation File</span></span>  <br/> |<span data-ttu-id="242f4-153">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="242f4-153">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="242f4-154">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="242f4-154">Can be Empty</span></span>  <br/> |<span data-ttu-id="242f4-155">False</span><span class="sxs-lookup"><span data-stu-id="242f4-155">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="242f4-156">См. также</span><span class="sxs-lookup"><span data-stu-id="242f4-156">See also</span></span>

- [<span data-ttu-id="242f4-157">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="242f4-157">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

