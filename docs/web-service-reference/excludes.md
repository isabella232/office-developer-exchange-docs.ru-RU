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
description: Элемент Excludes выполняет битовую маску указанного свойства и указанного значения.
ms.openlocfilehash: d5fcd8b86b454aa731bd43974b5b7d674fe76ed6
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530616"
---
# <a name="excludes"></a><span data-ttu-id="b103a-103">Исключает</span><span class="sxs-lookup"><span data-stu-id="b103a-103">Excludes</span></span>

<span data-ttu-id="b103a-104">Элемент **Excludes** выполняет битовую маску указанного свойства и указанного значения.</span><span class="sxs-lookup"><span data-stu-id="b103a-104">The **Excludes** element performs a bitwise mask of the specified property and a supplied value.</span></span> 
  
```xml
<Excludes>
   <FieldURI/>
   <Bitmask/>
</Excludes>
```

```xml
<Excludes>
   <ExtendedFieldURI/> 
   <Bitmask/>
</Excludes>
```

```xml
<Excludes>
   <IndexedFieldURI/> 
   <Bitmask/>
</Excludes>
```

<span data-ttu-id="b103a-105">**ексклудестипе**</span><span class="sxs-lookup"><span data-stu-id="b103a-105">**ExcludesType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="b103a-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="b103a-106">Attributes and elements</span></span>

<span data-ttu-id="b103a-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="b103a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b103a-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="b103a-108">Attributes</span></span>

<span data-ttu-id="b103a-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="b103a-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b103a-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="b103a-110">Child elements</span></span>

|<span data-ttu-id="b103a-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="b103a-111">**Element**</span></span>|<span data-ttu-id="b103a-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="b103a-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b103a-113">фиелдури</span><span class="sxs-lookup"><span data-stu-id="b103a-113">FieldURI</span></span>](fielduri.md) <br/> |<span data-ttu-id="b103a-114">Определяет часто упоминаемые свойства по URI.</span><span class="sxs-lookup"><span data-stu-id="b103a-114">Identifies frequently referenced properties by URI.</span></span>  <br/> |
|[<span data-ttu-id="b103a-115">индекседфиелдури</span><span class="sxs-lookup"><span data-stu-id="b103a-115">IndexedFieldURI</span></span>](indexedfielduri.md) <br/> |<span data-ttu-id="b103a-116">Определяет отдельные элементы словаря.</span><span class="sxs-lookup"><span data-stu-id="b103a-116">Identifies individual members of a dictionary.</span></span>  <br/> |
|[<span data-ttu-id="b103a-117">екстендедфиелдури</span><span class="sxs-lookup"><span data-stu-id="b103a-117">ExtendedFieldURI</span></span>](extendedfielduri.md) <br/> |<span data-ttu-id="b103a-118">Определяет свойства MAPI.</span><span class="sxs-lookup"><span data-stu-id="b103a-118">Identifies MAPI properties.</span></span>  <br/> |
|[<span data-ttu-id="b103a-119">Маски</span><span class="sxs-lookup"><span data-stu-id="b103a-119">Bitmask</span></span>](bitmask.md) <br/> |<span data-ttu-id="b103a-120">Представляет шестнадцатеричную или десятичную маску, используемую при выполнении операции ограничения [исключений](excludes.md) .</span><span class="sxs-lookup"><span data-stu-id="b103a-120">Represents a hexadecimal or decimal mask to be used during an [Excludes](excludes.md) restriction operation.</span></span> <span data-ttu-id="b103a-121">Если битовая маска представляет шестнадцатеричное число, она должна иметь префикс 0x или 0X.</span><span class="sxs-lookup"><span data-stu-id="b103a-121">If the bitmask represents a hexadecimal number, it must be prefixed by 0x or 0X.</span></span> <span data-ttu-id="b103a-122">В противном случае он будет считаться десятичным числом.</span><span class="sxs-lookup"><span data-stu-id="b103a-122">Otherwise, it will be considered a decimal number.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="b103a-123">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="b103a-123">Parent elements</span></span>

