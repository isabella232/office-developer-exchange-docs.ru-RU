---
title: IsGreaterThan
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsGreaterThan
api_type:
- schema
ms.assetid: a6e9d462-cfa7-40ec-903e-128c95050352
description: Элемент IsGreaterThan представляет выражение поиска, которое сравнивает свойство с постоянным значением или другим свойством и возвращает значение true, если первое свойство больше.
ms.openlocfilehash: f36ad646e6c2d415d14d4311a9971a56a85a3121
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19834031"
---
# <a name="isgreaterthan"></a><span data-ttu-id="b693f-103">IsGreaterThan</span><span class="sxs-lookup"><span data-stu-id="b693f-103">IsGreaterThan</span></span>

<span data-ttu-id="b693f-104">Элемент **IsGreaterThan** представляет выражение поиска, которое сравнивает свойство с постоянным значением или другим свойством и возвращает **значение true,** Если первое свойство больше.</span><span class="sxs-lookup"><span data-stu-id="b693f-104">The **IsGreaterThan** element represents a search expression that compares a property with either a constant value or another property and returns **true** if the first property is greater.</span></span> 
  
```xml
<IsGreaterThan>
   <FieldURI/>
   <FieldURIOrConstant/>
</IsGreaterThan>
```

 <span data-ttu-id="b693f-105">**IsGreaterThanType**</span><span class="sxs-lookup"><span data-stu-id="b693f-105">**IsGreaterThanType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b693f-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="b693f-106">Attributes and elements</span></span>

<span data-ttu-id="b693f-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="b693f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b693f-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="b693f-108">Attributes</span></span>

<span data-ttu-id="b693f-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="b693f-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b693f-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="b693f-110">Child elements</span></span>

|<span data-ttu-id="b693f-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="b693f-111">**Element**</span></span>|<span data-ttu-id="b693f-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="b693f-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b693f-113">FieldURI</span><span class="sxs-lookup"><span data-stu-id="b693f-113">FieldURI</span></span>](fielduri.md) <br/> |<span data-ttu-id="b693f-114">Идентифицирует часто упоминаемые свойства по URI.</span><span class="sxs-lookup"><span data-stu-id="b693f-114">Identifies frequently referenced properties by URI.</span></span>  <br/> |
|[<span data-ttu-id="b693f-115">IndexedFieldURI</span><span class="sxs-lookup"><span data-stu-id="b693f-115">IndexedFieldURI</span></span>](indexedfielduri.md) <br/> |<span data-ttu-id="b693f-116">Идентифицирует отдельных элементов словаря.</span><span class="sxs-lookup"><span data-stu-id="b693f-116">Identifies individual members of a dictionary.</span></span>  <br/> |
|[<span data-ttu-id="b693f-117">ExtendedFieldURI</span><span class="sxs-lookup"><span data-stu-id="b693f-117">ExtendedFieldURI</span></span>](extendedfielduri.md) <br/> |<span data-ttu-id="b693f-118">Задает свойства MAPI.</span><span class="sxs-lookup"><span data-stu-id="b693f-118">Identifies MAPI properties.</span></span>  <br/> |
|[<span data-ttu-id="b693f-119">FieldURIOrConstant</span><span class="sxs-lookup"><span data-stu-id="b693f-119">FieldURIOrConstant</span></span>](fielduriorconstant.md) <br/> |<span data-ttu-id="b693f-120">Представляет свойство или постоянное значение для использования при сравнении с другого свойства.</span><span class="sxs-lookup"><span data-stu-id="b693f-120">Represents either a property or a constant value to be used when comparing with another property.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="b693f-121">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="b693f-121">Parent elements</span></span>

|<span data-ttu-id="b693f-122">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="b693f-122">**Element**</span></span>|<span data-ttu-id="b693f-123">**Описание**</span><span class="sxs-lookup"><span data-stu-id="b693f-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b693f-124">Ограничения</span><span class="sxs-lookup"><span data-stu-id="b693f-124">Restriction</span></span>](restriction.md) <br/> |<span data-ttu-id="b693f-125">Представляет ограничение или запрос, используемый для фильтрации элементов или папок в папке операциях FindItem/FindFolder и поиска.</span><span class="sxs-lookup"><span data-stu-id="b693f-125">Represents the restriction or query that is used to filter items or folders in FindItem/FindFolder and search folder operations.</span></span>  <br/> |
|[<span data-ttu-id="b693f-126">Не</span><span class="sxs-lookup"><span data-stu-id="b693f-126">Not</span></span>](not.md) <br/> |<span data-ttu-id="b693f-127">Представляет выражение поиска, которое Инвертирует логическое значение выражения поиска, который он содержит.</span><span class="sxs-lookup"><span data-stu-id="b693f-127">Represents a search expression that negates the Boolean value of the search expression that it contains.</span></span>  <br/> |
|[<span data-ttu-id="b693f-128">И</span><span class="sxs-lookup"><span data-stu-id="b693f-128">And</span></span>](and.md) <br/> |<span data-ttu-id="b693f-129">Представляет выражение поиска, которое позволяет выполнять логическое и операции между двумя или более выражений для поиска.</span><span class="sxs-lookup"><span data-stu-id="b693f-129">Represents a search expression that enables you to perform a Boolean And operation between two or more search expressions.</span></span> <span data-ttu-id="b693f-130">Результат операции является **значение true** , если все выражения поиска, содержащихся в And имеют **значение true**.</span><span class="sxs-lookup"><span data-stu-id="b693f-130">The result of the And operation is **true** if all the search expressions contained within the And are **true**.</span></span>  <br/> |
|[<span data-ttu-id="b693f-131">Или</span><span class="sxs-lookup"><span data-stu-id="b693f-131">Or</span></span>](or.md) <br/> |<span data-ttu-id="b693f-132">Представляет выражение поиска, используемая для выполнения логического или выражения поиска, которые он содержит.</span><span class="sxs-lookup"><span data-stu-id="b693f-132">Represents a search expression that performs a logical OR on the search expression it contains.</span></span> <span data-ttu-id="b693f-133">[Или](or.md) возвращает **значение true,** Если какие-либо из их дочерних элементов возвращало **значение true**.</span><span class="sxs-lookup"><span data-stu-id="b693f-133">[Or](or.md) will return **true** if any of its children return **true**.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="b693f-134">Замечания</span><span class="sxs-lookup"><span data-stu-id="b693f-134">Remarks</span></span>

<span data-ttu-id="b693f-135">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="b693f-135">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b693f-136">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="b693f-136">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b693f-137">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="b693f-137">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="b693f-138">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="b693f-138">Schema Name</span></span>  <br/> |<span data-ttu-id="b693f-139">Схема Types</span><span class="sxs-lookup"><span data-stu-id="b693f-139">Types schema</span></span>  <br/> |
|<span data-ttu-id="b693f-140">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="b693f-140">Validation File</span></span>  <br/> |<span data-ttu-id="b693f-141">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="b693f-141">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="b693f-142">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="b693f-142">Can be Empty</span></span>  <br/> |<span data-ttu-id="b693f-143">False</span><span class="sxs-lookup"><span data-stu-id="b693f-143">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b693f-144">См. также</span><span class="sxs-lookup"><span data-stu-id="b693f-144">See also</span></span>



- [<span data-ttu-id="b693f-145">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="b693f-145">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

