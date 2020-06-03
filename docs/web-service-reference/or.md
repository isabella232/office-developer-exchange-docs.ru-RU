---
title: ИЛИ
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
description: Элемент or представляет выражение поиска, которое выполняет операцию логического или для содержащегося в нем выражения поиска. Или возвращает значение true, если любой из дочерних элементов возвращает значение true. Или должно иметь не менее двух дочерних элементов.
ms.openlocfilehash: 9bc676da5bbaad64f11f6717fb487c2e9bcf2d89
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462481"
---
# <a name="or"></a><span data-ttu-id="934d9-105">ИЛИ</span><span class="sxs-lookup"><span data-stu-id="934d9-105">Or</span></span>

<span data-ttu-id="934d9-106">Элемент **or** представляет выражение поиска, которое выполняет операцию логического **или** для содержащегося в нем выражения поиска.</span><span class="sxs-lookup"><span data-stu-id="934d9-106">The **Or** element represents a search expression that performs a logical **OR** on the search expression that it contains.</span></span> <span data-ttu-id="934d9-107">**Или** возвращает **значение true** , если любой из дочерних элементов возвращает **значение true**.</span><span class="sxs-lookup"><span data-stu-id="934d9-107">**Or** will return **true** if any of its children return **true**.</span></span> <span data-ttu-id="934d9-108">**Или** должно иметь не менее двух дочерних элементов.</span><span class="sxs-lookup"><span data-stu-id="934d9-108">**Or** must have two or more children.</span></span> 
  
```xml
<Or>
   <SearchExpression/>
   <SearchExpression/>
</Or>
```

 <span data-ttu-id="934d9-109">**ортипе**</span><span class="sxs-lookup"><span data-stu-id="934d9-109">**OrType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="934d9-110">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="934d9-110">Attributes and elements</span></span>

<span data-ttu-id="934d9-111">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="934d9-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="934d9-112">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="934d9-112">Attributes</span></span>

<span data-ttu-id="934d9-113">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="934d9-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="934d9-114">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="934d9-114">Child elements</span></span>

|<span data-ttu-id="934d9-115">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="934d9-115">**Element**</span></span>|<span data-ttu-id="934d9-116">**Описание**</span><span class="sxs-lookup"><span data-stu-id="934d9-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="934d9-117">сеарчекспрессион</span><span class="sxs-lookup"><span data-stu-id="934d9-117">SearchExpression</span></span>](searchexpression.md) <br/> | <span data-ttu-id="934d9-118">Представляет базовый класс для выражений в ограничении.</span><span class="sxs-lookup"><span data-stu-id="934d9-118">Represents the base class for expressions within a restriction.</span></span> <br/><br/><span data-ttu-id="934d9-119">Для элемента **сеарчекспрессион** необходимо заменить один из следующих элементов:</span><span class="sxs-lookup"><span data-stu-id="934d9-119">One of the following elements must be substituted for the **SearchExpression** element:</span></span> <br/> <br/><span data-ttu-id="934d9-120">- [Существует](exists.md)</span><span class="sxs-lookup"><span data-stu-id="934d9-120">- [Exists](exists.md)</span></span> <br/><span data-ttu-id="934d9-121">- [Исключает](excludes.md)</span><span class="sxs-lookup"><span data-stu-id="934d9-121">- [Excludes](excludes.md)</span></span> <br/><span data-ttu-id="934d9-122">- [исекуалто](isequalto.md)</span><span class="sxs-lookup"><span data-stu-id="934d9-122">- [IsEqualTo](isequalto.md)</span></span> <br/><span data-ttu-id="934d9-123">- [иснотекуалто](isnotequalto.md)</span><span class="sxs-lookup"><span data-stu-id="934d9-123">- [IsNotEqualTo](isnotequalto.md)</span></span> <br/><span data-ttu-id="934d9-124">- [исгреатерсан](isgreaterthan.md)</span><span class="sxs-lookup"><span data-stu-id="934d9-124">- [IsGreaterThan](isgreaterthan.md)</span></span> <br/><span data-ttu-id="934d9-125">- [исгреатерсанорекуалто](isgreaterthanorequalto.md)</span><span class="sxs-lookup"><span data-stu-id="934d9-125">- [IsGreaterThanOrEqualTo](isgreaterthanorequalto.md)</span></span> <br/><span data-ttu-id="934d9-126">- [ислесссан](islessthan.md)</span><span class="sxs-lookup"><span data-stu-id="934d9-126">- [IsLessThan](islessthan.md)</span></span> <br/><span data-ttu-id="934d9-127">- [ислесссанорекуалто](islessthanorequalto.md)</span><span class="sxs-lookup"><span data-stu-id="934d9-127">- [IsLessThanOrEqualTo](islessthanorequalto.md)</span></span> <br/><span data-ttu-id="934d9-128">- [Хранится](contains.md)</span><span class="sxs-lookup"><span data-stu-id="934d9-128">- [Contains](contains.md)</span></span> <br/><span data-ttu-id="934d9-129">- [Не](not.md)</span><span class="sxs-lookup"><span data-stu-id="934d9-129">- [Not](not.md)</span></span> <br/><span data-ttu-id="934d9-130">- [С](and.md)</span><span class="sxs-lookup"><span data-stu-id="934d9-130">- [And](and.md)</span></span> <br/><span data-ttu-id="934d9-131">- **Также**</span><span class="sxs-lookup"><span data-stu-id="934d9-131">- **Or**</span></span> <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="934d9-132">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="934d9-132">Parent elements</span></span>

