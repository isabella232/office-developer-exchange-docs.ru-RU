---
title: OriginalStart
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- OriginalStart
api_type:
- schema
ms.assetid: 4599dd34-15ee-4d57-b886-732081b50784
description: Элемент OriginalStart представляет исходное время начала элемента календаря.
ms.openlocfilehash: 9e5facb3df87ab08e05f23258abdf1767fae64e4
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19834668"
---
# <a name="originalstart"></a><span data-ttu-id="515eb-103">OriginalStart</span><span class="sxs-lookup"><span data-stu-id="515eb-103">OriginalStart</span></span>

<span data-ttu-id="515eb-104">Элемент **OriginalStart** представляет исходное время начала элемента календаря.</span><span class="sxs-lookup"><span data-stu-id="515eb-104">The **OriginalStart** element represents the original start time of a calendar item.</span></span> 
  
```xml
<OriginalStart/>
```

 <span data-ttu-id="515eb-105">**DateTime**</span><span class="sxs-lookup"><span data-stu-id="515eb-105">**DateTime**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="515eb-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="515eb-106">Attributes and elements</span></span>

<span data-ttu-id="515eb-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="515eb-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="515eb-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="515eb-108">Attributes</span></span>

<span data-ttu-id="515eb-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="515eb-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="515eb-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="515eb-110">Child elements</span></span>

<span data-ttu-id="515eb-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="515eb-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="515eb-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="515eb-112">Parent elements</span></span>

|<span data-ttu-id="515eb-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="515eb-113">**Element**</span></span>|<span data-ttu-id="515eb-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="515eb-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="515eb-115">Элемента календаря, имеющего</span><span class="sxs-lookup"><span data-stu-id="515eb-115">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="515eb-116">Представляет элемент календаря в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="515eb-116">Represents a calendar item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="515eb-117">FirstOccurrence</span><span class="sxs-lookup"><span data-stu-id="515eb-117">FirstOccurrence</span></span>](firstoccurrence.md) <br/> |<span data-ttu-id="515eb-118">Представляет первого появления повторяющегося элемента календаря.</span><span class="sxs-lookup"><span data-stu-id="515eb-118">Represents the first occurrence of a recurring calendar item.</span></span>  <br/> |
|[<span data-ttu-id="515eb-119">LastOccurrence</span><span class="sxs-lookup"><span data-stu-id="515eb-119">LastOccurrence</span></span>](lastoccurrence.md) <br/> |<span data-ttu-id="515eb-120">Представляет последнего вхождения повторяющегося элемента календаря.</span><span class="sxs-lookup"><span data-stu-id="515eb-120">Represents the last occurrence of a recurring calendar item.</span></span>  <br/> |
|[<span data-ttu-id="515eb-121">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="515eb-121">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="515eb-122">Представляет приглашение на собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="515eb-122">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="515eb-123">Вхождение</span><span class="sxs-lookup"><span data-stu-id="515eb-123">Occurrence</span></span>](occurrence.md) <br/> |<span data-ttu-id="515eb-124">Представляет измененной вхождения повторяющегося элемента календаря.</span><span class="sxs-lookup"><span data-stu-id="515eb-124">Represents a single modified occurrence of a recurring calendar item.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="515eb-125">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="515eb-125">Text value</span></span>

<span data-ttu-id="515eb-126">Текстовое значение, которое представляет дату и время является обязательным, если данный элемент используется.</span><span class="sxs-lookup"><span data-stu-id="515eb-126">A text value that represents a date and time is required if this element is used.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="515eb-127">Замечания</span><span class="sxs-lookup"><span data-stu-id="515eb-127">Remarks</span></span>

<span data-ttu-id="515eb-128">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="515eb-128">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="515eb-129">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="515eb-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="515eb-130">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="515eb-130">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="515eb-131">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="515eb-131">Schema Name</span></span>  <br/> |<span data-ttu-id="515eb-132">Схема Types</span><span class="sxs-lookup"><span data-stu-id="515eb-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="515eb-133">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="515eb-133">Validation File</span></span>  <br/> |<span data-ttu-id="515eb-134">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="515eb-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="515eb-135">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="515eb-135">Can be Empty</span></span>  <br/> |<span data-ttu-id="515eb-136">False</span><span class="sxs-lookup"><span data-stu-id="515eb-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="515eb-137">См. также</span><span class="sxs-lookup"><span data-stu-id="515eb-137">See also</span></span>



- [<span data-ttu-id="515eb-138">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="515eb-138">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

