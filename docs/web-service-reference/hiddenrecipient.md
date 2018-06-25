---
title: HiddenRecipient
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- HiddenRecipient
api_type:
- schema
ms.assetid: a8209f75-0070-4424-8dcd-273cfd192728
description: Элемент HiddenRecipient указывает, что получатель был добавлен политикой организации, должны быть скрыты от непривилегированным пользователям.
ms.openlocfilehash: 73b2e3e39c675cf3e2bc56105b1e76009d4a2451
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833810"
---
# <a name="hiddenrecipient"></a><span data-ttu-id="09693-103">HiddenRecipient</span><span class="sxs-lookup"><span data-stu-id="09693-103">HiddenRecipient</span></span>

<span data-ttu-id="09693-104">Элемент **HiddenRecipient** указывает, что получатель был добавлен политикой организации, должны быть скрыты от непривилегированным пользователям.</span><span class="sxs-lookup"><span data-stu-id="09693-104">The **HiddenRecipient** element indicates that the recipient was added by an organization policy that should be hidden from unprivileged users.</span></span> 
  
```XML
<HiddenRecipient>true | false</HiddenRecipient>
```

 <span data-ttu-id="09693-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="09693-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="09693-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="09693-106">Attributes and elements</span></span>

<span data-ttu-id="09693-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="09693-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="09693-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="09693-108">Attributes</span></span>

<span data-ttu-id="09693-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="09693-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="09693-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="09693-110">Child elements</span></span>

<span data-ttu-id="09693-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="09693-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="09693-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="09693-112">Parent elements</span></span>

|<span data-ttu-id="09693-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="09693-113">**Element**</span></span>|<span data-ttu-id="09693-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="09693-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="09693-115">RecipientTrackingEvent</span><span class="sxs-lookup"><span data-stu-id="09693-115">RecipientTrackingEvent</span></span>](recipienttrackingevent.md) <br/> |<span data-ttu-id="09693-116">Содержит сведения для одного события для получателя.</span><span class="sxs-lookup"><span data-stu-id="09693-116">Contains information for a single event for a recipient.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="09693-117">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="09693-117">Text value</span></span>

<span data-ttu-id="09693-118">Этот элемент может быть значение **true** или **false**.</span><span class="sxs-lookup"><span data-stu-id="09693-118">This element can be either **true** or **false**.</span></span> <span data-ttu-id="09693-119">Значение **true** указывает, что пользователь был добавлен политикой организации; значение **false** указывает, что пользователь не был добавлен политикой организации.</span><span class="sxs-lookup"><span data-stu-id="09693-119">A value of **true** indicates that the user was added by an organization policy; a value of **false** indicates that the user was not added by an organization policy.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="09693-120">Замечания</span><span class="sxs-lookup"><span data-stu-id="09693-120">Remarks</span></span>

<span data-ttu-id="09693-121">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="09693-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="09693-122">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="09693-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="09693-123">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="09693-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="09693-124">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="09693-124">Schema Name</span></span>  <br/> |<span data-ttu-id="09693-125">Схема Types</span><span class="sxs-lookup"><span data-stu-id="09693-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="09693-126">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="09693-126">Validation File</span></span>  <br/> |<span data-ttu-id="09693-127">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="09693-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="09693-128">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="09693-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="09693-129">False</span><span class="sxs-lookup"><span data-stu-id="09693-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="09693-130">См. также</span><span class="sxs-lookup"><span data-stu-id="09693-130">See also</span></span>



- [<span data-ttu-id="09693-131">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="09693-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

