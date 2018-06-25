---
title: AssistantPhoneNumbers
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f9bd9ac1-7db3-44ea-9117-18488dddde15
description: Элемент AssistantPhoneNumbers указывает массив помощник по номера телефонов и идентификаторы их атрибуты источника для связанного пользователя.
ms.openlocfilehash: 747835102af28d94d60b763fdbc5b2ea0947d47e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761505"
---
# <a name="assistantphonenumbers"></a><span data-ttu-id="362a9-103">AssistantPhoneNumbers</span><span class="sxs-lookup"><span data-stu-id="362a9-103">AssistantPhoneNumbers</span></span>

<span data-ttu-id="362a9-104">Элемент **AssistantPhoneNumbers** указывает массив помощник по номера телефонов и идентификаторы их атрибуты источника для связанного пользователя.</span><span class="sxs-lookup"><span data-stu-id="362a9-104">The **AssistantPhoneNumbers** element specifies an array of assistant phone numbers and the identifiers of their source attributions for the associated persona.</span></span> 
  
```XML
<AssistantPhoneNumbers>
    <PhoneNumberAttributedValue></PhoneNumberAttributedValue>
</AssistantPhoneNumbers>
```

 <span data-ttu-id="362a9-105">**ArrayOfPhoneNumberAttributedValuesType**</span><span class="sxs-lookup"><span data-stu-id="362a9-105">**ArrayOfPhoneNumberAttributedValuesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="362a9-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="362a9-106">Attributes and elements</span></span>

<span data-ttu-id="362a9-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="362a9-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="362a9-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="362a9-108">Attributes</span></span>

<span data-ttu-id="362a9-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="362a9-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="362a9-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="362a9-110">Child elements</span></span>

|<span data-ttu-id="362a9-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="362a9-111">**Element**</span></span>|<span data-ttu-id="362a9-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="362a9-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="362a9-113">PhoneNumberAttributedValue</span><span class="sxs-lookup"><span data-stu-id="362a9-113">PhoneNumberAttributedValue</span></span>](phonenumberattributedvalue.md) <br/> |<span data-ttu-id="362a9-114">Указывает экземпляр массив номеров телефонов и их связанные атрибуты.</span><span class="sxs-lookup"><span data-stu-id="362a9-114">Specifies an instance of an array of phone numbers and their associated attributions.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="362a9-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="362a9-115">Parent elements</span></span>

|<span data-ttu-id="362a9-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="362a9-116">**Element**</span></span>|<span data-ttu-id="362a9-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="362a9-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="362a9-118">Пользователь</span><span class="sxs-lookup"><span data-stu-id="362a9-118">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="362a9-119">Задает набор пользователя данные, возвращаемые запросом **GetPersona** .</span><span class="sxs-lookup"><span data-stu-id="362a9-119">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="362a9-120">Замечания</span><span class="sxs-lookup"><span data-stu-id="362a9-120">Remarks</span></span>

<span data-ttu-id="362a9-121">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="362a9-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="362a9-122">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="362a9-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="362a9-123">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="362a9-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="362a9-124">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="362a9-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="362a9-125">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="362a9-125">Schema Name</span></span>  <br/> |<span data-ttu-id="362a9-126">Схема типа</span><span class="sxs-lookup"><span data-stu-id="362a9-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="362a9-127">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="362a9-127">Validation File</span></span>  <br/> |<span data-ttu-id="362a9-128">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="362a9-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="362a9-129">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="362a9-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="362a9-130">См. также</span><span class="sxs-lookup"><span data-stu-id="362a9-130">See also</span></span>

- [<span data-ttu-id="362a9-131">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="362a9-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

