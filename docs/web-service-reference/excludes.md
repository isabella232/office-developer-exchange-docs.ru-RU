---
title: Исключает
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Excludes
api_type:
- schema
ms.assetid: bbaeddf6-9a67-4ee0-af99-7a7a5bbdc0e1
description: Элемент Excludes выполняет битовую маску указанного свойства и заданное значение.
ms.openlocfilehash: 73e4eb782a4f54c113ea9a9b67fcf185a9028153
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762423"
---
# <a name="excludes"></a><span data-ttu-id="3c83d-103">Исключает</span><span class="sxs-lookup"><span data-stu-id="3c83d-103">Excludes</span></span>

<span data-ttu-id="3c83d-104">Элемент **Excludes** выполняет битовую маску указанного свойства и заданное значение.</span><span class="sxs-lookup"><span data-stu-id="3c83d-104">The **Excludes** element performs a bitwise mask of the specified property and a supplied value.</span></span> 
  
```xml
<Excludes>
   <FieldURI/>
   <Bitmask/>
</Excludes>
```

 <span data-ttu-id="3c83d-105">**ExcludesType**</span><span class="sxs-lookup"><span data-stu-id="3c83d-105">**ExcludesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3c83d-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="3c83d-106">Attributes and elements</span></span>

<span data-ttu-id="3c83d-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="3c83d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3c83d-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="3c83d-108">Attributes</span></span>

<span data-ttu-id="3c83d-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="3c83d-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3c83d-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="3c83d-110">Child elements</span></span>

|<span data-ttu-id="3c83d-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="3c83d-111">**Element**</span></span>|<span data-ttu-id="3c83d-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="3c83d-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3c83d-113">FieldURI</span><span class="sxs-lookup"><span data-stu-id="3c83d-113">FieldURI</span></span>](fielduri.md) <br/> |<span data-ttu-id="3c83d-114">Идентифицирует часто упоминаемые свойства по URI.</span><span class="sxs-lookup"><span data-stu-id="3c83d-114">Identifies frequently referenced properties by URI.</span></span>  <br/> |
|[<span data-ttu-id="3c83d-115">IndexedFieldURI</span><span class="sxs-lookup"><span data-stu-id="3c83d-115">IndexedFieldURI</span></span>](indexedfielduri.md) <br/> |<span data-ttu-id="3c83d-116">Идентифицирует отдельных элементов словаря.</span><span class="sxs-lookup"><span data-stu-id="3c83d-116">Identifies individual members of a dictionary.</span></span>  <br/> |
|[<span data-ttu-id="3c83d-117">ExtendedFieldURI</span><span class="sxs-lookup"><span data-stu-id="3c83d-117">ExtendedFieldURI</span></span>](extendedfielduri.md) <br/> |<span data-ttu-id="3c83d-118">Задает свойства MAPI.</span><span class="sxs-lookup"><span data-stu-id="3c83d-118">Identifies MAPI properties.</span></span>  <br/> |
|[<span data-ttu-id="3c83d-119">Битовая маска</span><span class="sxs-lookup"><span data-stu-id="3c83d-119">Bitmask</span></span>](bitmask.md) <br/> |<span data-ttu-id="3c83d-120">Представляет шестнадцатеричную или целой и дробной маску, используемый во время операции ограничения [Excludes](excludes.md) .</span><span class="sxs-lookup"><span data-stu-id="3c83d-120">Represents a hexadecimal or decimal mask to be used during an [Excludes](excludes.md) restriction operation.</span></span> <span data-ttu-id="3c83d-121">Если битовая маска, которая представляет это шестнадцатеричный номер, он должен стоять 0 x или 0 X.</span><span class="sxs-lookup"><span data-stu-id="3c83d-121">If the bitmask represents a hexadecimal number, it must be prefixed by 0x or 0X.</span></span> <span data-ttu-id="3c83d-122">В противном случае считается десятичного числа.</span><span class="sxs-lookup"><span data-stu-id="3c83d-122">Otherwise, it will be considered a decimal number.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="3c83d-123">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="3c83d-123">Parent elements</span></span>

