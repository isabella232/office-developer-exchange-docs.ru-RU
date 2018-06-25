---
title: LastOccurrence
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- LastOccurrence
api_type:
- schema
ms.assetid: c9ef0fcb-4265-4e60-9986-fff0f211d00b
description: Элемент LastOccurrence представляет последнего вхождения повторяющегося элемента календаря.
ms.openlocfilehash: 2c8fdfc0005e86c9dda84a48ae1d3692b5134ca8
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834209"
---
# <a name="lastoccurrence"></a><span data-ttu-id="b6fc8-103">LastOccurrence</span><span class="sxs-lookup"><span data-stu-id="b6fc8-103">LastOccurrence</span></span>

<span data-ttu-id="b6fc8-104">Элемент **LastOccurrence** представляет последнего вхождения повторяющегося элемента календаря.</span><span class="sxs-lookup"><span data-stu-id="b6fc8-104">The **LastOccurrence** element represents the last occurrence of a recurring calendar item.</span></span> 
  
```xml
<LastOccurrence>
   <ItemId/>
   <Start/>
   <End/>
   <OriginalStart/>
</LastOccurrence>
```

 <span data-ttu-id="b6fc8-105">**OccurrenceInfoType**</span><span class="sxs-lookup"><span data-stu-id="b6fc8-105">**OccurrenceInfoType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b6fc8-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="b6fc8-106">Attributes and elements</span></span>

<span data-ttu-id="b6fc8-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="b6fc8-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b6fc8-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="b6fc8-108">Attributes</span></span>

<span data-ttu-id="b6fc8-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="b6fc8-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b6fc8-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="b6fc8-110">Child elements</span></span>

|<span data-ttu-id="b6fc8-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="b6fc8-111">**Element**</span></span>|<span data-ttu-id="b6fc8-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="b6fc8-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b6fc8-113">Идентификатор элемента</span><span class="sxs-lookup"><span data-stu-id="b6fc8-113">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="b6fc8-114">Содержит уникальный идентификатор и меняет ключ последнего вхождения повторяющегося элемента календаря.</span><span class="sxs-lookup"><span data-stu-id="b6fc8-114">Contains the unique identifier and change key of the last occurrence of a recurring calendar item.</span></span>  <br/> |
|[<span data-ttu-id="b6fc8-115">Start</span><span class="sxs-lookup"><span data-stu-id="b6fc8-115">Start</span></span>](start.md) <br/> |<span data-ttu-id="b6fc8-116">Представляет время начала последнего вхождения повторяющегося элемента календаря.</span><span class="sxs-lookup"><span data-stu-id="b6fc8-116">Represents the start time of the last occurrence of a recurring calendar item.</span></span>  <br/> |
|[<span data-ttu-id="b6fc8-117">End</span><span class="sxs-lookup"><span data-stu-id="b6fc8-117">End </span></span>](end-ex15websvcsotherref.md) <br/> |<span data-ttu-id="b6fc8-118">Представляет время окончания последнего вхождения повторяющегося элемента календаря.</span><span class="sxs-lookup"><span data-stu-id="b6fc8-118">Represents the end time of the last occurrence of a recurring calendar item.</span></span>  <br/> |
|[<span data-ttu-id="b6fc8-119">OriginalStart</span><span class="sxs-lookup"><span data-stu-id="b6fc8-119">OriginalStart</span></span>](originalstart.md) <br/> |<span data-ttu-id="b6fc8-120">Представляет исходное время начала последнего экземпляра повторяющегося элемента календаря.</span><span class="sxs-lookup"><span data-stu-id="b6fc8-120">Represents the original start time of the last occurrence of a recurring calendar item.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="b6fc8-121">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="b6fc8-121">Parent elements</span></span>

|<span data-ttu-id="b6fc8-122">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="b6fc8-122">**Element**</span></span>|<span data-ttu-id="b6fc8-123">**Описание**</span><span class="sxs-lookup"><span data-stu-id="b6fc8-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b6fc8-124">Элемента календаря, имеющего</span><span class="sxs-lookup"><span data-stu-id="b6fc8-124">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="b6fc8-125">Представляет элемент календаря Exchange.</span><span class="sxs-lookup"><span data-stu-id="b6fc8-125">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="b6fc8-126">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="b6fc8-126">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="b6fc8-127">Представляет приглашение на собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="b6fc8-127">Represents a meeting request in the Exchange store.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="b6fc8-128">Замечания</span><span class="sxs-lookup"><span data-stu-id="b6fc8-128">Remarks</span></span>

<span data-ttu-id="b6fc8-129">Этот элемент является допустимым, если [CalendarItemType](calendaritemtype.md) имеет значение RecurringMaster.</span><span class="sxs-lookup"><span data-stu-id="b6fc8-129">This element is valid if [CalendarItemType](calendaritemtype.md) has the RecurringMaster value.</span></span> 
  
<span data-ttu-id="b6fc8-130">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="b6fc8-130">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b6fc8-131">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="b6fc8-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b6fc8-132">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="b6fc8-132">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="b6fc8-133">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="b6fc8-133">Schema name</span></span>  <br/> |<span data-ttu-id="b6fc8-134">Схема Types</span><span class="sxs-lookup"><span data-stu-id="b6fc8-134">Types schema</span></span>  <br/> |
|<span data-ttu-id="b6fc8-135">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="b6fc8-135">Validation file</span></span>  <br/> |<span data-ttu-id="b6fc8-136">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="b6fc8-136">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="b6fc8-137">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="b6fc8-137">Can be empty</span></span>  <br/> |<span data-ttu-id="b6fc8-138">False</span><span class="sxs-lookup"><span data-stu-id="b6fc8-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b6fc8-139">См. также</span><span class="sxs-lookup"><span data-stu-id="b6fc8-139">See also</span></span>



- [<span data-ttu-id="b6fc8-140">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="b6fc8-140">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
  
[<span data-ttu-id="b6fc8-141">Справка по веб-служб Exchange для Exchange</span><span class="sxs-lookup"><span data-stu-id="b6fc8-141">EWS reference for Exchange</span></span>](ews-reference-for-exchange.md)

