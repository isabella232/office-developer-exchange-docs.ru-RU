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
ms.openlocfilehash: dfa7c221bb04e59f1ae12eeb5b9f2e1f09aea3ce
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/28/2018
ms.locfileid: "21353492"
---
# <a name="isgreaterthan"></a><span data-ttu-id="f9239-103">IsGreaterThan</span><span class="sxs-lookup"><span data-stu-id="f9239-103">IsGreaterThan</span></span>

<span data-ttu-id="f9239-104">Элемент **IsGreaterThan** представляет выражение поиска, которое сравнивает свойство с постоянным значением или другим свойством и возвращает **значение true,** Если первое свойство больше.</span><span class="sxs-lookup"><span data-stu-id="f9239-104">The **IsGreaterThan** element represents a search expression that compares a property with either a constant value or another property and returns **true** if the first property is greater.</span></span> 
  
```xml
<IsGreaterThan>
   <FieldURI/>
   <FieldURIOrConstant/>
</IsGreaterThan>
```

```xml
<IsGreaterThan>
   <IndexedFieldURI/> 
   <FieldURIOrConstant/>
</IsGreaterThan>
```

```xml
<IsGreaterThan>
   <ExtendedFieldURI/>
   <FieldURIOrConstant/>
</IsGreaterThan>
```

<span data-ttu-id="f9239-105">**IsGreaterThanType**</span><span class="sxs-lookup"><span data-stu-id="f9239-105">**IsGreaterThanType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="f9239-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="f9239-106">Attributes and elements</span></span>

<span data-ttu-id="f9239-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="f9239-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f9239-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="f9239-108">Attributes</span></span>

<span data-ttu-id="f9239-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="f9239-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f9239-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="f9239-110">Child elements</span></span>

|<span data-ttu-id="f9239-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="f9239-111">**Element**</span></span>|<span data-ttu-id="f9239-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="f9239-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f9239-113">FieldURI</span><span class="sxs-lookup"><span data-stu-id="f9239-113">FieldURI</span></span>](fielduri.md) <br/> |<span data-ttu-id="f9239-114">Идентифицирует часто упоминаемые свойства по URI.</span><span class="sxs-lookup"><span data-stu-id="f9239-114">Identifies frequently referenced properties by URI.</span></span>  <br/> |
|[<span data-ttu-id="f9239-115">IndexedFieldURI</span><span class="sxs-lookup"><span data-stu-id="f9239-115">IndexedFieldURI</span></span>](indexedfielduri.md) <br/> |<span data-ttu-id="f9239-116">Идентифицирует отдельных элементов словаря.</span><span class="sxs-lookup"><span data-stu-id="f9239-116">Identifies individual members of a dictionary.</span></span>  <br/> |
|[<span data-ttu-id="f9239-117">ExtendedFieldURI</span><span class="sxs-lookup"><span data-stu-id="f9239-117">ExtendedFieldURI</span></span>](extendedfielduri.md) <br/> |<span data-ttu-id="f9239-118">Задает свойства MAPI.</span><span class="sxs-lookup"><span data-stu-id="f9239-118">Identifies MAPI properties.</span></span>  <br/> |
|[<span data-ttu-id="f9239-119">FieldURIOrConstant</span><span class="sxs-lookup"><span data-stu-id="f9239-119">FieldURIOrConstant</span></span>](fielduriorconstant.md) <br/> |<span data-ttu-id="f9239-120">Представляет свойство или постоянное значение для использования при сравнении с другого свойства.</span><span class="sxs-lookup"><span data-stu-id="f9239-120">Represents either a property or a constant value to be used when comparing with another property.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f9239-121">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="f9239-121">Parent elements</span></span>

|<span data-ttu-id="f9239-122">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="f9239-122">**Element**</span></span>|<span data-ttu-id="f9239-123">**Описание**</span><span class="sxs-lookup"><span data-stu-id="f9239-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f9239-124">Restriction</span><span class="sxs-lookup"><span data-stu-id="f9239-124">Restriction</span></span>](restriction.md) <br/> |<span data-ttu-id="f9239-125">Представляет ограничение или запрос, используемый для фильтрации элементов или папок в папке операциях FindItem/FindFolder и поиска.</span><span class="sxs-lookup"><span data-stu-id="f9239-125">Represents the restriction or query that is used to filter items or folders in FindItem/FindFolder and search folder operations.</span></span>  <br/> |
|[<span data-ttu-id="f9239-126">Не</span><span class="sxs-lookup"><span data-stu-id="f9239-126">Not</span></span>](not.md) <br/> |<span data-ttu-id="f9239-127">Представляет выражение поиска, которое Инвертирует логическое значение выражения поиска, который он содержит.</span><span class="sxs-lookup"><span data-stu-id="f9239-127">Represents a search expression that negates the Boolean value of the search expression that it contains.</span></span>  <br/> |
|[<span data-ttu-id="f9239-128">И</span><span class="sxs-lookup"><span data-stu-id="f9239-128">And</span></span>](and.md) <br/> |<span data-ttu-id="f9239-129">Представляет выражение поиска, которое позволяет выполнять логическое и операции между двумя или более выражений для поиска.</span><span class="sxs-lookup"><span data-stu-id="f9239-129">Represents a search expression that enables you to perform a Boolean And operation between two or more search expressions.</span></span> <span data-ttu-id="f9239-130">Результат операции является **значение true** , если все выражения поиска, содержащихся в And имеют **значение true**.</span><span class="sxs-lookup"><span data-stu-id="f9239-130">The result of the And operation is **true** if all the search expressions contained within the And are **true**.</span></span>  <br/> |
|[<span data-ttu-id="f9239-131">Или</span><span class="sxs-lookup"><span data-stu-id="f9239-131">Or</span></span>](or.md) <br/> |<span data-ttu-id="f9239-132">Представляет выражение поиска, используемая для выполнения логического или выражения поиска, которые он содержит.</span><span class="sxs-lookup"><span data-stu-id="f9239-132">Represents a search expression that performs a logical OR on the search expression it contains.</span></span> <span data-ttu-id="f9239-133">[Или](or.md) возвращает **значение true,** Если какие-либо из их дочерних элементов возвращало **значение true**.</span><span class="sxs-lookup"><span data-stu-id="f9239-133">[Or](or.md) will return **true** if any of its children return **true**.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="f9239-134">Замечания</span><span class="sxs-lookup"><span data-stu-id="f9239-134">Remarks</span></span>

<span data-ttu-id="f9239-135">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="f9239-135">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f9239-136">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="f9239-136">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f9239-137">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="f9239-137">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="f9239-138">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="f9239-138">Schema Name</span></span>  <br/> |<span data-ttu-id="f9239-139">Схема Types</span><span class="sxs-lookup"><span data-stu-id="f9239-139">Types schema</span></span>  <br/> |
|<span data-ttu-id="f9239-140">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="f9239-140">Validation File</span></span>  <br/> |<span data-ttu-id="f9239-141">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="f9239-141">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="f9239-142">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="f9239-142">Can be Empty</span></span>  <br/> |<span data-ttu-id="f9239-143">False</span><span class="sxs-lookup"><span data-stu-id="f9239-143">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f9239-144">См. также</span><span class="sxs-lookup"><span data-stu-id="f9239-144">See also</span></span>

- [<span data-ttu-id="f9239-145">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="f9239-145">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

