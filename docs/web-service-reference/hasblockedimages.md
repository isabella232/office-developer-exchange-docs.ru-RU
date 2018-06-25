---
title: HasBlockedImages
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: ddeb11db-797d-4939-91d5-3e44be5f0778
description: Элемент HasBlockedImages задает логическое значение, указывающее, заблокирован ли элемент изображений.
ms.openlocfilehash: fbe9967c898016aeef27e3c86e8a1cf603bd87fc
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833795"
---
# <a name="hasblockedimages"></a><span data-ttu-id="72476-103">HasBlockedImages</span><span class="sxs-lookup"><span data-stu-id="72476-103">HasBlockedImages</span></span>

<span data-ttu-id="72476-104">Элемент **HasBlockedImages** задает логическое значение, указывающее, заблокирован ли элемент изображений.</span><span class="sxs-lookup"><span data-stu-id="72476-104">The **HasBlockedImages** element specifies a Boolean value that indicates whether the item has blocked images.</span></span> 
  
```XML
<HasBlockedImages> true | false </HasBlockedImages>
```

 <span data-ttu-id="72476-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="72476-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="72476-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="72476-106">Attributes and elements</span></span>

<span data-ttu-id="72476-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="72476-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="72476-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="72476-108">Attributes</span></span>

<span data-ttu-id="72476-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="72476-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="72476-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="72476-110">Child elements</span></span>

<span data-ttu-id="72476-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="72476-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="72476-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="72476-112">Parent elements</span></span>

|<span data-ttu-id="72476-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="72476-113">**Element**</span></span>|<span data-ttu-id="72476-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="72476-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="72476-115">Элемент</span><span class="sxs-lookup"><span data-stu-id="72476-115">Item</span></span>](item.md) <br/> |<span data-ttu-id="72476-116">Представляет универсальный элемент в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="72476-116">Represents a generic item in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="72476-117">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="72476-117">Text value</span></span>

<span data-ttu-id="72476-118">Текстовое значение **true** для элемента **HasBlockedImages** указывает, что элемент был заблокирован изображений.</span><span class="sxs-lookup"><span data-stu-id="72476-118">A text value of **true** for the **HasBlockedImages** element indicates that the item has blocked images.</span></span> <span data-ttu-id="72476-119">Значение **false** указывает, что элемент не имеет любое заблокированные изображения.</span><span class="sxs-lookup"><span data-stu-id="72476-119">A value of **false** indicates that the item does not have any blocked images.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="72476-120">Замечания</span><span class="sxs-lookup"><span data-stu-id="72476-120">Remarks</span></span>

<span data-ttu-id="72476-121">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="72476-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="72476-122">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="72476-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="72476-123">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="72476-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="72476-124">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="72476-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="72476-125">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="72476-125">Schema Name</span></span>  <br/> |<span data-ttu-id="72476-126">Схема типа</span><span class="sxs-lookup"><span data-stu-id="72476-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="72476-127">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="72476-127">Validation File</span></span>  <br/> |<span data-ttu-id="72476-128">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="72476-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="72476-129">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="72476-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="72476-130">См. также</span><span class="sxs-lookup"><span data-stu-id="72476-130">See also</span></span>



- [<span data-ttu-id="72476-131">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="72476-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

