---
title: исгреатерсан
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
description: Элемент Исгреатерсан представляет выражение поиска, которое сравнивает свойство со значением константы или другим свойством и возвращает значение true, если первое свойство больше.
ms.openlocfilehash: 52f2c1b84e4072649092637de091c0dbd8187032
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530045"
---
# <a name="isgreaterthan"></a><span data-ttu-id="66aff-103">исгреатерсан</span><span class="sxs-lookup"><span data-stu-id="66aff-103">IsGreaterThan</span></span>

<span data-ttu-id="66aff-104">Элемент **исгреатерсан** представляет выражение поиска, которое сравнивает свойство со значением константы или другим свойством и возвращает **значение true** , если первое свойство больше.</span><span class="sxs-lookup"><span data-stu-id="66aff-104">The **IsGreaterThan** element represents a search expression that compares a property with either a constant value or another property and returns **true** if the first property is greater.</span></span> 
  
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

<span data-ttu-id="66aff-105">**исгреатерсантипе**</span><span class="sxs-lookup"><span data-stu-id="66aff-105">**IsGreaterThanType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="66aff-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="66aff-106">Attributes and elements</span></span>

<span data-ttu-id="66aff-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="66aff-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="66aff-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="66aff-108">Attributes</span></span>

<span data-ttu-id="66aff-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="66aff-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="66aff-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="66aff-110">Child elements</span></span>

|<span data-ttu-id="66aff-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="66aff-111">**Element**</span></span>|<span data-ttu-id="66aff-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="66aff-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="66aff-113">фиелдури</span><span class="sxs-lookup"><span data-stu-id="66aff-113">FieldURI</span></span>](fielduri.md) <br/> |<span data-ttu-id="66aff-114">Определяет часто упоминаемые свойства по URI.</span><span class="sxs-lookup"><span data-stu-id="66aff-114">Identifies frequently referenced properties by URI.</span></span>  <br/> |
|[<span data-ttu-id="66aff-115">индекседфиелдури</span><span class="sxs-lookup"><span data-stu-id="66aff-115">IndexedFieldURI</span></span>](indexedfielduri.md) <br/> |<span data-ttu-id="66aff-116">Определяет отдельные элементы словаря.</span><span class="sxs-lookup"><span data-stu-id="66aff-116">Identifies individual members of a dictionary.</span></span>  <br/> |
|[<span data-ttu-id="66aff-117">екстендедфиелдури</span><span class="sxs-lookup"><span data-stu-id="66aff-117">ExtendedFieldURI</span></span>](extendedfielduri.md) <br/> |<span data-ttu-id="66aff-118">Определяет свойства MAPI.</span><span class="sxs-lookup"><span data-stu-id="66aff-118">Identifies MAPI properties.</span></span>  <br/> |
|[<span data-ttu-id="66aff-119">фиелдуриорконстант</span><span class="sxs-lookup"><span data-stu-id="66aff-119">FieldURIOrConstant</span></span>](fielduriorconstant.md) <br/> |<span data-ttu-id="66aff-120">Представляет свойство или значение константы, которое будет использоваться при сравнении с другим свойством.</span><span class="sxs-lookup"><span data-stu-id="66aff-120">Represents either a property or a constant value to be used when comparing with another property.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="66aff-121">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="66aff-121">Parent elements</span></span>

|<span data-ttu-id="66aff-122">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="66aff-122">**Element**</span></span>|<span data-ttu-id="66aff-123">**Описание**</span><span class="sxs-lookup"><span data-stu-id="66aff-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="66aff-124">Restriction</span><span class="sxs-lookup"><span data-stu-id="66aff-124">Restriction</span></span>](restriction.md) <br/> |<span data-ttu-id="66aff-125">Представляет ограничение или запрос, используемый для фильтрации элементов или папок в операциях FindItem/FindFolder и папках поиска.</span><span class="sxs-lookup"><span data-stu-id="66aff-125">Represents the restriction or query that is used to filter items or folders in FindItem/FindFolder and search folder operations.</span></span>  <br/> |
|[<span data-ttu-id="66aff-126">Not</span><span class="sxs-lookup"><span data-stu-id="66aff-126">Not</span></span>](not.md) <br/> |<span data-ttu-id="66aff-127">Представляет выражение поиска, которое инвертирует логическое значение содержащегося в нем выражения поиска.</span><span class="sxs-lookup"><span data-stu-id="66aff-127">Represents a search expression that negates the Boolean value of the search expression that it contains.</span></span>  <br/> |
|[<span data-ttu-id="66aff-128">And</span><span class="sxs-lookup"><span data-stu-id="66aff-128">And</span></span>](and.md) <br/> |<span data-ttu-id="66aff-129">Представляет выражение поиска, которое позволяет выполнять логическое действие и операцию между двумя или более выражениями поиска.</span><span class="sxs-lookup"><span data-stu-id="66aff-129">Represents a search expression that enables you to perform a Boolean And operation between two or more search expressions.</span></span> <span data-ttu-id="66aff-130">Результат операции and имеет **значение true** , если все выражения поиска, содержащиеся в элементе и, имеют **значение true**.</span><span class="sxs-lookup"><span data-stu-id="66aff-130">The result of the And operation is **true** if all the search expressions contained within the And are **true**.</span></span>  <br/> |
|[<span data-ttu-id="66aff-131">Or</span><span class="sxs-lookup"><span data-stu-id="66aff-131">Or</span></span>](or.md) <br/> |<span data-ttu-id="66aff-132">Представляет выражение поиска, которое выполняет операцию логического или для содержащегося в нем выражения поиска.</span><span class="sxs-lookup"><span data-stu-id="66aff-132">Represents a search expression that performs a logical OR on the search expression it contains.</span></span> <span data-ttu-id="66aff-133">[Или](or.md) возвращает **значение true** , если любой из дочерних элементов возвращает **значение true**.</span><span class="sxs-lookup"><span data-stu-id="66aff-133">[Or](or.md) will return **true** if any of its children return **true**.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="66aff-134">Примечания</span><span class="sxs-lookup"><span data-stu-id="66aff-134">Remarks</span></span>

<span data-ttu-id="66aff-135">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="66aff-135">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="66aff-136">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="66aff-136">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="66aff-137">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="66aff-137">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="66aff-138">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="66aff-138">Schema Name</span></span>  <br/> |<span data-ttu-id="66aff-139">Схема Types</span><span class="sxs-lookup"><span data-stu-id="66aff-139">Types schema</span></span>  <br/> |
|<span data-ttu-id="66aff-140">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="66aff-140">Validation File</span></span>  <br/> |<span data-ttu-id="66aff-141">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="66aff-141">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="66aff-142">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="66aff-142">Can be Empty</span></span>  <br/> |<span data-ttu-id="66aff-143">False</span><span class="sxs-lookup"><span data-stu-id="66aff-143">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="66aff-144">См. также</span><span class="sxs-lookup"><span data-stu-id="66aff-144">See also</span></span>

- [<span data-ttu-id="66aff-145">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="66aff-145">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

