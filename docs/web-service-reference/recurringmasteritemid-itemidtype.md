---
title: RecurringMasterItemId (ItemIdType)
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 48d831cf-10d8-480b-86d2-f9c0b14b8167
description: Элемент RecurringMasterItemId (ItemIdType) идентифицирует элемент шаблона повторения с учетом идентификаторы одного из его элементы, связанных с ними вхождение.
ms.openlocfilehash: 89089067963e99ac1a6cae6ea6e1e8350d148e82
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19835010"
---
# <a name="recurringmasteritemid-itemidtype"></a><span data-ttu-id="af68a-103">RecurringMasterItemId (ItemIdType)</span><span class="sxs-lookup"><span data-stu-id="af68a-103">RecurringMasterItemId (ItemIdType)</span></span>

<span data-ttu-id="af68a-104">Элемент **RecurringMasterItemId (ItemIdType)** идентифицирует элемент шаблона повторения с учетом идентификаторы одного из его элементы, связанных с ними вхождение.</span><span class="sxs-lookup"><span data-stu-id="af68a-104">The **RecurringMasterItemId (ItemIdType)** element identifies a recurrence master item by identifying the identifiers of one of its related occurrence items.</span></span> 
  
```XML
<RecurringMasterItemId Id="" ChangeKey=""/>
```

 <span data-ttu-id="af68a-105">**ItemIdType**</span><span class="sxs-lookup"><span data-stu-id="af68a-105">**ItemIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="af68a-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="af68a-106">Attributes and elements</span></span>

<span data-ttu-id="af68a-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="af68a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="af68a-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="af68a-108">Attributes</span></span>

****

|<span data-ttu-id="af68a-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="af68a-109">**Attribute**</span></span>|<span data-ttu-id="af68a-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="af68a-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="af68a-111">Id</span><span class="sxs-lookup"><span data-stu-id="af68a-111">Id</span></span>  <br/> |<span data-ttu-id="af68a-112">Определяет одно вхождение повторяющегося элемента шаблона.</span><span class="sxs-lookup"><span data-stu-id="af68a-112">Identifies a single occurrence of a recurring master item.</span></span> <span data-ttu-id="af68a-113">Этот атрибут является обязательным.</span><span class="sxs-lookup"><span data-stu-id="af68a-113">This attribute is required.</span></span>  <br/> |
|<span data-ttu-id="af68a-114">ChangeKey</span><span class="sxs-lookup"><span data-stu-id="af68a-114">ChangeKey</span></span>  <br/> |<span data-ttu-id="af68a-115">Идентифицирует определенной версии одного экземпляра повторяющегося элемента шаблона.</span><span class="sxs-lookup"><span data-stu-id="af68a-115">Identifies a specific version of a single occurrence of a recurring master item.</span></span> <span data-ttu-id="af68a-116">Кроме того повторяющегося элемента шаблона также определены, так как он и одно вхождение будет содержать тем же ключом изменений.</span><span class="sxs-lookup"><span data-stu-id="af68a-116">Additionally, the recurring master item is also identified because it and the single occurrence will contain the same change key.</span></span> <span data-ttu-id="af68a-117">Этот атрибут является необязательным.</span><span class="sxs-lookup"><span data-stu-id="af68a-117">This attribute is optional.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="af68a-118">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="af68a-118">Child elements</span></span>

<span data-ttu-id="af68a-119">Нет.</span><span class="sxs-lookup"><span data-stu-id="af68a-119">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="af68a-120">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="af68a-120">Parent elements</span></span>

[<span data-ttu-id="af68a-121">Памятки</span><span class="sxs-lookup"><span data-stu-id="af68a-121">Reminder</span></span>](reminder.md)
  
## <a name="remarks"></a><span data-ttu-id="af68a-122">Замечания</span><span class="sxs-lookup"><span data-stu-id="af68a-122">Remarks</span></span>

<span data-ttu-id="af68a-123">Этот элемент появился в Exchange Server 2013 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="af68a-123">This element was introduced in Exchange Server 2013 Service Pack 1 (SP1).</span></span>
  
<span data-ttu-id="af68a-124">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="af68a-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="af68a-125">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="af68a-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="af68a-126">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="af68a-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="af68a-127">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="af68a-127">Schema Name</span></span>  <br/> |<span data-ttu-id="af68a-128">Схема Types</span><span class="sxs-lookup"><span data-stu-id="af68a-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="af68a-129">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="af68a-129">Validation File</span></span>  <br/> |<span data-ttu-id="af68a-130">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="af68a-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="af68a-131">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="af68a-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="af68a-132">True</span><span class="sxs-lookup"><span data-stu-id="af68a-132">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="af68a-133">См. также</span><span class="sxs-lookup"><span data-stu-id="af68a-133">See also</span></span>



[<span data-ttu-id="af68a-134">Памятки</span><span class="sxs-lookup"><span data-stu-id="af68a-134">Reminder</span></span>](reminder.md)


- [<span data-ttu-id="af68a-135">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="af68a-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

