---
title: HomePhones2
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: ba9bb159-362d-48e0-889d-823cb46ecebf
description: Элемент HomePhones2 указывает массив значений HomePhone2 и идентификаторы их атрибуты источника для связанного пользователя.
ms.openlocfilehash: 205f2f71421a0dfc7d0057412529bcefdb6636d5
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833842"
---
# <a name="homephones2"></a><span data-ttu-id="9d5e4-103">HomePhones2</span><span class="sxs-lookup"><span data-stu-id="9d5e4-103">HomePhones2</span></span>

<span data-ttu-id="9d5e4-104">Элемент **HomePhones2** указывает массив значений **HomePhone2** и идентификаторы их атрибуты источника для связанного пользователя.</span><span class="sxs-lookup"><span data-stu-id="9d5e4-104">The **HomePhones2** element specifies an array of **HomePhone2** values and the identifiers of their source attributions for the associated persona.</span></span> 
  
```XML
<HomePhones2>
    <PhoneNumberAttributedValue/>
</HomePhones2>
```

 <span data-ttu-id="9d5e4-105">**ArrayOfPhoneNumberAttributedValuesType**</span><span class="sxs-lookup"><span data-stu-id="9d5e4-105">**ArrayOfPhoneNumberAttributedValuesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9d5e4-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="9d5e4-106">Attributes and elements</span></span>

<span data-ttu-id="9d5e4-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="9d5e4-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9d5e4-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="9d5e4-108">Attributes</span></span>

<span data-ttu-id="9d5e4-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="9d5e4-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9d5e4-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="9d5e4-110">Child elements</span></span>

|<span data-ttu-id="9d5e4-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="9d5e4-111">**Element**</span></span>|<span data-ttu-id="9d5e4-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="9d5e4-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9d5e4-113">PhoneNumberAttributedValue</span><span class="sxs-lookup"><span data-stu-id="9d5e4-113">PhoneNumberAttributedValue</span></span>](phonenumberattributedvalue.md) <br/> |<span data-ttu-id="9d5e4-114">Содержит один атрибутами номер телефона для пользователя.</span><span class="sxs-lookup"><span data-stu-id="9d5e4-114">Contains a single attributed phone number for a persona.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="9d5e4-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="9d5e4-115">Parent elements</span></span>

|<span data-ttu-id="9d5e4-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="9d5e4-116">**Element**</span></span>|<span data-ttu-id="9d5e4-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="9d5e4-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9d5e4-118">Пользователь</span><span class="sxs-lookup"><span data-stu-id="9d5e4-118">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="9d5e4-119">Задает набор пользователя данные, возвращаемые запросом **GetPersona** .</span><span class="sxs-lookup"><span data-stu-id="9d5e4-119">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="9d5e4-120">Замечания</span><span class="sxs-lookup"><span data-stu-id="9d5e4-120">Remarks</span></span>

<span data-ttu-id="9d5e4-121">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="9d5e4-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="9d5e4-122">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="9d5e4-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9d5e4-123">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="9d5e4-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9d5e4-124">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="9d5e4-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="9d5e4-125">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="9d5e4-125">Schema Name</span></span>  <br/> |<span data-ttu-id="9d5e4-126">Схема типа</span><span class="sxs-lookup"><span data-stu-id="9d5e4-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="9d5e4-127">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="9d5e4-127">Validation File</span></span>  <br/> |<span data-ttu-id="9d5e4-128">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="9d5e4-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="9d5e4-129">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="9d5e4-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="9d5e4-130">См. также</span><span class="sxs-lookup"><span data-stu-id="9d5e4-130">See also</span></span>



- [<span data-ttu-id="9d5e4-131">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="9d5e4-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

