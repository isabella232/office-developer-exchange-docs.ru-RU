---
title: иснотекуалто
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsNotEqualTo
api_type:
- schema
ms.assetid: e2eff26c-3403-45cd-bb74-1eb98c7dbfcd
description: Элемент Иснотекуалто представляет выражение поиска, которое сравнивает свойство со значением константы или другим свойством и возвращает значение true, если значения не совпадают.
ms.openlocfilehash: 8c40fd1ce8c7c1f14b70f4fccfd3a24e4c99f1b5
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44464191"
---
# <a name="isnotequalto"></a><span data-ttu-id="24dc6-103">иснотекуалто</span><span class="sxs-lookup"><span data-stu-id="24dc6-103">IsNotEqualTo</span></span>

<span data-ttu-id="24dc6-104">Элемент **иснотекуалто** представляет выражение поиска, которое сравнивает свойство со значением константы или другим свойством и возвращает **значение true** , если значения не совпадают.</span><span class="sxs-lookup"><span data-stu-id="24dc6-104">The **IsNotEqualTo** element represents a search expression that compares a property with either a constant value or another property and returns **true** if the values are not the same.</span></span> 
  
```xml
<IsNotEqualTo>
   <FieldURI/>
   <FieldURIOrConstant/>
</IsNotEqualTo>
```

```xml
<IsNotEqualTo>
   <ExtendedFieldURI/> 
   <FieldURIOrConstant/>
</IsNotEqualTo>
```

```xml
<IsNotEqualTo>
   <IndexedFieldURI/>
   <FieldURIOrConstant/>
</IsNotEqualTo>
```

<span data-ttu-id="24dc6-105">**иснотекуалтотипе**</span><span class="sxs-lookup"><span data-stu-id="24dc6-105">**IsNotEqualToType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="24dc6-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="24dc6-106">Attributes and elements</span></span>

<span data-ttu-id="24dc6-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="24dc6-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="24dc6-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="24dc6-108">Attributes</span></span>

<span data-ttu-id="24dc6-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="24dc6-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="24dc6-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="24dc6-110">Child elements</span></span>

|<span data-ttu-id="24dc6-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="24dc6-111">**Element**</span></span>|<span data-ttu-id="24dc6-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="24dc6-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="24dc6-113">фиелдури</span><span class="sxs-lookup"><span data-stu-id="24dc6-113">FieldURI</span></span>](fielduri.md) <br/> |<span data-ttu-id="24dc6-114">Определяет часто упоминаемые свойства по URI.</span><span class="sxs-lookup"><span data-stu-id="24dc6-114">Identifies frequently referenced properties by URI.</span></span>  <br/> |
|[<span data-ttu-id="24dc6-115">индекседфиелдури</span><span class="sxs-lookup"><span data-stu-id="24dc6-115">IndexedFieldURI</span></span>](indexedfielduri.md) <br/> |<span data-ttu-id="24dc6-116">Определяет отдельные элементы словаря.</span><span class="sxs-lookup"><span data-stu-id="24dc6-116">Identifies individual members of a dictionary.</span></span>  <br/> |
|[<span data-ttu-id="24dc6-117">екстендедфиелдури</span><span class="sxs-lookup"><span data-stu-id="24dc6-117">ExtendedFieldURI</span></span>](extendedfielduri.md) <br/> |<span data-ttu-id="24dc6-118">Определяет свойства MAPI.</span><span class="sxs-lookup"><span data-stu-id="24dc6-118">Identifies MAPI properties.</span></span>  <br/> |
|[<span data-ttu-id="24dc6-119">фиелдуриорконстант</span><span class="sxs-lookup"><span data-stu-id="24dc6-119">FieldURIOrConstant</span></span>](fielduriorconstant.md) <br/> |<span data-ttu-id="24dc6-120">Представляет свойство или значение константы, которое будет использоваться при сравнении с другим свойством.</span><span class="sxs-lookup"><span data-stu-id="24dc6-120">Represents either a property or a constant value to be used when comparing with another property.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="24dc6-121">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="24dc6-121">Parent elements</span></span>

