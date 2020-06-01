---
title: локатионсаурце
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: fc4d77d5-6200-4cf3-848a-1088fec0e0d6
description: Элемент Локатионсаурце указывает сведения о происхождении связанного почтового адреса, например контакт или телефонной книги.
ms.openlocfilehash: ceba52c43d1c798bb8f5492b779c7c45d7d00b0b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44467104"
---
# <a name="locationsource"></a><span data-ttu-id="d8153-103">локатионсаурце</span><span class="sxs-lookup"><span data-stu-id="d8153-103">LocationSource</span></span>

<span data-ttu-id="d8153-104">Элемент **локатионсаурце** указывает сведения о происхождении связанного почтового адреса, например контакт или телефонной книги.</span><span class="sxs-lookup"><span data-stu-id="d8153-104">The **LocationSource** element specifies information about the origin of the associated postal address, for example, a contact or a telephone book.</span></span> 
  
```XML
<LocationSource> None | LocationServices | PhonebookServices | Device | Contact | Resource </LocationSource>
```

 <span data-ttu-id="d8153-105">**локатионсаурцетипе**</span><span class="sxs-lookup"><span data-stu-id="d8153-105">**LocationSourceType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d8153-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="d8153-106">Attributes and elements</span></span>

<span data-ttu-id="d8153-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="d8153-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d8153-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="d8153-108">Attributes</span></span>

<span data-ttu-id="d8153-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="d8153-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d8153-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="d8153-110">Child elements</span></span>

<span data-ttu-id="d8153-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="d8153-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="d8153-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="d8153-112">Parent elements</span></span>

<span data-ttu-id="d8153-113">[Значение (персонапосталаддресстипе)](value-personapostaladdresstype.md)  |  [Посталаддресс (персонапосталаддресстипе)](postaladdress-personapostaladdresstype.md)</span><span class="sxs-lookup"><span data-stu-id="d8153-113">[Value (PersonaPostalAddressType)](value-personapostaladdresstype.md) | [PostalAddress (PersonaPostalAddressType)](postaladdress-personapostaladdresstype.md)</span></span>
  
## <a name="text-value"></a><span data-ttu-id="d8153-114">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="d8153-114">Text value</span></span>

<span data-ttu-id="d8153-115">Текстовые значения для элемента **локатионсаурце** перечислены в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="d8153-115">The text values for the **LocationSource** element are listed in the following table:</span></span> 
  
<span data-ttu-id="d8153-116">**Текстовые значения элементов Локатионсаурце**</span><span class="sxs-lookup"><span data-stu-id="d8153-116">**LocationSource element text values**</span></span>

|<span data-ttu-id="d8153-117">**Значение**</span><span class="sxs-lookup"><span data-stu-id="d8153-117">**Value**</span></span>|<span data-ttu-id="d8153-118">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d8153-118">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="d8153-119">Нет</span><span class="sxs-lookup"><span data-stu-id="d8153-119">None</span></span>  <br/> |<span data-ttu-id="d8153-120">Источник расположения отсутствует.</span><span class="sxs-lookup"><span data-stu-id="d8153-120">There is no location source.</span></span>  <br/> |
|<span data-ttu-id="d8153-121">локатионсервицес</span><span class="sxs-lookup"><span data-stu-id="d8153-121">LocationServices</span></span>  <br/> |<span data-ttu-id="d8153-122">Сведения получены из служб расположения.</span><span class="sxs-lookup"><span data-stu-id="d8153-122">The information was obtained from location services.</span></span>  <br/> |
|<span data-ttu-id="d8153-123">фонебуксервицес</span><span class="sxs-lookup"><span data-stu-id="d8153-123">PhonebookServices</span></span>  <br/> |<span data-ttu-id="d8153-124">Сведения получены из службы телефонной книги.</span><span class="sxs-lookup"><span data-stu-id="d8153-124">The information was obtained from phonebook services.</span></span>  <br/> |
|<span data-ttu-id="d8153-125">Device</span><span class="sxs-lookup"><span data-stu-id="d8153-125">Device</span></span>  <br/> |<span data-ttu-id="d8153-126">Сведения получены с устройства.</span><span class="sxs-lookup"><span data-stu-id="d8153-126">The information was obtained from the device.</span></span>  <br/> |
|<span data-ttu-id="d8153-127">Контакт</span><span class="sxs-lookup"><span data-stu-id="d8153-127">Contact</span></span>  <br/> |<span data-ttu-id="d8153-128">Сведения получены из контакта.</span><span class="sxs-lookup"><span data-stu-id="d8153-128">The information was obtained from a contact.</span></span>  <br/> |
|<span data-ttu-id="d8153-129">Resource</span><span class="sxs-lookup"><span data-stu-id="d8153-129">Resource</span></span>  <br/> |<span data-ttu-id="d8153-130">Сведения получены из ресурса.</span><span class="sxs-lookup"><span data-stu-id="d8153-130">The information was obtained from a resource.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="d8153-131">Примечания</span><span class="sxs-lookup"><span data-stu-id="d8153-131">Remarks</span></span>

<span data-ttu-id="d8153-132">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="d8153-132">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="d8153-133">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="d8153-133">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  

