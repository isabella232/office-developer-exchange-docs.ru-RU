---
title: каллбаккфонес
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 8a7c1377-aac3-42c5-820f-d01cd8e9cf5c
description: Элемент Каллбаккфонес указывает массив телефонных номеров для обратного вызова и идентификаторы их исходных атрибутов для связанного пользователя.
ms.openlocfilehash: 79d74beffb8de8981e042b0c80e1aa5505a1048c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529464"
---
# <a name="callbackphones"></a><span data-ttu-id="b0a2a-103">каллбаккфонес</span><span class="sxs-lookup"><span data-stu-id="b0a2a-103">CallbackPhones</span></span>

<span data-ttu-id="b0a2a-104">Элемент **каллбаккфонес** указывает массив телефонных номеров для обратного вызова и идентификаторы их исходных атрибутов для связанного пользователя.</span><span class="sxs-lookup"><span data-stu-id="b0a2a-104">The **CallbackPhones** element specifies an array of call-back phone numbers and the identifiers of their source attributions for the associated persona.</span></span> 
  
```XML
<CallbackPhones>
    <Value></Value>
    <Attributions></Attributions>
</CallbackPhones>
```

 <span data-ttu-id="b0a2a-105">**аррайоффоненумбераттрибутедвалуестипе**</span><span class="sxs-lookup"><span data-stu-id="b0a2a-105">**ArrayOfPhoneNumberAttributedValuesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b0a2a-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="b0a2a-106">Attributes and elements</span></span>

<span data-ttu-id="b0a2a-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="b0a2a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b0a2a-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="b0a2a-108">Attributes</span></span>

<span data-ttu-id="b0a2a-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="b0a2a-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b0a2a-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="b0a2a-110">Child elements</span></span>

|<span data-ttu-id="b0a2a-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="b0a2a-111">**Element**</span></span>|<span data-ttu-id="b0a2a-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="b0a2a-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b0a2a-113">Значение (Персонафоненумбертипе)</span><span class="sxs-lookup"><span data-stu-id="b0a2a-113">Value (PersonaPhoneNumberType)</span></span>](value-personaphonenumbertype.md) <br/> |<span data-ttu-id="b0a2a-114">Указывает номер телефона и тип сведений, а также связанный с набором сопоставлений.</span><span class="sxs-lookup"><span data-stu-id="b0a2a-114">Specifies a phone number and type information and is associated with a set of attributions.</span></span>  <br/> |
|[<span data-ttu-id="b0a2a-115">Атрибуты (Аррайофвалуеаттрибутионстипе)</span><span class="sxs-lookup"><span data-stu-id="b0a2a-115">Attributions (ArrayOfValueAttributionsType)</span></span>](attributions-arrayofvalueattributionstype.md) <br/> |<span data-ttu-id="b0a2a-116">Задает массив атрибутов для связанного элемента **value** .</span><span class="sxs-lookup"><span data-stu-id="b0a2a-116">Specifies an array of attributions for its associated **Value** element.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="b0a2a-117">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="b0a2a-117">Parent elements</span></span>

|<span data-ttu-id="b0a2a-118">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="b0a2a-118">**Element**</span></span>|<span data-ttu-id="b0a2a-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="b0a2a-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b0a2a-120">Роль</span><span class="sxs-lookup"><span data-stu-id="b0a2a-120">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="b0a2a-121">Задает набор данных о пользователях, возвращаемых запросом к **другому человеку** .</span><span class="sxs-lookup"><span data-stu-id="b0a2a-121">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="b0a2a-122">Примечания</span><span class="sxs-lookup"><span data-stu-id="b0a2a-122">Remarks</span></span>

<span data-ttu-id="b0a2a-123">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="b0a2a-123">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="b0a2a-124">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="b0a2a-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b0a2a-125">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="b0a2a-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b0a2a-126">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="b0a2a-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="b0a2a-127">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="b0a2a-127">Schema Name</span></span>  <br/> |<span data-ttu-id="b0a2a-128">Схема типа</span><span class="sxs-lookup"><span data-stu-id="b0a2a-128">Type schema</span></span>  <br/> |
|<span data-ttu-id="b0a2a-129">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="b0a2a-129">Validation File</span></span>  <br/> |<span data-ttu-id="b0a2a-130">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="b0a2a-130">types.xsd</span></span>  <br/> |
|<span data-ttu-id="b0a2a-131">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="b0a2a-131">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="b0a2a-132">См. также</span><span class="sxs-lookup"><span data-stu-id="b0a2a-132">See also</span></span>



- [<span data-ttu-id="b0a2a-133">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="b0a2a-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

