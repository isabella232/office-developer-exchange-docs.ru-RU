---
title: CarPhones
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: ad096246-113c-42ea-9e63-861b546003e8
description: Элемент Автомобильный телефон указывает массив car номера телефонов и идентификаторы их атрибуты источника для связанного пользователя.
ms.openlocfilehash: 694b3578e127a84dfd2fb844c6e81b28553b687c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761668"
---
# <a name="carphones"></a><span data-ttu-id="e944d-103">CarPhones</span><span class="sxs-lookup"><span data-stu-id="e944d-103">CarPhones</span></span>

<span data-ttu-id="e944d-104">Элемент **Автомобильный телефон** указывает массив car номера телефонов и идентификаторы их атрибуты источника для связанного пользователя.</span><span class="sxs-lookup"><span data-stu-id="e944d-104">The **CarPhone** element specifies an array of car phone numbers and the identifiers of their source attributions for the associated persona.</span></span> 
  
```XML
<CarPhones>
    <Value></Value>
    <Attributions></Attributions>
</CarPhones>
```

 <span data-ttu-id="e944d-105">**ArrayOfPhoneNumberAttributedValuesType**</span><span class="sxs-lookup"><span data-stu-id="e944d-105">**ArrayOfPhoneNumberAttributedValuesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e944d-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="e944d-106">Attributes and elements</span></span>

<span data-ttu-id="e944d-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="e944d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e944d-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="e944d-108">Attributes</span></span>

<span data-ttu-id="e944d-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="e944d-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e944d-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="e944d-110">Child elements</span></span>

|<span data-ttu-id="e944d-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="e944d-111">**Element**</span></span>|<span data-ttu-id="e944d-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="e944d-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e944d-113">Значение (PersonaPhoneNumberType)</span><span class="sxs-lookup"><span data-stu-id="e944d-113">Value (PersonaPhoneNumberType)</span></span>](value-personaphonenumbertype.md) <br/> |<span data-ttu-id="e944d-114">Указывает номер и введите сведения о номерах телефонов и связанный с набором атрибуты.</span><span class="sxs-lookup"><span data-stu-id="e944d-114">Specifies a phone number and type information and is associated with a set of attributions.</span></span>  <br/> |
|[<span data-ttu-id="e944d-115">Атрибуты (ArrayOfValueAttributionsType)</span><span class="sxs-lookup"><span data-stu-id="e944d-115">Attributions (ArrayOfValueAttributionsType)</span></span>](attributions-arrayofvalueattributionstype.md) <br/> |<span data-ttu-id="e944d-116">Указывает массив атрибуты для его связанное **значение** элемента.</span><span class="sxs-lookup"><span data-stu-id="e944d-116">Specifies an array of attributions for its associated **Value** element.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="e944d-117">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="e944d-117">Parent elements</span></span>

|<span data-ttu-id="e944d-118">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="e944d-118">**Element**</span></span>|<span data-ttu-id="e944d-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="e944d-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e944d-120">Пользователь</span><span class="sxs-lookup"><span data-stu-id="e944d-120">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="e944d-121">Задает набор пользователя данные, возвращаемые запросом **GetPersona** .</span><span class="sxs-lookup"><span data-stu-id="e944d-121">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="e944d-122">Замечания</span><span class="sxs-lookup"><span data-stu-id="e944d-122">Remarks</span></span>

<span data-ttu-id="e944d-123">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="e944d-123">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="e944d-124">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="e944d-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e944d-125">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="e944d-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e944d-126">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="e944d-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="e944d-127">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="e944d-127">Schema Name</span></span>  <br/> |<span data-ttu-id="e944d-128">Схема типа</span><span class="sxs-lookup"><span data-stu-id="e944d-128">Type schema</span></span>  <br/> |
|<span data-ttu-id="e944d-129">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="e944d-129">Validation File</span></span>  <br/> |<span data-ttu-id="e944d-130">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="e944d-130">types.xsd</span></span>  <br/> |
|<span data-ttu-id="e944d-131">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="e944d-131">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="e944d-132">См. также</span><span class="sxs-lookup"><span data-stu-id="e944d-132">See also</span></span>



- [<span data-ttu-id="e944d-133">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="e944d-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

