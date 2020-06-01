---
title: екстендедпропертяттрибутедвалуе
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 90f3c5c5-f612-4e1b-b1f5-f92dd8524179
description: Элемент Екстендедпропертяттрибутедвалуе указывает расширенные свойства для пользователя.
ms.openlocfilehash: 5c2ad5918d7ac666d5e26af6597b2c4c3dde6202
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460129"
---
# <a name="extendedpropertyattributedvalue"></a><span data-ttu-id="9b219-103">екстендедпропертяттрибутедвалуе</span><span class="sxs-lookup"><span data-stu-id="9b219-103">ExtendedPropertyAttributedValue</span></span>

<span data-ttu-id="9b219-104">Элемент **екстендедпропертяттрибутедвалуе** указывает расширенные свойства для пользователя.</span><span class="sxs-lookup"><span data-stu-id="9b219-104">The **ExtendedPropertyAttributedValue** element specifies extended properties for a persona.</span></span> 
  
```XML
<ExtendedPropertyAttributedValue>
    <Value/>
    <Attributions/>
</ExtendedPropertyAttributedValue>
```

 <span data-ttu-id="9b219-105">**екстендедпропертяттрибутедвалуетипе**</span><span class="sxs-lookup"><span data-stu-id="9b219-105">**ExtendedPropertyAttributedValueType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9b219-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="9b219-106">Attributes and elements</span></span>

<span data-ttu-id="9b219-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="9b219-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9b219-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="9b219-108">Attributes</span></span>

<span data-ttu-id="9b219-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="9b219-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9b219-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="9b219-110">Child elements</span></span>

|<span data-ttu-id="9b219-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="9b219-111">**Element**</span></span>|<span data-ttu-id="9b219-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="9b219-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9b219-113">Значение (Екстендедпропертитипе)</span><span class="sxs-lookup"><span data-stu-id="9b219-113">Value (ExtendedPropertyType)</span></span>](value-extendedpropertytype.md) <br/> |<span data-ttu-id="9b219-114">Указывает массив расширенных свойств для пользователя.</span><span class="sxs-lookup"><span data-stu-id="9b219-114">Specifies an array of extended properties for a persona.</span></span>  <br/> |
|[<span data-ttu-id="9b219-115">Атрибуты (Аррайофвалуеаттрибутионстипе)</span><span class="sxs-lookup"><span data-stu-id="9b219-115">Attributions (ArrayOfValueAttributionsType)</span></span>](attributions-arrayofvalueattributionstype.md) <br/> |<span data-ttu-id="9b219-116">Задает массив атрибутов для связанного элемента **value** .</span><span class="sxs-lookup"><span data-stu-id="9b219-116">Specifies an array of attributions for its associated **Value** element.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="9b219-117">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="9b219-117">Parent elements</span></span>

|<span data-ttu-id="9b219-118">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="9b219-118">**Element**</span></span>|<span data-ttu-id="9b219-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="9b219-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9b219-120">Екстендедпропертиес (Аррайофекстендедпропертяттрибутедвалуетипе)</span><span class="sxs-lookup"><span data-stu-id="9b219-120">ExtendedProperties (ArrayOfExtendedPropertyAttributedValueType)</span></span>](extendedproperties-arrayofextendedpropertyattributedvaluetype.md) <br/> |<span data-ttu-id="9b219-121">Содержит расширенные свойства, используемые для операций с единым хранилищем контактов.</span><span class="sxs-lookup"><span data-stu-id="9b219-121">Contains the extended properties used for Unified Contact Store operations.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="9b219-122">Примечания</span><span class="sxs-lookup"><span data-stu-id="9b219-122">Remarks</span></span>

<span data-ttu-id="9b219-123">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="9b219-123">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="9b219-124">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="9b219-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9b219-125">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="9b219-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9b219-126">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="9b219-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="9b219-127">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="9b219-127">Schema Name</span></span>  <br/> |<span data-ttu-id="9b219-128">Схема типа</span><span class="sxs-lookup"><span data-stu-id="9b219-128">Type schema</span></span>  <br/> |
|<span data-ttu-id="9b219-129">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="9b219-129">Validation File</span></span>  <br/> |<span data-ttu-id="9b219-130">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="9b219-130">types.xsd</span></span>  <br/> |
|<span data-ttu-id="9b219-131">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="9b219-131">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="9b219-132">См. также</span><span class="sxs-lookup"><span data-stu-id="9b219-132">See also</span></span>



- [<span data-ttu-id="9b219-133">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="9b219-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

