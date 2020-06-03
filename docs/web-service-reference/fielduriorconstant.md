---
title: фиелдуриорконстант
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FieldURIOrConstant
api_type:
- schema
ms.assetid: 89d7a87e-7c93-49b8-83ec-8798e08c1052
description: Элемент Фиелдуриорконстант представляет свойство или значение константы, которое будет использоваться при сравнении с другим свойством.
ms.openlocfilehash: 8b5cb888a3bd2026b15e38fc8c005ab5ef5a2b11
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461228"
---
# <a name="fielduriorconstant"></a><span data-ttu-id="0bf78-103">фиелдуриорконстант</span><span class="sxs-lookup"><span data-stu-id="0bf78-103">FieldURIOrConstant</span></span>

<span data-ttu-id="0bf78-104">Элемент **фиелдуриорконстант** представляет свойство или значение константы, которое будет использоваться при сравнении с другим свойством.</span><span class="sxs-lookup"><span data-stu-id="0bf78-104">The **FieldURIOrConstant** element represents either a property or a constant value to be used when comparing with another property.</span></span> 
  
```xml
<FieldURIOrConstant>
   <Constant/>
</FieldURIOrConstant>
```

```xml
<FieldURIOrConstant>
    <IndexedFieldURI/> 
</FieldURIOrConstant>
```

```xml
<FieldURIOrConstant>
   <FieldURI/>
</FieldURIOrConstant>
```

```xml
<FieldURIOrConstant>
   <ExtendedFieldURI/> 
</FieldURIOrConstant>
```

<span data-ttu-id="0bf78-105">**фиелдуриорконстанттипе**</span><span class="sxs-lookup"><span data-stu-id="0bf78-105">**FieldURIOrConstantType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="0bf78-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="0bf78-106">Attributes and elements</span></span>

<span data-ttu-id="0bf78-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="0bf78-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0bf78-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="0bf78-108">Attributes</span></span>

<span data-ttu-id="0bf78-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="0bf78-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0bf78-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="0bf78-110">Child elements</span></span>

|<span data-ttu-id="0bf78-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="0bf78-111">**Element**</span></span>|<span data-ttu-id="0bf78-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="0bf78-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0bf78-113">Константа</span><span class="sxs-lookup"><span data-stu-id="0bf78-113">Constant</span></span>](constant.md) <br/> |<span data-ttu-id="0bf78-114">Определяет постоянное значение в ограничении.</span><span class="sxs-lookup"><span data-stu-id="0bf78-114">Identifies a constant value in a restriction.</span></span>  <br/> |
|[<span data-ttu-id="0bf78-115">фиелдури</span><span class="sxs-lookup"><span data-stu-id="0bf78-115">FieldURI</span></span>](fielduri.md) <br/> |<span data-ttu-id="0bf78-116">Определяет часто упоминаемые свойства по URI.</span><span class="sxs-lookup"><span data-stu-id="0bf78-116">Identifies frequently referenced properties by URI.</span></span>  <br/> |
|[<span data-ttu-id="0bf78-117">индекседфиелдури</span><span class="sxs-lookup"><span data-stu-id="0bf78-117">IndexedFieldURI</span></span>](indexedfielduri.md) <br/> |<span data-ttu-id="0bf78-118">Определяет отдельные элементы словаря.</span><span class="sxs-lookup"><span data-stu-id="0bf78-118">Identifies individual members of a dictionary.</span></span>  <br/> |
|[<span data-ttu-id="0bf78-119">екстендедфиелдури</span><span class="sxs-lookup"><span data-stu-id="0bf78-119">ExtendedFieldURI</span></span>](extendedfielduri.md) <br/> |<span data-ttu-id="0bf78-120">Определяет свойства MAPI.</span><span class="sxs-lookup"><span data-stu-id="0bf78-120">Identifies MAPI properties.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="0bf78-121">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="0bf78-121">Parent elements</span></span>

