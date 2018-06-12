---
title: ContactSource
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ContactSource
api_type:
- schema
ms.assetid: 500b0423-864e-4cde-a39b-6b5b06d1aa6a
description: Элемент ContactSource описание, находится ли контакт в хранилище Exchange или доменных служб Active Directory (AD DS).
ms.openlocfilehash: a82b766fc81b9397fc707415ea82e2f2d63d952d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761741"
---
# <a name="contactsource"></a><span data-ttu-id="284bd-103">ContactSource</span><span class="sxs-lookup"><span data-stu-id="284bd-103">ContactSource</span></span>

<span data-ttu-id="284bd-104">Элемент **ContactSource** описание, находится ли контакт в хранилище Exchange или доменных служб Active Directory (AD DS).</span><span class="sxs-lookup"><span data-stu-id="284bd-104">The **ContactSource** element describes whether the contact is located in the Exchange store or Active Directory Domain Services (AD DS).</span></span> 
  
```xml
<ContactSource/>
```

 <span data-ttu-id="284bd-105">**ContactSourceType**</span><span class="sxs-lookup"><span data-stu-id="284bd-105">**ContactSourceType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="284bd-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="284bd-106">Attributes and elements</span></span>

<span data-ttu-id="284bd-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="284bd-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="284bd-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="284bd-108">Attributes</span></span>

<span data-ttu-id="284bd-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="284bd-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="284bd-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="284bd-110">Child elements</span></span>

<span data-ttu-id="284bd-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="284bd-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="284bd-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="284bd-112">Parent elements</span></span>

|<span data-ttu-id="284bd-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="284bd-113">**Element**</span></span>|<span data-ttu-id="284bd-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="284bd-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="284bd-115">Контакт</span><span class="sxs-lookup"><span data-stu-id="284bd-115">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="284bd-116">Представляет контакт в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="284bd-116">Represents a contact item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="284bd-117">DistributionList</span><span class="sxs-lookup"><span data-stu-id="284bd-117">DistributionList</span></span>](distributionlist.md) <br/> |<span data-ttu-id="284bd-118">Представляет список рассылки.</span><span class="sxs-lookup"><span data-stu-id="284bd-118">Represents a distribution list.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="284bd-119">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="284bd-119">Text value</span></span>

<span data-ttu-id="284bd-120">Ниже приведены возможные значения для этого элемента:</span><span class="sxs-lookup"><span data-stu-id="284bd-120">The following are the possible values for this element:</span></span>
  
- <span data-ttu-id="284bd-121">ActiveDirectory</span><span class="sxs-lookup"><span data-stu-id="284bd-121">ActiveDirectory</span></span>
    
- <span data-ttu-id="284bd-122">Магазин</span><span class="sxs-lookup"><span data-stu-id="284bd-122">Store</span></span>
    
## <a name="remarks"></a><span data-ttu-id="284bd-123">Замечания</span><span class="sxs-lookup"><span data-stu-id="284bd-123">Remarks</span></span>

<span data-ttu-id="284bd-124">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="284bd-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="284bd-125">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="284bd-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="284bd-126">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="284bd-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="284bd-127">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="284bd-127">Schema name</span></span>  <br/> |<span data-ttu-id="284bd-128">Схема Types</span><span class="sxs-lookup"><span data-stu-id="284bd-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="284bd-129">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="284bd-129">Validation file</span></span>  <br/> |<span data-ttu-id="284bd-130">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="284bd-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="284bd-131">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="284bd-131">Can be empty</span></span>  <br/> |<span data-ttu-id="284bd-132">False</span><span class="sxs-lookup"><span data-stu-id="284bd-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="284bd-133">См. также</span><span class="sxs-lookup"><span data-stu-id="284bd-133">See also</span></span>



- [<span data-ttu-id="284bd-134">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="284bd-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