|<span data-ttu-id="3c83d-124">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="3c83d-124">**Element**</span></span>|<span data-ttu-id="3c83d-125">**Описание**</span><span class="sxs-lookup"><span data-stu-id="3c83d-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3c83d-126">Ограничения</span><span class="sxs-lookup"><span data-stu-id="3c83d-126">Restriction</span></span>](restriction.md) <br/> |<span data-ttu-id="3c83d-127">Представляет ограничение или запрос, используемый для фильтрации элементов или папок в папке операциях FindItem/FindFolder и поиска.</span><span class="sxs-lookup"><span data-stu-id="3c83d-127">Represents the restriction or query that is used to filter items or folders in FindItem/FindFolder and search folder operations.</span></span>  <br/> |
|[<span data-ttu-id="3c83d-128">Не</span><span class="sxs-lookup"><span data-stu-id="3c83d-128">Not</span></span>](not.md) <br/> |<span data-ttu-id="3c83d-129">Представляет выражение поиска, которое Инвертирует логическое значение выражения поиска, который он содержит.</span><span class="sxs-lookup"><span data-stu-id="3c83d-129">Represents a search expression that negates the Boolean value of the search expression that it contains.</span></span>  <br/> |
|[<span data-ttu-id="3c83d-130">И</span><span class="sxs-lookup"><span data-stu-id="3c83d-130">And</span></span>](and.md) <br/> |<span data-ttu-id="3c83d-131">Представляет выражение поиска, которое позволяет выполнять логическое и операции между двумя или более выражений для поиска.</span><span class="sxs-lookup"><span data-stu-id="3c83d-131">Represents a search expression that allows you to perform a Boolean And operation between two or more search expressions.</span></span> <span data-ttu-id="3c83d-132">Операции получается **значение true,** **Если все выражения поиска, содержащихся в And**.</span><span class="sxs-lookup"><span data-stu-id="3c83d-132">The result of the And operation is **true** if all of the search expressions contained within the And are **true**.</span></span>  <br/> |
|[<span data-ttu-id="3c83d-133">Или</span><span class="sxs-lookup"><span data-stu-id="3c83d-133">Or</span></span>](or.md) <br/> |<span data-ttu-id="3c83d-134">Представляет выражение поиска, используемая для выполнения логического или выражения поиска, которые он содержит.</span><span class="sxs-lookup"><span data-stu-id="3c83d-134">Represents a search expression that performs a logical OR on the search expression it contains.</span></span> <span data-ttu-id="3c83d-135">Элемент [или](or.md) возвращает **значение true** , если какие-либо из их дочерних элементов возвращало **значение true**.</span><span class="sxs-lookup"><span data-stu-id="3c83d-135">The [Or](or.md) element will return **true** if any of its children return **true**.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="3c83d-136">Замечания</span><span class="sxs-lookup"><span data-stu-id="3c83d-136">Remarks</span></span>

 <span data-ttu-id="3c83d-137">**Excludes** решит значение **true** , если операция выполнена на следующих разрешается в 0:</span><span class="sxs-lookup"><span data-stu-id="3c83d-137">**Excludes** will resolve to **true** if an AND operation performed on the following resolves to 0:</span></span> 
  
1. <span data-ttu-id="3c83d-138">Побитовое значение для свойства</span><span class="sxs-lookup"><span data-stu-id="3c83d-138">The bitwise value for the property</span></span>
    
2. <span data-ttu-id="3c83d-139">Битовая маска значение для свойства</span><span class="sxs-lookup"><span data-stu-id="3c83d-139">The bitmask value for the property</span></span>
    
 <span data-ttu-id="3c83d-140">**Excludes** может применяться только для свойства, которое имеет значение типа integer.</span><span class="sxs-lookup"><span data-stu-id="3c83d-140">**Excludes** can only be applied to a property that has an integer value.</span></span> <span data-ttu-id="3c83d-141">Если тип свойства — это что-либо кроме целое число, код ошибки **ErrorUnsupportedPathForQuery** возвращается в ответе.</span><span class="sxs-lookup"><span data-stu-id="3c83d-141">If the property type is anything other than an integer, an error code of **ErrorUnsupportedPathForQuery** is returned in the response.</span></span> 
  
<span data-ttu-id="3c83d-142">Обратный операции можно выполнить путем вызова Not(Excludes).</span><span class="sxs-lookup"><span data-stu-id="3c83d-142">You can perform the reverse operation by calling Not(Excludes).</span></span>
  
<span data-ttu-id="3c83d-143">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="3c83d-143">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3c83d-144">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="3c83d-144">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3c83d-145">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="3c83d-145">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="3c83d-146">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="3c83d-146">Schema Name</span></span>  <br/> |<span data-ttu-id="3c83d-147">Схема Types</span><span class="sxs-lookup"><span data-stu-id="3c83d-147">Types schema</span></span>  <br/> |
|<span data-ttu-id="3c83d-148">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="3c83d-148">Validation File</span></span>  <br/> |<span data-ttu-id="3c83d-149">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="3c83d-149">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="3c83d-150">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="3c83d-150">Can be Empty</span></span>  <br/> |<span data-ttu-id="3c83d-151">False</span><span class="sxs-lookup"><span data-stu-id="3c83d-151">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3c83d-152">См. также</span><span class="sxs-lookup"><span data-stu-id="3c83d-152">See also</span></span>



- [<span data-ttu-id="3c83d-153">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="3c83d-153">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

