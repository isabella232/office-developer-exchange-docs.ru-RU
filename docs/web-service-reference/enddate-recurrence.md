---
title: EndDate (повторение)
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
description: Элемент EndDate представляет дату окончания повторяющейся задачи или элемент календаря с типом шаблона Енддатерекурренце.
ms.openlocfilehash: 53d9b04faf1d8f740c858080b5fcbeadf577df0d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460164"
---
# <a name="enddate-recurrence"></a><span data-ttu-id="7915b-103">EndDate (повторение)</span><span class="sxs-lookup"><span data-stu-id="7915b-103">EndDate (Recurrence)</span></span>

<span data-ttu-id="7915b-104">Элемент **EndDate** представляет дату окончания повторяющейся задачи или элемент календаря с типом шаблона енддатерекурренце.</span><span class="sxs-lookup"><span data-stu-id="7915b-104">The **EndDate** element represents the end date of a recurring task or a calendar item that has the EndDateRecurrence pattern type.</span></span> 
  
```xml
<EndDate/>
```

 <span data-ttu-id="7915b-105">**дата**</span><span class="sxs-lookup"><span data-stu-id="7915b-105">**date**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7915b-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="7915b-106">Attributes and elements</span></span>

<span data-ttu-id="7915b-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="7915b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7915b-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="7915b-108">Attributes</span></span>

<span data-ttu-id="7915b-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="7915b-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7915b-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="7915b-110">Child elements</span></span>

<span data-ttu-id="7915b-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="7915b-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="7915b-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="7915b-112">Parent elements</span></span>

|<span data-ttu-id="7915b-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="7915b-113">**Element**</span></span>|<span data-ttu-id="7915b-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="7915b-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7915b-115">енддатерекурренце</span><span class="sxs-lookup"><span data-stu-id="7915b-115">EndDateRecurrence</span></span>](enddaterecurrence.md) <br/> |<span data-ttu-id="7915b-116">Описывает дату начала и дату окончания расписания повторения элемента.</span><span class="sxs-lookup"><span data-stu-id="7915b-116">Describes the start date and the end date of an item recurrence pattern.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="7915b-117">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="7915b-117">Text value</span></span>

<span data-ttu-id="7915b-118">Текстовое значение, представляющее дату, является обязательным при использовании этого элемента.</span><span class="sxs-lookup"><span data-stu-id="7915b-118">A text value that represents a date is required if this element is used.</span></span> <span data-ttu-id="7915b-119">Значение не может превышать 1 сентября 4500 00:00:00.</span><span class="sxs-lookup"><span data-stu-id="7915b-119">The value cannot be larger than September 1, 4500 00:00:00.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="7915b-120">Примечания</span><span class="sxs-lookup"><span data-stu-id="7915b-120">Remarks</span></span>

<span data-ttu-id="7915b-121">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="7915b-121">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7915b-122">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="7915b-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7915b-123">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="7915b-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="7915b-124">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="7915b-124">Schema name</span></span>  <br/> |<span data-ttu-id="7915b-125">Схема Types</span><span class="sxs-lookup"><span data-stu-id="7915b-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="7915b-126">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="7915b-126">Validation file</span></span>  <br/> |<span data-ttu-id="7915b-127">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="7915b-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="7915b-128">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="7915b-128">Can be empty</span></span>  <br/> |<span data-ttu-id="7915b-129">False</span><span class="sxs-lookup"><span data-stu-id="7915b-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7915b-130">См. также</span><span class="sxs-lookup"><span data-stu-id="7915b-130">See also</span></span>



- [<span data-ttu-id="7915b-131">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="7915b-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

