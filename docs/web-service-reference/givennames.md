---
title: GivenNames
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 64d86c24-07b8-448d-ad37-47f104777df3
description: Элемент GivenNames указывает массив значений заданным именем и идентификаторы их атрибуты источника для связанного пользователя.
ms.openlocfilehash: dc86517a06dab0f74350c71488f68bb06e2272bd
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833709"
---
# <a name="givennames"></a><span data-ttu-id="0cb53-103">GivenNames</span><span class="sxs-lookup"><span data-stu-id="0cb53-103">GivenNames</span></span>

<span data-ttu-id="0cb53-104">Элемент **GivenNames** указывает массив значений заданным именем и идентификаторы их атрибуты источника для связанного пользователя.</span><span class="sxs-lookup"><span data-stu-id="0cb53-104">The **GivenNames** element specifies an array of given name values and the identifiers of their source attributions for the associated persona.</span></span> 
  
```xml
<GivenNames>
    <StringAttributedValue/>
</GivenNames>
```

 <span data-ttu-id="0cb53-105">**ArrayOfStringAttributedValuesType**</span><span class="sxs-lookup"><span data-stu-id="0cb53-105">**ArrayOfStringAttributedValuesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0cb53-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="0cb53-106">Attributes and elements</span></span>

<span data-ttu-id="0cb53-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="0cb53-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0cb53-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="0cb53-108">Attributes</span></span>

<span data-ttu-id="0cb53-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="0cb53-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0cb53-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="0cb53-110">Child elements</span></span>

|<span data-ttu-id="0cb53-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="0cb53-111">**Element**</span></span>|<span data-ttu-id="0cb53-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="0cb53-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0cb53-113">StringAttributedValue</span><span class="sxs-lookup"><span data-stu-id="0cb53-113">StringAttributedValue</span></span>](stringattributedvalue.md) <br/> |<span data-ttu-id="0cb53-114">Задает экземпляр в массиве атрибутов, связанных с элементом пользователя.</span><span class="sxs-lookup"><span data-stu-id="0cb53-114">Specifies an instance in an array of attributes associated with a persona element.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="0cb53-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="0cb53-115">Parent elements</span></span>

|<span data-ttu-id="0cb53-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="0cb53-116">**Element**</span></span>|<span data-ttu-id="0cb53-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="0cb53-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0cb53-118">Пользователь</span><span class="sxs-lookup"><span data-stu-id="0cb53-118">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="0cb53-119">Задает набор пользователя данные, возвращаемые запросом **GetPersona** .</span><span class="sxs-lookup"><span data-stu-id="0cb53-119">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="0cb53-120">Замечания</span><span class="sxs-lookup"><span data-stu-id="0cb53-120">Remarks</span></span>

<span data-ttu-id="0cb53-121">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="0cb53-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="0cb53-122">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="0cb53-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0cb53-123">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="0cb53-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0cb53-124">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="0cb53-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="0cb53-125">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="0cb53-125">Schema Name</span></span>  <br/> |<span data-ttu-id="0cb53-126">Схема типа</span><span class="sxs-lookup"><span data-stu-id="0cb53-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="0cb53-127">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="0cb53-127">Validation File</span></span>  <br/> |<span data-ttu-id="0cb53-128">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="0cb53-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="0cb53-129">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="0cb53-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="0cb53-130">См. также</span><span class="sxs-lookup"><span data-stu-id="0cb53-130">See also</span></span>



- [<span data-ttu-id="0cb53-131">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="0cb53-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

