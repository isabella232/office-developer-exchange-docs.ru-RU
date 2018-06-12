---
title: BaseShape (PreviewItemBaseShapeType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 7b9e2fdd-5678-4178-9297-7f12a3ca9d64
description: Элемент BaseShape указывает предварительного просмотра по умолчанию возвращаются все свойства или compact предварительного просмотра с меньшим количеством возвращаемых свойств.
ms.openlocfilehash: 1f060ae9adf52cc2916a634e3d954e3fc0903941
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761549"
---
# <a name="baseshape-previewitembaseshapetype"></a><span data-ttu-id="61367-103">BaseShape (PreviewItemBaseShapeType)</span><span class="sxs-lookup"><span data-stu-id="61367-103">BaseShape (PreviewItemBaseShapeType)</span></span>

<span data-ttu-id="61367-104">Элемент **BaseShape** указывает предварительного просмотра по умолчанию возвращаются все свойства или compact предварительного просмотра с меньшим количеством возвращаемых свойств.</span><span class="sxs-lookup"><span data-stu-id="61367-104">The **BaseShape** element specifies either the default preview with all properties returned or a compact preview with fewer properties returned.</span></span> 
  
```XML
<BaseShape> Default | Compact</BaseShape>
```

 <span data-ttu-id="61367-105">**PreviewItemBaseShapeType**</span><span class="sxs-lookup"><span data-stu-id="61367-105">**PreviewItemBaseShapeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="61367-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="61367-106">Attributes and elements</span></span>

<span data-ttu-id="61367-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="61367-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="61367-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="61367-108">Attributes</span></span>

<span data-ttu-id="61367-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="61367-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="61367-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="61367-110">Child elements</span></span>

<span data-ttu-id="61367-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="61367-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="61367-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="61367-112">Parent elements</span></span>

|<span data-ttu-id="61367-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="61367-113">**Element**</span></span>|<span data-ttu-id="61367-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="61367-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="61367-115">PreviewItemResponseShape</span><span class="sxs-lookup"><span data-stu-id="61367-115">PreviewItemResponseShape</span></span>](previewitemresponseshape.md) <br/> |<span data-ttu-id="61367-116">Содержит фигуры ответа.</span><span class="sxs-lookup"><span data-stu-id="61367-116">Contains the shape of the response.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="61367-117">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="61367-117">Text value</span></span>

<span data-ttu-id="61367-118">**BaseShape элемент текстовые значения**</span><span class="sxs-lookup"><span data-stu-id="61367-118">**BaseShape element text values**</span></span>

|<span data-ttu-id="61367-119">**Значение**</span><span class="sxs-lookup"><span data-stu-id="61367-119">**Value**</span></span>|<span data-ttu-id="61367-120">**Описание**</span><span class="sxs-lookup"><span data-stu-id="61367-120">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="61367-121">Значение по умолчанию</span><span class="sxs-lookup"><span data-stu-id="61367-121">Default</span></span>  <br/> |<span data-ttu-id="61367-122">Указывает, что отображаются все свойства.</span><span class="sxs-lookup"><span data-stu-id="61367-122">Indicates that all properties are shown.</span></span>  <br/> |
|<span data-ttu-id="61367-123">Сжатие</span><span class="sxs-lookup"><span data-stu-id="61367-123">Compact</span></span>  <br/> |<span data-ttu-id="61367-124">Указывает, что отображаются только выбранных свойств.</span><span class="sxs-lookup"><span data-stu-id="61367-124">Indicates that only selected properties are shown.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="61367-125">Замечания</span><span class="sxs-lookup"><span data-stu-id="61367-125">Remarks</span></span>

<span data-ttu-id="61367-126">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="61367-126">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="61367-127">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="61367-127">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="61367-128">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="61367-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="61367-129">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="61367-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="61367-130">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="61367-130">Schema Name</span></span>  <br/> |<span data-ttu-id="61367-131">Схема типа</span><span class="sxs-lookup"><span data-stu-id="61367-131">Type schema</span></span>  <br/> |
|<span data-ttu-id="61367-132">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="61367-132">Validation File</span></span>  <br/> |<span data-ttu-id="61367-133">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="61367-133">types.xsd</span></span>  <br/> |
|<span data-ttu-id="61367-134">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="61367-134">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="61367-135">См. также</span><span class="sxs-lookup"><span data-stu-id="61367-135">See also</span></span>



- [<span data-ttu-id="61367-136">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="61367-136">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

