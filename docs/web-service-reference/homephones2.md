---
title: HomePhones2
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: ba9bb159-362d-48e0-889d-823cb46ecebf
description: Элемент HomePhones2 указывает массив значений HomePhone2 и идентификаторы их исходных атрибутов для связанного пользователя.
ms.openlocfilehash: 205f2f71421a0dfc7d0057412529bcefdb6636d5
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833842"
---
# <a name="homephones2"></a><span data-ttu-id="02d0b-103">HomePhones2</span><span class="sxs-lookup"><span data-stu-id="02d0b-103">HomePhones2</span></span>

<span data-ttu-id="02d0b-104">Элемент **HomePhones2** указывает массив значений **HomePhone2** и идентификаторы их исходных атрибутов для связанного пользователя.</span><span class="sxs-lookup"><span data-stu-id="02d0b-104">The **HomePhones2** element specifies an array of **HomePhone2** values and the identifiers of their source attributions for the associated persona.</span></span> 
  
```XML
<HomePhones2>
    <PhoneNumberAttributedValue/>
</HomePhones2>
```

 <span data-ttu-id="02d0b-105">**аррайоффоненумбераттрибутедвалуестипе**</span><span class="sxs-lookup"><span data-stu-id="02d0b-105">**ArrayOfPhoneNumberAttributedValuesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="02d0b-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="02d0b-106">Attributes and elements</span></span>

<span data-ttu-id="02d0b-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="02d0b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="02d0b-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="02d0b-108">Attributes</span></span>

<span data-ttu-id="02d0b-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="02d0b-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="02d0b-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="02d0b-110">Child elements</span></span>

|<span data-ttu-id="02d0b-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="02d0b-111">**Element**</span></span>|<span data-ttu-id="02d0b-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="02d0b-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="02d0b-113">фоненумбераттрибутедвалуе</span><span class="sxs-lookup"><span data-stu-id="02d0b-113">PhoneNumberAttributedValue</span></span>](phonenumberattributedvalue.md) <br/> |<span data-ttu-id="02d0b-114">Содержит номер телефона с одним атрибутом для пользователя.</span><span class="sxs-lookup"><span data-stu-id="02d0b-114">Contains a single attributed phone number for a persona.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="02d0b-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="02d0b-115">Parent elements</span></span>

|<span data-ttu-id="02d0b-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="02d0b-116">**Element**</span></span>|<span data-ttu-id="02d0b-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="02d0b-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="02d0b-118">Роль</span><span class="sxs-lookup"><span data-stu-id="02d0b-118">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="02d0b-119">Задает набор данных о пользователях, возвращаемых запросом к **другому человеку** .</span><span class="sxs-lookup"><span data-stu-id="02d0b-119">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="02d0b-120">Примечания</span><span class="sxs-lookup"><span data-stu-id="02d0b-120">Remarks</span></span>

<span data-ttu-id="02d0b-121">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="02d0b-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="02d0b-122">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="02d0b-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="02d0b-123">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="02d0b-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="02d0b-124">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="02d0b-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="02d0b-125">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="02d0b-125">Schema Name</span></span>  <br/> |<span data-ttu-id="02d0b-126">Схема типа</span><span class="sxs-lookup"><span data-stu-id="02d0b-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="02d0b-127">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="02d0b-127">Validation File</span></span>  <br/> |<span data-ttu-id="02d0b-128">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="02d0b-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="02d0b-129">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="02d0b-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="02d0b-130">См. также</span><span class="sxs-lookup"><span data-stu-id="02d0b-130">See also</span></span>



- [<span data-ttu-id="02d0b-131">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="02d0b-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

