---
title: IsPartiallyIndexed
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 542e7b90-eafe-4711-a9d7-71bbc30d9646
description: Элемент IsPartiallyIndexed указывает ли элемент частично индексированы.
ms.openlocfilehash: e780fac23aeec1d80e547a47b322073fecdc2a0b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834082"
---
# <a name="ispartiallyindexed"></a><span data-ttu-id="930d0-103">IsPartiallyIndexed</span><span class="sxs-lookup"><span data-stu-id="930d0-103">IsPartiallyIndexed</span></span>

<span data-ttu-id="930d0-104">Элемент **IsPartiallyIndexed** указывает ли элемент частично индексированы.</span><span class="sxs-lookup"><span data-stu-id="930d0-104">The **IsPartiallyIndexed** element indicates whether the item is partially indexed.</span></span> 
  
```XML
<IsPartiallyIndexed>true | false</IsPartiallyIndexed>
```

 <span data-ttu-id="930d0-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="930d0-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="930d0-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="930d0-106">Attributes and elements</span></span>

<span data-ttu-id="930d0-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="930d0-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="930d0-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="930d0-108">Attributes</span></span>

<span data-ttu-id="930d0-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="930d0-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="930d0-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="930d0-110">Child elements</span></span>

<span data-ttu-id="930d0-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="930d0-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="930d0-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="930d0-112">Parent elements</span></span>

[<span data-ttu-id="930d0-113">NonIndexableItemDetail</span><span class="sxs-lookup"><span data-stu-id="930d0-113">NonIndexableItemDetail</span></span>](nonindexableitemdetail.md)
  
## <a name="text-value"></a><span data-ttu-id="930d0-114">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="930d0-114">Text value</span></span>

<span data-ttu-id="930d0-115">Текстовое значение **true** для элемента **IsPartiallyIndexed** указывает, что элемент почтового ящика частично индексируются.</span><span class="sxs-lookup"><span data-stu-id="930d0-115">A text value of **true** for the **IsPartiallyIndexed** element indicates that the mailbox item is partially indexed.</span></span> <span data-ttu-id="930d0-116">Значение **false** указывает, что элемент почтового ящика не индексируются частично.</span><span class="sxs-lookup"><span data-stu-id="930d0-116">A value of **false** indicates that the mailbox item is not partially indexed.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="930d0-117">Замечания</span><span class="sxs-lookup"><span data-stu-id="930d0-117">Remarks</span></span>

<span data-ttu-id="930d0-118">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="930d0-118">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="930d0-119">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="930d0-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="930d0-120">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="930d0-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="930d0-121">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="930d0-121">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="930d0-122">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="930d0-122">Schema name</span></span>  <br/> |<span data-ttu-id="930d0-123">Схема Types</span><span class="sxs-lookup"><span data-stu-id="930d0-123">Types schema</span></span>  <br/> |
|<span data-ttu-id="930d0-124">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="930d0-124">Validation file</span></span>  <br/> |<span data-ttu-id="930d0-125">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="930d0-125">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="930d0-126">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="930d0-126">Can be empty</span></span>  <br/> |<span data-ttu-id="930d0-127">Нет</span><span class="sxs-lookup"><span data-stu-id="930d0-127">false</span></span>  <br/> |
   

