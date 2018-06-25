---
title: ParentId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: bb7aaa46-3a04-4197-aebb-8881ff10603f
description: Элемент ParentId указывает идентификатор родительского элемента в Предварительный просмотр результатов поиска.
ms.openlocfilehash: ddc76320b1c482e3518a98fb63fc2296143d163c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834698"
---
# <a name="parentid"></a><span data-ttu-id="6b23e-103">ParentId</span><span class="sxs-lookup"><span data-stu-id="6b23e-103">ParentId</span></span>

<span data-ttu-id="6b23e-104">Элемент **ParentId** указывает идентификатор родительского элемента в Предварительный просмотр результатов поиска.</span><span class="sxs-lookup"><span data-stu-id="6b23e-104">The **ParentId** element specifies the identifier of the parent item in a search preview.</span></span> 
  
```XML
<ParentId Id="" ChangeKey=""/>
```

<span data-ttu-id="6b23e-105">**ItemIdType**</span><span class="sxs-lookup"><span data-stu-id="6b23e-105">**ItemIdType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="6b23e-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="6b23e-106">Attributes and elements</span></span>

<span data-ttu-id="6b23e-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="6b23e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6b23e-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="6b23e-108">Attributes</span></span>

|<span data-ttu-id="6b23e-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="6b23e-109">**Attribute**</span></span>|<span data-ttu-id="6b23e-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="6b23e-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="6b23e-111">Id</span><span class="sxs-lookup"><span data-stu-id="6b23e-111">Id</span></span>  <br/> |<span data-ttu-id="6b23e-112">Текстовое значение атрибута **Id** является идентификатор родительского элемента.</span><span class="sxs-lookup"><span data-stu-id="6b23e-112">The text value of the **Id** attribute is the identifier of the parent item.</span></span>  <br/> |
|<span data-ttu-id="6b23e-113">ChangeKey</span><span class="sxs-lookup"><span data-stu-id="6b23e-113">ChangeKey</span></span>  <br/> |<span data-ttu-id="6b23e-114">Текстовое значение атрибута **ChangeKey** — это ключ изменения родительского элемента.</span><span class="sxs-lookup"><span data-stu-id="6b23e-114">The text value of the **ChangeKey** attribute is the change key of the parent item.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="6b23e-115">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="6b23e-115">Child elements</span></span>

<span data-ttu-id="6b23e-116">Нет.</span><span class="sxs-lookup"><span data-stu-id="6b23e-116">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="6b23e-117">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="6b23e-117">Parent elements</span></span>

[<span data-ttu-id="6b23e-118">SearchPreviewItem</span><span class="sxs-lookup"><span data-stu-id="6b23e-118">SearchPreviewItem</span></span>](searchpreviewitem.md)
  
## <a name="remarks"></a><span data-ttu-id="6b23e-119">Замечания</span><span class="sxs-lookup"><span data-stu-id="6b23e-119">Remarks</span></span>

<span data-ttu-id="6b23e-120">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="6b23e-120">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="6b23e-121">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="6b23e-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6b23e-122">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="6b23e-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6b23e-123">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="6b23e-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="6b23e-124">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="6b23e-124">Schema name</span></span>  <br/> |<span data-ttu-id="6b23e-125">Схема Types</span><span class="sxs-lookup"><span data-stu-id="6b23e-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="6b23e-126">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="6b23e-126">Validation file</span></span>  <br/> |<span data-ttu-id="6b23e-127">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="6b23e-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="6b23e-128">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="6b23e-128">Can be empty</span></span>  <br/> |<span data-ttu-id="6b23e-129">true</span><span class="sxs-lookup"><span data-stu-id="6b23e-129">true</span></span>  <br/> |
   

