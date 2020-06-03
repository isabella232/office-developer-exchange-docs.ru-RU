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
description: Элемент not представляет выражение поиска, которое инвертирует логическое значение содержащегося в нем выражения поиска.
ms.openlocfilehash: 84c64a6d9d39f260d416fc32e4e5f5fcdef027e5
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44466719"
---
# <a name="not"></a><span data-ttu-id="5d363-103">Не</span><span class="sxs-lookup"><span data-stu-id="5d363-103">Not</span></span>

<span data-ttu-id="5d363-104">Элемент **Not** представляет выражение поиска, которое инвертирует логическое значение содержащегося в нем выражения поиска.</span><span class="sxs-lookup"><span data-stu-id="5d363-104">The **Not** element represents a search expression that negates the Boolean value of the search expression that it contains.</span></span> 
  
```xml
<Not>
   <SearchExpression/>
</Not>
```

 <span data-ttu-id="5d363-105">**ноттипе**</span><span class="sxs-lookup"><span data-stu-id="5d363-105">**NotType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5d363-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="5d363-106">Attributes and elements</span></span>

<span data-ttu-id="5d363-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="5d363-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5d363-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="5d363-108">Attributes</span></span>

<span data-ttu-id="5d363-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="5d363-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5d363-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="5d363-110">Child elements</span></span>

|<span data-ttu-id="5d363-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="5d363-111">**Element**</span></span>|<span data-ttu-id="5d363-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="5d363-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5d363-113">сеарчекспрессион</span><span class="sxs-lookup"><span data-stu-id="5d363-113">SearchExpression</span></span>](searchexpression.md) <br/> | <span data-ttu-id="5d363-114">Представляет базовый класс для выражений в ограничении.</span><span class="sxs-lookup"><span data-stu-id="5d363-114">Represents the base class for expressions within a restriction.</span></span> <br/><br/><span data-ttu-id="5d363-115">Для элемента **сеарчекспрессион** необходимо заменить один из следующих элементов:</span><span class="sxs-lookup"><span data-stu-id="5d363-115">One of the following elements must be substituted for the **SearchExpression** element:</span></span> <br/> <br/><span data-ttu-id="5d363-116">- [Существует](exists.md)</span><span class="sxs-lookup"><span data-stu-id="5d363-116">- [Exists](exists.md)</span></span> <br/><span data-ttu-id="5d363-117">- [Исключает](excludes.md)</span><span class="sxs-lookup"><span data-stu-id="5d363-117">- [Excludes](excludes.md)</span></span> <br/><span data-ttu-id="5d363-118">- [исекуалто](isequalto.md)</span><span class="sxs-lookup"><span data-stu-id="5d363-118">- [IsEqualTo](isequalto.md)</span></span> <br/><span data-ttu-id="5d363-119">- [иснотекуалто](isnotequalto.md)</span><span class="sxs-lookup"><span data-stu-id="5d363-119">- [IsNotEqualTo](isnotequalto.md)</span></span> <br/><span data-ttu-id="5d363-120">- [исгреатерсан](isgreaterthan.md)</span><span class="sxs-lookup"><span data-stu-id="5d363-120">- [IsGreaterThan](isgreaterthan.md)</span></span> <br/><span data-ttu-id="5d363-121">- [исгреатерсанорекуалто](isgreaterthanorequalto.md)</span><span class="sxs-lookup"><span data-stu-id="5d363-121">- [IsGreaterThanOrEqualTo](isgreaterthanorequalto.md)</span></span> <br/><span data-ttu-id="5d363-122">- [ислесссан](islessthan.md)</span><span class="sxs-lookup"><span data-stu-id="5d363-122">- [IsLessThan](islessthan.md)</span></span> <br/><span data-ttu-id="5d363-123">- [ислесссанорекуалто](islessthanorequalto.md)</span><span class="sxs-lookup"><span data-stu-id="5d363-123">- [IsLessThanOrEqualTo](islessthanorequalto.md)</span></span> <br/><span data-ttu-id="5d363-124">- [Хранится](contains.md)</span><span class="sxs-lookup"><span data-stu-id="5d363-124">- [Contains](contains.md)</span></span> <br/><span data-ttu-id="5d363-125">- **Не**</span><span class="sxs-lookup"><span data-stu-id="5d363-125">- **Not**</span></span> <br/><span data-ttu-id="5d363-126">- [С](and.md)</span><span class="sxs-lookup"><span data-stu-id="5d363-126">- [And](and.md)</span></span> <br/><span data-ttu-id="5d363-127">- [Также](or.md)</span><span class="sxs-lookup"><span data-stu-id="5d363-127">- [Or](or.md)</span></span> <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="5d363-128">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="5d363-128">Parent elements</span></span>

