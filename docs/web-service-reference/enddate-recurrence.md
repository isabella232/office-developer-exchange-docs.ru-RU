---
title: Дата окончания (повторения)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- EndDate
api_type:
- schema
ms.assetid: 16026595-26f8-4770-8a6d-0d3e4157effd
description: Элемент EndDate представляет дату окончания повторяющейся задачи или элемента календаря, который имеет тип шаблона EndDateRecurrence.
ms.openlocfilehash: b8570a069fc0a2d05044a9c85ab2d5c39d70ccdf
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762337"
---
# <a name="enddate-recurrence"></a><span data-ttu-id="a2271-103">Дата окончания (повторения)</span><span class="sxs-lookup"><span data-stu-id="a2271-103">EndDate (Recurrence)</span></span>

<span data-ttu-id="a2271-104">Элемент **EndDate** представляет дату окончания повторяющейся задачи или элемента календаря, который имеет тип шаблона EndDateRecurrence.</span><span class="sxs-lookup"><span data-stu-id="a2271-104">The **EndDate** element represents the end date of a recurring task or a calendar item that has the EndDateRecurrence pattern type.</span></span> 
  
```xml
<EndDate/>
```

 <span data-ttu-id="a2271-105">**Дата**</span><span class="sxs-lookup"><span data-stu-id="a2271-105">**date**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a2271-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="a2271-106">Attributes and elements</span></span>

<span data-ttu-id="a2271-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="a2271-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a2271-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="a2271-108">Attributes</span></span>

<span data-ttu-id="a2271-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="a2271-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a2271-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="a2271-110">Child elements</span></span>

<span data-ttu-id="a2271-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="a2271-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="a2271-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="a2271-112">Parent elements</span></span>

|<span data-ttu-id="a2271-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="a2271-113">**Element**</span></span>|<span data-ttu-id="a2271-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="a2271-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a2271-115">EndDateRecurrence</span><span class="sxs-lookup"><span data-stu-id="a2271-115">EndDateRecurrence</span></span>](enddaterecurrence.md) <br/> |<span data-ttu-id="a2271-116">Описание, Дата начала и Дата окончания повторения элемента.</span><span class="sxs-lookup"><span data-stu-id="a2271-116">Describes the start date and the end date of an item recurrence pattern.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="a2271-117">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="a2271-117">Text value</span></span>

<span data-ttu-id="a2271-118">Текстовое значение, которое представляет дату является обязательным, если данный элемент используется.</span><span class="sxs-lookup"><span data-stu-id="a2271-118">A text value that represents a date is required if this element is used.</span></span> <span data-ttu-id="a2271-119">Значение не должен превышать 1 сентября 4500 00:00:00.</span><span class="sxs-lookup"><span data-stu-id="a2271-119">The value cannot be larger than September 1, 4500 00:00:00.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="a2271-120">Замечания</span><span class="sxs-lookup"><span data-stu-id="a2271-120">Remarks</span></span>

<span data-ttu-id="a2271-121">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="a2271-121">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a2271-122">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="a2271-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a2271-123">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="a2271-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="a2271-124">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="a2271-124">Schema name</span></span>  <br/> |<span data-ttu-id="a2271-125">Схема Types</span><span class="sxs-lookup"><span data-stu-id="a2271-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="a2271-126">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="a2271-126">Validation file</span></span>  <br/> |<span data-ttu-id="a2271-127">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="a2271-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="a2271-128">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="a2271-128">Can be empty</span></span>  <br/> |<span data-ttu-id="a2271-129">False</span><span class="sxs-lookup"><span data-stu-id="a2271-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a2271-130">См. также</span><span class="sxs-lookup"><span data-stu-id="a2271-130">See also</span></span>



- [<span data-ttu-id="a2271-131">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="a2271-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

