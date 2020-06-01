---
title: IsHidden
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 2377b584-bd1e-49fc-b80a-a6634721a297
description: Элемент Hidden содержит логическое значение, которое указывает, следует ли скрыть или отобразить основной контакт в составе персонажа.
ms.openlocfilehash: a22628e9ab4a46de04fe395f2d6c1b70083a5c77
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44464240"
---
# <a name="ishidden"></a><span data-ttu-id="c3f98-103">IsHidden</span><span class="sxs-lookup"><span data-stu-id="c3f98-103">IsHidden</span></span>

<span data-ttu-id="c3f98-104">Элемент **Hidden** содержит логическое значение, которое указывает, следует ли скрыть или отобразить основной контакт в составе персонажа.</span><span class="sxs-lookup"><span data-stu-id="c3f98-104">The **IsHidden** element contains a Boolean value that indicates whether the underlying contact should be hidden or displayed as part of the persona.</span></span> 
  
```XML
<IsHidden>true | false</IsHidden>
```

 <span data-ttu-id="c3f98-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="c3f98-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c3f98-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="c3f98-106">Attributes and elements</span></span>

<span data-ttu-id="c3f98-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="c3f98-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c3f98-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="c3f98-108">Attributes</span></span>

<span data-ttu-id="c3f98-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="c3f98-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c3f98-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="c3f98-110">Child elements</span></span>

<span data-ttu-id="c3f98-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="c3f98-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="c3f98-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="c3f98-112">Parent elements</span></span>

|<span data-ttu-id="c3f98-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="c3f98-113">**Element**</span></span>|<span data-ttu-id="c3f98-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="c3f98-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c3f98-115">Атрибуты (Персонааттрибутионтипе)</span><span class="sxs-lookup"><span data-stu-id="c3f98-115">Attribution (PersonaAttributionType)</span></span>](attribution-personaattributiontype.md) <br/> |<span data-ttu-id="c3f98-116">Указывает экземпляр в массиве атрибутов для элемента **персоны** .</span><span class="sxs-lookup"><span data-stu-id="c3f98-116">Specifies an instance in an array of attributes for a **Persona** element.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="c3f98-117">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="c3f98-117">Text value</span></span>

<span data-ttu-id="c3f98-118">Текстовое значение **true** для элемента **Hidden** указывает на то, что основной контакт должен быть скрыт или отображаться в составе персонажа.</span><span class="sxs-lookup"><span data-stu-id="c3f98-118">A text value of **true** for the **IsHidden** element indicates that the underlying contact should be hidden or displayed as part of the persona.</span></span> <span data-ttu-id="c3f98-119">Значение **false** указывает, что базовый контакт не должен быть скрытым или отображаться как часть персонажа.</span><span class="sxs-lookup"><span data-stu-id="c3f98-119">A value of **false** indicates that the underlying contact should not be hidden or displayed as part of the persona.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="c3f98-120">Примечания</span><span class="sxs-lookup"><span data-stu-id="c3f98-120">Remarks</span></span>

<span data-ttu-id="c3f98-121">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="c3f98-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="c3f98-122">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="c3f98-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c3f98-123">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="c3f98-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c3f98-124">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="c3f98-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="c3f98-125">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="c3f98-125">Schema Name</span></span>  <br/> |<span data-ttu-id="c3f98-126">Схема типа</span><span class="sxs-lookup"><span data-stu-id="c3f98-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="c3f98-127">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="c3f98-127">Validation File</span></span>  <br/> |<span data-ttu-id="c3f98-128">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="c3f98-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="c3f98-129">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="c3f98-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="c3f98-130">См. также</span><span class="sxs-lookup"><span data-stu-id="c3f98-130">See also</span></span>



- [<span data-ttu-id="c3f98-131">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="c3f98-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

