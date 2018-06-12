---
title: IsExternalMailbox
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 5cc83174-e684-42c8-b72a-f82d3de3bb2f
description: Элемент IsExternalMailbox указывает, является ли почтовом ящике внешними по отношению к организации.
ms.openlocfilehash: cf9f71e9b955cffd1bebefd5f23acba66ba1b894
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19834010"
---
# <a name="isexternalmailbox"></a><span data-ttu-id="6cb9d-103">IsExternalMailbox</span><span class="sxs-lookup"><span data-stu-id="6cb9d-103">IsExternalMailbox</span></span>

<span data-ttu-id="6cb9d-104">Элемент **IsExternalMailbox** указывает, является ли почтовом ящике внешними по отношению к организации.</span><span class="sxs-lookup"><span data-stu-id="6cb9d-104">The **IsExternalMailbox** element indicates whether the mailbox is external to the organization.</span></span> 
  
```XML
<IsExternalMailbox>true | false</IsExternalMailbox>
```

 <span data-ttu-id="6cb9d-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="6cb9d-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6cb9d-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="6cb9d-106">Attributes and elements</span></span>

<span data-ttu-id="6cb9d-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="6cb9d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6cb9d-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="6cb9d-108">Attributes</span></span>

<span data-ttu-id="6cb9d-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="6cb9d-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6cb9d-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="6cb9d-110">Child elements</span></span>

<span data-ttu-id="6cb9d-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="6cb9d-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="6cb9d-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="6cb9d-112">Parent elements</span></span>

[<span data-ttu-id="6cb9d-113">SearchableMailbox</span><span class="sxs-lookup"><span data-stu-id="6cb9d-113">SearchableMailbox</span></span>](searchablemailbox.md)
  
## <a name="text-value"></a><span data-ttu-id="6cb9d-114">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="6cb9d-114">Text value</span></span>

<span data-ttu-id="6cb9d-115">Текстовое значение **true** для элемента **IsExternalMailbox** указывает, что почтовый ящик относится к внешней организации.</span><span class="sxs-lookup"><span data-stu-id="6cb9d-115">A text value of **true** for the **IsExternalMailbox** element indicates that the mailbox is in an external organization.</span></span> <span data-ttu-id="6cb9d-116">Значение **false** указывает, что почтовый ящик в организации.</span><span class="sxs-lookup"><span data-stu-id="6cb9d-116">A value of **false** indicates that the mailbox is in the organization.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="6cb9d-117">Замечания</span><span class="sxs-lookup"><span data-stu-id="6cb9d-117">Remarks</span></span>

<span data-ttu-id="6cb9d-118">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="6cb9d-118">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="6cb9d-119">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="6cb9d-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6cb9d-120">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="6cb9d-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6cb9d-121">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="6cb9d-121">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="6cb9d-122">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="6cb9d-122">Schema name</span></span>  <br/> |<span data-ttu-id="6cb9d-123">Схема Types</span><span class="sxs-lookup"><span data-stu-id="6cb9d-123">Types schema</span></span>  <br/> |
|<span data-ttu-id="6cb9d-124">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="6cb9d-124">Validation file</span></span>  <br/> |<span data-ttu-id="6cb9d-125">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="6cb9d-125">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="6cb9d-126">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="6cb9d-126">Can be empty</span></span>  <br/> |<span data-ttu-id="6cb9d-127">False</span><span class="sxs-lookup"><span data-stu-id="6cb9d-127">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6cb9d-128">См. также</span><span class="sxs-lookup"><span data-stu-id="6cb9d-128">See also</span></span>



- [<span data-ttu-id="6cb9d-129">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="6cb9d-129">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

