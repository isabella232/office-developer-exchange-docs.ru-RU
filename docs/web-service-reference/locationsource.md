---
title: LocationSource
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: fc4d77d5-6200-4cf3-848a-1088fec0e0d6
description: Элемент LocationSource определяет информацию о происхождении связанный почтовый адрес, например, контакт или телефонной книги.
ms.openlocfilehash: 7f5cf5fcca0a72287593349fcf5090a74225d012
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19834248"
---
# <a name="locationsource"></a><span data-ttu-id="0b430-103">LocationSource</span><span class="sxs-lookup"><span data-stu-id="0b430-103">LocationSource</span></span>

<span data-ttu-id="0b430-104">Элемент **LocationSource** определяет информацию о происхождении связанный почтовый адрес, например, контакт или телефонной книги.</span><span class="sxs-lookup"><span data-stu-id="0b430-104">The **LocationSource** element specifies information about the origin of the associated postal address, for example, a contact or a telephone book.</span></span> 
  
```XML
<LocationSource> None | LocationServices | PhonebookServices | Device | Contact | Resource </LocationSource>
```

 <span data-ttu-id="0b430-105">**LocationSourceType**</span><span class="sxs-lookup"><span data-stu-id="0b430-105">**LocationSourceType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0b430-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="0b430-106">Attributes and elements</span></span>

<span data-ttu-id="0b430-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="0b430-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0b430-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="0b430-108">Attributes</span></span>

<span data-ttu-id="0b430-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="0b430-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0b430-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="0b430-110">Child elements</span></span>

<span data-ttu-id="0b430-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="0b430-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="0b430-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="0b430-112">Parent elements</span></span>

<span data-ttu-id="0b430-113">[Значение (PersonaPostalAddressType)](value-personapostaladdresstype.md) | [PostalAddress (PersonaPostalAddressType)](postaladdress-personapostaladdresstype.md)</span><span class="sxs-lookup"><span data-stu-id="0b430-113">[Value (PersonaPostalAddressType)](value-personapostaladdresstype.md) | [PostalAddress (PersonaPostalAddressType)](postaladdress-personapostaladdresstype.md)</span></span>
  
## <a name="text-value"></a><span data-ttu-id="0b430-114">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="0b430-114">Text value</span></span>

<span data-ttu-id="0b430-115">Текстовые значения для элемента **LocationSource** перечислены в следующей таблице:</span><span class="sxs-lookup"><span data-stu-id="0b430-115">The text values for the **LocationSource** element are listed in the following table:</span></span> 
  
<span data-ttu-id="0b430-116">**LocationSource элемент текстовые значения**</span><span class="sxs-lookup"><span data-stu-id="0b430-116">**LocationSource element text values**</span></span>

|<span data-ttu-id="0b430-117">**Значение**</span><span class="sxs-lookup"><span data-stu-id="0b430-117">**Value**</span></span>|<span data-ttu-id="0b430-118">**Описание**</span><span class="sxs-lookup"><span data-stu-id="0b430-118">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="0b430-119">Нет</span><span class="sxs-lookup"><span data-stu-id="0b430-119">None</span></span>  <br/> |<span data-ttu-id="0b430-120">Не указан источник расположения.</span><span class="sxs-lookup"><span data-stu-id="0b430-120">There is no location source.</span></span>  <br/> |
|<span data-ttu-id="0b430-121">LocationServices</span><span class="sxs-lookup"><span data-stu-id="0b430-121">LocationServices</span></span>  <br/> |<span data-ttu-id="0b430-122">Сведения о был получен из расположения служб.</span><span class="sxs-lookup"><span data-stu-id="0b430-122">The information was obtained from location services.</span></span>  <br/> |
|<span data-ttu-id="0b430-123">PhonebookServices</span><span class="sxs-lookup"><span data-stu-id="0b430-123">PhonebookServices</span></span>  <br/> |<span data-ttu-id="0b430-124">Сведения о был получен из службы телефонной книги.</span><span class="sxs-lookup"><span data-stu-id="0b430-124">The information was obtained from phonebook services.</span></span>  <br/> |
|<span data-ttu-id="0b430-125">Устройство</span><span class="sxs-lookup"><span data-stu-id="0b430-125">Device</span></span>  <br/> |<span data-ttu-id="0b430-126">Сведения о был получен из устройства.</span><span class="sxs-lookup"><span data-stu-id="0b430-126">The information was obtained from the device.</span></span>  <br/> |
|<span data-ttu-id="0b430-127">Контакт</span><span class="sxs-lookup"><span data-stu-id="0b430-127">Contact</span></span>  <br/> |<span data-ttu-id="0b430-128">Сведения о был получен контакт.</span><span class="sxs-lookup"><span data-stu-id="0b430-128">The information was obtained from a contact.</span></span>  <br/> |
|<span data-ttu-id="0b430-129">Resource</span><span class="sxs-lookup"><span data-stu-id="0b430-129">Resource</span></span>  <br/> |<span data-ttu-id="0b430-130">Сведения о был получен из ресурса.</span><span class="sxs-lookup"><span data-stu-id="0b430-130">The information was obtained from a resource.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="0b430-131">Замечания</span><span class="sxs-lookup"><span data-stu-id="0b430-131">Remarks</span></span>

<span data-ttu-id="0b430-132">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="0b430-132">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="0b430-133">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="0b430-133">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  

