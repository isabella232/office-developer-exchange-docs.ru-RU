---
title: IsHidden
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 2377b584-bd1e-49fc-b80a-a6634721a297
description: Элемент IsHidden содержит логическое значение, указывающее, скрыто или отображается как часть пользователя базового контакта.
ms.openlocfilehash: ee20bf0af287e3cddaedb5bc6d3c63ef9a7a7006
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834032"
---
# <a name="ishidden"></a><span data-ttu-id="02176-103">IsHidden</span><span class="sxs-lookup"><span data-stu-id="02176-103">IsHidden</span></span>

<span data-ttu-id="02176-104">Элемент **IsHidden** содержит логическое значение, указывающее, скрыто или отображается как часть пользователя базового контакта.</span><span class="sxs-lookup"><span data-stu-id="02176-104">The **IsHidden** element contains a Boolean value that indicates whether the underlying contact should be hidden or displayed as part of the persona.</span></span> 
  
```XML
<IsHidden>true | false</IsHidden>
```

 <span data-ttu-id="02176-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="02176-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="02176-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="02176-106">Attributes and elements</span></span>

<span data-ttu-id="02176-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="02176-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="02176-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="02176-108">Attributes</span></span>

<span data-ttu-id="02176-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="02176-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="02176-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="02176-110">Child elements</span></span>

<span data-ttu-id="02176-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="02176-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="02176-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="02176-112">Parent elements</span></span>

|<span data-ttu-id="02176-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="02176-113">**Element**</span></span>|<span data-ttu-id="02176-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="02176-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="02176-115">Атрибуты (PersonaAttributionType)</span><span class="sxs-lookup"><span data-stu-id="02176-115">Attribution (PersonaAttributionType)</span></span>](attribution-personaattributiontype.md) <br/> |<span data-ttu-id="02176-116">Задает экземпляр в массиве атрибутов элемента **пользователя** .</span><span class="sxs-lookup"><span data-stu-id="02176-116">Specifies an instance in an array of attributes for a **Persona** element.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="02176-117">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="02176-117">Text value</span></span>

<span data-ttu-id="02176-118">Текстовое значение **true** для элемента **IsHidden** указывает, что основной контакт необходимо скрыть или отобразить как часть пользователя.</span><span class="sxs-lookup"><span data-stu-id="02176-118">A text value of **true** for the **IsHidden** element indicates that the underlying contact should be hidden or displayed as part of the persona.</span></span> <span data-ttu-id="02176-119">Значение **false** показывает, что основной контакт не следует скрыты или отображается как часть пользователя.</span><span class="sxs-lookup"><span data-stu-id="02176-119">A value of **false** indicates that the underlying contact should not be hidden or displayed as part of the persona.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="02176-120">Замечания</span><span class="sxs-lookup"><span data-stu-id="02176-120">Remarks</span></span>

<span data-ttu-id="02176-121">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="02176-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="02176-122">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="02176-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="02176-123">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="02176-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="02176-124">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="02176-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="02176-125">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="02176-125">Schema Name</span></span>  <br/> |<span data-ttu-id="02176-126">Схема типа</span><span class="sxs-lookup"><span data-stu-id="02176-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="02176-127">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="02176-127">Validation File</span></span>  <br/> |<span data-ttu-id="02176-128">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="02176-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="02176-129">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="02176-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="02176-130">См. также</span><span class="sxs-lookup"><span data-stu-id="02176-130">See also</span></span>



- [<span data-ttu-id="02176-131">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="02176-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

