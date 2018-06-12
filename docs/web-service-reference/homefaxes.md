---
title: HomeFaxes
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 459ddb1c-8cff-4125-b6fa-dc93c183dee8
description: Элемент HomeFaxes указывает массив номера домашнего факсов и идентификаторы их атрибуты источника для связанного пользователя.
ms.openlocfilehash: dd2cd8bba2c4cc7d08e88787d648e96ea996a251
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833840"
---
# <a name="homefaxes"></a><span data-ttu-id="8389d-103">HomeFaxes</span><span class="sxs-lookup"><span data-stu-id="8389d-103">HomeFaxes</span></span>

<span data-ttu-id="8389d-104">Элемент **HomeFaxes** указывает массив номера домашнего факсов и идентификаторы их атрибуты источника для связанного пользователя.</span><span class="sxs-lookup"><span data-stu-id="8389d-104">The **HomeFaxes** element specifies an array of home fax numbers and the identifiers of their source attributions for the associated persona.</span></span> 
  
```XML
<HomeFaxes>
    <PhoneNumberAttributedValue/>
</HomeFaxes>
```

 <span data-ttu-id="8389d-105">**ArrayOfPhoneNumberAttributedValuesType**</span><span class="sxs-lookup"><span data-stu-id="8389d-105">**ArrayOfPhoneNumberAttributedValuesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="8389d-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="8389d-106">Attributes and elements</span></span>

<span data-ttu-id="8389d-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="8389d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8389d-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="8389d-108">Attributes</span></span>

<span data-ttu-id="8389d-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="8389d-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8389d-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="8389d-110">Child elements</span></span>

|<span data-ttu-id="8389d-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="8389d-111">**Element**</span></span>|<span data-ttu-id="8389d-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="8389d-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8389d-113">PhoneNumberAttributedValue</span><span class="sxs-lookup"><span data-stu-id="8389d-113">PhoneNumberAttributedValue</span></span>](phonenumberattributedvalue.md) <br/> |<span data-ttu-id="8389d-114">Содержит один атрибутами номер телефона для пользователя.</span><span class="sxs-lookup"><span data-stu-id="8389d-114">Contains a single attributed phone number for a persona.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="8389d-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="8389d-115">Parent elements</span></span>

|<span data-ttu-id="8389d-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="8389d-116">**Element**</span></span>|<span data-ttu-id="8389d-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="8389d-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8389d-118">Пользователь</span><span class="sxs-lookup"><span data-stu-id="8389d-118">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="8389d-119">Задает набор пользователя данные, возвращаемые запросом **GetPersona** .</span><span class="sxs-lookup"><span data-stu-id="8389d-119">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="8389d-120">Замечания</span><span class="sxs-lookup"><span data-stu-id="8389d-120">Remarks</span></span>

<span data-ttu-id="8389d-121">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="8389d-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="8389d-122">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="8389d-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="8389d-123">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="8389d-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8389d-124">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="8389d-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="8389d-125">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="8389d-125">Schema Name</span></span>  <br/> |<span data-ttu-id="8389d-126">Схема типа</span><span class="sxs-lookup"><span data-stu-id="8389d-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="8389d-127">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="8389d-127">Validation File</span></span>  <br/> |<span data-ttu-id="8389d-128">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="8389d-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="8389d-129">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="8389d-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="8389d-130">См. также</span><span class="sxs-lookup"><span data-stu-id="8389d-130">See also</span></span>



- [<span data-ttu-id="8389d-131">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="8389d-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

