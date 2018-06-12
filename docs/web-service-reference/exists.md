---
title: Exists
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Exists
api_type:
- schema
ms.assetid: 55d568bd-8dbc-4d50-b9d7-54b74a54d4b5
description: Элемент Exists представляет выражение поиска, которое возвращает значение true, если задано указанное свойство элемента.
ms.openlocfilehash: d30f4b505afcac32afbfeaf2289c964ba145668e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762426"
---
# <a name="exists"></a><span data-ttu-id="b41dd-103">Exists</span><span class="sxs-lookup"><span data-stu-id="b41dd-103">Exists</span></span>

<span data-ttu-id="b41dd-104">Элемент **Exists** представляет выражение поиска, которое возвращает **значение true, если существует указанное свойство элемента** .</span><span class="sxs-lookup"><span data-stu-id="b41dd-104">The **Exists** element represents a search expression that returns **true** if the supplied property exists on an item.</span></span> 
  
```xml
<Exists>
   <Path/>
</Exists>
```

 <span data-ttu-id="b41dd-105">**ExistsType**</span><span class="sxs-lookup"><span data-stu-id="b41dd-105">**ExistsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b41dd-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="b41dd-106">Attributes and elements</span></span>

<span data-ttu-id="b41dd-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="b41dd-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b41dd-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="b41dd-108">Attributes</span></span>

<span data-ttu-id="b41dd-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="b41dd-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b41dd-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="b41dd-110">Child elements</span></span>

|<span data-ttu-id="b41dd-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="b41dd-111">**Element**</span></span>|<span data-ttu-id="b41dd-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="b41dd-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b41dd-113">FieldURI</span><span class="sxs-lookup"><span data-stu-id="b41dd-113">FieldURI</span></span>](fielduri.md) <br/> |<span data-ttu-id="b41dd-114">Идентифицирует часто упоминаемые свойства по URI.</span><span class="sxs-lookup"><span data-stu-id="b41dd-114">Identifies frequently referenced properties by URI.</span></span>  <br/> |
|[<span data-ttu-id="b41dd-115">IndexedFieldURI</span><span class="sxs-lookup"><span data-stu-id="b41dd-115">IndexedFieldURI</span></span>](indexedfielduri.md) <br/> |<span data-ttu-id="b41dd-116">Идентифицирует отдельных элементов словаря.</span><span class="sxs-lookup"><span data-stu-id="b41dd-116">Identifies individual members of a dictionary.</span></span>  <br/> |
|[<span data-ttu-id="b41dd-117">ExtendedFieldURI</span><span class="sxs-lookup"><span data-stu-id="b41dd-117">ExtendedFieldURI</span></span>](extendedfielduri.md) <br/> |<span data-ttu-id="b41dd-118">Задает свойства MAPI.</span><span class="sxs-lookup"><span data-stu-id="b41dd-118">Identifies MAPI properties.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="b41dd-119">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="b41dd-119">Parent elements</span></span>

|<span data-ttu-id="b41dd-120">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="b41dd-120">**Element**</span></span>|<span data-ttu-id="b41dd-121">**Описание**</span><span class="sxs-lookup"><span data-stu-id="b41dd-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b41dd-122">Ограничения</span><span class="sxs-lookup"><span data-stu-id="b41dd-122">Restriction</span></span>](restriction.md) <br/> |<span data-ttu-id="b41dd-123">Представляет ограничение или запрос, используемый для фильтрации элементов или папок в папке операциях FindItem/FindFolder и поиска.</span><span class="sxs-lookup"><span data-stu-id="b41dd-123">Represents the restriction or query that is used to filter items or folders in FindItem/FindFolder and search folder operations.</span></span>  <br/> |
|[<span data-ttu-id="b41dd-124">Не</span><span class="sxs-lookup"><span data-stu-id="b41dd-124">Not</span></span>](not.md) <br/> |<span data-ttu-id="b41dd-125">Представляет выражение поиска, которое Инвертирует логическое значение выражения поиска, который он содержит.</span><span class="sxs-lookup"><span data-stu-id="b41dd-125">Represents a search expression that negates the Boolean value of the search expression that it contains.</span></span>  <br/> |
|[<span data-ttu-id="b41dd-126">И</span><span class="sxs-lookup"><span data-stu-id="b41dd-126">And</span></span>](and.md) <br/> |<span data-ttu-id="b41dd-127">Представляет выражение поиска, которое позволяет выполнять логическое и операции между двумя или более выражений для поиска.</span><span class="sxs-lookup"><span data-stu-id="b41dd-127">Represents a search expression that enables you to perform a Boolean And operation between two or more search expressions.</span></span> <span data-ttu-id="b41dd-128">Результат операции является **значение true** , если все выражения поиска, содержащихся в And имеют **значение true**.</span><span class="sxs-lookup"><span data-stu-id="b41dd-128">The result of the And operation is **true** if all the search expressions contained within the And are **true**.</span></span>  <br/> |
|[<span data-ttu-id="b41dd-129">Или</span><span class="sxs-lookup"><span data-stu-id="b41dd-129">Or</span></span>](or.md) <br/> |<span data-ttu-id="b41dd-130">Представляет выражение поиска, используемая для выполнения логического или на нем выражением поиска.</span><span class="sxs-lookup"><span data-stu-id="b41dd-130">Represents a search expression that performs a logical OR on the search expression that it contains.</span></span> <span data-ttu-id="b41dd-131">[Или](or.md) возвращает **значение true,** Если какие-либо из их дочерних элементов возвращало **значение true**.</span><span class="sxs-lookup"><span data-stu-id="b41dd-131">[Or](or.md) will return **true** if any of its children return **true**.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="b41dd-132">Замечания</span><span class="sxs-lookup"><span data-stu-id="b41dd-132">Remarks</span></span>

<span data-ttu-id="b41dd-133">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="b41dd-133">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b41dd-134">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="b41dd-134">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b41dd-135">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="b41dd-135">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="b41dd-136">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="b41dd-136">Schema Name</span></span>  <br/> |<span data-ttu-id="b41dd-137">Схема Types</span><span class="sxs-lookup"><span data-stu-id="b41dd-137">Types schema</span></span>  <br/> |
|<span data-ttu-id="b41dd-138">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="b41dd-138">Validation File</span></span>  <br/> |<span data-ttu-id="b41dd-139">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="b41dd-139">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="b41dd-140">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="b41dd-140">Can be Empty</span></span>  <br/> |<span data-ttu-id="b41dd-141">False</span><span class="sxs-lookup"><span data-stu-id="b41dd-141">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b41dd-142">См. также</span><span class="sxs-lookup"><span data-stu-id="b41dd-142">See also</span></span>



- [<span data-ttu-id="b41dd-143">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="b41dd-143">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

