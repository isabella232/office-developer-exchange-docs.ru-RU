---
title: бусинессфоненумберс
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: ecbe4f1c-1c9e-44e0-a8f7-08c160a0fddb
description: Элемент Бусинессфоненумберс указывает массив номеров рабочих телефонов и идентификаторы их исходных атрибутов для связанного пользователя.
ms.openlocfilehash: 8713af3ad302a2940cab247ff7188e55e8021ca0
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44461620"
---
# <a name="businessphonenumbers"></a><span data-ttu-id="65ed5-103">бусинессфоненумберс</span><span class="sxs-lookup"><span data-stu-id="65ed5-103">BusinessPhoneNumbers</span></span>

<span data-ttu-id="65ed5-104">Элемент **бусинессфоненумберс** указывает массив номеров рабочих телефонов и идентификаторы их исходных атрибутов для связанного пользователя.</span><span class="sxs-lookup"><span data-stu-id="65ed5-104">The **BusinessPhoneNumbers** element specifies an array of business phone numbers and the identifiers of their source attributions for the associated persona.</span></span> 
  
```XML
<BusinessPhoneNumbers>
    <Value></Value>
    <Attributions></Attributions>
</BusinessPhoneNumbers>
```

 <span data-ttu-id="65ed5-105">**аррайоффоненумбераттрибутедвалуестипе**</span><span class="sxs-lookup"><span data-stu-id="65ed5-105">**ArrayOfPhoneNumberAttributedValuesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="65ed5-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="65ed5-106">Attributes and elements</span></span>

<span data-ttu-id="65ed5-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="65ed5-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="65ed5-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="65ed5-108">Attributes</span></span>

<span data-ttu-id="65ed5-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="65ed5-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="65ed5-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="65ed5-110">Child elements</span></span>

|<span data-ttu-id="65ed5-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="65ed5-111">**Element**</span></span>|<span data-ttu-id="65ed5-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="65ed5-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="65ed5-113">Значение (Персонафоненумбертипе)</span><span class="sxs-lookup"><span data-stu-id="65ed5-113">Value (PersonaPhoneNumberType)</span></span>](value-personaphonenumbertype.md) <br/> |<span data-ttu-id="65ed5-114">Указывает номер телефона и тип сведений, а также связанный с набором сопоставлений.</span><span class="sxs-lookup"><span data-stu-id="65ed5-114">Specifies a phone number and type information and is associated with a set of attributions.</span></span>  <br/> |
|[<span data-ttu-id="65ed5-115">Атрибуты (Аррайофвалуеаттрибутионстипе)</span><span class="sxs-lookup"><span data-stu-id="65ed5-115">Attributions (ArrayOfValueAttributionsType)</span></span>](attributions-arrayofvalueattributionstype.md) <br/> |<span data-ttu-id="65ed5-116">Задает массив атрибутов для связанного элемента **value** .</span><span class="sxs-lookup"><span data-stu-id="65ed5-116">Specifies an array of attributions for its associated **Value** element.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="65ed5-117">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="65ed5-117">Parent elements</span></span>

|<span data-ttu-id="65ed5-118">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="65ed5-118">**Element**</span></span>|<span data-ttu-id="65ed5-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="65ed5-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="65ed5-120">Роль</span><span class="sxs-lookup"><span data-stu-id="65ed5-120">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="65ed5-121">Задает набор данных о пользователях, возвращаемых запросом к **другому человеку** .</span><span class="sxs-lookup"><span data-stu-id="65ed5-121">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="65ed5-122">Примечания</span><span class="sxs-lookup"><span data-stu-id="65ed5-122">Remarks</span></span>

<span data-ttu-id="65ed5-123">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="65ed5-123">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="65ed5-124">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="65ed5-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="65ed5-125">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="65ed5-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="65ed5-126">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="65ed5-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="65ed5-127">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="65ed5-127">Schema Name</span></span>  <br/> |<span data-ttu-id="65ed5-128">Схема типа</span><span class="sxs-lookup"><span data-stu-id="65ed5-128">Type schema</span></span>  <br/> |
|<span data-ttu-id="65ed5-129">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="65ed5-129">Validation File</span></span>  <br/> |<span data-ttu-id="65ed5-130">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="65ed5-130">types.xsd</span></span>  <br/> |
|<span data-ttu-id="65ed5-131">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="65ed5-131">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="65ed5-132">См. также</span><span class="sxs-lookup"><span data-stu-id="65ed5-132">See also</span></span>



- [<span data-ttu-id="65ed5-133">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="65ed5-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

