---
title: ModifiedOccurrences
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ModifiedOccurrences
api_type:
- schema
ms.assetid: 552932fc-b3b4-486e-8d73-32c0bb10bd68
description: Элемент ModifiedOccurrences содержит массив повторяющихся вхождения элемента календаря, которые были изменены, отличного от элемента шаблона повторения.
ms.openlocfilehash: 53f60740bcaa2de6713e1b6a3d2874153285645a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19834472"
---
# <a name="modifiedoccurrences"></a><span data-ttu-id="8b3a0-103">ModifiedOccurrences</span><span class="sxs-lookup"><span data-stu-id="8b3a0-103">ModifiedOccurrences</span></span>

<span data-ttu-id="8b3a0-104">Элемент **ModifiedOccurrences** содержит массив повторяющихся вхождения элемента календаря, которые были изменены, отличного от элемента шаблона повторения.</span><span class="sxs-lookup"><span data-stu-id="8b3a0-104">The **ModifiedOccurrences** element contains an array of recurring calendar item occurrences that have been modified so that they are different than the recurrence master item.</span></span> 
  
```xml
<ModifiedOccurrences>
   <Occurrence/>
</ModifiedOccurrences>
```

 <span data-ttu-id="8b3a0-105">**NonEmptyArrayOfOccurrenceInfoType**</span><span class="sxs-lookup"><span data-stu-id="8b3a0-105">**NonEmptyArrayOfOccurrenceInfoType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="8b3a0-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="8b3a0-106">Attributes and elements</span></span>

<span data-ttu-id="8b3a0-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="8b3a0-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8b3a0-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="8b3a0-108">Attributes</span></span>

<span data-ttu-id="8b3a0-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="8b3a0-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8b3a0-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="8b3a0-110">Child elements</span></span>

|<span data-ttu-id="8b3a0-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="8b3a0-111">**Element**</span></span>|<span data-ttu-id="8b3a0-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="8b3a0-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8b3a0-113">Вхождение</span><span class="sxs-lookup"><span data-stu-id="8b3a0-113">Occurrence</span></span>](occurrence.md) <br/> |<span data-ttu-id="8b3a0-114">Представляет измененной вхождения повторяющегося элемента календаря.</span><span class="sxs-lookup"><span data-stu-id="8b3a0-114">Represents a single modified occurrence of a recurring calendar item.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="8b3a0-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="8b3a0-115">Parent elements</span></span>

|<span data-ttu-id="8b3a0-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="8b3a0-116">**Element**</span></span>|<span data-ttu-id="8b3a0-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="8b3a0-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8b3a0-118">Элемента календаря, имеющего</span><span class="sxs-lookup"><span data-stu-id="8b3a0-118">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="8b3a0-119">Представляет элемент календаря Exchange.</span><span class="sxs-lookup"><span data-stu-id="8b3a0-119">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="8b3a0-120">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="8b3a0-120">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="8b3a0-121">Представляет приглашение на собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="8b3a0-121">Represents a meeting request in the Exchange store.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="8b3a0-122">Замечания</span><span class="sxs-lookup"><span data-stu-id="8b3a0-122">Remarks</span></span>

<span data-ttu-id="8b3a0-123">Этот элемент является допустимым, если [CalendarItemType](calendaritemtype.md) имеет значение RecurringMaster.</span><span class="sxs-lookup"><span data-stu-id="8b3a0-123">This element is valid if [CalendarItemType](calendaritemtype.md) has the RecurringMaster value.</span></span> 
  
<span data-ttu-id="8b3a0-124">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="8b3a0-124">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="8b3a0-125">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="8b3a0-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8b3a0-126">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="8b3a0-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="8b3a0-127">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="8b3a0-127">Schema name</span></span>  <br/> |<span data-ttu-id="8b3a0-128">Схема Types</span><span class="sxs-lookup"><span data-stu-id="8b3a0-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="8b3a0-129">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="8b3a0-129">Validation file</span></span>  <br/> |<span data-ttu-id="8b3a0-130">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="8b3a0-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="8b3a0-131">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="8b3a0-131">Can be empty</span></span>  <br/> |<span data-ttu-id="8b3a0-132">False</span><span class="sxs-lookup"><span data-stu-id="8b3a0-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="8b3a0-133">См. также</span><span class="sxs-lookup"><span data-stu-id="8b3a0-133">See also</span></span>



- [<span data-ttu-id="8b3a0-134">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="8b3a0-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

