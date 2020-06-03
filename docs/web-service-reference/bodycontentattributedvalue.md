---
title: бодиконтентаттрибутедвалуе
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f99e9590-8388-4203-ac30-1ea394f351a6
description: Элемент Бодиконтентаттрибутедвалуе указывает содержимое тела элемента.
ms.openlocfilehash: 3550d9307e9bd652afc217f72610379a0a5b2f68
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44527399"
---
# <a name="bodycontentattributedvalue"></a><span data-ttu-id="13a0d-103">бодиконтентаттрибутедвалуе</span><span class="sxs-lookup"><span data-stu-id="13a0d-103">BodyContentAttributedValue</span></span>

<span data-ttu-id="13a0d-104">Элемент **бодиконтентаттрибутедвалуе** указывает содержимое тела элемента.</span><span class="sxs-lookup"><span data-stu-id="13a0d-104">The **BodyContentAttributedValue** element specifies the body content of an item.</span></span> 
  
```XML
<BodyContentAttributedValue>
   <Value></Value>
   <Attributions></Attributions>
</ BodyContentAttributedValue>
```

 <span data-ttu-id="13a0d-105">**бодиконтентаттрибутедвалуетипе**</span><span class="sxs-lookup"><span data-stu-id="13a0d-105">**BodyContentAttributedValueType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="13a0d-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="13a0d-106">Attributes and elements</span></span>

<span data-ttu-id="13a0d-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="13a0d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="13a0d-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="13a0d-108">Attributes</span></span>

<span data-ttu-id="13a0d-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="13a0d-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="13a0d-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="13a0d-110">Child elements</span></span>

|<span data-ttu-id="13a0d-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="13a0d-111">**Element**</span></span>|<span data-ttu-id="13a0d-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="13a0d-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="13a0d-113">Значение (Бодиконтенттипе)</span><span class="sxs-lookup"><span data-stu-id="13a0d-113">Value (BodyContentType)</span></span>](value-bodycontenttype.md) <br/> |<span data-ttu-id="13a0d-114">Задает значение элемента **бодиконтентаттрибутедвалуе** .</span><span class="sxs-lookup"><span data-stu-id="13a0d-114">Specifies the value of a **BodyContentAttributedValue** element.</span></span>  <br/> |
|[<span data-ttu-id="13a0d-115">Атрибуты (Аррайофперсонааттрибутионстипе)</span><span class="sxs-lookup"><span data-stu-id="13a0d-115">Attributions (ArrayOfPersonaAttributionsType)</span></span>](attributions-arrayofpersonaattributionstype.md) <br/> |<span data-ttu-id="13a0d-116">Задает массив сведений о сопоставлении для одного или нескольких контактов или получателей Active Directory, собранных в сопоставленный с ним пользователь.</span><span class="sxs-lookup"><span data-stu-id="13a0d-116">Specifies an array of attribution information for one or more of the contacts or active directory recipients aggregated into the associated persona.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="13a0d-117">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="13a0d-117">Parent elements</span></span>

|<span data-ttu-id="13a0d-118">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="13a0d-118">**Element**</span></span>|<span data-ttu-id="13a0d-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="13a0d-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="13a0d-120">Тексты</span><span class="sxs-lookup"><span data-stu-id="13a0d-120">Bodies</span></span>](bodies.md) <br/> |<span data-ttu-id="13a0d-121">Указывает массив элементов **бодиконтентаттрибутедвалуе** .</span><span class="sxs-lookup"><span data-stu-id="13a0d-121">Specifies an array of **BodyContentAttributedValue** elements.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="13a0d-122">Примечания</span><span class="sxs-lookup"><span data-stu-id="13a0d-122">Remarks</span></span>

<span data-ttu-id="13a0d-123">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="13a0d-123">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="13a0d-124">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="13a0d-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="13a0d-125">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="13a0d-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="13a0d-126">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="13a0d-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="13a0d-127">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="13a0d-127">Schema Name</span></span>  <br/> |<span data-ttu-id="13a0d-128">Схема типа</span><span class="sxs-lookup"><span data-stu-id="13a0d-128">Type schema</span></span>  <br/> |
|<span data-ttu-id="13a0d-129">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="13a0d-129">Validation File</span></span>  <br/> |<span data-ttu-id="13a0d-130">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="13a0d-130">types.xsd</span></span>  <br/> |
|<span data-ttu-id="13a0d-131">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="13a0d-131">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="13a0d-132">См. также</span><span class="sxs-lookup"><span data-stu-id="13a0d-132">See also</span></span>



- [<span data-ttu-id="13a0d-133">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="13a0d-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