|<span data-ttu-id="934d9-133">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="934d9-133">**Element**</span></span>|<span data-ttu-id="934d9-134">**Описание**</span><span class="sxs-lookup"><span data-stu-id="934d9-134">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="934d9-135">Restriction</span><span class="sxs-lookup"><span data-stu-id="934d9-135">Restriction</span></span>](restriction.md) <br/> |<span data-ttu-id="934d9-136">Представляет ограничение или запрос, используемый для фильтрации элементов или папок в операциях FindItem/FindFolder и папках поиска.</span><span class="sxs-lookup"><span data-stu-id="934d9-136">Represents the restriction or query that is used to filter items or folders in FindItem/FindFolder and search folder operations.</span></span>  <br/> |
|[<span data-ttu-id="934d9-137">Not</span><span class="sxs-lookup"><span data-stu-id="934d9-137">Not</span></span>](not.md) <br/> |<span data-ttu-id="934d9-138">Представляет выражение поиска, которое инвертирует логическое значение содержащегося в нем выражения поиска.</span><span class="sxs-lookup"><span data-stu-id="934d9-138">Represents a search expression that negates the Boolean value of the search expression that it contains.</span></span>  <br/> |
|[<span data-ttu-id="934d9-139">And</span><span class="sxs-lookup"><span data-stu-id="934d9-139">And</span></span>](and.md) <br/> |<span data-ttu-id="934d9-140">Представляет выражение поиска, которое позволяет выполнять логическую операцию **и** операцию между двумя или более выражениями поиска.</span><span class="sxs-lookup"><span data-stu-id="934d9-140">Represents a search expression that allows you to perform a Boolean **AND** operation between two or more search expressions.</span></span> <span data-ttu-id="934d9-141">Результат операции **and** имеет **значение true** , если все выражения поиска, содержащиеся в элементе **и** , имеют **значение true**.</span><span class="sxs-lookup"><span data-stu-id="934d9-141">The result of the **AND** operation is **true** if all the search expressions contained within the **And** element are **true**.</span></span>  <br/> |
|<span data-ttu-id="934d9-142">**Or**</span><span class="sxs-lookup"><span data-stu-id="934d9-142">**Or**</span></span> <br/> |<span data-ttu-id="934d9-143">Представляет выражение поиска, которое выполняет логическую операцию **or** над выражением поиска, которое оно содержит.</span><span class="sxs-lookup"><span data-stu-id="934d9-143">Represents a search expression that performs a logical **OR** operation on the search expression that it contains.</span></span> <span data-ttu-id="934d9-144">**Или** возвращает **значение true** , если любой из дочерних элементов возвращает **значение true**.</span><span class="sxs-lookup"><span data-stu-id="934d9-144">**Or** will return **true** if any of its children return **true**.</span></span> <span data-ttu-id="934d9-145">**Или** должно иметь не менее двух дочерних элементов.</span><span class="sxs-lookup"><span data-stu-id="934d9-145">**Or** must have two or more children.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="934d9-146">Примечания</span><span class="sxs-lookup"><span data-stu-id="934d9-146">Remarks</span></span>

<span data-ttu-id="934d9-147">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="934d9-147">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="934d9-148">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="934d9-148">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="934d9-149">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="934d9-149">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="934d9-150">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="934d9-150">Schema Name</span></span>  <br/> |<span data-ttu-id="934d9-151">Схема Types</span><span class="sxs-lookup"><span data-stu-id="934d9-151">Types schema</span></span>  <br/> |
|<span data-ttu-id="934d9-152">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="934d9-152">Validation File</span></span>  <br/> |<span data-ttu-id="934d9-153">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="934d9-153">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="934d9-154">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="934d9-154">Can be Empty</span></span>  <br/> |<span data-ttu-id="934d9-155">False</span><span class="sxs-lookup"><span data-stu-id="934d9-155">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="934d9-156">См. также</span><span class="sxs-lookup"><span data-stu-id="934d9-156">See also</span></span>

- [<span data-ttu-id="934d9-157">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="934d9-157">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