|<span data-ttu-id="0bf78-122">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="0bf78-122">**Element**</span></span>|<span data-ttu-id="0bf78-123">**Описание**</span><span class="sxs-lookup"><span data-stu-id="0bf78-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0bf78-124">исекуалто</span><span class="sxs-lookup"><span data-stu-id="0bf78-124">IsEqualTo</span></span>](isequalto.md) <br/> |<span data-ttu-id="0bf78-125">Представляет выражение поиска, которое сравнивает свойство со значением константы или другим свойством и принимает значение true, если они равны.</span><span class="sxs-lookup"><span data-stu-id="0bf78-125">Represents a search expression that compares a property with either a constant value or another property and evaluates to true if they are equal.</span></span>  <br/> |
|[<span data-ttu-id="0bf78-126">исгреатерсан</span><span class="sxs-lookup"><span data-stu-id="0bf78-126">IsGreaterThan</span></span>](isgreaterthan.md) <br/> |<span data-ttu-id="0bf78-127">Представляет выражение поиска, которое сравнивает свойство со значением константы или другим свойством и возвращает значение true, если первое свойство больше.</span><span class="sxs-lookup"><span data-stu-id="0bf78-127">Represents a search expression that compares a property with either a constant value or another property and returns true if the first property is greater.</span></span>  <br/> |
|[<span data-ttu-id="0bf78-128">исгреатерсанорекуалто</span><span class="sxs-lookup"><span data-stu-id="0bf78-128">IsGreaterThanOrEqualTo</span></span>](isgreaterthanorequalto.md) <br/> |<span data-ttu-id="0bf78-129">Представляет выражение поиска, которое сравнивает свойство со значением константы или другим свойством и возвращает значение true, если первое свойство больше или равно второму значению или свойству.</span><span class="sxs-lookup"><span data-stu-id="0bf78-129">Represents a search expression that compares a property with either a constant value or another property and returns true if the first property is greater than or equal to the second value or property.</span></span>  <br/> |
|[<span data-ttu-id="0bf78-130">ислесссан</span><span class="sxs-lookup"><span data-stu-id="0bf78-130">IsLessThan</span></span>](islessthan.md) <br/> |<span data-ttu-id="0bf78-131">Представляет выражение поиска, которое сравнивает свойство со значением константы или другим свойством и возвращает значение true, если первое свойство меньше второго значения или свойства.</span><span class="sxs-lookup"><span data-stu-id="0bf78-131">Represents a search expression that compares a property with either a constant value or another property and returns true if the first property is less than the second value or property.</span></span>  <br/> |
|[<span data-ttu-id="0bf78-132">ислесссанорекуалто</span><span class="sxs-lookup"><span data-stu-id="0bf78-132">IsLessThanOrEqualTo</span></span>](islessthanorequalto.md) <br/> |<span data-ttu-id="0bf78-133">Представляет выражение поиска, которое сравнивает свойство со значением константы или другим свойством и возвращает значение true, если первое свойство меньше второго значения или свойства или равно ему.</span><span class="sxs-lookup"><span data-stu-id="0bf78-133">Represents a search expression that compares a property with either a constant value or another property and returns true if the first property is less than or equal to the second value or property.</span></span>  <br/> |
|[<span data-ttu-id="0bf78-134">иснотекуалто</span><span class="sxs-lookup"><span data-stu-id="0bf78-134">IsNotEqualTo</span></span>](isnotequalto.md) <br/> |<span data-ttu-id="0bf78-135">Представляет выражение поиска, которое сравнивает свойство со значением константы или другим свойством и возвращает значение true, если значения не совпадают.</span><span class="sxs-lookup"><span data-stu-id="0bf78-135">Represents a search expression that compares a property with either a constant value or another property and returns true if the values are not the same.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="0bf78-136">Примечания</span><span class="sxs-lookup"><span data-stu-id="0bf78-136">Remarks</span></span>

<span data-ttu-id="0bf78-137">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="0bf78-137">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="example"></a><span data-ttu-id="0bf78-138">Пример</span><span class="sxs-lookup"><span data-stu-id="0bf78-138">Example</span></span>

<span data-ttu-id="0bf78-139">В приведенном ниже примере XML-кода показан элемент Фиелдуриорконстант, используемый с URI константы и поля.</span><span class="sxs-lookup"><span data-stu-id="0bf78-139">The following XML example shows the FieldURIOrConstant element used with both a constant and field URI.</span></span>
  
```xml
<Restriction>
  <Or xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
    <IsEqualTo>
      <FieldURI FieldURI="item:DateTimeCreated"/>
      <FieldURIOrConstant>
        <FieldURI FieldURI="item:DateTimeReceived"/>
      </FieldURIOrConstant>
    </IsEqualTo>
    <IsEqualTo>
      <FieldURI FieldURI="item:Subject"/>
      <FieldURIOrConstant>
        <Constant Value="Here is a test message"/>
      </FieldURIOrConstant>
    </IsEqualTo>
  </Or>
</Restriction>
```

## <a name="element-information"></a><span data-ttu-id="0bf78-140">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="0bf78-140">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0bf78-141">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="0bf78-141">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="0bf78-142">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="0bf78-142">Schema Name</span></span>  <br/> |<span data-ttu-id="0bf78-143">Схема Types</span><span class="sxs-lookup"><span data-stu-id="0bf78-143">Types schema</span></span>  <br/> |
|<span data-ttu-id="0bf78-144">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="0bf78-144">Validation File</span></span>  <br/> |<span data-ttu-id="0bf78-145">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="0bf78-145">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="0bf78-146">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="0bf78-146">Can be Empty</span></span>  <br/> |<span data-ttu-id="0bf78-147">False</span><span class="sxs-lookup"><span data-stu-id="0bf78-147">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0bf78-148">См. также</span><span class="sxs-lookup"><span data-stu-id="0bf78-148">See also</span></span>

- [<span data-ttu-id="0bf78-149">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="0bf78-149">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

