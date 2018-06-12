---
title: DisplayNameFirstLast
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 013c17c9-cb37-4028-9fe6-c3f47441d0f7
description: Элемент DisplayNameFirstLast указывает отображаемое имя связанного пользователя в формате, имя, Фамилия.
ms.openlocfilehash: 7a8c269c7e1b03448d176a630fbcae979926bdf4
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762172"
---
# <a name="displaynamefirstlast"></a><span data-ttu-id="dfba9-103">DisplayNameFirstLast</span><span class="sxs-lookup"><span data-stu-id="dfba9-103">DisplayNameFirstLast</span></span>

<span data-ttu-id="dfba9-104">Элемент **DisplayNameFirstLast** указывает отображаемое имя связанного пользователя в формате «Имя», «Фамилия».</span><span class="sxs-lookup"><span data-stu-id="dfba9-104">The **DisplayNameFirstLast** element specifies the display name of the associated persona in the format, "First Name", "Last Name".</span></span> 
  
```XML
<DisplayNameFirstLast>
```

 <span data-ttu-id="dfba9-105">**string**</span><span class="sxs-lookup"><span data-stu-id="dfba9-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="dfba9-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="dfba9-106">Attributes and elements</span></span>

<span data-ttu-id="dfba9-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="dfba9-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="dfba9-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="dfba9-108">Attributes</span></span>

<span data-ttu-id="dfba9-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="dfba9-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="dfba9-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="dfba9-110">Child elements</span></span>

<span data-ttu-id="dfba9-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="dfba9-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="dfba9-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="dfba9-112">Parent elements</span></span>

|<span data-ttu-id="dfba9-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="dfba9-113">**Element**</span></span>|<span data-ttu-id="dfba9-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="dfba9-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="dfba9-115">Пользователь</span><span class="sxs-lookup"><span data-stu-id="dfba9-115">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="dfba9-116">Задает набор пользователя данные, возвращаемые запросом **GetPersona** .</span><span class="sxs-lookup"><span data-stu-id="dfba9-116">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="dfba9-117">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="dfba9-117">Text value</span></span>

<span data-ttu-id="dfba9-118">Текстовое значение элемента **DisplayNameFirstLast** — это значение string, содержащая отображаемое имя, с заданным именем сначала.</span><span class="sxs-lookup"><span data-stu-id="dfba9-118">The text value of the **DisplayNameFirstLast** element is a string value containing the display name, with the given name first.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="dfba9-119">Замечания</span><span class="sxs-lookup"><span data-stu-id="dfba9-119">Remarks</span></span>

<span data-ttu-id="dfba9-120">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="dfba9-120">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="dfba9-121">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="dfba9-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="dfba9-122">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="dfba9-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="dfba9-123">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="dfba9-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="dfba9-124">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="dfba9-124">Schema Name</span></span>  <br/> |<span data-ttu-id="dfba9-125">Схема типа</span><span class="sxs-lookup"><span data-stu-id="dfba9-125">Type schema</span></span>  <br/> |
|<span data-ttu-id="dfba9-126">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="dfba9-126">Validation File</span></span>  <br/> |<span data-ttu-id="dfba9-127">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="dfba9-127">types.xsd</span></span>  <br/> |
|<span data-ttu-id="dfba9-128">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="dfba9-128">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="dfba9-129">См. также</span><span class="sxs-lookup"><span data-stu-id="dfba9-129">See also</span></span>

- [<span data-ttu-id="dfba9-130">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="dfba9-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

