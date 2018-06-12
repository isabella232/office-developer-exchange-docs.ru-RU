---
title: IsQuickContact
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 1c9542d6-ef72-4743-828a-bb671e783836
description: Элемент IsQuickContact задает логическое значение, указывающее, является ли базовый контакт быстрого контакта.
ms.openlocfilehash: 979dbd3c0358eacd443eed79b258f7dd6bb9bc7d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19834092"
---
# <a name="isquickcontact"></a><span data-ttu-id="86480-103">IsQuickContact</span><span class="sxs-lookup"><span data-stu-id="86480-103">IsQuickContact</span></span>

<span data-ttu-id="86480-104">Элемент **IsQuickContact** задает логическое значение, указывающее, является ли базовый контакт быстрого контакта.</span><span class="sxs-lookup"><span data-stu-id="86480-104">The **IsQuickContact** element specifies a Boolean value that indicates whether the underlying contact is a quick contact.</span></span> 
  
```XML
<IsQuickContact>true | false</IsQuickContact>
```

 <span data-ttu-id="86480-105">**boolean**</span><span class="sxs-lookup"><span data-stu-id="86480-105">**boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="86480-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="86480-106">Attributes and elements</span></span>

<span data-ttu-id="86480-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="86480-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="86480-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="86480-108">Attributes</span></span>

<span data-ttu-id="86480-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="86480-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="86480-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="86480-110">Child elements</span></span>

<span data-ttu-id="86480-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="86480-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="86480-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="86480-112">Parent elements</span></span>

|<span data-ttu-id="86480-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="86480-113">**Element**</span></span>|<span data-ttu-id="86480-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="86480-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="86480-115">Атрибуты (PersonaAttributionType)</span><span class="sxs-lookup"><span data-stu-id="86480-115">Attribution (PersonaAttributionType)</span></span>](attribution-personaattributiontype.md) <br/> |<span data-ttu-id="86480-116">Задает экземпляр в массиве атрибутов элемента **пользователя** .</span><span class="sxs-lookup"><span data-stu-id="86480-116">Specifies an instance in an array of attributes for a **Persona** element.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="86480-117">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="86480-117">Text value</span></span>

<span data-ttu-id="86480-118">Текстовое значение **true** для элемента **IsQuickContact** указывает, что контакт является быстрого.</span><span class="sxs-lookup"><span data-stu-id="86480-118">A text value of **true** for the **IsQuickContact** element indicates that the contact is a quick contact.</span></span> <span data-ttu-id="86480-119">Значение **false** указывает, что контакта нет быстрого контакта.</span><span class="sxs-lookup"><span data-stu-id="86480-119">A value of **false** indicates that the contact is not a quick contact.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="86480-120">Замечания</span><span class="sxs-lookup"><span data-stu-id="86480-120">Remarks</span></span>

<span data-ttu-id="86480-121">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="86480-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="86480-122">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="86480-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="86480-123">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="86480-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="86480-124">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="86480-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="86480-125">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="86480-125">Schema Name</span></span>  <br/> |<span data-ttu-id="86480-126">Схема типа</span><span class="sxs-lookup"><span data-stu-id="86480-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="86480-127">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="86480-127">Validation File</span></span>  <br/> |<span data-ttu-id="86480-128">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="86480-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="86480-129">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="86480-129">Can Be Empty</span></span>  <br/> |<span data-ttu-id="86480-130">Нет</span><span class="sxs-lookup"><span data-stu-id="86480-130">false</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="86480-131">См. также</span><span class="sxs-lookup"><span data-stu-id="86480-131">See also</span></span>



- [<span data-ttu-id="86480-132">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="86480-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

