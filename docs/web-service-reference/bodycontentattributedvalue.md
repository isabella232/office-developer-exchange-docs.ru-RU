---
title: BodyContentAttributedValue
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f99e9590-8388-4203-ac30-1ea394f351a6
description: Элемент BodyContentAttributedValue указывает тела элемента.
ms.openlocfilehash: f5b8f0a19b77ce550b1d7f1c415cc8ee4340863a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761598"
---
# <a name="bodycontentattributedvalue"></a><span data-ttu-id="3d44f-103">BodyContentAttributedValue</span><span class="sxs-lookup"><span data-stu-id="3d44f-103">BodyContentAttributedValue</span></span>

<span data-ttu-id="3d44f-104">Элемент **BodyContentAttributedValue** указывает тела элемента.</span><span class="sxs-lookup"><span data-stu-id="3d44f-104">The **BodyContentAttributedValue** element specifies the body content of an item.</span></span> 
  
```XML
<BodyContentAttributedValue>
   <Value></Value>
   <Attributions></Attributions>
</ BodyContentAttributedValue>
```

 <span data-ttu-id="3d44f-105">**BodyContentAttributedValueType**</span><span class="sxs-lookup"><span data-stu-id="3d44f-105">**BodyContentAttributedValueType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3d44f-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="3d44f-106">Attributes and elements</span></span>

<span data-ttu-id="3d44f-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="3d44f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3d44f-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="3d44f-108">Attributes</span></span>

<span data-ttu-id="3d44f-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="3d44f-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3d44f-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="3d44f-110">Child elements</span></span>

|<span data-ttu-id="3d44f-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="3d44f-111">**Element**</span></span>|<span data-ttu-id="3d44f-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="3d44f-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3d44f-113">Значение (BodyContentType)</span><span class="sxs-lookup"><span data-stu-id="3d44f-113">Value (BodyContentType)</span></span>](value-bodycontenttype.md) <br/> |<span data-ttu-id="3d44f-114">Указывает значение элемента **BodyContentAttributedValue** .</span><span class="sxs-lookup"><span data-stu-id="3d44f-114">Specifies the value of a **BodyContentAttributedValue** element.</span></span>  <br/> |
|[<span data-ttu-id="3d44f-115">Атрибуты (ArrayOfPersonaAttributionsType)</span><span class="sxs-lookup"><span data-stu-id="3d44f-115">Attributions (ArrayOfPersonaAttributionsType)</span></span>](attributions-arrayofpersonaattributionstype.md) <br/> |<span data-ttu-id="3d44f-116">Указывает массив сведений атрибуты для одного или нескольких контактов или объединить в связанного пользователя active directory получателей.</span><span class="sxs-lookup"><span data-stu-id="3d44f-116">Specifies an array of attribution information for one or more of the contacts or active directory recipients aggregated into the associated persona.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="3d44f-117">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="3d44f-117">Parent elements</span></span>

|<span data-ttu-id="3d44f-118">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="3d44f-118">**Element**</span></span>|<span data-ttu-id="3d44f-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="3d44f-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3d44f-120">Текст сообщений</span><span class="sxs-lookup"><span data-stu-id="3d44f-120">Bodies</span></span>](bodies.md) <br/> |<span data-ttu-id="3d44f-121">Указывает массив элементов **BodyContentAttributedValue** .</span><span class="sxs-lookup"><span data-stu-id="3d44f-121">Specifies an array of **BodyContentAttributedValue** elements.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="3d44f-122">Замечания</span><span class="sxs-lookup"><span data-stu-id="3d44f-122">Remarks</span></span>

<span data-ttu-id="3d44f-123">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="3d44f-123">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="3d44f-124">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="3d44f-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3d44f-125">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="3d44f-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3d44f-126">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="3d44f-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="3d44f-127">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="3d44f-127">Schema Name</span></span>  <br/> |<span data-ttu-id="3d44f-128">Схема типа</span><span class="sxs-lookup"><span data-stu-id="3d44f-128">Type schema</span></span>  <br/> |
|<span data-ttu-id="3d44f-129">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="3d44f-129">Validation File</span></span>  <br/> |<span data-ttu-id="3d44f-130">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="3d44f-130">types.xsd</span></span>  <br/> |
|<span data-ttu-id="3d44f-131">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="3d44f-131">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="3d44f-132">См. также</span><span class="sxs-lookup"><span data-stu-id="3d44f-132">See also</span></span>



- [<span data-ttu-id="3d44f-133">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="3d44f-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

