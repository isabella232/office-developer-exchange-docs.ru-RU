---
title: дисплайнамепрефикс
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 60363698-7603-4051-a66e-007c02db17cb
description: Элемент Дисплайнамепрефикс указывает префикс отображаемого имени соответствующего пользователя.
ms.openlocfilehash: 120a6402be386bc0c11f5859265098324ce4687f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762180"
---
# <a name="displaynameprefix"></a><span data-ttu-id="75dda-103">дисплайнамепрефикс</span><span class="sxs-lookup"><span data-stu-id="75dda-103">DisplayNamePrefix</span></span>

<span data-ttu-id="75dda-104">Элемент **дисплайнамепрефикс** указывает префикс отображаемого имени соответствующего пользователя.</span><span class="sxs-lookup"><span data-stu-id="75dda-104">The **DisplayNamePrefix** element specifies the prefix of the display name of the associated persona.</span></span> 
  
```xml
<DisplayNamePrefix></DisplayNamePrefix>
```

 <span data-ttu-id="75dda-105">**строка**</span><span class="sxs-lookup"><span data-stu-id="75dda-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="75dda-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="75dda-106">Attributes and elements</span></span>

<span data-ttu-id="75dda-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="75dda-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="75dda-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="75dda-108">Attributes</span></span>

<span data-ttu-id="75dda-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="75dda-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="75dda-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="75dda-110">Child elements</span></span>

<span data-ttu-id="75dda-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="75dda-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="75dda-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="75dda-112">Parent elements</span></span>

|<span data-ttu-id="75dda-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="75dda-113">**Element**</span></span>|<span data-ttu-id="75dda-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="75dda-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="75dda-115">Роль</span><span class="sxs-lookup"><span data-stu-id="75dda-115">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="75dda-116">Задает набор данных о пользователях, возвращаемых запросом к **другому человеку** .</span><span class="sxs-lookup"><span data-stu-id="75dda-116">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="75dda-117">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="75dda-117">Text value</span></span>

<span data-ttu-id="75dda-118">Текстовое значение элемента **дисплайнамепрефикс** — это строковое значение, задающее префикс для отображаемого имени.</span><span class="sxs-lookup"><span data-stu-id="75dda-118">The text value of the **DisplayNamePrefix** element is a string value that specifies the prefix for the display name.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="75dda-119">Примечания</span><span class="sxs-lookup"><span data-stu-id="75dda-119">Remarks</span></span>

<span data-ttu-id="75dda-120">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="75dda-120">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="75dda-121">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="75dda-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="75dda-122">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="75dda-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="75dda-123">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="75dda-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="75dda-124">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="75dda-124">Schema Name</span></span>  <br/> |<span data-ttu-id="75dda-125">Схема типа</span><span class="sxs-lookup"><span data-stu-id="75dda-125">Type schema</span></span>  <br/> |
|<span data-ttu-id="75dda-126">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="75dda-126">Validation File</span></span>  <br/> |<span data-ttu-id="75dda-127">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="75dda-127">types.xsd</span></span>  <br/> |
|<span data-ttu-id="75dda-128">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="75dda-128">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="75dda-129">См. также</span><span class="sxs-lookup"><span data-stu-id="75dda-129">See also</span></span>

- [<span data-ttu-id="75dda-130">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="75dda-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

