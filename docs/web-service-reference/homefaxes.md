---
title: хомефаксес
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 459ddb1c-8cff-4125-b6fa-dc93c183dee8
description: Элемент Хомефаксес указывает массив номеров домашнего факса и идентификаторы их исходных атрибутов для связанного пользователя.
ms.openlocfilehash: d49eb9e12547e4011e4ba403cb898c0fe6e9bf02
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460850"
---
# <a name="homefaxes"></a><span data-ttu-id="2969c-103">хомефаксес</span><span class="sxs-lookup"><span data-stu-id="2969c-103">HomeFaxes</span></span>

<span data-ttu-id="2969c-104">Элемент **хомефаксес** указывает массив номеров домашнего факса и идентификаторы их исходных атрибутов для связанного пользователя.</span><span class="sxs-lookup"><span data-stu-id="2969c-104">The **HomeFaxes** element specifies an array of home fax numbers and the identifiers of their source attributions for the associated persona.</span></span> 
  
```XML
<HomeFaxes>
    <PhoneNumberAttributedValue/>
</HomeFaxes>
```

 <span data-ttu-id="2969c-105">**аррайоффоненумбераттрибутедвалуестипе**</span><span class="sxs-lookup"><span data-stu-id="2969c-105">**ArrayOfPhoneNumberAttributedValuesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2969c-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="2969c-106">Attributes and elements</span></span>

<span data-ttu-id="2969c-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="2969c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2969c-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="2969c-108">Attributes</span></span>

<span data-ttu-id="2969c-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="2969c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2969c-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="2969c-110">Child elements</span></span>

|<span data-ttu-id="2969c-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="2969c-111">**Element**</span></span>|<span data-ttu-id="2969c-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="2969c-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2969c-113">фоненумбераттрибутедвалуе</span><span class="sxs-lookup"><span data-stu-id="2969c-113">PhoneNumberAttributedValue</span></span>](phonenumberattributedvalue.md) <br/> |<span data-ttu-id="2969c-114">Содержит номер телефона с одним атрибутом для пользователя.</span><span class="sxs-lookup"><span data-stu-id="2969c-114">Contains a single attributed phone number for a persona.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="2969c-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="2969c-115">Parent elements</span></span>

|<span data-ttu-id="2969c-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="2969c-116">**Element**</span></span>|<span data-ttu-id="2969c-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="2969c-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2969c-118">Роль</span><span class="sxs-lookup"><span data-stu-id="2969c-118">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="2969c-119">Задает набор данных о пользователях, возвращаемых запросом к **другому человеку** .</span><span class="sxs-lookup"><span data-stu-id="2969c-119">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="2969c-120">Примечания</span><span class="sxs-lookup"><span data-stu-id="2969c-120">Remarks</span></span>

<span data-ttu-id="2969c-121">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="2969c-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="2969c-122">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="2969c-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2969c-123">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="2969c-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2969c-124">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="2969c-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="2969c-125">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="2969c-125">Schema Name</span></span>  <br/> |<span data-ttu-id="2969c-126">Схема типа</span><span class="sxs-lookup"><span data-stu-id="2969c-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="2969c-127">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="2969c-127">Validation File</span></span>  <br/> |<span data-ttu-id="2969c-128">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="2969c-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="2969c-129">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="2969c-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="2969c-130">См. также</span><span class="sxs-lookup"><span data-stu-id="2969c-130">See also</span></span>



- [<span data-ttu-id="2969c-131">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="2969c-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

