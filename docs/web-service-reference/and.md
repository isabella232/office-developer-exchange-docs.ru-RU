---
title: И
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
description: Элемент and представляет выражение поиска, которое позволяет выполнять логическую операцию и операцию между двумя или более выражениями поиска. Результат операции AND имеет значение true, если все выражения поиска, содержащиеся в элементе и, имеют значение true.
ms.openlocfilehash: f5239f19c2b5a931eefa9ff4a9dd8ed9d775bae2
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44464723"
---
# <a name="and"></a><span data-ttu-id="46756-104">И</span><span class="sxs-lookup"><span data-stu-id="46756-104">And</span></span>

<span data-ttu-id="46756-105">Элемент **and** представляет выражение поиска, которое позволяет выполнять логическую операцию **и** операцию между двумя или более выражениями поиска.</span><span class="sxs-lookup"><span data-stu-id="46756-105">The **And** element represents a search expression that allows you to perform a Boolean **AND** operation between two or more search expressions.</span></span> <span data-ttu-id="46756-106">Результат операции **and** имеет **значение true** , если все выражения поиска, содержащиеся в элементе **и** , имеют **значение true**.</span><span class="sxs-lookup"><span data-stu-id="46756-106">The result of the **AND** operation is **true** if all the search expressions contained within the **And** element are **true**.</span></span>
  
```xml
<And>
   <SearchExpression/>
   <SearchExpression/>
</And>
```

 <span data-ttu-id="46756-107">**андтипе**</span><span class="sxs-lookup"><span data-stu-id="46756-107">**AndType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="46756-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="46756-108">Attributes and elements</span></span>

<span data-ttu-id="46756-109">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="46756-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="46756-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="46756-110">Attributes</span></span>

<span data-ttu-id="46756-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="46756-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="46756-112">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="46756-112">Child elements</span></span>

|<span data-ttu-id="46756-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="46756-113">**Element**</span></span>|<span data-ttu-id="46756-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="46756-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="46756-115">сеарчекспрессион</span><span class="sxs-lookup"><span data-stu-id="46756-115">SearchExpression</span></span>](searchexpression.md) <br/> | <span data-ttu-id="46756-116">Представляет базовый класс для выражений в ограничении.</span><span class="sxs-lookup"><span data-stu-id="46756-116">Represents the base class for expressions within a restriction.</span></span> <span data-ttu-id="46756-117">В операции and должно быть два или больше выражений поиска.</span><span class="sxs-lookup"><span data-stu-id="46756-117">There must be two or more search expressions in an And operation.</span></span><br/><br/>  <span data-ttu-id="46756-118">Для элемента **сеарчекспрессион** необходимо заменить один из следующих элементов:</span><span class="sxs-lookup"><span data-stu-id="46756-118">One of the following elements must be substituted for the **SearchExpression** element:</span></span><ul><li> [<span data-ttu-id="46756-119">Exists</span><span class="sxs-lookup"><span data-stu-id="46756-119">Exists</span></span>](exists.md)</li><li>[<span data-ttu-id="46756-120">Исключает</span><span class="sxs-lookup"><span data-stu-id="46756-120">Excludes</span></span>](excludes.md)</li><li>[<span data-ttu-id="46756-121">исекуалто</span><span class="sxs-lookup"><span data-stu-id="46756-121">IsEqualTo</span></span>](isequalto.md)</li><li>[<span data-ttu-id="46756-122">иснотекуалто</span><span class="sxs-lookup"><span data-stu-id="46756-122">IsNotEqualTo</span></span>](isnotequalto.md)</li><li>[<span data-ttu-id="46756-123">исгреатерсан</span><span class="sxs-lookup"><span data-stu-id="46756-123">IsGreaterThan</span></span>](isgreaterthan.md)</li><li>[<span data-ttu-id="46756-124">исгреатерсанорекуалто</span><span class="sxs-lookup"><span data-stu-id="46756-124">IsGreaterThanOrEqualTo</span></span>](isgreaterthanorequalto.md)</li><li>[<span data-ttu-id="46756-125">ислесссан</span><span class="sxs-lookup"><span data-stu-id="46756-125">IsLessThan</span></span>](islessthan.md)</li><li>[<span data-ttu-id="46756-126">ислесссанорекуалто</span><span class="sxs-lookup"><span data-stu-id="46756-126">IsLessThanOrEqualTo</span></span>](islessthanorequalto.md)</li><li>[<span data-ttu-id="46756-127">Contains</span><span class="sxs-lookup"><span data-stu-id="46756-127">Contains</span></span>](contains.md)</li><li>[<span data-ttu-id="46756-128">Not</span><span class="sxs-lookup"><span data-stu-id="46756-128">Not</span></span>](not.md)</li><li><span data-ttu-id="46756-129">**And**</span><span class="sxs-lookup"><span data-stu-id="46756-129">**And**</span></span></li><li>[<span data-ttu-id="46756-130">Or</span><span class="sxs-lookup"><span data-stu-id="46756-130">Or</span></span>](or.md) </li></ul> |
   
