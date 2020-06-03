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
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461620"
---
# <a name="businessphonenumbers"></a><span data-ttu-id="7a51b-103">бусинессфоненумберс</span><span class="sxs-lookup"><span data-stu-id="7a51b-103">BusinessPhoneNumbers</span></span>

<span data-ttu-id="7a51b-104">Элемент **бусинессфоненумберс** указывает массив номеров рабочих телефонов и идентификаторы их исходных атрибутов для связанного пользователя.</span><span class="sxs-lookup"><span data-stu-id="7a51b-104">The **BusinessPhoneNumbers** element specifies an array of business phone numbers and the identifiers of their source attributions for the associated persona.</span></span> 
  
```XML
<BusinessPhoneNumbers>
    <Value></Value>
    <Attributions></Attributions>
</BusinessPhoneNumbers>
```

 <span data-ttu-id="7a51b-105">**аррайоффоненумбераттрибутедвалуестипе**</span><span class="sxs-lookup"><span data-stu-id="7a51b-105">**ArrayOfPhoneNumberAttributedValuesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7a51b-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="7a51b-106">Attributes and elements</span></span>

<span data-ttu-id="7a51b-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="7a51b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7a51b-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="7a51b-108">Attributes</span></span>

<span data-ttu-id="7a51b-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="7a51b-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7a51b-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="7a51b-110">Child elements</span></span>

|<span data-ttu-id="7a51b-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="7a51b-111">**Element**</span></span>|<span data-ttu-id="7a51b-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="7a51b-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7a51b-113">Значение (Персонафоненумбертипе)</span><span class="sxs-lookup"><span data-stu-id="7a51b-113">Value (PersonaPhoneNumberType)</span></span>](value-personaphonenumbertype.md) <br/> |<span data-ttu-id="7a51b-114">Указывает номер телефона и тип сведений, а также связанный с набором сопоставлений.</span><span class="sxs-lookup"><span data-stu-id="7a51b-114">Specifies a phone number and type information and is associated with a set of attributions.</span></span>  <br/> |
|[<span data-ttu-id="7a51b-115">Атрибуты (Аррайофвалуеаттрибутионстипе)</span><span class="sxs-lookup"><span data-stu-id="7a51b-115">Attributions (ArrayOfValueAttributionsType)</span></span>](attributions-arrayofvalueattributionstype.md) <br/> |<span data-ttu-id="7a51b-116">Задает массив атрибутов для связанного элемента **value** .</span><span class="sxs-lookup"><span data-stu-id="7a51b-116">Specifies an array of attributions for its associated **Value** element.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="7a51b-117">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="7a51b-117">Parent elements</span></span>

|<span data-ttu-id="7a51b-118">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="7a51b-118">**Element**</span></span>|<span data-ttu-id="7a51b-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="7a51b-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7a51b-120">Роль</span><span class="sxs-lookup"><span data-stu-id="7a51b-120">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="7a51b-121">Задает набор данных о пользователях, возвращаемых запросом к **другому человеку** .</span><span class="sxs-lookup"><span data-stu-id="7a51b-121">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="7a51b-122">Примечания</span><span class="sxs-lookup"><span data-stu-id="7a51b-122">Remarks</span></span>

<span data-ttu-id="7a51b-123">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="7a51b-123">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="7a51b-124">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="7a51b-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7a51b-125">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="7a51b-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7a51b-126">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="7a51b-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="7a51b-127">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="7a51b-127">Schema Name</span></span>  <br/> |<span data-ttu-id="7a51b-128">Схема типа</span><span class="sxs-lookup"><span data-stu-id="7a51b-128">Type schema</span></span>  <br/> |
|<span data-ttu-id="7a51b-129">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="7a51b-129">Validation File</span></span>  <br/> |<span data-ttu-id="7a51b-130">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="7a51b-130">types.xsd</span></span>  <br/> |
|<span data-ttu-id="7a51b-131">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="7a51b-131">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="7a51b-132">См. также</span><span class="sxs-lookup"><span data-stu-id="7a51b-132">See also</span></span>



- [<span data-ttu-id="7a51b-133">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="7a51b-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

