---
title: PostedTime
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- PostedTime
api_type:
- schema
ms.assetid: e8b3813c-fc7e-4674-a4c6-6818c13d2bcf
description: Элемент PostedTime представляет время учета PostItem. Этот элемент доступен только для чтения. Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).
ms.openlocfilehash: 8280fc26c534b280d0f30f663b6cc3a3958036c5
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19834860"
---
# <a name="postedtime"></a><span data-ttu-id="20fea-105">PostedTime</span><span class="sxs-lookup"><span data-stu-id="20fea-105">PostedTime</span></span>

<span data-ttu-id="20fea-106">Элемент **PostedTime** представляет время учета [PostItem](postitem.md) .</span><span class="sxs-lookup"><span data-stu-id="20fea-106">The **PostedTime** element represents the time at which a [PostItem](postitem.md) was posted.</span></span> <span data-ttu-id="20fea-107">Этот элемент доступен только для чтения.</span><span class="sxs-lookup"><span data-stu-id="20fea-107">This element is read-only.</span></span> <span data-ttu-id="20fea-108">Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="20fea-108">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<PostedTime/>
```

 <span data-ttu-id="20fea-109">**dateTime**</span><span class="sxs-lookup"><span data-stu-id="20fea-109">**dateTime**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="20fea-110">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="20fea-110">Attributes and elements</span></span>

<span data-ttu-id="20fea-111">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="20fea-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="20fea-112">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="20fea-112">Attributes</span></span>

<span data-ttu-id="20fea-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="20fea-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="20fea-114">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="20fea-114">Child elements</span></span>

<span data-ttu-id="20fea-115">Нет.</span><span class="sxs-lookup"><span data-stu-id="20fea-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="20fea-116">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="20fea-116">Parent elements</span></span>

|<span data-ttu-id="20fea-117">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="20fea-117">**Element**</span></span>|<span data-ttu-id="20fea-118">**Описание**</span><span class="sxs-lookup"><span data-stu-id="20fea-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="20fea-119">PostItem</span><span class="sxs-lookup"><span data-stu-id="20fea-119">PostItem</span></span>](postitem.md) <br/> |<span data-ttu-id="20fea-120">Представляет PostItem в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="20fea-120">Represents a PostItem in the Exchange store.</span></span> <span data-ttu-id="20fea-121">Этот элемент появился в Exchange 2007 с пакетом обновления 1.</span><span class="sxs-lookup"><span data-stu-id="20fea-121">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="20fea-122">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="20fea-122">Text value</span></span>

<span data-ttu-id="20fea-123">Текстовое значение dateTime, который представляет при учете **PostItem** .</span><span class="sxs-lookup"><span data-stu-id="20fea-123">The text value is a dateTime that represents when a **PostItem** was posted.</span></span> <span data-ttu-id="20fea-124">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="20fea-124">This property is read-only.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="20fea-125">Замечания</span><span class="sxs-lookup"><span data-stu-id="20fea-125">Remarks</span></span>

<span data-ttu-id="20fea-126">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="20fea-126">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="20fea-127">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="20fea-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="20fea-128">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="20fea-128">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="20fea-129">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="20fea-129">Schema Name</span></span>  <br/> |<span data-ttu-id="20fea-130">Схема Types</span><span class="sxs-lookup"><span data-stu-id="20fea-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="20fea-131">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="20fea-131">Validation File</span></span>  <br/> |<span data-ttu-id="20fea-132">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="20fea-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="20fea-133">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="20fea-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="20fea-134">False</span><span class="sxs-lookup"><span data-stu-id="20fea-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="20fea-135">См. также</span><span class="sxs-lookup"><span data-stu-id="20fea-135">See also</span></span>



- [<span data-ttu-id="20fea-136">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="20fea-136">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

