---
title: хомефонес
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 8ea43d5a-4bcf-497e-a559-6efe94fa604b
description: Элемент Хомефонес указывает массив номеров домашнего телефона и идентификаторы их исходных атрибутов для связанного пользователя.
ms.openlocfilehash: 487d37e6a18bbd480a814de7570b0789f148096e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833844"
---
# <a name="homephones"></a><span data-ttu-id="f701f-103">хомефонес</span><span class="sxs-lookup"><span data-stu-id="f701f-103">HomePhones</span></span>

<span data-ttu-id="f701f-104">Элемент **хомефонес** указывает массив номеров домашнего телефона и идентификаторы их исходных атрибутов для связанного пользователя.</span><span class="sxs-lookup"><span data-stu-id="f701f-104">The **HomePhones** element specifies an array of home phone numbers and the identifiers of their source attributions for the associated persona.</span></span> 
  
```XML
<HomePhones>
    <PhoneNumberAttributedValue/>
</HomePhones>
```

 <span data-ttu-id="f701f-105">**аррайоффоненумбераттрибутедвалуестипе**</span><span class="sxs-lookup"><span data-stu-id="f701f-105">**ArrayOfPhoneNumberAttributedValuesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f701f-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="f701f-106">Attributes and elements</span></span>

<span data-ttu-id="f701f-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="f701f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f701f-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="f701f-108">Attributes</span></span>

<span data-ttu-id="f701f-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="f701f-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f701f-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="f701f-110">Child elements</span></span>

|<span data-ttu-id="f701f-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="f701f-111">**Element**</span></span>|<span data-ttu-id="f701f-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="f701f-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f701f-113">фоненумбераттрибутедвалуе</span><span class="sxs-lookup"><span data-stu-id="f701f-113">PhoneNumberAttributedValue</span></span>](phonenumberattributedvalue.md) <br/> |<span data-ttu-id="f701f-114">Содержит номер телефона с одним атрибутом для пользователя.</span><span class="sxs-lookup"><span data-stu-id="f701f-114">Contains a single attributed phone number for a persona.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f701f-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="f701f-115">Parent elements</span></span>

|<span data-ttu-id="f701f-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="f701f-116">**Element**</span></span>|<span data-ttu-id="f701f-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="f701f-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f701f-118">Роль</span><span class="sxs-lookup"><span data-stu-id="f701f-118">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="f701f-119">Задает набор данных о пользователях, возвращаемых запросом к **другому человеку** .</span><span class="sxs-lookup"><span data-stu-id="f701f-119">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="f701f-120">Примечания</span><span class="sxs-lookup"><span data-stu-id="f701f-120">Remarks</span></span>

<span data-ttu-id="f701f-121">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="f701f-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="f701f-122">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="f701f-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f701f-123">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="f701f-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f701f-124">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="f701f-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="f701f-125">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="f701f-125">Schema Name</span></span>  <br/> |<span data-ttu-id="f701f-126">Схема типа</span><span class="sxs-lookup"><span data-stu-id="f701f-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="f701f-127">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="f701f-127">Validation File</span></span>  <br/> |<span data-ttu-id="f701f-128">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="f701f-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="f701f-129">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="f701f-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="f701f-130">См. также</span><span class="sxs-lookup"><span data-stu-id="f701f-130">See also</span></span>



- [<span data-ttu-id="f701f-131">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="f701f-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

