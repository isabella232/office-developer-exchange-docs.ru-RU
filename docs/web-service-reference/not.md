---
title: Не
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Not
api_type:
- schema
ms.assetid: 1aa16318-7e90-4b19-bce8-dd1a20a66223
description: Элемент не представляет выражение поиска, которое Инвертирует логическое значение выражения поиска, который он содержит.
ms.openlocfilehash: f5bc709d8b1e77a13b3598905651ac1750436f03
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19834553"
---
# <a name="not"></a><span data-ttu-id="2c465-103">Не</span><span class="sxs-lookup"><span data-stu-id="2c465-103">Not</span></span>

<span data-ttu-id="2c465-104">Элемент **не** представляет выражение поиска, которое Инвертирует логическое значение выражения поиска, который он содержит.</span><span class="sxs-lookup"><span data-stu-id="2c465-104">The **Not** element represents a search expression that negates the Boolean value of the search expression that it contains.</span></span> 
  
```xml
<Not>
   <SearchExpression/>
</Not>
```

 <span data-ttu-id="2c465-105">**NotType**</span><span class="sxs-lookup"><span data-stu-id="2c465-105">**NotType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2c465-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="2c465-106">Attributes and elements</span></span>

<span data-ttu-id="2c465-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="2c465-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2c465-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="2c465-108">Attributes</span></span>

<span data-ttu-id="2c465-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="2c465-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2c465-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="2c465-110">Child elements</span></span>

|<span data-ttu-id="2c465-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="2c465-111">**Element**</span></span>|<span data-ttu-id="2c465-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="2c465-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2c465-113">SearchExpression</span><span class="sxs-lookup"><span data-stu-id="2c465-113">SearchExpression</span></span>](searchexpression.md) <br/> | <span data-ttu-id="2c465-114">Представляет базовый класс для выражений с ограничением.</span><span class="sxs-lookup"><span data-stu-id="2c465-114">Represents the base class for expressions within a restriction.</span></span> <br/><br/><span data-ttu-id="2c465-115">Элемент **SearchExpression** необходимо заменить один из следующих элементов:</span><span class="sxs-lookup"><span data-stu-id="2c465-115">One of the following elements must be substituted for the **SearchExpression** element:</span></span> <br/> <br/><span data-ttu-id="2c465-116">- [Существует](exists.md)</span><span class="sxs-lookup"><span data-stu-id="2c465-116">- [Exists](exists.md)</span></span> <br/><span data-ttu-id="2c465-117">- [Исключает](excludes.md)</span><span class="sxs-lookup"><span data-stu-id="2c465-117">- [Excludes](excludes.md)</span></span> <br/><span data-ttu-id="2c465-118">- [Выражение IsEqualTo](isequalto.md)</span><span class="sxs-lookup"><span data-stu-id="2c465-118">- [IsEqualTo](isequalto.md)</span></span> <br/><span data-ttu-id="2c465-119">- [IsNotEqualTo](isnotequalto.md)</span><span class="sxs-lookup"><span data-stu-id="2c465-119">- [IsNotEqualTo](isnotequalto.md)</span></span> <br/><span data-ttu-id="2c465-120">- [IsGreaterThan](isgreaterthan.md)</span><span class="sxs-lookup"><span data-stu-id="2c465-120">- [IsGreaterThan](isgreaterthan.md)</span></span> <br/><span data-ttu-id="2c465-121">- [IsGreaterThanOrEqualTo](isgreaterthanorequalto.md)</span><span class="sxs-lookup"><span data-stu-id="2c465-121">- [IsGreaterThanOrEqualTo](isgreaterthanorequalto.md)</span></span> <br/><span data-ttu-id="2c465-122">- [IsLessThan](islessthan.md)</span><span class="sxs-lookup"><span data-stu-id="2c465-122">- [IsLessThan](islessthan.md)</span></span> <br/><span data-ttu-id="2c465-123">- [IsLessThanOrEqualTo](islessthanorequalto.md)</span><span class="sxs-lookup"><span data-stu-id="2c465-123">- [IsLessThanOrEqualTo](islessthanorequalto.md)</span></span> <br/><span data-ttu-id="2c465-124">- [Содержит](contains.md)</span><span class="sxs-lookup"><span data-stu-id="2c465-124">- [Contains](contains.md)</span></span> <br/><span data-ttu-id="2c465-125">- **Не**</span><span class="sxs-lookup"><span data-stu-id="2c465-125">- **Not**</span></span> <br/><span data-ttu-id="2c465-126">- [И](and.md)</span><span class="sxs-lookup"><span data-stu-id="2c465-126">- [And](and.md)</span></span> <br/><span data-ttu-id="2c465-127">- [Или](or.md)</span><span class="sxs-lookup"><span data-stu-id="2c465-127">- [Or](or.md)</span></span> <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="2c465-128">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="2c465-128">Parent elements</span></span>