|<span data-ttu-id="b103a-124">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="b103a-124">**Element**</span></span>|<span data-ttu-id="b103a-125">**Описание**</span><span class="sxs-lookup"><span data-stu-id="b103a-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b103a-126">Restriction</span><span class="sxs-lookup"><span data-stu-id="b103a-126">Restriction</span></span>](restriction.md) <br/> |<span data-ttu-id="b103a-127">Представляет ограничение или запрос, используемый для фильтрации элементов или папок в операциях FindItem/FindFolder и папках поиска.</span><span class="sxs-lookup"><span data-stu-id="b103a-127">Represents the restriction or query that is used to filter items or folders in FindItem/FindFolder and search folder operations.</span></span>  <br/> |
|[<span data-ttu-id="b103a-128">Not</span><span class="sxs-lookup"><span data-stu-id="b103a-128">Not</span></span>](not.md) <br/> |<span data-ttu-id="b103a-129">Представляет выражение поиска, которое инвертирует логическое значение содержащегося в нем выражения поиска.</span><span class="sxs-lookup"><span data-stu-id="b103a-129">Represents a search expression that negates the Boolean value of the search expression that it contains.</span></span>  <br/> |
|[<span data-ttu-id="b103a-130">And</span><span class="sxs-lookup"><span data-stu-id="b103a-130">And</span></span>](and.md) <br/> |<span data-ttu-id="b103a-131">Представляет выражение поиска, которое позволяет выполнять логическую операцию и операцию между двумя или более выражениями поиска.</span><span class="sxs-lookup"><span data-stu-id="b103a-131">Represents a search expression that allows you to perform a Boolean And operation between two or more search expressions.</span></span> <span data-ttu-id="b103a-132">Результат операции and имеет **значение true** , если все выражения поиска, содержащиеся в элементе и, имеют **значение true**.</span><span class="sxs-lookup"><span data-stu-id="b103a-132">The result of the And operation is **true** if all of the search expressions contained within the And are **true**.</span></span>  <br/> |
|[<span data-ttu-id="b103a-133">Or</span><span class="sxs-lookup"><span data-stu-id="b103a-133">Or</span></span>](or.md) <br/> |<span data-ttu-id="b103a-134">Представляет выражение поиска, которое выполняет операцию логического или для содержащегося в нем выражения поиска.</span><span class="sxs-lookup"><span data-stu-id="b103a-134">Represents a search expression that performs a logical OR on the search expression it contains.</span></span> <span data-ttu-id="b103a-135">Элемент [or](or.md) возвращает **значение true** , если любой из дочерних элементов возвращает **значение true**.</span><span class="sxs-lookup"><span data-stu-id="b103a-135">The [Or](or.md) element will return **true** if any of its children return **true**.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="b103a-136">Примечания</span><span class="sxs-lookup"><span data-stu-id="b103a-136">Remarks</span></span>

<span data-ttu-id="b103a-137">**Исключение** будет устранено до **true** , если выполняемая операция, выполняемая над следующими разрешениями, равна 0:</span><span class="sxs-lookup"><span data-stu-id="b103a-137">**Excludes** will resolve to **true** if an AND operation performed on the following resolves to 0:</span></span> 
  
1. <span data-ttu-id="b103a-138">Побитовое значение свойства</span><span class="sxs-lookup"><span data-stu-id="b103a-138">The bitwise value for the property</span></span>
    
2. <span data-ttu-id="b103a-139">Значение битовой маски для свойства.</span><span class="sxs-lookup"><span data-stu-id="b103a-139">The bitmask value for the property</span></span>
    
<span data-ttu-id="b103a-140">**Исключения** можно применять только к свойству, которое имеет целое значение.</span><span class="sxs-lookup"><span data-stu-id="b103a-140">**Excludes** can only be applied to a property that has an integer value.</span></span> <span data-ttu-id="b103a-141">Если тип свойства не является целым числом, в ответе возвращается код ошибки **еррорунсуппортедпасфоркуери** .</span><span class="sxs-lookup"><span data-stu-id="b103a-141">If the property type is anything other than an integer, an error code of **ErrorUnsupportedPathForQuery** is returned in the response.</span></span> 
  
<span data-ttu-id="b103a-142">Можно выполнить обратную операцию, вызвав not (исключение).</span><span class="sxs-lookup"><span data-stu-id="b103a-142">You can perform the reverse operation by calling Not(Excludes).</span></span>
  
<span data-ttu-id="b103a-143">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="b103a-143">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b103a-144">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="b103a-144">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b103a-145">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="b103a-145">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="b103a-146">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="b103a-146">Schema Name</span></span>  <br/> |<span data-ttu-id="b103a-147">Схема Types</span><span class="sxs-lookup"><span data-stu-id="b103a-147">Types schema</span></span>  <br/> |
|<span data-ttu-id="b103a-148">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="b103a-148">Validation File</span></span>  <br/> |<span data-ttu-id="b103a-149">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="b103a-149">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="b103a-150">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="b103a-150">Can be Empty</span></span>  <br/> |<span data-ttu-id="b103a-151">False</span><span class="sxs-lookup"><span data-stu-id="b103a-151">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b103a-152">См. также</span><span class="sxs-lookup"><span data-stu-id="b103a-152">See also</span></span>

- [<span data-ttu-id="b103a-153">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="b103a-153">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