|<span data-ttu-id="24dc6-122">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="24dc6-122">**Element**</span></span>|<span data-ttu-id="24dc6-123">**Описание**</span><span class="sxs-lookup"><span data-stu-id="24dc6-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="24dc6-124">Restriction</span><span class="sxs-lookup"><span data-stu-id="24dc6-124">Restriction</span></span>](restriction.md) <br/> |<span data-ttu-id="24dc6-125">Представляет ограничение или запрос, используемый для фильтрации элементов или папок в операциях FindItem/FindFolder и папках поиска.</span><span class="sxs-lookup"><span data-stu-id="24dc6-125">Represents the restriction or query that is used to filter items or folders in FindItem/FindFolder and search folder operations.</span></span>  <br/> |
|[<span data-ttu-id="24dc6-126">Not</span><span class="sxs-lookup"><span data-stu-id="24dc6-126">Not</span></span>](not.md) <br/> |<span data-ttu-id="24dc6-127">Представляет выражение поиска, которое инвертирует логическое значение содержащегося в нем выражения поиска.</span><span class="sxs-lookup"><span data-stu-id="24dc6-127">Represents a search expression that negates the Boolean value of the search expression that it contains.</span></span>  <br/> |
|[<span data-ttu-id="24dc6-128">And</span><span class="sxs-lookup"><span data-stu-id="24dc6-128">And</span></span>](and.md) <br/> |<span data-ttu-id="24dc6-129">Представляет выражение поиска, которое позволяет выполнять логическую операцию и операцию между двумя или более выражениями поиска.</span><span class="sxs-lookup"><span data-stu-id="24dc6-129">Represents a search expression that allows you to perform a Boolean And operation between two or more search expressions.</span></span> <span data-ttu-id="24dc6-130">Результат операции and имеет **значение true** , если все выражения поиска, содержащиеся в элементе и, имеют **значение true**.</span><span class="sxs-lookup"><span data-stu-id="24dc6-130">The result of the And operation is **true** if all of the search expressions contained within the And are **true**.</span></span>  <br/> |
|[<span data-ttu-id="24dc6-131">Or</span><span class="sxs-lookup"><span data-stu-id="24dc6-131">Or</span></span>](or.md) <br/> |<span data-ttu-id="24dc6-132">Представляет выражение поиска, которое выполняет логическую операцию OR для содержащегося в нем выражения поиска.</span><span class="sxs-lookup"><span data-stu-id="24dc6-132">Represents a search expression that performs a logical OR on the search expression that it contains.</span></span> <span data-ttu-id="24dc6-133">[Или](or.md) возвращает **значение true** , если любой из дочерних элементов возвращает **значение true**.</span><span class="sxs-lookup"><span data-stu-id="24dc6-133">[Or](or.md) will return **true** if any of its children return **true**.</span></span> <span data-ttu-id="24dc6-134">**Или** должно иметь не менее двух дочерних элементов.</span><span class="sxs-lookup"><span data-stu-id="24dc6-134">**Or** must have two or more children.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="24dc6-135">Примечания</span><span class="sxs-lookup"><span data-stu-id="24dc6-135">Remarks</span></span>

<span data-ttu-id="24dc6-136">Чтобы выполнить сравнение строк, рассмотрите возможность использования элемента [Contains](contains.md) , так как он предоставляет параметры для сопоставления параметров, таких как регистр и пробел.</span><span class="sxs-lookup"><span data-stu-id="24dc6-136">To perform string comparisons, consider using the [Contains](contains.md) element, as it provides options for matching parameters such as case and white space.</span></span> <span data-ttu-id="24dc6-137">Используйте элемент [Not](not.md) вместе с элементом [Contains](contains.md) , чтобы инвертировать результат.</span><span class="sxs-lookup"><span data-stu-id="24dc6-137">Use the [Not](not.md) element in conjunction with the [Contains](contains.md) element to negate the result.</span></span> 
  
<span data-ttu-id="24dc6-138">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="24dc6-138">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="24dc6-139">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="24dc6-139">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="24dc6-140">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="24dc6-140">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="24dc6-141">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="24dc6-141">Schema Name</span></span>  <br/> |<span data-ttu-id="24dc6-142">Схема Types</span><span class="sxs-lookup"><span data-stu-id="24dc6-142">Types schema</span></span>  <br/> |
|<span data-ttu-id="24dc6-143">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="24dc6-143">Validation File</span></span>  <br/> |<span data-ttu-id="24dc6-144">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="24dc6-144">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="24dc6-145">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="24dc6-145">Can be Empty</span></span>  <br/> |<span data-ttu-id="24dc6-146">False</span><span class="sxs-lookup"><span data-stu-id="24dc6-146">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="24dc6-147">См. также</span><span class="sxs-lookup"><span data-stu-id="24dc6-147">See also</span></span>

- [<span data-ttu-id="24dc6-148">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="24dc6-148">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