|<span data-ttu-id="2c465-129">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="2c465-129">**Element**</span></span>|<span data-ttu-id="2c465-130">**Описание**</span><span class="sxs-lookup"><span data-stu-id="2c465-130">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2c465-131">Ограничения</span><span class="sxs-lookup"><span data-stu-id="2c465-131">Restriction</span></span>](restriction.md) <br/> |<span data-ttu-id="2c465-132">Представляет ограничение или запрос, используемый для фильтрации элементов или папок в папке операциях FindItem/FindFolder и поиска.</span><span class="sxs-lookup"><span data-stu-id="2c465-132">Represents the restriction or query that is used to filter items or folders in FindItem/FindFolder and search folder operations.</span></span>  <br/> |
|<span data-ttu-id="2c465-133">**Не**</span><span class="sxs-lookup"><span data-stu-id="2c465-133">**Not**</span></span> <br/> |<span data-ttu-id="2c465-134">Представляет выражение поиска, которое Инвертирует логическое значение выражения поиска, который он содержит.</span><span class="sxs-lookup"><span data-stu-id="2c465-134">Represents a search expression that negates the Boolean value of the search expression that it contains.</span></span>  <br/> |
|[<span data-ttu-id="2c465-135">И</span><span class="sxs-lookup"><span data-stu-id="2c465-135">And</span></span>](and.md) <br/> |<span data-ttu-id="2c465-136">Представляет выражение поиска, которое позволяет выполнять операцию логическое **AND** между двумя или более выражений для поиска.</span><span class="sxs-lookup"><span data-stu-id="2c465-136">Represents a search expression that allows you to perform a Boolean **AND** operation between two or more search expressions.</span></span> <span data-ttu-id="2c465-137">Результат **операции** является **значение true** , если все выражения поиска, содержащиеся в элементе **и** имеют **значение true**.</span><span class="sxs-lookup"><span data-stu-id="2c465-137">The result of the **AND** operation is **true** if all the search expressions contained within the **And** element are **true**.</span></span>  <br/> |
|[<span data-ttu-id="2c465-138">Или</span><span class="sxs-lookup"><span data-stu-id="2c465-138">Or</span></span>](or.md) <br/> |<span data-ttu-id="2c465-139">Представляет выражение поиска, которое выполняет операцию логической **или** на нем выражением поиска.</span><span class="sxs-lookup"><span data-stu-id="2c465-139">Represents a search expression that performs a logical **OR** operation on the search expression that it contains.</span></span> <span data-ttu-id="2c465-140">**Или** возвращает **значение true,** Если какие-либо из их дочерних элементов возвращало **значение true**.</span><span class="sxs-lookup"><span data-stu-id="2c465-140">**Or** will return **true** if any of its children return **true**.</span></span> <span data-ttu-id="2c465-141">**Или** должен иметь два или несколько дочерних элементов.</span><span class="sxs-lookup"><span data-stu-id="2c465-141">**Or** must have two or more children.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="2c465-142">Замечания</span><span class="sxs-lookup"><span data-stu-id="2c465-142">Remarks</span></span>

<span data-ttu-id="2c465-143">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="2c465-143">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2c465-144">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="2c465-144">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2c465-145">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="2c465-145">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="2c465-146">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="2c465-146">Schema Name</span></span>  <br/> |<span data-ttu-id="2c465-147">Схема Types</span><span class="sxs-lookup"><span data-stu-id="2c465-147">Types schema</span></span>  <br/> |
|<span data-ttu-id="2c465-148">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="2c465-148">Validation File</span></span>  <br/> |<span data-ttu-id="2c465-149">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="2c465-149">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="2c465-150">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="2c465-150">Can be Empty</span></span>  <br/> |<span data-ttu-id="2c465-151">False</span><span class="sxs-lookup"><span data-stu-id="2c465-151">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="2c465-152">См. также</span><span class="sxs-lookup"><span data-stu-id="2c465-152">See also</span></span>

- [<span data-ttu-id="2c465-153">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="2c465-153">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

