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
ms.openlocfilehash: b55d6ca752a5b00a27eb158c6a22412a9f4ecdda
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460836"
---
# <a name="homephones"></a><span data-ttu-id="86d13-103">хомефонес</span><span class="sxs-lookup"><span data-stu-id="86d13-103">HomePhones</span></span>

<span data-ttu-id="86d13-104">Элемент **хомефонес** указывает массив номеров домашнего телефона и идентификаторы их исходных атрибутов для связанного пользователя.</span><span class="sxs-lookup"><span data-stu-id="86d13-104">The **HomePhones** element specifies an array of home phone numbers and the identifiers of their source attributions for the associated persona.</span></span> 
  
```XML
<HomePhones>
    <PhoneNumberAttributedValue/>
</HomePhones>
```

 <span data-ttu-id="86d13-105">**аррайоффоненумбераттрибутедвалуестипе**</span><span class="sxs-lookup"><span data-stu-id="86d13-105">**ArrayOfPhoneNumberAttributedValuesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="86d13-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="86d13-106">Attributes and elements</span></span>

<span data-ttu-id="86d13-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="86d13-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="86d13-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="86d13-108">Attributes</span></span>

<span data-ttu-id="86d13-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="86d13-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="86d13-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="86d13-110">Child elements</span></span>

|<span data-ttu-id="86d13-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="86d13-111">**Element**</span></span>|<span data-ttu-id="86d13-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="86d13-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="86d13-113">фоненумбераттрибутедвалуе</span><span class="sxs-lookup"><span data-stu-id="86d13-113">PhoneNumberAttributedValue</span></span>](phonenumberattributedvalue.md) <br/> |<span data-ttu-id="86d13-114">Содержит номер телефона с одним атрибутом для пользователя.</span><span class="sxs-lookup"><span data-stu-id="86d13-114">Contains a single attributed phone number for a persona.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="86d13-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="86d13-115">Parent elements</span></span>

|<span data-ttu-id="86d13-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="86d13-116">**Element**</span></span>|<span data-ttu-id="86d13-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="86d13-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="86d13-118">Роль</span><span class="sxs-lookup"><span data-stu-id="86d13-118">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="86d13-119">Задает набор данных о пользователях, возвращаемых запросом к **другому человеку** .</span><span class="sxs-lookup"><span data-stu-id="86d13-119">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="86d13-120">Примечания</span><span class="sxs-lookup"><span data-stu-id="86d13-120">Remarks</span></span>

<span data-ttu-id="86d13-121">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="86d13-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="86d13-122">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="86d13-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="86d13-123">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="86d13-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="86d13-124">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="86d13-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="86d13-125">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="86d13-125">Schema Name</span></span>  <br/> |<span data-ttu-id="86d13-126">Схема типа</span><span class="sxs-lookup"><span data-stu-id="86d13-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="86d13-127">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="86d13-127">Validation File</span></span>  <br/> |<span data-ttu-id="86d13-128">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="86d13-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="86d13-129">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="86d13-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="86d13-130">См. также</span><span class="sxs-lookup"><span data-stu-id="86d13-130">See also</span></span>



- [<span data-ttu-id="86d13-131">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="86d13-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