|<span data-ttu-id="5d363-129">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="5d363-129">**Element**</span></span>|<span data-ttu-id="5d363-130">**Описание**</span><span class="sxs-lookup"><span data-stu-id="5d363-130">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5d363-131">Restriction</span><span class="sxs-lookup"><span data-stu-id="5d363-131">Restriction</span></span>](restriction.md) <br/> |<span data-ttu-id="5d363-132">Представляет ограничение или запрос, используемый для фильтрации элементов или папок в операциях FindItem/FindFolder и папках поиска.</span><span class="sxs-lookup"><span data-stu-id="5d363-132">Represents the restriction or query that is used to filter items or folders in FindItem/FindFolder and search folder operations.</span></span>  <br/> |
|<span data-ttu-id="5d363-133">**Not**</span><span class="sxs-lookup"><span data-stu-id="5d363-133">**Not**</span></span> <br/> |<span data-ttu-id="5d363-134">Представляет выражение поиска, которое инвертирует логическое значение содержащегося в нем выражения поиска.</span><span class="sxs-lookup"><span data-stu-id="5d363-134">Represents a search expression that negates the Boolean value of the search expression that it contains.</span></span>  <br/> |
|[<span data-ttu-id="5d363-135">And</span><span class="sxs-lookup"><span data-stu-id="5d363-135">And</span></span>](and.md) <br/> |<span data-ttu-id="5d363-136">Представляет выражение поиска, которое позволяет выполнять логическую операцию **и** операцию между двумя или более выражениями поиска.</span><span class="sxs-lookup"><span data-stu-id="5d363-136">Represents a search expression that allows you to perform a Boolean **AND** operation between two or more search expressions.</span></span> <span data-ttu-id="5d363-137">Результат операции **and** имеет **значение true** , если все выражения поиска, содержащиеся в элементе **и** , имеют **значение true**.</span><span class="sxs-lookup"><span data-stu-id="5d363-137">The result of the **AND** operation is **true** if all the search expressions contained within the **And** element are **true**.</span></span>  <br/> |
|[<span data-ttu-id="5d363-138">Or</span><span class="sxs-lookup"><span data-stu-id="5d363-138">Or</span></span>](or.md) <br/> |<span data-ttu-id="5d363-139">Представляет выражение поиска, которое выполняет логическую операцию **or** над выражением поиска, которое оно содержит.</span><span class="sxs-lookup"><span data-stu-id="5d363-139">Represents a search expression that performs a logical **OR** operation on the search expression that it contains.</span></span> <span data-ttu-id="5d363-140">**Или** возвращает **значение true** , если любой из дочерних элементов возвращает **значение true**.</span><span class="sxs-lookup"><span data-stu-id="5d363-140">**Or** will return **true** if any of its children return **true**.</span></span> <span data-ttu-id="5d363-141">**Или** должно иметь не менее двух дочерних элементов.</span><span class="sxs-lookup"><span data-stu-id="5d363-141">**Or** must have two or more children.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="5d363-142">Примечания</span><span class="sxs-lookup"><span data-stu-id="5d363-142">Remarks</span></span>

<span data-ttu-id="5d363-143">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="5d363-143">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5d363-144">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="5d363-144">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5d363-145">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="5d363-145">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="5d363-146">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="5d363-146">Schema Name</span></span>  <br/> |<span data-ttu-id="5d363-147">Схема Types</span><span class="sxs-lookup"><span data-stu-id="5d363-147">Types schema</span></span>  <br/> |
|<span data-ttu-id="5d363-148">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="5d363-148">Validation File</span></span>  <br/> |<span data-ttu-id="5d363-149">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="5d363-149">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="5d363-150">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="5d363-150">Can be Empty</span></span>  <br/> |<span data-ttu-id="5d363-151">False</span><span class="sxs-lookup"><span data-stu-id="5d363-151">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="5d363-152">См. также</span><span class="sxs-lookup"><span data-stu-id="5d363-152">See also</span></span>

- [<span data-ttu-id="5d363-153">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="5d363-153">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

