---
title: BusinessHomePages
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 9961c0c2-7cac-4af1-84ac-0eafdce0a6ab
description: Элемент BusinessHomePages указывает массив business домашних страниц и идентификаторы их атрибуты источника для связанного пользователя.
ms.openlocfilehash: 52a6c3ca158827b81141e3e174ef79dc511babd7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761624"
---
# <a name="businesshomepages"></a><span data-ttu-id="843e8-103">BusinessHomePages</span><span class="sxs-lookup"><span data-stu-id="843e8-103">BusinessHomePages</span></span>

<span data-ttu-id="843e8-104">Элемент **BusinessHomePages** указывает массив business домашних страниц и идентификаторы их атрибуты источника для связанного пользователя.</span><span class="sxs-lookup"><span data-stu-id="843e8-104">The **BusinessHomePages** element specifies an array of business home pages and the identifiers of their source attributions for the associated persona.</span></span> 
  
```XML
<BusinessHomePages>
    <StringAttributedValue></StringAttributedValue>
</BusinessHomePages>
```

 <span data-ttu-id="843e8-105">**ArrayOfStringAttributedValuesType**</span><span class="sxs-lookup"><span data-stu-id="843e8-105">**ArrayOfStringAttributedValuesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="843e8-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="843e8-106">Attributes and elements</span></span>

<span data-ttu-id="843e8-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="843e8-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="843e8-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="843e8-108">Attributes</span></span>

<span data-ttu-id="843e8-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="843e8-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="843e8-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="843e8-110">Child elements</span></span>

|<span data-ttu-id="843e8-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="843e8-111">**Element**</span></span>|<span data-ttu-id="843e8-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="843e8-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="843e8-113">StringAttributedValue</span><span class="sxs-lookup"><span data-stu-id="843e8-113">StringAttributedValue</span></span>](stringattributedvalue.md) <br/> |<span data-ttu-id="843e8-114">Задает экземпляр в массиве атрибутов, связанных с элементом пользователя.</span><span class="sxs-lookup"><span data-stu-id="843e8-114">Specifies an instance in an array of attributes associated with a persona element.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="843e8-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="843e8-115">Parent elements</span></span>

|<span data-ttu-id="843e8-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="843e8-116">**Element**</span></span>|<span data-ttu-id="843e8-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="843e8-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="843e8-118">Пользователь</span><span class="sxs-lookup"><span data-stu-id="843e8-118">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="843e8-119">Задает набор пользователя данные, возвращаемые запросом **GetPersona** .</span><span class="sxs-lookup"><span data-stu-id="843e8-119">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="843e8-120">Замечания</span><span class="sxs-lookup"><span data-stu-id="843e8-120">Remarks</span></span>

<span data-ttu-id="843e8-121">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="843e8-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="843e8-122">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="843e8-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="843e8-123">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="843e8-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="843e8-124">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="843e8-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="843e8-125">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="843e8-125">Schema Name</span></span>  <br/> |<span data-ttu-id="843e8-126">Схема типа</span><span class="sxs-lookup"><span data-stu-id="843e8-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="843e8-127">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="843e8-127">Validation File</span></span>  <br/> |<span data-ttu-id="843e8-128">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="843e8-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="843e8-129">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="843e8-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="843e8-130">См. также</span><span class="sxs-lookup"><span data-stu-id="843e8-130">See also</span></span>



- [<span data-ttu-id="843e8-131">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="843e8-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