### <a name="parent-elements"></a><span data-ttu-id="46756-131">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="46756-131">Parent elements</span></span>

|<span data-ttu-id="46756-132">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="46756-132">**Element**</span></span>|<span data-ttu-id="46756-133">**Описание**</span><span class="sxs-lookup"><span data-stu-id="46756-133">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="46756-134">Restriction</span><span class="sxs-lookup"><span data-stu-id="46756-134">Restriction</span></span>](restriction.md) <br/> |<span data-ttu-id="46756-135">Представляет ограничение или запрос, используемый для фильтрации элементов или папок в операциях FindItem/FindFolder и папках поиска.</span><span class="sxs-lookup"><span data-stu-id="46756-135">Represents the restriction or query that is used to filter items or folders in FindItem/FindFolder and search folder operations.</span></span>  <br/> |
|[<span data-ttu-id="46756-136">Not</span><span class="sxs-lookup"><span data-stu-id="46756-136">Not</span></span>](not.md) <br/> |<span data-ttu-id="46756-137">Представляет выражение поиска, которое инвертирует логическое значение содержащегося в нем выражения поиска.</span><span class="sxs-lookup"><span data-stu-id="46756-137">Represents a search expression that negates the Boolean value of the search expression that it contains.</span></span>  <br/> |
|<span data-ttu-id="46756-138">**And**</span><span class="sxs-lookup"><span data-stu-id="46756-138">**And**</span></span> <br/> |<span data-ttu-id="46756-139">Представляет выражение поиска, которое позволяет выполнять логическую операцию **и** операцию между двумя или более выражениями поиска.</span><span class="sxs-lookup"><span data-stu-id="46756-139">Represents a search expression that allows you to perform a Boolean **AND** operation between two or more search expressions.</span></span> <span data-ttu-id="46756-140">Результат операции **and** имеет **значение true** , если все выражения поиска, содержащиеся в элементе **и** , имеют **значение true**.</span><span class="sxs-lookup"><span data-stu-id="46756-140">The result of the **AND** operation is **true** if all of the search expressions contained within the **And** element are **true**.</span></span>  <br/> |
|[<span data-ttu-id="46756-141">Or</span><span class="sxs-lookup"><span data-stu-id="46756-141">Or</span></span>](or.md) <br/> |<span data-ttu-id="46756-142">Представляет выражение поиска, которое выполняет логическую операцию **or** над выражением поиска, которое оно содержит.</span><span class="sxs-lookup"><span data-stu-id="46756-142">Represents a search expression that performs a logical **OR** operation on the search expression that it contains.</span></span> <span data-ttu-id="46756-143">**Или** возвращает **значение true** , если любой из дочерних элементов возвращает **значение true**.</span><span class="sxs-lookup"><span data-stu-id="46756-143">**Or** will return **true** if any of its children return **true**.</span></span> <span data-ttu-id="46756-144">**Или** должно иметь не менее двух дочерних элементов.</span><span class="sxs-lookup"><span data-stu-id="46756-144">**Or** must have two or more children.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="46756-145">Примечания</span><span class="sxs-lookup"><span data-stu-id="46756-145">Remarks</span></span>

<span data-ttu-id="46756-146">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="46756-146">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="46756-147">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="46756-147">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="46756-148">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="46756-148">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="46756-149">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="46756-149">Schema Name</span></span>  <br/> |<span data-ttu-id="46756-150">Схема Types</span><span class="sxs-lookup"><span data-stu-id="46756-150">Types schema</span></span>  <br/> |
|<span data-ttu-id="46756-151">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="46756-151">Validation File</span></span>  <br/> |<span data-ttu-id="46756-152">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="46756-152">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="46756-153">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="46756-153">Can be Empty</span></span>  <br/> |<span data-ttu-id="46756-154">False</span><span class="sxs-lookup"><span data-stu-id="46756-154">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="46756-155">См. также</span><span class="sxs-lookup"><span data-stu-id="46756-155">See also</span></span>

- [<span data-ttu-id="46756-156">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="46756-156">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

